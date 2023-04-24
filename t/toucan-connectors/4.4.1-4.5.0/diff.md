# Comparing `tmp/toucan_connectors-4.4.1.tar.gz` & `tmp/toucan_connectors-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toucan_connectors-4.4.1.tar", max compression
+gzip compressed data, was "toucan_connectors-4.5.0.tar", max compression
```

## Comparing `toucan_connectors-4.4.1.tar` & `toucan_connectors-4.5.0.tar`

### file list

```diff
@@ -1,201 +1,181 @@
--rw-r--r--   0        0        0     1510 2023-03-31 07:13:50.239990 toucan_connectors-4.4.1/LICENSE
--rw-r--r--   0        0        0     9980 2023-03-31 07:13:50.239990 toucan_connectors-4.4.1/README.md
--rw-r--r--   0        0        0     6077 2023-03-31 07:13:50.243990 toucan_connectors-4.4.1/pyproject.toml
--rw-r--r--   0        0        0    11576 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/adobe_analytics/__init__.py
--rw-r--r--   0        0        0    13648 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/adobe_analytics/adobe-analytics.png
--rw-r--r--   0        0        0     1740 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
--rw-r--r--   0        0        0    11170 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/aircall/Aircall.svg
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/aircall/__init__.py
--rw-r--r--   0        0        0    13395 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/aircall/aircall_connector.py
--rw-r--r--   0        0        0      431 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/aircall/constants.py
--rw-r--r--   0        0        0      285 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/aircall/doc.md
--rw-r--r--   0        0        0     4191 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/aircall/helpers.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/anaplan/__init__.py
--rw-r--r--   0        0        0     7277 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/anaplan/anaplan.png
--rw-r--r--   0        0        0     7006 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/anaplan/anaplan_connector.py
--rw-r--r--   0        0        0     4623 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/auth.py
--rw-r--r--   0        0        0    61900 2023-03-31 07:13:50.259990 toucan_connectors-4.4.1/toucan_connectors/aws/aws.png
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/awsathena/__init__.py
--rw-r--r--   0        0        0     2524 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/awsathena/athena.png
--rw-r--r--   0        0        0     8476 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/awsathena/awsathena_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/azure_mssql/__init__.py
--rw-r--r--   0        0        0     2404 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/azure_mssql/azure_mssql_connector.py
--rw-r--r--   0        0        0    24249 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/azure_mssql/sql-azure.png
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/clickhouse/__init__.py
--rw-r--r--   0        0        0     1780 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/clickhouse/clickhouse.png
--rw-r--r--   0        0        0     4541 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/clickhouse/clickhouse_connector.py
--rw-r--r--   0        0        0    15750 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/common.py
--rw-r--r--   0        0        0     5549 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/condition_translator.py
--rw-r--r--   0        0        0     8162 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/connection_manager.py
--rw-r--r--   0        0        0     3534 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/databricks/databricks.png
--rw-r--r--   0        0        0     5236 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/databricks/databricks_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/dataiku/__init__.py
--rw-r--r--   0        0        0    10971 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/dataiku/dataiku.png
--rw-r--r--   0        0        0     1100 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/dataiku/dataiku_connector.py
--rwxr-xr-x   0        0        0      235 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/default-logo.png
--rw-r--r--   0        0        0     3331 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/denodo/denodo.png
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/elasticsearch/__init__.py
--rw-r--r--   0        0        0    29549 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/elasticsearch/elasticsearch.png
--rw-r--r--   0        0        0     5118 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/elasticsearch/elasticsearch_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_ads/__init__.py
--rw-r--r--   0        0        0      452 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_ads/doc.md
--rw-r--r--   0        0        0      183 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_ads/enums.py
--rw-r--r--   0        0        0     5283 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_ads/facebook_ads_connector.py
--rw-r--r--   0        0        0    27755 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_ads/facebook_logo.png
--rw-r--r--   0        0        0      126 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_ads/helpers.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_insights/__init__.py
--rw-r--r--   0        0        0    38402 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_insights/facebook-insights.png
--rw-r--r--   0        0        0     3985 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/facebook_insights/facebook_insights_connector.py
--rw-r--r--   0        0        0    13001 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/github/GitHub_Logo.png
--rw-r--r--   0        0        0      412 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/github/doc.md
--rw-r--r--   0        0        0    17081 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/github/github_connector.py
--rw-r--r--   0        0        0    15903 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/github/helpers.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_adwords/__init__.py
--rw-r--r--   0        0        0      469 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_adwords/doc.md
--rw-r--r--   0        0        0    68711 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_adwords/google_adwords.jpg
--rw-r--r--   0        0        0     9049 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_adwords/google_adwords_connector.py
--rw-r--r--   0        0        0      834 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_adwords/helpers.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_analytics/__init__.py
--rw-r--r--   0        0        0     6243 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_analytics/google-analytics.png
--rw-r--r--   0        0        0     6799 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_analytics/google_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.263990 toucan_connectors-4.4.1/toucan_connectors/google_big_query/__init__.py
--rw-r--r--   0        0        0    17667 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_big_query/google-bigquery.png
--rw-r--r--   0        0        0    12428 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_big_query/google_big_query_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_cloud_mysql/__init__.py
--rw-r--r--   0        0        0    24008 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
--rw-r--r--   0        0        0     2488 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
--rw-r--r--   0        0        0     2473 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_credentials.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_my_business/__init__.py
--rw-r--r--   0        0        0     4045 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_my_business/google-my-business.png
--rw-r--r--   0        0        0     3024 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_my_business/google_my_business_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_sheets/__init__.py
--rw-r--r--   0        0        0    14238 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_sheets/google-sheets.png
--rw-r--r--   0        0        0     9062 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_sheets/google_sheets_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_sheets_2/__init__.py
--rw-r--r--   0        0        0      361 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_sheets_2/doc.md
--rw-r--r--   0        0        0     9559 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_spreadsheet/__init__.py
--rw-r--r--   0        0        0    14238 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png
--rw-r--r--   0        0        0     2986 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hive/__init__.py
--rw-r--r--   0        0        0    37138 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hive/hive.png
--rw-r--r--   0        0        0     1707 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hive/hive_connector.py
--rw-r--r--   0        0        0    13342 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hive/indexima.png
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/http_api/__init__.py
--rw-r--r--   0        0        0    19694 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/http_api/http-api.png
--rw-r--r--   0        0        0     7584 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/http_api/http_api_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot/__init__.py
--rw-r--r--   0        0        0      380 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot/doc.md
--rw-r--r--   0        0        0      294 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot/enums.py
--rw-r--r--   0        0        0      173 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot/helpers.py
--rw-r--r--   0        0        0    33203 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot/hubspot.png
--rw-r--r--   0        0        0     5738 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot/hubspot_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot_private_app/__init__.py
--rw-r--r--   0        0        0     5197 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/hubspot_private_app/hubspot_connector.py
--rw-r--r--   0        0        0      140 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/install_scripts/__init__.py
--rwxr-xr-x   0        0        0      726 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/install_scripts/databricks.sh
--rwxr-xr-x   0        0        0      509 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/install_scripts/mssql.sh
--rwxr-xr-x   0        0        0      926 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
--rwxr-xr-x   0        0        0      908 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/install_scripts/odbc.sh
--rwxr-xr-x   0        0        0      706 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/install_scripts/oracle.sh
--rw-r--r--   0        0        0     3285 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/json_wrapper.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/lightspeed/__init__.py
--rw-r--r--   0        0        0    10876 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/lightspeed/lightspeed.png
--rw-r--r--   0        0        0     1142 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/lightspeed/lightspeed_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/linkedinads/__init__.py
--rw-r--r--   0        0        0      365 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/linkedinads/doc.md
--rw-r--r--   0        0        0     9990 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/linkedinads/linkedinads.png
--rw-r--r--   0        0        0     7507 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/linkedinads/linkedinads_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/micro_strategy/__init__.py
--rw-r--r--   0        0        0     1853 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/micro_strategy/client.py
--rw-r--r--   0        0        0     4454 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/micro_strategy/data.py
--rw-r--r--   0        0        0     4664 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/micro_strategy/micro_strategy_connector.py
--rw-r--r--   0        0        0    13133 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/micro_strategy/microstrategy.png
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.267990 toucan_connectors-4.4.1/toucan_connectors/mongo/__init__.py
--rw-r--r--   0        0        0    26880 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mongo/mongo-db.png
--rw-r--r--   0        0        0    17097 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mongo/mongo_connector.py
--rw-r--r--   0        0        0     1822 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mongo/mongo_translator.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mssql/__init__.py
--rw-r--r--   0        0        0    26319 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mssql/mssql.png
--rw-r--r--   0        0        0     4673 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mssql/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mssql_TLSv1_0/__init__.py
--rw-r--r--   0        0        0    26319 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mssql_TLSv1_0/mssql.png
--rw-r--r--   0        0        0     4893 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mysql/__init__.py
--rw-r--r--   0        0        0     3761 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mysql/mysql.png
--rw-r--r--   0        0        0    14522 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/mysql/mysql_connector.py
--rw-r--r--   0        0        0     2401 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/net_explorer/net_explorer.png
--rwxr-xr-x   0        0        0     3537 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/net_explorer/net_explorer_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/oauth2_connector/__init__.py
--rw-r--r--   0        0        0     6029 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/oauth2_connector/oauth2connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/odata/__init__.py
--rw-r--r--   0        0        0    31781 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/odata/odata.png
--rw-r--r--   0        0        0     2048 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/odata/odata_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/odbc/__init__.py
--rw-r--r--   0        0        0     3141 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/odbc/odbc.png
--rw-r--r--   0        0        0     1299 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/odbc/odbc_connector.py
--rw-r--r--   0        0        0    10551 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/one_drive/one_drive.png
--rwxr-xr-x   0        0        0    12312 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/one_drive/one_drive_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/oracle_sql/__init__.py
--rw-r--r--   0        0        0    12887 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/oracle_sql/oracle-sql.png
--rw-r--r--   0        0        0     3375 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/oracle_sql/oracle_sql_connector.py
--rw-r--r--   0        0        0     3948 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/pagination.py
--rw-r--r--   0        0        0     2638 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/pandas_translator.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/peakina/__init__.py
--rw-r--r--   0        0        0     1377 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/peakina/peakina.png
--rw-r--r--   0        0        0      509 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/peakina/peakina_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/postgres/__init__.py
--rw-r--r--   0        0        0    28440 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/postgres/postgres.png
--rw-r--r--   0        0        0    10332 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/postgres/postgresql_connector.py
--rw-r--r--   0        0        0    17824 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/postgres/utils.py
--rw-r--r--   0        0        0     1498 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/query_manager.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/redshift/__init__.py
--rw-r--r--   0        0        0     8867 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/redshift/redshift.png
--rw-r--r--   0        0        0    16447 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/redshift/redshift_database_connector.py
--rw-r--r--   0        0        0     1850 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/redshift/utils.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/revinate/__init__.py
--rw-r--r--   0        0        0      874 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/revinate/helpers.py
--rw-r--r--   0        0        0     2575 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/revinate/revinate.png
--rw-r--r--   0        0        0     4605 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/revinate/revinate_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/rok/__init__.py
--rw-r--r--   0        0        0     5325 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/rok/rok.png
--rw-r--r--   0        0        0     5321 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/rok/rok_connector.py
--rw-r--r--   0        0        0      410 2023-03-31 07:13:50.271990 toucan_connectors-4.4.1/toucan_connectors/salesforce/doc.md
--rw-r--r--   0        0        0   165347 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/salesforce/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/salesforce/salesforce.jpg
--rw-r--r--   0        0        0     7429 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/salesforce/salesforce_connector.py
--rw-r--r--   0        0        0      410 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/salesforce_sandbox/doc.md
--rw-r--r--   0        0        0   165347 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/salesforce_sandbox/salesforce.jpg
--rw-r--r--   0        0        0       84 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/sap_hana/__init__.py
--rw-r--r--   0        0        0    20257 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/sap_hana/sap-hana.png
--rw-r--r--   0        0        0     1264 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/sap_hana/sap_hana_connector.py
--rw-r--r--   0        0        0    20013 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/share_point/share_point.png
--rw-r--r--   0        0        0      143 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/snowflake/__init__.py
--rw-r--r--   0        0        0    15417 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/snowflake/snowflake.png
--rw-r--r--   0        0        0    18251 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/snowflake/snowflake_connector.py
--rw-r--r--   0        0        0    12795 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/snowflake_common.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/snowflake_oauth2/__init__.py
--rw-r--r--   0        0        0    15417 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/snowflake_oauth2/snowflake.png
--rw-r--r--   0        0        0    12246 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/soap/__init__.py
--rw-r--r--   0        0        0      609 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/soap/helpers.py
--rw-r--r--   0        0        0    42145 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/soap/soap.png
--rw-r--r--   0        0        0     4325 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/soap/soap_connector.py
--rw-r--r--   0        0        0     3080 2023-03-31 07:13:50.275990 toucan_connectors-4.4.1/toucan_connectors/sql_query_helper.py
--rw-r--r--   0        0        0    21205 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/toucan_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/toucan_toco/__init__.py
--rwxr-xr-x   0        0        0     4372 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/toucan_toco/toucan.png
--rw-r--r--   0        0        0     1289 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/toucan_toco/toucan_toco_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/trello/__init__.py
--rw-r--r--   0        0        0     3966 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/trello/trello.png
--rw-r--r--   0        0        0     6603 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/trello/trello_connector.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/utils/__init__.py
--rw-r--r--   0        0        0      492 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/utils/datetime.py
--rw-r--r--   0        0        0      629 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/utils/pem.py
--rw-r--r--   0        0        0        0 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/wootric/__init__.py
--rw-r--r--   0        0        0     8734 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/wootric/wootric.png
--rw-r--r--   0        0        0     5228 2023-03-31 07:13:50.279990 toucan_connectors-4.4.1/toucan_connectors/wootric/wootric_connector.py
--rw-r--r--   0        0        0    14957 1970-01-01 00:00:00.000000 toucan_connectors-4.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-04-24 14:57:47.480448 toucan_connectors-4.5.0/LICENSE
+-rw-r--r--   0        0        0     9969 2023-04-24 14:57:47.480448 toucan_connectors-4.5.0/README.md
+-rw-r--r--   0        0        0     5557 2023-04-24 14:57:47.484448 toucan_connectors-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10795 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/__init__.py
+-rw-r--r--   0        0        0    13648 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe-analytics.png
+-rw-r--r--   0        0        0     1740 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/anaplan/__init__.py
+-rw-r--r--   0        0        0     7277 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan.png
+-rw-r--r--   0        0        0     7006 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan_connector.py
+-rw-r--r--   0        0        0     4623 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/auth.py
+-rw-r--r--   0        0        0    61900 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/aws/aws.png
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/awsathena/__init__.py
+-rw-r--r--   0        0        0     2524 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/awsathena/athena.png
+-rw-r--r--   0        0        0     8464 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/awsathena/awsathena_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/azure_mssql/__init__.py
+-rw-r--r--   0        0        0     2404 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/azure_mssql/azure_mssql_connector.py
+-rw-r--r--   0        0        0    24249 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/azure_mssql/sql-azure.png
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1780 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse.png
+-rw-r--r--   0        0        0     4541 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse_connector.py
+-rw-r--r--   0        0        0    15750 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/common.py
+-rw-r--r--   0        0        0     5549 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/condition_translator.py
+-rw-r--r--   0        0        0     8162 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/connection_manager.py
+-rw-r--r--   0        0        0     3534 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/databricks/databricks.png
+-rw-r--r--   0        0        0     5236 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/databricks/databricks_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/dataiku/__init__.py
+-rw-r--r--   0        0        0    10971 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku.png
+-rw-r--r--   0        0        0     1100 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku_connector.py
+-rwxr-xr-x   0        0        0      235 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/default-logo.png
+-rw-r--r--   0        0        0     3331 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/denodo/denodo.png
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    29549 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch.png
+-rw-r--r--   0        0        0     5118 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/__init__.py
+-rw-r--r--   0        0        0      452 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/doc.md
+-rw-r--r--   0        0        0      183 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/enums.py
+-rw-r--r--   0        0        0     5283 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_ads_connector.py
+-rw-r--r--   0        0        0    27755 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_logo.png
+-rw-r--r--   0        0        0      126 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_ads/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_insights/__init__.py
+-rw-r--r--   0        0        0    38402 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook-insights.png
+-rw-r--r--   0        0        0     3985 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook_insights_connector.py
+-rw-r--r--   0        0        0    13001 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/GitHub_Logo.png
+-rw-r--r--   0        0        0      412 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/doc.md
+-rw-r--r--   0        0        0    17081 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/github_connector.py
+-rw-r--r--   0        0        0    15903 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/github/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.496449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/__init__.py
+-rw-r--r--   0        0        0      469 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/doc.md
+-rw-r--r--   0        0        0    68711 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords.jpg
+-rw-r--r--   0        0        0     9049 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords_connector.py
+-rw-r--r--   0        0        0      834 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_adwords/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_analytics/__init__.py
+-rw-r--r--   0        0        0     6243 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_analytics/google-analytics.png
+-rw-r--r--   0        0        0     6799 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_analytics/google_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_big_query/__init__.py
+-rw-r--r--   0        0        0    17667 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_big_query/google-bigquery.png
+-rw-r--r--   0        0        0    12920 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_big_query/google_big_query_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/__init__.py
+-rw-r--r--   0        0        0    24008 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
+-rw-r--r--   0        0        0     2488 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
+-rw-r--r--   0        0        0     2473 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_credentials.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_my_business/__init__.py
+-rw-r--r--   0        0        0     4045 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_my_business/google-my-business.png
+-rw-r--r--   0        0        0     3024 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_my_business/google_my_business_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets/__init__.py
+-rw-r--r--   0        0        0    14238 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets/google-sheets.png
+-rw-r--r--   0        0        0     9062 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets/google_sheets_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/__init__.py
+-rw-r--r--   0        0        0      361 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/doc.md
+-rw-r--r--   0        0        0     9559 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/__init__.py
+-rw-r--r--   0        0        0    14238 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png
+-rw-r--r--   0        0        0     2986 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/http_api/__init__.py
+-rw-r--r--   0        0        0    19694 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/http_api/http-api.png
+-rw-r--r--   0        0        0     7584 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/http_api/http_api_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/doc.md
+-rw-r--r--   0        0        0      294 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/enums.py
+-rw-r--r--   0        0        0      173 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/helpers.py
+-rw-r--r--   0        0        0    33203 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot.png
+-rw-r--r--   0        0        0     5738 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot_private_app/__init__.py
+-rw-r--r--   0        0        0     5197 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/hubspot_private_app/hubspot_connector.py
+-rw-r--r--   0        0        0      140 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/__init__.py
+-rwxr-xr-x   0        0        0      726 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/databricks.sh
+-rwxr-xr-x   0        0        0      509 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/mssql.sh
+-rwxr-xr-x   0        0        0      926 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
+-rwxr-xr-x   0        0        0      908 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/odbc.sh
+-rwxr-xr-x   0        0        0      706 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/install_scripts/oracle.sh
+-rw-r--r--   0        0        0     3285 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/json_wrapper.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/__init__.py
+-rw-r--r--   0        0        0      365 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/doc.md
+-rw-r--r--   0        0        0     9990 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads.png
+-rw-r--r--   0        0        0     7544 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/__init__.py
+-rw-r--r--   0        0        0     1853 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/client.py
+-rw-r--r--   0        0        0     4454 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/data.py
+-rw-r--r--   0        0        0     4664 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/micro_strategy_connector.py
+-rw-r--r--   0        0        0    13133 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/micro_strategy/microstrategy.png
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/__init__.py
+-rw-r--r--   0        0        0    26880 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/mongo-db.png
+-rw-r--r--   0        0        0    17097 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_connector.py
+-rw-r--r--   0        0        0     1822 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_translator.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql/__init__.py
+-rw-r--r--   0        0        0    26319 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql/mssql.png
+-rw-r--r--   0        0        0     4673 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/__init__.py
+-rw-r--r--   0        0        0    26319 2023-04-24 14:57:47.500449 toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql.png
+-rw-r--r--   0        0        0     4893 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mysql/__init__.py
+-rw-r--r--   0        0        0     3761 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mysql/mysql.png
+-rw-r--r--   0        0        0    14657 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/mysql/mysql_connector.py
+-rw-r--r--   0        0        0     2401 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer.png
+-rwxr-xr-x   0        0        0     3537 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oauth2_connector/__init__.py
+-rw-r--r--   0        0        0     6029 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oauth2_connector/oauth2connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odata/__init__.py
+-rw-r--r--   0        0        0    31781 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odata/odata.png
+-rw-r--r--   0        0        0     2048 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odata/odata_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odbc/__init__.py
+-rw-r--r--   0        0        0     3141 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odbc/odbc.png
+-rw-r--r--   0        0        0     1299 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/odbc/odbc_connector.py
+-rw-r--r--   0        0        0    10551 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive.png
+-rwxr-xr-x   0        0        0    12312 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oracle_sql/__init__.py
+-rw-r--r--   0        0        0    12887 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle-sql.png
+-rw-r--r--   0        0        0     3375 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle_sql_connector.py
+-rw-r--r--   0        0        0     3948 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/pagination.py
+-rw-r--r--   0        0        0     2638 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/pandas_translator.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/peakina/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/peakina/peakina.png
+-rw-r--r--   0        0        0      509 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/peakina/peakina_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/__init__.py
+-rw-r--r--   0        0        0    28440 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/postgres.png
+-rw-r--r--   0        0        0    10400 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/postgresql_connector.py
+-rw-r--r--   0        0        0    17824 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/postgres/utils.py
+-rw-r--r--   0        0        0     1498 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/query_manager.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/__init__.py
+-rw-r--r--   0        0        0     8867 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/redshift.png
+-rw-r--r--   0        0        0    16551 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/redshift_database_connector.py
+-rw-r--r--   0        0        0     1850 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/redshift/utils.py
+-rw-r--r--   0        0        0      410 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/doc.md
+-rw-r--r--   0        0        0   165347 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce.jpg
+-rw-r--r--   0        0        0     7429 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce_connector.py
+-rw-r--r--   0        0        0      410 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/doc.md
+-rw-r--r--   0        0        0   165347 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce.jpg
+-rw-r--r--   0        0        0       84 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/sap_hana/__init__.py
+-rw-r--r--   0        0        0    20257 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap-hana.png
+-rw-r--r--   0        0        0     1264 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap_hana_connector.py
+-rw-r--r--   0        0        0    20013 2023-04-24 14:57:47.504449 toucan_connectors-4.5.0/toucan_connectors/share_point/share_point.png
+-rw-r--r--   0        0        0      143 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake/__init__.py
+-rw-r--r--   0        0        0    15417 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake.png
+-rw-r--r--   0        0        0    18251 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake_connector.py
+-rw-r--r--   0        0        0    12795 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_common.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/__init__.py
+-rw-r--r--   0        0        0    15417 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake.png
+-rw-r--r--   0        0        0    12246 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/__init__.py
+-rw-r--r--   0        0        0      609 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/helpers.py
+-rw-r--r--   0        0        0    42145 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/soap.png
+-rw-r--r--   0        0        0     4325 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/soap/soap_connector.py
+-rw-r--r--   0        0        0     3080 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/sql_query_helper.py
+-rw-r--r--   0        0        0    21205 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_toco/__init__.py
+-rwxr-xr-x   0        0        0     4372 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan.png
+-rw-r--r--   0        0        0     1289 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan_toco_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/trello/__init__.py
+-rw-r--r--   0        0        0     3966 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/trello/trello.png
+-rw-r--r--   0        0        0     6603 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/trello/trello_connector.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/utils/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/utils/datetime.py
+-rw-r--r--   0        0        0      629 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/utils/pem.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/wootric/__init__.py
+-rw-r--r--   0        0        0     8734 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/wootric/wootric.png
+-rw-r--r--   0        0        0     5228 2023-04-24 14:57:47.508449 toucan_connectors-4.5.0/toucan_connectors/wootric/wootric_connector.py
+-rw-r--r--   0        0        0    14576 1970-01-01 00:00:00.000000 toucan_connectors-4.5.0/PKG-INFO
```

### Comparing `toucan_connectors-4.4.1/LICENSE` & `toucan_connectors-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/README.md` & `toucan_connectors-4.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -103,30 +103,30 @@
 make test
 ```
 
 Some connectors are tested using mocks (cf. `trello`), others are tested by making calls to data providers (cf. `elasticsearch`) running on the system in docker containers. The required images are in the `tests/docker-compose.yml` file, they need to be pulled (cf. `pytest --pull`) to run the relevant tests.
 
 ## Contributing
 
-This is an open source repository under the [BSD 3-Clause Licence](https://github.com/ToucanToco/toucan-connectors/blob/master/LICENSE). The Toucan Toco tech team are the maintainers of this repository, we welcome contributions. 
+This is an open source repository under the [BSD 3-Clause Licence](https://github.com/ToucanToco/toucan-connectors/blob/master/LICENSE). The Toucan Toco tech team are the maintainers of this repository, we welcome contributions.
 
 At the moment the main use of this code is its integration into Toucan Toco commercially licenced software, as a result our dev and maintenance efforts applied here are mostly driven by Toucan Toco internal priorities.
 
 The starting point of a contribution should be an [Issue](https://github.com/ToucanToco/toucan-connectors/issues), either one you create or an existing one. This allows us (maintainers) to discuss the contribution before it is produced and avoids back and forth in reviews or stalled pull requests.
 
 ### Step 1: Generate base classes and tests files
 
 To generate the connector and test modules from boilerplate, run:
 
 ```
 make new_connector type=mytype
 ```
 
 `mytype` should be the name of a system we would like to build a connector for,
-such as `MySQL` or `Hive` or `Magento`.
+such as `MySQL` or `Magento`.
 
 Open the folder in `tests` for the new connector. You can start writing your tests before implementing it.
 
 Some connectors are tested with calls to the actual data systems that they target,
 for example `elasticsearch`, `mongo`, `mssql`.
 
 Others are tested with mocks of the
```

### Comparing `toucan_connectors-4.4.1/pyproject.toml` & `toucan_connectors-4.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,139 +7,128 @@
 profile = "black"
 include_trailing_comma = true
 line_length = 100
 multi_line_output = 3
 
 [tool.poetry]
 name = "toucan-connectors"
-version = "4.4.1"
+version = "4.5.0"
 description = "Toucan Toco Connectors"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 license = "BSD"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-# <3.11 required by awswrangler < 3.0
-# https://github.com/aws/aws-sdk-pandas/issues/1714
-# https://github.com/aws/aws-sdk-pandas/pull/1992
 python = ">=3.10,<3.12"
 Authlib = "^1.0.1"
-# FIXME: Bump to ^3.8.4 and remove the marker once we have awswrangler >=3.0
-aiohttp = { version = "^3.8.1", python = "<3.11" }
 cached-property = "^1.5.2"
 Jinja2 = "^3.0.3"
 jq = "^1.2.2"
 pydantic = "^1.9.1"
 requests = "^2.28.0"
 tenacity = "^8.0.1"
-toucan-data-sdk = "^7.4.2"
+toucan-data-sdk = "^7.6.0"
 
 # Dependencies for extras
 adobe-analytics = {version = "^1.2.3", optional = true}
 bearer = {version = "3.1.0", optional = true}
 oauthlib = {version = "3.2.2", optional = true}
 requests-oauthlib = {version = "1.3.1", optional = true}
-# FIXME: Remove the marker once we're in >=3.0
-awswrangler = {version = "^2.15.1", optional = true, python = "<3.11"}
+awswrangler = {version = "^3.0.0", optional = true}
 pyodbc = {version = "^4", optional = true}
 clickhouse-driver = {version = ">=0.2.3,<1.0", optional = true}
 dataiku-api-client = {version = "^9.0.1", optional = true}
 elasticsearch = {version = ">=7.11.0,<8", optional = true}
 facebook-sdk = {version = "^3.1.0", optional = true}
 python-graphql-client = {version = ">=0.4.3,<1.0", optional = true}
 google-api-python-client = {version = "^2", optional = true}
 oauth2client = {version = "^4.1.3", optional = true}
 googleads = {version = ">=32,<34", optional = true}
 google-cloud-bigquery = {version = ">=3,<4", extras = ["bqstorage", "pandas"], optional = true}
 PyMySQL = {version = "^1.0.2", optional = true}
 gspread = {version = "^5.4.0", optional = true}
-PyHive = {extras = ["hive"], version = ">=0.6.5,<1.0", optional = true}
 xmltodict = {version = ">=0.13.0,<1.0", optional = true}
 pymongo = {version = ">=3.12.0", optional = true}
 tctc-odata = {version = ">=0.3,<1.0", optional = true}
 cx-Oracle = {version = "^8.3.0", optional = true}
 openpyxl = {version = "^3.0.9", optional = true}
 psycopg2 = {version = "^2.7.4", optional = true}
 redshift-connector = {version = "^2.0.907", optional = true}
 lxml = {version = "^4.6.5", optional = true}
 PyJWT = {version = ">=1.5.3,<3", optional = true}
 simplejson = {version = "^3.17.6", optional = true}
 pyhdb = {version = ">=0.3.4,<1.0", optional = true}
 zeep = {version = "^4.1.0", optional = true}
 snowflake-connector-python = {version = ">=2.7.12,<4.0.0", optional = true}
-pyarrow = {version = "<11", optional = true}
+pyarrow = {version = "<12", optional = true}
 toucan-client = {version = "^1.0.1", optional = true}
-peakina = {version = "^0.10.0", optional = true}
+peakina = {version = "^0.11.0", optional = true}
 hubspot-api-client = {version = "^7.4.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 Authlib = "^1.0.1"
 aioresponses = ">=0.7.3,<1.0"
 black = "^22.12.0"
 click = "^8.1.3"
-cryptography = "<39"
+cryptography = ">=40.0.2"
 docker = "^6.0.1"
 flake8 = "^6.0.0"
 flake8-quotes = "^3.3.2"
 isort = "^5.12.0"
-mock = "^5.0.1"
+mock = "^5.0.2"
 pytest-aiohttp = "^1.0.4"
 pytest-asyncio = ">=0.19.0,<1"
 pytest-cov = "^4.0.0"
 pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
 pytest-rerunfailures = "^11.1"
-python-slugify = "<6"
+python-slugify = "<7"
 PyYAML = "<6"
 responses = ">=0.21.0,<1"
 psycopg2 = "^2.9.3"
 xmltodict = ">=0.13.0,<1"
 python-graphql-client = ">=0.4.3,<1"
 clickhouse-driver = ">=0.2.3,<1"
 lxml = "4.9.1"
 zeep = "^4.1.0"
-mypy = "^1.0"
-pandas-stubs = "^1.5.3.230304"
-types-requests = "^2.28.11.15"
-types-simplejson = "^3.18.0.1"
-types-python-slugify = "^8.0.0.1"
-types-pyopenssl = "^23.0.0.4"
+mypy = "^1.2"
+pandas-stubs = "^2.0.0.230412"
+types-requests = "^2.28.11.17"
+types-simplejson = "^3.19.0.0"
+types-python-slugify = "^8.0.0.2"
+types-pyopenssl = "^23.1.0.2"
 
 [tool.poetry.extras]
 adobe = ["adobe-analytics"]
-aircall = ["bearer"]
 awsathena = ["awswrangler"]
 azure_mssql = ["pyodbc"]
 clickhouse = ["clickhouse-driver"]
 dataiku = ["dataiku-api-client"]
 elasticsearch = ["elasticsearch"]
 facebook = ["facebook-sdk"]
 github = ["python-graphql-client"]
 google_analytics = ["google-api-python-client", "oauth2client"]
 google_adwords = ["google-adwords"]
 google_big_query = ["google-cloud-bigquery"]
 google_cloud_mysql = ["PyMySQL"]
 google_my_business = ["google-api-python-client"]
 google_sheets = ["google-api-python-client"]
 google_spreadsheet = ["gspread", "oauth2client"]
-hive = ["PyHive"]
 http_api = ["oauthlib", "requests-oauthlib", "xmltodict"]
 hubspot = ["hubspot-api-client"]
-lightspeed = ["bearer"]
 mongo = ["pymongo"]
 mssql = ["pyodbc"]
 mssql_TLSv1_0 = ["pyodbc"]
 mysql = ["PyMySQL"]
 odata = ["oauthlib", "requests-oauthlib", "tctc_odata"]
 odbc = ["pydobc"]
 oracle_sql = ["cx_Oracle"]
 net_explorer = ["openpyxl"]
 postgres = ["psycopg2"]
 Redshift = ["redshift_connector", "lxml"]
-ROK = ["requests", "PyJWT", "simplejson"]
 sap_hana = ["pyhdb"]
 soap = ["zeep", "lxml"]
 snowflake = ["snowflake-connector-python", "PyJWT", "pyarrow"]
 toucan_toco = ["toucan_client"]
 
 # All
 all = [
@@ -160,15 +149,14 @@
     "oauth2client",
     "oauthlib",
     "openpyxl",
     "peakina",
     "psycopg2",
     "pyarrow",
     "pyhdb",
-    "PyHive",
     "PyJWT",
     "pymongo",
     "PyMySQL",
     "pyodbc",
     "python-graphql-client",
     "redshift-connector",
     "requests-oauthlib",
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/__init__.py` & `toucan_connectors-4.5.0/toucan_connectors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 
 CONNECTORS_REGISTRY = {
     'AdobeAnalytics': {
         'connector': 'adobe_analytics.adobe_analytics_connector.AdobeAnalyticsConnector',
         'label': 'Adobe Analytics',
         'logo': 'adobe_analytics/adobe-analytics.png',
     },
-    'Aircall': {
-        'connector': 'aircall.aircall_connector.AircallConnector',
-        'logo': 'aircall/Aircall.svg',
-    },
     'Anaplan': {
         'connector': 'anaplan.anaplan_connector.AnaplanConnector',
         'label': 'Anaplan',
         'logo': 'anaplan/anaplan.png',
     },
     'AWSAthena': {
         'connector': 'awsathena.awsathena_connector.AwsathenaConnector',
@@ -119,18 +115,14 @@
         'logo': 'google_sheets/google-sheets.png',
     },
     'GoogleSpreadsheet': {
         'connector': 'google_spreadsheet.google_spreadsheet_connector.GoogleSpreadsheetConnector',
         'label': 'Google Spreadsheet',
         'logo': 'google_spreadsheet/google-spreadsheet.png',
     },
-    'Hive': {
-        'connector': 'hive.hive_connector.HiveConnector',
-        'logo': 'hive/hive.png',
-    },
     'HttpAPI': {
         'connector': 'http_api.http_api_connector.HttpAPIConnector',
         'label': 'Http API',
         'logo': 'http_api/http-api.png',
     },
     'Hubspot': {
         'connector': 'hubspot.hubspot_connector.HubspotConnector',
@@ -138,22 +130,14 @@
         'logo': 'hubspot/hubspot.png',
     },
     'HubspotPrivateApp': {
         'connector': 'hubspot_private_app.hubspot_connector.HubspotConnector',
         'label': 'Hubspot (Private App)',
         'logo': 'hubspot/hubspot.png',
     },
-    'Indexima': {
-        'connector': 'hive.hive_connector.HiveConnector',
-        'logo': 'hive/indexima.png',
-    },
-    'Lightspeed': {
-        'connector': 'lightspeed.lightspeed_connector.LightspeedConnector',
-        'logo': 'lightspeed/lightspeed.png',
-    },
     'LinkedinAds': {
         'connector': 'linkedinads.linkedinads_connector.LinkedinadsConnector',
         'logo': 'linkedinads/linkedinads.png',
     },
     'MicroStrategy': {
         'connector': 'micro_strategy.micro_strategy_connector.MicroStrategyConnector',
         'logo': 'micro_strategy/microstrategy.png',
@@ -209,23 +193,14 @@
         'logo': 'postgres/postgres.png',
     },
     'Redshift': {
         'connector': 'redshift.redshift_database_connector.RedshiftConnector',
         'label': 'Redshift',
         'logo': 'redshift/redshift.png',
     },
-    'Revinate': {
-        'connector': 'revinate.revinate_connector.RevinateConnector',
-        'label': 'Revinate',
-        'logo': 'revinate/revinate.png',
-    },
-    'ROK': {
-        'connector': 'rok.rok_connector.RokConnector',
-        'logo': 'rok/rok.png',
-    },
     'Salesforce': {
         'connector': 'salesforce.salesforce_connector.SalesforceConnector',
         'label': 'Salesforce Service Cloud (SFSC)',
         'logo': 'salesforce/salesforce-service-cloud.png',
     },
     'SalesforceSandbox': {
         'connector': 'salesforce_sandbox.salesforce_sandbox_connector.SalesforceConnector',
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/adobe_analytics/adobe-analytics.png` & `toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/aircall/aircall_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/github/github_connector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,189 +1,109 @@
 import asyncio
 import logging
 import os
-import time
+from contextlib import suppress
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import List, Optional
 
+import numpy as np
 import pandas as pd
-from aiohttp import ClientSession
-from pydantic import Field, PrivateAttr
+import requests
+from dateutil import relativedelta
+from pydantic import Field, PrivateAttr, create_model
+from python_graphql_client import GraphqlClient
 
 from toucan_connectors.common import ConnectorStatus, get_loop
 from toucan_connectors.oauth2_connector.oauth2connector import (
     OAuth2Connector,
     OAuth2ConnectorConfig,
 )
 from toucan_connectors.toucan_connector import (
     ConnectorSecretsForm,
     DataSlice,
     ToucanConnector,
     ToucanDataSource,
+    strlist_to_enum,
 )
 
-from .constants import MAX_RUNS, PER_PAGE
-from .helpers import DICTIONARY_OF_FORMATTERS, build_df, build_empty_df
+from .helpers import (
+    GithubError,
+    KeyNotFoundException,
+    RateLimitExhaustedException,
+    dataset_formatter,
+    extraction_funcs_names,
+    extraction_funcs_pages_1,
+    extraction_funcs_pages_2,
+    extraction_keys,
+    format_functions,
+    get_cursor,
+    get_data,
+    get_errors,
+    get_message,
+    get_nodes,
+    get_organization,
+    get_page_info,
+    get_rate_limit_info,
+    has_next_page,
+    queries_funcs_names,
+    queries_funcs_pages,
+)
 
-AUTHORIZATION_URL: str = 'https://dashboard-v2.aircall.io/oauth/authorize'
-SCOPE: str = 'public_api'
-TOKEN_URL: str = 'https://api.aircall.io/v1/oauth/token'
-BASE_ROUTE: str = 'https://api.aircall.io/v1'
+AUTHORIZATION_URL: str = 'https://github.com/login/oauth/authorize'
+SCOPE: str = 'user repo read:org read:discussion'
+TOKEN_URL: str = 'https://github.com/login/oauth/access_token'
+BASE_ROUTE: str = 'https://api.github.com/graphql'
+BASE_ROUTE_REST: str = 'https://api.github.com/'
 NO_CREDENTIALS_ERROR = 'No credentials'
-
-
-class AircallRateLimitExhaustedException(Exception):
-    """Raised when the extraction reached the max amount of request"""
+extraction_start_date = datetime.strftime(
+    datetime.now() - relativedelta.relativedelta(years=1), '%Y-%m-%dT%H:%M:%SZ'
+)
 
 
 class NoCredentialsError(Exception):
-    """Raised when no secrets avaiable."""
-
-
-class AircallDataset(str, Enum):
-    calls = 'calls'
-    tags = 'tags'
-    users = 'users'
-
-
-async def fetch_page(
-    dataset: str,
-    data_list: List[dict],
-    session: ClientSession,
-    limit,
-    current_pass: int,
-    new_page=1,
-    delay_counter=0,
-    *,
-    query_params=None,
-) -> List[dict]:
-    """
-    Fetches data from AirCall API
-
-    dependent on existence of other pages and call limit
-    """
-    endpoint = f'{BASE_ROUTE}/{dataset}?per_page={PER_PAGE}&page={new_page}'
-    try:
-        if query_params:
-            data: dict = await fetch(endpoint, session, query_params)
-        else:
-            data: dict = await fetch(endpoint, session)
-
-        logging.getLogger(__name__).info(
-            f'Request sent to Aircall for page {new_page} for dataset {dataset}'
-        )
-
-        aircall_error = data.get('error')
-        if aircall_error:
-            logging.getLogger(__name__).error(f'Aircall error has occurred: {aircall_error}')
-            delay_timer = 1
-            max_num_of_retries = 3
-            await asyncio.sleep(delay_timer)
-            if delay_counter < max_num_of_retries:
-                delay_counter += 1
-                logging.getLogger(__name__).info('Retrying Aircall API')
-                data_list = await fetch_page(
-                    dataset,
-                    data_list,
-                    session,
-                    limit,
-                    current_pass,
-                    new_page,
-                    delay_counter,
-                    query_params=query_params,
-                )
-            else:
-                logging.getLogger(__name__).error('Aborting Aircall requests')
-                raise AircallException(f'Aborting Aircall requests due to {aircall_error}')
+    """Raised when no secrets available."""
 
-        delay_counter = 0
-        data_list.append(data)
 
-        next_page_link = None
-        meta_data = data.get('meta')
-        if meta_data is not None:
-            next_page_link: Optional[str] = meta_data.get('next_page_link')
-
-        if limit > -1:
-            current_pass += 1
-
-            if next_page_link is not None and current_pass < limit:
-                next_page = meta_data['current_page'] + 1
-                data_list = await fetch_page(
-                    dataset,
-                    data_list,
-                    session,
-                    limit,
-                    current_pass,
-                    next_page,
-                    query_params=query_params,
-                )
-        else:
-            if next_page_link is not None:
-                next_page = meta_data['current_page'] + 1
-                data_list = await fetch_page(
-                    dataset,
-                    data_list,
-                    session,
-                    limit,
-                    current_pass,
-                    next_page,
-                    query_params=query_params,
-                )
-
-    except AircallRateLimitExhaustedException as a:
-        reset_timestamp = int(a.args[0])
-        delay = reset_timestamp - (int(datetime.timestamp(datetime.utcnow())) + 1)
-        logging.getLogger(__name__).info(f'Rate limit reached, pausing {delay} seconds')
-        time.sleep(delay)
-        logging.getLogger(__name__).info('Extraction restarted')
-        data_list = await fetch_page(
-            dataset,
-            data_list,
-            session,
-            limit,
-            current_pass,
-            new_page,
-            delay_counter,
-            query_params=query_params,
-        )
-
-    return data_list
+class GithubDataSet(str, Enum):
+    pull_requests = 'pull requests'
+    teams = 'teams'
+
+
+class GithubDataSource(ToucanDataSource):
+    dataset: GithubDataSet = GithubDataSet('teams')
+    organization: Optional[str] = Field(
+        None, title='Organization', description='The organization to extract the data from'
+    )
+    page_limit: int = Field(10, description='Limit of entries (default is 10 pages)', ge=0)
+    entities_limit: int = Field(
+        None,
+        title='Entities Limit',
+        description='Max Number of entities such as teams and repositories to extract',
+    )
+    _oauth_trigger = 'instance'
+    oauth2_version = Field('1', **{'ui.hidden': True})
 
+    @classmethod
+    def get_form(cls, connector: 'GithubConnector', current_config, **kwargs):
+        """Retrieve a form filled with suggestions of available organizations."""
+        # Always add the suggestions for the available organizations
+        constraints = {}
+        with suppress(Exception):
+            available_organizations = connector.get_organizations()
+            constraints['organization'] = strlist_to_enum('organization', available_organizations)
+        return create_model('FormSchema', **constraints, __base__=cls).schema()
 
-async def fetch(new_endpoint, session: ClientSession, query_params=None) -> dict:
-    """The basic fetch function"""
-    async with session.get(new_endpoint, params=query_params) as res:
-        try:
-            rate_limit_reset = res.headers['X-AircallApi-Reset']
-            raise AircallRateLimitExhaustedException(rate_limit_reset)
-        except KeyError:
-            pass
-        return await res.json()
-
-
-class AircallDataSource(ToucanDataSource):
-    limit: int = Field(MAX_RUNS, description='Limit of entries (default is 1 run)', ge=-1)
-    dataset: AircallDataset = 'calls'
-
-
-class AircallConnector(ToucanConnector):
-    """
-    This is a connector for [Aircall](https://developer.aircall.io/api-references/#endpoints)
-    using oAuth2 for authentication
-    """
 
+class GithubConnector(ToucanConnector):
     _auth_flow = 'oauth2'
-    provided_token: Optional[str]
     auth_flow_id: Optional[str]
-    data_source_model: AircallDataSource
+    data_source_model: GithubDataSource
     _oauth_trigger = 'instance'
-    oauth2_version = Field('1', **{'ui.hidden': True})
     _oauth2_connector: OAuth2Connector = PrivateAttr()
 
     @staticmethod
     def get_connector_secrets_form() -> ConnectorSecretsForm:
         return ConnectorSecretsForm(
             documentation_md=(Path(os.path.dirname(__file__)) / 'doc.md').read_text(),
             secrets_schema=OAuth2ConnectorConfig.schema(),
@@ -201,176 +121,331 @@
             secrets_keeper=kwargs['secrets_keeper'],
             redirect_uri=kwargs['redirect_uri'],
             config=OAuth2ConnectorConfig(
                 client_id=kwargs['client_id'],
                 client_secret=kwargs['client_secret'],
             ),
         )
-        self.provided_token = kwargs.get('provided_token', None)
 
     def build_authorization_url(self, **kwargs):
         return self._oauth2_connector.build_authorization_url(**kwargs)
 
+    def get_organizations(self):
+        """Retrieve a list of organizations available to the connector"""
+
+        access_token = self.get_access_token()
+
+        if not access_token:
+            raise NoCredentialsError('No credentials')
+
+        headers = {'Authorization': f'Bearer {access_token}'}
+        logging.getLogger(__name__).info('Retrieving organization')
+        data = requests.get(f'{BASE_ROUTE_REST}user/orgs', headers=headers).json()
+        return [str(x['login']) for x in data]
+
     def retrieve_tokens(self, authorization_response: str):
         """
-        In the Aircall oAuth2 authentication process, client_id & client_secret
+        In the Github's oAuth2 authentication process, client_id & client_secret
         must be sent in the body of the request so we have to set them in
         the mother class. This way they'll be added to her get_access_token method
         """
         return self._oauth2_connector.retrieve_tokens(authorization_response)
 
     def get_access_token(self):
-        if self.provided_token:
-            return self.provided_token
         return self._oauth2_connector.get_access_token()
 
-    async def _fetch(self, url, headers=None, query_params=None):
-        """Build the final request along with headers."""
-        async with ClientSession(headers=headers) as session:
-            return await fetch(url, session, query_params=query_params)
+    def get_names(
+        self,
+        client: GraphqlClient,
+        organization: str,
+        dataset: str,
+        names=None,
+        variables=None,
+    ) -> list:
+        """
+        Retrieve either repositories names or teams names
+        :param client an authenticated python_graphql_client
+        :param organization the organization from which team names will be extracted
+        :param dataset a GithubDataset the function will retrieve
+        :param names a list receiving the names extracted from API
+        :variables a dict receiving pagination info
 
-    def _run_fetch(self, url):
-        """Run loop."""
-        access_token = self.get_access_token()
-        if not access_token:
-            raise NoCredentialsError(NO_CREDENTIALS_ERROR)
-        headers = {'Authorization': f'Bearer {access_token}'}
+        return: a list of repositories or teams names
+        """
+        if names is None:
+            names = []
+        if variables is None:
+            variables = {}
+        q = queries_funcs_names[dataset](organization=organization)
+        data = client.execute(query=q, variables=variables)
 
-        loop = get_loop()
-        future = asyncio.ensure_future(self._fetch(url, headers))
-        return loop.run_until_complete(future)
+        try:
+            get_errors(data)
+            get_message(data)
 
-    async def _get_data(
-        self, dataset: str, limit, query_params=None
-    ) -> Tuple[List[dict], List[dict]]:
-        """Triggers fetches for data and does preliminary filtering process"""
-        access_token = self.get_access_token()
-        if not access_token:
-            raise NoCredentialsError(NO_CREDENTIALS_ERROR)
-        headers = {'Authorization': f'Bearer {access_token}'}
+            extracted_data = extraction_funcs_names[dataset](get_organization(get_data(data)))
+            page_info = get_page_info(extracted_data)
+            names.extend([t[extraction_keys[dataset]] for t in get_nodes(extracted_data)])
+
+            if has_next_page(page_info):
+                variables['cursor'] = get_cursor(page_info)
+                self.get_names(
+                    client, organization, names=names, variables=variables, dataset=dataset
+                )
+        except (GithubError, KeyNotFoundException) as g:
+            logging.getLogger(__name__).error(f'Aborting query due to {g}')
 
-        async with ClientSession(headers=headers) as session:
-            team_data, variable_data = await asyncio.gather(
-                fetch_page(
-                    'teams',
-                    [],
-                    session,
-                    limit,
-                    0,
-                    query_params=None,  # for now we don't provide param while querying the teams endpoint
-                ),
-                fetch_page(dataset, [], session, limit, 0, query_params=query_params),
-            )
-            team_response_list = []
-            variable_response_list = []
-            if len(team_data) > 0:
-                for data in team_data:
-                    for team_obj in data['teams']:
-                        team_response_list += DICTIONARY_OF_FORMATTERS['teams'](team_obj)
-            if len(variable_data) > 0:
-                for data in variable_data:
-                    variable_response_list += [
-                        DICTIONARY_OF_FORMATTERS.get(dataset, 'users')(obj) for obj in data[dataset]
-                    ]
-            return team_response_list, variable_response_list
+        return names
 
-    async def _get_tags(self, dataset: str, limit) -> List[dict]:
-        """Triggers fetches for tags and does preliminary filtering process"""
-        access_token = self.get_access_token()
-        if not access_token:
-            raise NoCredentialsError(NO_CREDENTIALS_ERROR)
-        headers = {'Authorization': f'Bearer {access_token}'}
+    async def get_pages(
+        self,
+        name: str,
+        client: GraphqlClient,
+        organization: str,
+        dataset: str,
+        page_limit: int,
+        variables=None,
+        data_list=None,
+        retrieved_pages=0,
+        retries=0,
+        retry_limit=2,
+        latest_retrieved_object=None,
+    ) -> List[dict]:
+        """
+        Extracts pages of either members or pull requests
+        :param name a str representing the repo name
+        :param client an authenticated python_graphql_client
+        :param organization a str representing the organization
+        :param dataset a GithubDataset the connector will have to retrieve
+        :param: variables dict to store pagination information
+        :param: data_list list to store extracted pull requests data
+        :param: page_limit pages limit of the extraction
+        :param: retrieved_pages int number of pages retrieved
+        :param: retries the number of retries done when we got an error
+        :param: retry_limit the max number of retries the connector can do
+        :param: latest_retrieved_object str of either the latest user name or pull request name retrieved
+        in a previous extraction. This will allow to call get_pages to extract only new object (users or pr)
+        since the last extraction
+        :return: list of extracted data
+        """
+        if variables is None:
+            variables = {}
+        if data_list is None:
+            data_list = []
+        q = queries_funcs_pages[dataset](organization=organization, name=name)
+        await asyncio.sleep(0.200)
+        data = await client.execute_async(query=q, variables=variables)
 
-        async with ClientSession(headers=headers) as session:
-            raw_data = await fetch_page(
-                dataset,
-                [],
-                session,
-                limit,
-                1,
+        try:
+            get_message(data)
+            get_errors(data)
+            data_value = get_data(data)
+            extracted_data = extraction_funcs_pages_1[dataset](
+                extraction_funcs_pages_2[dataset](get_organization(data_value))
             )
-            tags_data_list = []
-            for data in raw_data:
-                tags_data_list += data['tags']
-            return tags_data_list
+            page_info = get_page_info(extracted_data)
+            formatted_data = format_functions[dataset](extracted_data, name)
 
-    def run_fetches(self, dataset, limit, query_params=None) -> Tuple[List[dict], List[dict]]:
-        """sets up event loop and fetches for 'calls' and 'users' datasets"""
-        loop = get_loop()
-        future = asyncio.ensure_future(self._get_data(dataset, limit, query_params))
-        return loop.run_until_complete(future)
+            # Check if the extraction script can see a previously extracted object (e.g PR)
+            # in current page
 
-    def run_fetches_for_tags(self, dataset, limit):
-        """sets up event loop and fetches for 'tags' dataset"""
-        loop = get_loop()
-        future = asyncio.ensure_future(self._get_tags(dataset, limit))
-        return loop.run_until_complete(future)
+            if latest_retrieved_object and dataset == GithubDataSet('pull requests'):
+                # check if latest_retrieved_object is in current page
 
-    def _retrieve_data(self, data_source: AircallDataSource, query_params=None) -> pd.DataFrame:
-        """retrieves data from AirCall API"""
-        dataset = data_source.dataset
-        empty_df = build_empty_df(dataset)
+                try:
+                    index = [pr['PR Name'] for pr in formatted_data].index(latest_retrieved_object)
+                    formatted_data = formatted_data[:index]
+                    data_list.extend(formatted_data)
+                    return data_list
+                except ValueError:
+                    pass
+
+            # For now we want to retrieve only max 1 year of Pull requests
+            # TODO change this to be able to receive a extraction_start_date date for extraction as a parameter
+            if dataset == GithubDataSet('pull requests'):
+                try:
+                    # Find the first index where PR Creation Date is < extraction_start_date
+                    # Throws IndexError if such index cannot be found
+                    index = np.where(
+                        np.array([pr['PR Creation Date'] for pr in formatted_data])
+                        < extraction_start_date
+                    )[0][0]
+                    formatted_data = formatted_data[:index]
+                    data_list.extend(formatted_data)
+                    return data_list
+                except (IndexError, TypeError):
+                    pass
 
-        # NOTE: no check needed on limit here because a non-valid limit
-        # raises a Pydantic ValidationError
-        limit = data_source.limit
-
-        if dataset == 'tags':
-            non_empty_df = pd.DataFrame([])
-            if limit != 0:
-                res = self.run_fetches_for_tags(dataset, limit)
-                non_empty_df = pd.DataFrame(res)
-            return pd.concat([empty_df, non_empty_df])
-        else:
-            team_data = pd.DataFrame([])
-            variable_data = pd.DataFrame([])
-            if limit != 0:
-                team_data, variable_data = self.run_fetches(dataset, limit, query_params)
+            if dataset == GithubDataSet('pull requests'):
+                data_list.extend(formatted_data)
+            else:
+                data_list.append(formatted_data)
+
+            if has_next_page(page_info) and retrieved_pages < page_limit:
+                retrieved_pages += 1
+                variables['cursor'] = get_cursor(page_info)
+                get_rate_limit_info(data_value)
+
+                await self.get_pages(
+                    name=name,
+                    client=client,
+                    organization=organization,
+                    dataset=dataset,
+                    variables=variables,
+                    data_list=data_list,
+                    retrieved_pages=retrieved_pages,
+                    page_limit=page_limit,
+                    latest_retrieved_object=latest_retrieved_object,
+                )
+
+        except GithubError:
+            logging.getLogger(__name__).info('Retrying in 15 seconds')
+            await asyncio.sleep(15)
+            retries += 1
+            if retries <= retry_limit:
+                await self.get_pages(
+                    name=name,
+                    client=client,
+                    organization=organization,
+                    dataset=dataset,
+                    variables=variables,
+                    data_list=data_list,
+                    retrieved_pages=retrieved_pages,
+                    retries=retries,
+                    page_limit=page_limit,
+                    retry_limit=retry_limit,
+                    latest_retrieved_object=latest_retrieved_object,
+                )
+            else:
+                raise GithubError('Max number of retries reached, aborting connection')
+
+        except KeyNotFoundException as k:
+            logging.getLogger(__name__).error(f'{k}')
 
-            return build_df(
-                dataset, [empty_df, pd.DataFrame(team_data), pd.DataFrame(variable_data)]
+        except RateLimitExhaustedException as r:
+            sleep_time = r.args[0]  # Value to wait is sent within the Exception
+            logging.getLogger(__name__).info(f'Pausing until reset, waiting {sleep_time}')
+            await asyncio.sleep(sleep_time)
+            await self.get_pages(
+                name=name,
+                client=client,
+                organization=organization,
+                dataset=dataset,
+                variables=variables,
+                data_list=data_list,
+                retrieved_pages=retrieved_pages,
+                retries=retries,
+                page_limit=page_limit,
+                retry_limit=retry_limit,
+                latest_retrieved_object=latest_retrieved_object,
             )
 
-    def get_status(self) -> ConnectorStatus:
+        return data_list
+
+    async def _fetch_data(
+        self,
+        dataset: GithubDataSet,
+        organization: str,
+        client: GraphqlClient,
+        page_limit: int,
+        names_limit=None,
+        latest_retrieved_object=None,
+    ) -> pd.DataFrame:
         """
-        Test the Aircall connexion.
+         Builds the coroutines ran by _retrieve_data
+        :param dataset  GithubDataSet, the GithubDataSet to query
+        :param organization a str representing the organization from
+        which the data will be extracted
+        :param client a GraphqlClient that will make the requests to Github's API
+        :param page_limit max number of pages to be retrieved by get_pages
+        :param names_limit number max of "names" (teams/repos) to extract the data from
+        :param latest_retrieved_object a dict with object as key and entity as value e. g {'repo': 'plop', 'pr: stuff'}
+        :return: a Pandas DataFrame of pull requests or team memberships
         """
-        try:
-            access_token = self.get_access_token()
-            if access_token:
-                return ConnectorStatus(status=True)
-        except Exception:
-            return ConnectorStatus(status=False, error='Credentials are missing')
+        logging.getLogger(__name__).info(f'Starting fetch for {dataset}')
+        names = self.get_names(client=client, organization=organization, dataset=dataset)
+        subtasks = [
+            self.get_pages(
+                name=name,
+                client=client,
+                dataset=dataset,
+                organization=organization,
+                page_limit=page_limit,
+                latest_retrieved_object=latest_retrieved_object.get(name)
+                if latest_retrieved_object
+                else None,
+            )
+            for name in names[:names_limit]
+        ]
+        unformatted_data = await asyncio.gather(*subtasks)
+        return dataset_formatter[dataset]([e for sublist in unformatted_data for e in sublist])
+
+    def _retrieve_data(self, data_source: GithubDataSource) -> pd.DataFrame:
+        """
+
+        :param data_source:  GithubDataSource, the GithubDataSource to query
+        :return: a Pandas DataFrame of pull requests or team memberships
+        """
+        dataset = data_source.dataset
+        access_token = self.get_access_token()
+        organization = data_source.organization
+
         if not access_token:
-            return ConnectorStatus(status=False, error='Credentials are missing')
+            raise NoCredentialsError(NO_CREDENTIALS_ERROR)
+
+        headers = {'Authorization': f'token {access_token}'}
+        client = GraphqlClient(BASE_ROUTE, headers)
+        loop = get_loop()
+        return loop.run_until_complete(
+            self._fetch_data(
+                dataset=dataset,
+                organization=organization,
+                client=client,
+                page_limit=data_source.page_limit,
+                names_limit=data_source.entities_limit,
+            )
+        )
 
     def get_slice(
         self,
-        data_source: AircallDataSource,
+        data_source: GithubDataSource,
         permissions: Optional[dict] = None,
         offset: int = 0,
         limit: Optional[int] = None,
         get_row_count: Optional[bool] = False,
     ) -> DataSlice:
         """
         Method to retrieve a part of the data as a pandas dataframe
         and the total size filtered with permissions
 
         - offset is the index of the starting row
         - limit is the number of pages to retrieve
         Exemple: if offset = 5 and limit = 10 then 10 results are expected from 6th row
         """
-        preview_datasource = AircallDataSource(
-            limit=1,
+        preview_datasource = GithubDataSource(
+            page_limit=1,
             dataset=data_source.dataset,
             domain=f'preview_{data_source.domain}',
             name=data_source.name,
+            organization=data_source.organization,
+            entities_limit=3,
         )
         df = self.get_df(preview_datasource, permissions)
         if limit is not None:
             return DataSlice(df[offset : offset + limit], len(df))
         else:
             return DataSlice(df[offset:], len(df))
 
-
-class AircallException(Exception):
-    """Raised when an error occured when querying Aircall's API"""
+    def get_status(self) -> ConnectorStatus:
+        """
+        Test the Github's connexion.
+        :return: a ConnectorStatus with the current status
+        """
+        try:
+            access_token = self.get_access_token()
+            if access_token:
+                c = ConnectorStatus(status=True)
+                return c
+            else:
+                return ConnectorStatus(status=False)
+        except Exception:
+            return ConnectorStatus(status=False, error='Credentials are missing')
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/anaplan/anaplan.png` & `toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/anaplan/anaplan_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/anaplan/anaplan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/auth.py` & `toucan_connectors-4.5.0/toucan_connectors/auth.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/aws/aws.png` & `toucan_connectors-4.5.0/toucan_connectors/aws/aws.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/awsathena/athena.png` & `toucan_connectors-4.5.0/toucan_connectors/awsathena/athena.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/awsathena/awsathena_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/awsathena/awsathena_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,18 +106,14 @@
             return f'SELECT * FROM ({cls._strip_trailing_semicolumn(query)}) LIMIT {limit};'
         return query
 
     @cached_property_with_ttl(ttl=10)
     def available_dbs(self) -> list[str]:
         return self._list_db_names()
 
-    @cached_property_with_ttl(ttl=60)
-    def project_tree(self) -> list[TableInfo]:
-        return self._get_project_structure()
-
     def _retrieve_data(
         self,
         data_source: AwsathenaDataSource,
         offset: int = 0,
         limit: Optional[int] = None,
     ) -> pd.DataFrame:
         df = wr.athena.read_sql_query(
@@ -135,18 +131,19 @@
         return df
 
     def _list_db_names(self) -> list[str]:
         return wr.catalog.databases(
             boto3_session=self.get_session(),
         )['Database'].values
 
-    def _get_project_structure(self) -> list[TableInfo]:
+    def _get_project_structure(self, db_name: str | None = None) -> list[TableInfo]:
         table_list: list[TableInfo] = []
+        available_dbs = self.available_dbs if db_name is None else [db_name]
         session = self.get_session()
-        for db in self.available_dbs:
+        for db in available_dbs:
             tables = wr.catalog.tables(boto3_session=session, database=db)[
                 ['Table', 'TableType']
             ].to_dict(orient='records')
             for table_object in tables:
                 if 'temp_table' not in table_object['Table']:
                     columns = wr.catalog.get_table_types(
                         boto3_session=session, database=db, table=table_object['Table']
@@ -217,8 +214,8 @@
                     status=False,
                     details=[(c, False) for c in checks],
                     error=f'Cannot verify connection to Athena: {exc}, {sts_exc}',
                 )
 
     def get_model(self, db_name: str | None = None) -> list[TableInfo]:
         """Retrieves the database tree structure using current session"""
-        return self.project_tree
+        return self._get_project_structure(db_name)
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/azure_mssql/azure_mssql_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/azure_mssql/azure_mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/azure_mssql/sql-azure.png` & `toucan_connectors-4.5.0/toucan_connectors/azure_mssql/sql-azure.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/clickhouse/clickhouse.png` & `toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/clickhouse/clickhouse_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/clickhouse/clickhouse_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/common.py` & `toucan_connectors-4.5.0/toucan_connectors/common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/condition_translator.py` & `toucan_connectors-4.5.0/toucan_connectors/condition_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/connection_manager.py` & `toucan_connectors-4.5.0/toucan_connectors/connection_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/databricks/databricks.png` & `toucan_connectors-4.5.0/toucan_connectors/databricks/databricks.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/databricks/databricks_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/databricks/databricks_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/dataiku/dataiku.png` & `toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/dataiku/dataiku_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/dataiku/dataiku_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/denodo/denodo.png` & `toucan_connectors-4.5.0/toucan_connectors/denodo/denodo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/elasticsearch/elasticsearch.png` & `toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/elasticsearch/elasticsearch_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/elasticsearch/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/facebook_ads/facebook_ads_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_ads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/facebook_ads/facebook_logo.png` & `toucan_connectors-4.5.0/toucan_connectors/facebook_ads/facebook_logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/facebook_insights/facebook-insights.png` & `toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook-insights.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/facebook_insights/facebook_insights_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/facebook_insights/facebook_insights_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/github/GitHub_Logo.png` & `toucan_connectors-4.5.0/toucan_connectors/github/GitHub_Logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/github/github_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/mysql/mysql_connector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,451 +1,373 @@
-import asyncio
-import logging
 import os
-from contextlib import suppress
-from datetime import datetime
 from enum import Enum
-from pathlib import Path
-from typing import List, Optional
+from itertools import groupby as groupby
+from tempfile import NamedTemporaryFile
+from typing import Any, Generator, Optional
 
-import numpy as np
 import pandas as pd
-import requests
-from dateutil import relativedelta
-from pydantic import Field, PrivateAttr, create_model
-from python_graphql_client import GraphqlClient
-
-from toucan_connectors.common import ConnectorStatus, get_loop
-from toucan_connectors.oauth2_connector.oauth2connector import (
-    OAuth2Connector,
-    OAuth2ConnectorConfig,
-)
+import pymysql
+from cached_property import cached_property_with_ttl
+from pydantic import Field, SecretStr, constr, create_model, validator
+from pymysql.constants import CR, ER
+
+from toucan_connectors.common import ConnectorStatus, pandas_read_sql
 from toucan_connectors.toucan_connector import (
-    ConnectorSecretsForm,
-    DataSlice,
+    DiscoverableConnector,
+    TableInfo,
     ToucanConnector,
     ToucanDataSource,
+    UnavailableVersion,
+    VersionableEngineConnector,
     strlist_to_enum,
 )
+from toucan_connectors.utils.pem import sanitize_spaces_pem
 
-from .helpers import (
-    GithubError,
-    KeyNotFoundException,
-    RateLimitExhaustedException,
-    dataset_formatter,
-    extraction_funcs_names,
-    extraction_funcs_pages_1,
-    extraction_funcs_pages_2,
-    extraction_keys,
-    format_functions,
-    get_cursor,
-    get_data,
-    get_errors,
-    get_message,
-    get_nodes,
-    get_organization,
-    get_page_info,
-    get_rate_limit_info,
-    has_next_page,
-    queries_funcs_names,
-    queries_funcs_pages,
-)
-
-AUTHORIZATION_URL: str = 'https://github.com/login/oauth/authorize'
-SCOPE: str = 'user repo read:org read:discussion'
-TOKEN_URL: str = 'https://github.com/login/oauth/access_token'
-BASE_ROUTE: str = 'https://api.github.com/graphql'
-BASE_ROUTE_REST: str = 'https://api.github.com/'
-NO_CREDENTIALS_ERROR = 'No credentials'
-extraction_start_date = datetime.strftime(
-    datetime.now() - relativedelta.relativedelta(years=1), '%Y-%m-%dT%H:%M:%SZ'
-)
 
+def handle_date_0(df: pd.DataFrame) -> pd.DataFrame:
+    # Mysql driver doesnt translate date '0000-00-00 00:00:00'
+    # to a datetime, so the Series has a 'object' dtype instead of 'datetime'.
+    # This util fixes this behaviour, by replacing it with NaT.
+    return df.replace({'0000-00-00 00:00:00': pd.NaT}).infer_objects()
 
-class NoCredentialsError(Exception):
-    """Raised when no secrets available."""
 
+class NoQuerySpecified(Exception):
+    def __init__(self) -> None:
+        super().__init__('no query was specified')
 
-class GithubDataSet(str, Enum):
-    pull_requests = 'pull requests'
-    teams = 'teams'
 
+class MySQLDataSource(ToucanDataSource):
+    """
+    Either `query` or `table` are required, both at the same time are not supported.
+    """
 
-class GithubDataSource(ToucanDataSource):
-    dataset: GithubDataSet = GithubDataSet('teams')
-    organization: Optional[str] = Field(
-        None, title='Organization', description='The organization to extract the data from'
+    database: str = Field(..., description='The name of the database you want to query')
+    follow_relations: bool | None = Field(
+        None,
+        **{'ui.hidden': True},
+        description='Deprecated, kept for compatibility purpose with old data sources configs',
+    )  # Deprecated
+    table: str = Field(
+        None, **{'ui.hidden': True}
+    )  # To avoid previous config migrations, won't be used
+    query: constr(min_length=1) = Field(
+        None,
+        description='You can write a custom query against your '
+        'database here. It will take precedence over '
+        'the "table" parameter',
+        widget='sql',
     )
-    page_limit: int = Field(10, description='Limit of entries (default is 10 pages)', ge=0)
-    entities_limit: int = Field(
+    query_object: dict = Field(
         None,
-        title='Entities Limit',
-        description='Max Number of entities such as teams and repositories to extract',
+        description='An object describing a simple select query' 'This field is used internally',
+        **{'ui.hidden': True},
     )
-    _oauth_trigger = 'instance'
-    oauth2_version = Field('1', **{'ui.hidden': True})
+    language: str = Field('sql', **{'ui.hidden': True})
 
     @classmethod
-    def get_form(cls, connector: 'GithubConnector', current_config, **kwargs):
-        """Retrieve a form filled with suggestions of available organizations."""
-        # Always add the suggestions for the available organizations
-        constraints = {}
-        with suppress(Exception):
-            available_organizations = connector.get_organizations()
-            constraints['organization'] = strlist_to_enum('organization', available_organizations)
-        return create_model('FormSchema', **constraints, __base__=cls).schema()
-
-
-class GithubConnector(ToucanConnector):
-    _auth_flow = 'oauth2'
-    auth_flow_id: Optional[str]
-    data_source_model: GithubDataSource
-    _oauth_trigger = 'instance'
-    _oauth2_connector: OAuth2Connector = PrivateAttr()
+    def get_form(cls, connector: 'MySQLConnector', current_config: dict[str, Any]) -> dict:
+        return create_model(
+            'FormSchema',
+            database=strlist_to_enum('database', connector.available_dbs),
+            __base__=cls,
+        ).schema()
+
+
+_DATABASE_MODEL_EXTRACTION_QUERY = (
+    # table_schema is selected twice because the frontend components needs it but
+    # mysql provides it only for compliance with the SQL-92 standard.
+    # https://dba.stackexchange.com/questions/3774/what-is-the-point-of-the-table-catalog-column-in-information-schema-tables
+    "SELECT t.table_schema AS 'database', t.table_schema AS 'schema', "
+    # Table type and name
+    "CASE WHEN t.table_type = 'BASE TABLE' THEN 'table' ELSE LOWER(t.table_type) END AS table_type, t.table_name, "
+    # Columns from the columns table
+    'c.column_name, c.data_type FROM information_schema.tables t INNER JOIN information_schema.columns c '
+    # Inner join on table name
+    'ON t.table_name = c.table_name '
+    # Filtering on concrete tables/views
+    "WHERE t.table_type in ('BASE TABLE', 'VIEW') AND t.table_schema NOT IN ('mysql', 'information_schema', 'performance_schema', 'sys') "
+)
 
-    @staticmethod
-    def get_connector_secrets_form() -> ConnectorSecretsForm:
-        return ConnectorSecretsForm(
-            documentation_md=(Path(os.path.dirname(__file__)) / 'doc.md').read_text(),
-            secrets_schema=OAuth2ConnectorConfig.schema(),
-        )
-
-    def __init__(self, **kwargs):
-        super().__init__(
-            **{k: v for k, v in kwargs.items() if k not in OAuth2Connector.init_params}
-        )
-        self._oauth2_connector = OAuth2Connector(
-            auth_flow_id=self.auth_flow_id,
-            authorization_url=AUTHORIZATION_URL,
-            scope=SCOPE,
-            token_url=TOKEN_URL,
-            secrets_keeper=kwargs['secrets_keeper'],
-            redirect_uri=kwargs['redirect_uri'],
-            config=OAuth2ConnectorConfig(
-                client_id=kwargs['client_id'],
-                client_secret=kwargs['client_secret'],
-            ),
-        )
-
-    def build_authorization_url(self, **kwargs):
-        return self._oauth2_connector.build_authorization_url(**kwargs)
-
-    def get_organizations(self):
-        """Retrieve a list of organizations available to the connector"""
-
-        access_token = self.get_access_token()
-
-        if not access_token:
-            raise NoCredentialsError('No credentials')
-
-        headers = {'Authorization': f'Bearer {access_token}'}
-        logging.getLogger(__name__).info('Retrieving organization')
-        data = requests.get(f'{BASE_ROUTE_REST}user/orgs', headers=headers).json()
-        return [str(x['login']) for x in data]
 
-    def retrieve_tokens(self, authorization_response: str):
-        """
-        In the Github's oAuth2 authentication process, client_id & client_secret
-        must be sent in the body of the request so we have to set them in
-        the mother class. This way they'll be added to her get_access_token method
-        """
-        return self._oauth2_connector.retrieve_tokens(authorization_response)
+class SSLMode(str, Enum):
+    VERIFY_IDENTITY = 'VERIFY_IDENTITY'
+    VERIFY_CA = 'VERIFY_CA'
+    REQUIRED = 'REQUIRED'
+
+
+class MySQLConnector(ToucanConnector, DiscoverableConnector, VersionableEngineConnector):
+    """
+    Import data from MySQL database.
+    """
+
+    data_source_model: MySQLDataSource
+
+    host: str = Field(
+        ...,
+        description='The domain name (preferred option as more dynamic) or '
+        'the hardcoded IP address of your database server',
+    )
+    port: int = Field(None, description='The listening port of your database server')
+    user: str = Field(..., description='Your login username')
+    password: SecretStr = Field(None, description='Your login password')
+    charset: str = Field(
+        'utf8mb4',
+        title='Charset',
+        description='Character encoding. You should generally let the default "utf8mb4" here.',
+    )
+    connect_timeout: int = Field(
+        None,
+        title='Connection timeout',
+        description='You can set a connection timeout in seconds here, '
+        'i.e. the maximum length of time you want to wait '
+        'for the server to respond. None by default',
+    )
+    # SSL options
+    ssl_ca: SecretStr = Field(
+        None,
+        description='The CA certificate content in PEM format to use to connect to the MySQL '
+        'server. Equivalent of the --ssl-ca option of the MySQL client',
+    )
+    ssl_cert: SecretStr = Field(
+        None,
+        description='The X509 certificate content in PEM format to use to connect to the MySQL '
+        'server. Equivalent of the --ssl-cert option of the MySQL client',
+    )
+    ssl_key: SecretStr = Field(
+        None,
+        description='The X509 certificate key content in PEM format to use to connect to the MySQL '
+        'server. Equivalent of the --ssl-key option of the MySQL client',
+    )
+    ssl_mode: SSLMode = Field(
+        None,
+        description='SSL Mode to use to connect to the MySQL server. '
+        'Equivalent of the --ssl-mode option of the MySQL client. Must be set in order to use SSL',
+    )
 
-    def get_access_token(self):
-        return self._oauth2_connector.get_access_token()
+    class Config:
+        underscore_attrs_are_private = True
+        keep_untouched = (cached_property_with_ttl,)
 
-    def get_names(
-        self,
-        client: GraphqlClient,
-        organization: str,
-        dataset: str,
-        names=None,
-        variables=None,
-    ) -> list:
-        """
-        Retrieve either repositories names or teams names
-        :param client an authenticated python_graphql_client
-        :param organization the organization from which team names will be extracted
-        :param dataset a GithubDataset the function will retrieve
-        :param names a list receiving the names extracted from API
-        :variables a dict receiving pagination info
+    @validator('ssl_key')
+    @classmethod
+    def ssl_key_validator(cls, ssl_key: str, values: dict) -> str:
+        ssl_cert = values.get('ssl_cert', None)
+        # if one is present, the other one should be specified
+        if ssl_cert is not None and ssl_key is None:
+            raise ValueError('SSL option "ssl_key" should be specified if "ssl_cert" is provided !')
+        elif ssl_key is not None and ssl_cert is None:
+            raise ValueError('SSL option "ssl_cert" should be specified if "ssl_key" is provided !')
+
+        return ssl_key
+
+    def _sanitize_ssl_params(self) -> dict[str, Any]:
+        params = {}
+        if self.ssl_mode in (SSLMode.VERIFY_CA, SSLMode.VERIFY_IDENTITY):
+
+            for ssl_opt in ('ssl_ca', 'ssl_key', 'ssl_cert'):
+                opt = getattr(self, ssl_opt)
+                if opt is None:
+                    continue
+                secret = opt.get_secret_value()
+                if secret.strip() != '':
+                    params[ssl_opt] = sanitize_spaces_pem(secret)
+        return params
+
+    def _list_db_names(self) -> list[str]:
+        connection = self._connect(cursorclass=None, database=None)
+        # Always add the suggestions for the available databases
+        with connection.cursor() as cursor:
+            cursor.execute('SHOW DATABASES;')
+            res = cursor.fetchall()
+            return [
+                db_name
+                for (db_name,) in res
+                if db_name not in ('information_schema', 'mysql', 'performance_schema')
+            ]
+
+    def _get_project_structure(
+        self, db_name: str | None = None
+    ) -> Generator[TableInfo, None, None]:
+        connection = self._connect(cursorclass=None, database=db_name)
+
+        extraction_query = _DATABASE_MODEL_EXTRACTION_QUERY
+        if db_name:
+            # If the db name is specified, filter on it
+            extraction_query += f"AND t.table_schema = '{db_name}'"
+        extraction_query += ';'
+
+        with connection.cursor() as cursor:
+            cursor.execute(extraction_query)
+            results = cursor.fetchall()
+
+        column_names = ('database', 'schema', 'table_type', 'table_name', 'columns')
+        # Grouping by DB name, schema name, Table type, Table name
+        for group, grouper in groupby(sorted(results), key=lambda x: x[:4]):
+            col_info = [{'name': x[4], 'type': x[5]} for x in grouper]
+            yield dict(zip(column_names, group + (col_info,)))
+
+    @cached_property_with_ttl(ttl=10)
+    def available_dbs(self) -> list[str]:
+        return self._list_db_names()
+
+    def project_tree(self, db_name: str | None = None) -> list[TableInfo]:
+        return list(self._get_project_structure(db_name=db_name))
+
+    def get_connection_params(
+        self, *, database: str | None = None, cursorclass=pymysql.cursors.DictCursor
+    ):
+        conv = pymysql.converters.conversions.copy()
+        conv[246] = float
+        con_params = {
+            'host': self.host,
+            'user': self.user,
+            'password': self.password.get_secret_value() if self.password else None,
+            'port': self.port,
+            'database': database,
+            'charset': self.charset,
+            'connect_timeout': self.connect_timeout,
+            'conv': conv,
+            'cursorclass': cursorclass,
+        }
+        # remove None values
+        return {k: v for k, v in con_params.items() if v is not None}
+
+    def _connect(
+        self, *, database: str | None = None, cursorclass=pymysql.cursors.DictCursor
+    ) -> pymysql.Connection:
+        connection_params = self.get_connection_params(database=database, cursorclass=cursorclass)
+        if self.ssl_mode is not None:
+            connection_params |= {
+                'ssl_disabled': False,
+                # Verify the server's certificate. This one is actually required by pymysql, as no
+                # SSL context will be created otherwise:
+                # https://github.com/PyMySQL/PyMySQL/blob/main/pymysql/connections.py#L266
+                'ssl_verify_cert': True,
+            }
+
+        if self.ssl_mode in (SSLMode.VERIFY_CA, SSLMode.VERIFY_IDENTITY):
+            ssl_params = self._sanitize_ssl_params()
+            ssl_files = []
+            for ssl_opt in ('ssl_ca', 'ssl_key', 'ssl_cert'):
+                if ssl_opt in ssl_params:
+                    ssl_opt_file = NamedTemporaryFile(prefix=ssl_opt, delete=False)
+                    ssl_opt_file.write(ssl_params[ssl_opt].encode())
+                    ssl_opt_file.seek(0)
+
+                    connection_params[ssl_opt] = ssl_opt_file.name
+                    ssl_files.append(ssl_opt_file)
+
+            connection_params['ssl_verify_identity'] = self.ssl_mode == SSLMode.VERIFY_IDENTITY
+
+            try:
+                connection = pymysql.connect(**connection_params)
+            finally:
+                for ssl_file in ssl_files:
+                    ssl_file.close()
+                    os.unlink(ssl_file.name)  # needed otherwise file is not closed.
+            return connection
+        return pymysql.connect(**connection_params)
 
-        return: a list of repositories or teams names
-        """
-        if names is None:
-            names = []
-        if variables is None:
-            variables = {}
-        q = queries_funcs_names[dataset](organization=organization)
-        data = client.execute(query=q, variables=variables)
+    @staticmethod
+    def _get_details(index: int, status: Optional[bool]):
+        checks = ['Hostname resolved', 'Port opened', 'Host connection', 'Authenticated']
+        ok_checks = [(c, True) for i, c in enumerate(checks) if i < index]
+        new_check = (checks[index], status)
+        not_validated_checks = [(c, None) for i, c in enumerate(checks) if i > index]
+        return ok_checks + [new_check] + not_validated_checks
 
+    def get_status(self) -> ConnectorStatus:
+        # Check hostname
         try:
-            get_errors(data)
-            get_message(data)
-
-            extracted_data = extraction_funcs_names[dataset](get_organization(get_data(data)))
-            page_info = get_page_info(extracted_data)
-            names.extend([t[extraction_keys[dataset]] for t in get_nodes(extracted_data)])
-
-            if has_next_page(page_info):
-                variables['cursor'] = get_cursor(page_info)
-                self.get_names(
-                    client, organization, names=names, variables=variables, dataset=dataset
-                )
-        except (GithubError, KeyNotFoundException) as g:
-            logging.getLogger(__name__).error(f'Aborting query due to {g}')
-
-        return names
+            self.check_hostname(self.host)
+        except Exception as e:
+            return ConnectorStatus(status=False, details=self._get_details(0, False), error=str(e))
 
-    async def get_pages(
-        self,
-        name: str,
-        client: GraphqlClient,
-        organization: str,
-        dataset: str,
-        page_limit: int,
-        variables=None,
-        data_list=None,
-        retrieved_pages=0,
-        retries=0,
-        retry_limit=2,
-        latest_retrieved_object=None,
-    ) -> List[dict]:
-        """
-        Extracts pages of either members or pull requests
-        :param name a str representing the repo name
-        :param client an authenticated python_graphql_client
-        :param organization a str representing the organization
-        :param dataset a GithubDataset the connector will have to retrieve
-        :param: variables dict to store pagination information
-        :param: data_list list to store extracted pull requests data
-        :param: page_limit pages limit of the extraction
-        :param: retrieved_pages int number of pages retrieved
-        :param: retries the number of retries done when we got an error
-        :param: retry_limit the max number of retries the connector can do
-        :param: latest_retrieved_object str of either the latest user name or pull request name retrieved
-        in a previous extraction. This will allow to call get_pages to extract only new object (users or pr)
-        since the last extraction
-        :return: list of extracted data
-        """
-        if variables is None:
-            variables = {}
-        if data_list is None:
-            data_list = []
-        q = queries_funcs_pages[dataset](organization=organization, name=name)
-        await asyncio.sleep(0.200)
-        data = await client.execute_async(query=q, variables=variables)
+        # Check port
+        try:
+            self.check_port(self.host, self.port)
+        except Exception as e:
+            return ConnectorStatus(status=False, details=self._get_details(1, False), error=str(e))
 
+        # Check basic access
         try:
-            get_message(data)
-            get_errors(data)
-            data_value = get_data(data)
-            extracted_data = extraction_funcs_pages_1[dataset](
-                extraction_funcs_pages_2[dataset](get_organization(data_value))
-            )
-            page_info = get_page_info(extracted_data)
-            formatted_data = format_functions[dataset](extracted_data, name)
-
-            # Check if the extraction script can see a previously extracted object (e.g PR)
-            # in current page
-
-            if latest_retrieved_object and dataset == GithubDataSet('pull requests'):
-                # check if latest_retrieved_object is in current page
-
-                try:
-                    index = [pr['PR Name'] for pr in formatted_data].index(latest_retrieved_object)
-                    formatted_data = formatted_data[:index]
-                    data_list.extend(formatted_data)
-                    return data_list
-                except ValueError:
-                    pass
-
-            # For now we want to retrieve only max 1 year of Pull requests
-            # TODO change this to be able to receive a extraction_start_date date for extraction as a parameter
-            if dataset == GithubDataSet('pull requests'):
-                try:
-                    # Find the first index where PR Creation Date is < extraction_start_date
-                    # Throws IndexError if such index cannot be found
-                    index = np.where(
-                        np.array([pr['PR Creation Date'] for pr in formatted_data])
-                        < extraction_start_date
-                    )[0][0]
-                    formatted_data = formatted_data[:index]
-                    data_list.extend(formatted_data)
-                    return data_list
-                except (IndexError, TypeError):
-                    pass
-
-            if dataset == GithubDataSet('pull requests'):
-                data_list.extend(formatted_data)
-            else:
-                data_list.append(formatted_data)
-
-            if has_next_page(page_info) and retrieved_pages < page_limit:
-                retrieved_pages += 1
-                variables['cursor'] = get_cursor(page_info)
-                get_rate_limit_info(data_value)
-
-                await self.get_pages(
-                    name=name,
-                    client=client,
-                    organization=organization,
-                    dataset=dataset,
-                    variables=variables,
-                    data_list=data_list,
-                    retrieved_pages=retrieved_pages,
-                    page_limit=page_limit,
-                    latest_retrieved_object=latest_retrieved_object,
+            self._connect()
+        except pymysql.err.OperationalError as e:
+            error_code = e.args[0]
+
+            # Can't connect to full URI
+            if error_code == CR.CR_CONN_HOST_ERROR:
+                return ConnectorStatus(
+                    status=False, details=self._get_details(2, False), error=e.args[1]
                 )
 
-        except GithubError:
-            logging.getLogger(__name__).info('Retrying in 15 seconds')
-            await asyncio.sleep(15)
-            retries += 1
-            if retries <= retry_limit:
-                await self.get_pages(
-                    name=name,
-                    client=client,
-                    organization=organization,
-                    dataset=dataset,
-                    variables=variables,
-                    data_list=data_list,
-                    retrieved_pages=retrieved_pages,
-                    retries=retries,
-                    page_limit=page_limit,
-                    retry_limit=retry_limit,
-                    latest_retrieved_object=latest_retrieved_object,
+            # Wrong user/password
+            if error_code == ER.ACCESS_DENIED_ERROR:
+                return ConnectorStatus(
+                    status=False, details=self._get_details(3, False), error=e.args[1]
                 )
-            else:
-                raise GithubError('Max number of retries reached, aborting connection')
 
-        except KeyNotFoundException as k:
-            logging.getLogger(__name__).error(f'{k}')
+        return ConnectorStatus(status=True, details=self._get_details(3, True), error=None)
+
+    def get_model(self, db_name: str | None = None) -> list[Any]:
+        """Retrieves the database tree structure using current connection"""
+        return DiscoverableConnector.format_db_model(self.project_tree(db_name=db_name))
 
-        except RateLimitExhaustedException as r:
-            sleep_time = r.args[0]  # Value to wait is sent within the Exception
-            logging.getLogger(__name__).info(f'Pausing until reset, waiting {sleep_time}')
-            await asyncio.sleep(sleep_time)
-            await self.get_pages(
-                name=name,
-                client=client,
-                organization=organization,
-                dataset=dataset,
-                variables=variables,
-                data_list=data_list,
-                retrieved_pages=retrieved_pages,
-                retries=retries,
-                page_limit=page_limit,
-                retry_limit=retry_limit,
-                latest_retrieved_object=latest_retrieved_object,
-            )
-
-        return data_list
-
-    async def _fetch_data(
-        self,
-        dataset: GithubDataSet,
-        organization: str,
-        client: GraphqlClient,
-        page_limit: int,
-        names_limit=None,
-        latest_retrieved_object=None,
-    ) -> pd.DataFrame:
+    @staticmethod
+    def decode_df(df):
         """
-         Builds the coroutines ran by _retrieve_data
-        :param dataset  GithubDataSet, the GithubDataSet to query
-        :param organization a str representing the organization from
-        which the data will be extracted
-        :param client a GraphqlClient that will make the requests to Github's API
-        :param page_limit max number of pages to be retrieved by get_pages
-        :param names_limit number max of "names" (teams/repos) to extract the data from
-        :param latest_retrieved_object a dict with object as key and entity as value e. g {'repo': 'plop', 'pr: stuff'}
-        :return: a Pandas DataFrame of pull requests or team memberships
+        Used to change bytes columns to string columns
+        (can be moved to be applied for all connectors if needed)
+        It retrieves all the string columns and converts them all together.
+        The string columns become nan columns so we remove them from the result,
+        we keep the rest and insert it back to the dataframe
         """
-        logging.getLogger(__name__).info(f'Starting fetch for {dataset}')
-        names = self.get_names(client=client, organization=organization, dataset=dataset)
-        subtasks = [
-            self.get_pages(
-                name=name,
-                client=client,
-                dataset=dataset,
-                organization=organization,
-                page_limit=page_limit,
-                latest_retrieved_object=latest_retrieved_object.get(name)
-                if latest_retrieved_object
-                else None,
-            )
-            for name in names[:names_limit]
-        ]
-        unformatted_data = await asyncio.gather(*subtasks)
-        return dataset_formatter[dataset]([e for sublist in unformatted_data for e in sublist])
+        str_df = df.select_dtypes([object])
+        if str_df.empty:
+            return df
 
-    def _retrieve_data(self, data_source: GithubDataSource) -> pd.DataFrame:
-        """
+        str_df = str_df.stack().str.decode('utf8').unstack().dropna(axis=1, how='all')
+        for col in str_df.columns:
+            df[col] = str_df[col]
+        return df
 
-        :param data_source:  GithubDataSource, the GithubDataSource to query
-        :return: a Pandas DataFrame of pull requests or team memberships
+    def _retrieve_data(self, datasource):
         """
-        dataset = data_source.dataset
-        access_token = self.get_access_token()
-        organization = data_source.organization
-
-        if not access_token:
-            raise NoCredentialsError(NO_CREDENTIALS_ERROR)
-
-        headers = {'Authorization': f'token {access_token}'}
-        client = GraphqlClient(BASE_ROUTE, headers)
-        loop = get_loop()
-        return loop.run_until_complete(
-            self._fetch_data(
-                dataset=dataset,
-                organization=organization,
-                client=client,
-                page_limit=data_source.page_limit,
-                names_limit=data_source.entities_limit,
-            )
-        )
-
-    def get_slice(
-        self,
-        data_source: GithubDataSource,
-        permissions: Optional[dict] = None,
-        offset: int = 0,
-        limit: Optional[int] = None,
-        get_row_count: Optional[bool] = False,
-    ) -> DataSlice:
+        Transform a table into a DataFrame and recursively merge tables
+        with a foreign key.
+        Returns: DataFrames from config['table'].
         """
-        Method to retrieve a part of the data as a pandas dataframe
-        and the total size filtered with permissions
 
-        - offset is the index of the starting row
-        - limit is the number of pages to retrieve
-        Exemple: if offset = 5 and limit = 10 then 10 results are expected from 6th row
-        """
-        preview_datasource = GithubDataSource(
-            page_limit=1,
-            dataset=data_source.dataset,
-            domain=f'preview_{data_source.domain}',
-            name=data_source.name,
-            organization=data_source.organization,
-            entities_limit=3,
-        )
-        df = self.get_df(preview_datasource, permissions)
-        if limit is not None:
-            return DataSlice(df[offset : offset + limit], len(df))
-        else:
-            return DataSlice(df[offset:], len(df))
+        if not datasource.query or not datasource.query.strip():
+            raise NoQuerySpecified
 
-    def get_status(self) -> ConnectorStatus:
+        connection = self._connect(database=datasource.database)
+
+        # ----- Prepare -----
+        # As long as frontend builds queries with '"' we need to replace them
+        query = datasource.query.replace('"', '`')
+        MySQLConnector.logger.debug(f'Executing query : {datasource.query}')
+        query_params = datasource.parameters or {}
+
+        df = pandas_read_sql(query, con=connection, params=query_params)
+        df = self.decode_df(df)
+        df = handle_date_0(df)
+        connection.close()
+        return df
+
+    def get_engine_version(self) -> tuple:
         """
-        Test the Github's connexion.
-        :return: a ConnectorStatus with the current status
+        We try to get the MySQL version by running a query with our connection
         """
-        try:
-            access_token = self.get_access_token()
-            if access_token:
-                c = ConnectorStatus(status=True)
-                return c
-            else:
-                return ConnectorStatus(status=False)
-        except Exception:
-            return ConnectorStatus(status=False, error='Credentials are missing')
+        connection = pymysql.connect(**self.get_connection_params())
+
+        with connection.cursor() as cursor:
+            cursor.execute('SELECT VERSION()')
+            version = cursor.fetchone()
+            try:
+                return super()._format_version(version['VERSION()'])
+            except (TypeError, KeyError) as exc:
+                raise UnavailableVersion from exc
+
+
+class InvalidQuery(Exception):
+    """raised when a query is invalid"""
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/github/helpers.py` & `toucan_connectors-4.5.0/toucan_connectors/github/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_adwords/google_adwords.jpg` & `toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_adwords/google_adwords_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_adwords/google_adwords_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_adwords/helpers.py` & `toucan_connectors-4.5.0/toucan_connectors/google_adwords/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_analytics/google-analytics.png` & `toucan_connectors-4.5.0/toucan_connectors/google_analytics/google-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_analytics/google_analytics_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_analytics/google_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_big_query/google-bigquery.png` & `toucan_connectors-4.5.0/toucan_connectors/google_big_query/google-bigquery.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_big_query/google_big_query_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_big_query/google_big_query_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,14 @@
                     'execution_time': end - start,
                     'connector': 'google_big_query',
                 }
             },
         )
         return client
 
-    @cached_property
     def project_tree(self) -> list[TableInfo]:
         return self._get_project_structure()
 
     @staticmethod
     def _execute_query(client: bigquery.Client, query: str, parameters: list) -> pandas.DataFrame:
         try:
             start = timer()
@@ -158,15 +157,15 @@
                         'execution_time': end - start,
                         'connector': 'google_big_query',
                     }
                 },
             )
             return result
         except TypeError as e:
-            _LOGGER.error(f'Error to execute request {query} - {e}')
+            _LOGGER.error(f'Failed to execute request {query} - {e}')
             raise e
 
     @staticmethod
     def _prepare_query_and_parameters(
         query: str, parameters: dict[str, object] | None
     ) -> tuple[str, list]:
         """Replace ToucanToco variable definitions by Google Big Query variable
@@ -213,42 +212,51 @@
             unformatted_db_tree['column_name']
             + ' '
             + unformatted_db_tree['data_type'].apply(lambda x: x.lower())
         )
 
         unformatted_db_tree['columns'] = unformatted_db_tree['columns'].apply(_format_columns)
         return (
-            unformatted_db_tree.groupby(['name', 'schema', 'database', 'type'])['columns']
+            unformatted_db_tree.groupby(['name', 'schema', 'database', 'type'], group_keys=False)[
+                'columns'
+            ]
             .apply(list)
             .reset_index()
             .to_dict(orient='records')
         )
 
     @staticmethod
-    def _build_dataset_info_query(dataset_ids: Iterable[str]) -> str:
+    def _build_dataset_info_query_for_ds(dataset_id: str, db_name: str | None) -> str:
+        output = f"""
+SELECT C.table_name AS name, C.table_schema AS schema, T.table_catalog AS database,
+T.table_type AS type, C.column_name, C.data_type FROM {dataset_id}.INFORMATION_SCHEMA.COLUMNS C
+JOIN {dataset_id}.INFORMATION_SCHEMA.TABLES T ON C.table_name = T.table_name
+WHERE IS_SYSTEM_DEFINED='NO' AND IS_PARTITIONING_COLUMN='NO' AND IS_HIDDEN='NO'
+"""
+        if db_name is not None:
+            output += f"AND T.table_catalog = '{db_name}'\n"
+        return output
+
+    def _build_dataset_info_query(self, dataset_ids: Iterable[str], db_name: str | None) -> str:
         return '\nUNION ALL\n'.join(
-            f"""SELECT C.table_name AS name, C.table_schema AS schema, T.table_catalog AS database,
-                T.table_type AS type, C.column_name, C.data_type FROM {dataset_id}.INFORMATION_SCHEMA.COLUMNS C
-                JOIN {dataset_id}.INFORMATION_SCHEMA.TABLES T ON C.table_name = T.table_name
-                WHERE IS_SYSTEM_DEFINED='NO' AND IS_PARTITIONING_COLUMN='NO' AND IS_HIDDEN='NO'"""
-            for dataset_id in dataset_ids
+            self._build_dataset_info_query_for_ds(dataset_id, db_name) for dataset_id in dataset_ids
         )
 
     def _get_project_structure_fast(
-        self, client: bigquery.Client, dataset_ids: Iterable[str]
+        self, client: bigquery.Client, db_name: str | None, dataset_ids: Iterable[str]
     ) -> pd.DataFrame:
         """Retrieves the project structure in a single query.
 
         Only works if all datasets are in the same location.
         """
-        query = self._build_dataset_info_query(dataset_ids)
+        query = self._build_dataset_info_query(dataset_ids, db_name)
         return client.query(query).to_dataframe()
 
     def _get_project_structure_slow(
-        self, client: bigquery.Client, dataset_ids: Iterable[str]
+        self, client: bigquery.Client, db_name: str | None, dataset_ids: Iterable[str]
     ) -> pd.DataFrame:
         """Retrieves the project structure in multiple queries.
 
         Works even if the project's datasets are in different locations.
         """
         # In case datasets are not in the same location, we need to get information for every dataset in the
         # list, in order to retrieve their location (it's not returned by list_datasets).
@@ -256,35 +264,40 @@
         dataset_info = [client.get_dataset(dataset_id) for dataset_id in dataset_ids]
         _LOGGER.info('Done retrieving location information for every dataset.')
         dataset_info.sort(key=lambda x: x.location)
         dfs = []
         # We then build and execute a query for every distinct location
         for location, datasets_for_region in groupby(dataset_info, key=lambda x: x.location):
             _LOGGER.info(f'Retrieving dataset structure for datasets located in {location}')
-            query = self._build_dataset_info_query(ds.dataset_id for ds in datasets_for_region)
+            query = self._build_dataset_info_query(
+                (ds.dataset_id for ds in datasets_for_region), db_name
+            )
             dfs.append(client.query(query, location=location).to_dataframe())
 
         # Then, we returning a single dataframe containing all results
         return pd.concat(dfs)
 
-    def _get_project_structure(self) -> List[TableInfo]:
+    def _get_project_structure(self, db_name: str | None = None) -> List[TableInfo]:
         creds = self._get_google_credentials(self.credentials, self.scopes)
         client = self._connect(creds)
         datasets = list(client.list_datasets())
-
         # Here, we're trying to retrieve table info for all datasets at once. However, this will
         # only work if all datasets are in same location. Unfortunately, there is no way to
         # retrieve the location along with the dataset list, so we're optimistic here.
         try:
-            df = self._get_project_structure_fast(client, (ds.dataset_id for ds in datasets))
+            df = self._get_project_structure_fast(
+                client, db_name, (ds.dataset_id for ds in datasets)
+            )
         except GoogleAPIError as exc:
             _LOGGER.info(
                 f'Got an exception when trying to retrieve domains for project: {exc}. '
                 'Falling back on listing by location...'
             )
-            df = self._get_project_structure_slow(client, (ds.dataset_id for ds in datasets))
+            df = self._get_project_structure_slow(
+                client, db_name, (ds.dataset_id for ds in datasets)
+            )
 
         return self._format_db_model(df)
 
     def get_model(self, db_name: str | None = None) -> list[TableInfo]:
         """Retrieves the database tree structure using current connection"""
-        return self.project_tree
+        return self._get_project_structure(db_name)
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png` & `toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_credentials.py` & `toucan_connectors-4.5.0/toucan_connectors/google_credentials.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_my_business/google-my-business.png` & `toucan_connectors-4.5.0/toucan_connectors/google_my_business/google-my-business.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_my_business/google_my_business_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_my_business/google_my_business_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_sheets/google-sheets.png` & `toucan_connectors-4.5.0/toucan_connectors/google_sheets/google-sheets.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_sheets/google_sheets_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_sheets/google_sheets_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png` & `toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/http_api/http-api.png` & `toucan_connectors-4.5.0/toucan_connectors/http_api/http-api.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/http_api/http_api_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/http_api/http_api_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/hubspot/hubspot.png` & `toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/hubspot/hubspot_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/hubspot/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/hubspot_private_app/hubspot_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/hubspot_private_app/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/install_scripts/databricks.sh` & `toucan_connectors-4.5.0/toucan_connectors/install_scripts/databricks.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh` & `toucan_connectors-4.5.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/install_scripts/odbc.sh` & `toucan_connectors-4.5.0/toucan_connectors/install_scripts/odbc.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/install_scripts/oracle.sh` & `toucan_connectors-4.5.0/toucan_connectors/install_scripts/oracle.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/json_wrapper.py` & `toucan_connectors-4.5.0/toucan_connectors/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/linkedinads/linkedinads.png` & `toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/linkedinads/linkedinads_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/linkedinads/linkedinads_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         try:
             splitted_start = datetime.strptime(data_source.start_date, '%d/%m/%Y')
         except ValueError:
             splitted_start = dateutil.parser.parse(data_source.start_date)
         # Build the query, 1 mandatory parameters
         query = (
             f'dateRange.start.day={splitted_start.day}&dateRange.start.month={splitted_start.month}'
-            f'&dateRange.start.year={splitted_start.year}&timeGranularity={data_source.time_granularity}'
+            f'&dateRange.start.year={splitted_start.year}&timeGranularity={data_source.time_granularity.value}'
         )
 
         if data_source.end_date:
             try:
                 splitted_end = datetime.strptime(data_source.end_date, '%d/%m/%Y')
             except ValueError:
                 splitted_end = dateutil.parser.parse(data_source.end_date)
@@ -175,15 +175,17 @@
         # Build the query, 2 optional array parameters
         if data_source.parameters:
             for p in data_source.parameters.keys():
                 query += f'&{p}={data_source.parameters.get(p)}'
 
         # Get the data
         res = requests.get(
-            url=f'{self._baseroute}{data_source.finder_methods}', params=query, headers=headers
+            url=f'{self._baseroute}{data_source.finder_methods.value}',
+            params=query,
+            headers=headers,
         )
 
         try:
             assert res.ok
             data = res.json().get('elements')
 
         except AssertionError:
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/micro_strategy/client.py` & `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/client.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/micro_strategy/data.py` & `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/data.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/micro_strategy/micro_strategy_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/micro_strategy_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/micro_strategy/microstrategy.png` & `toucan_connectors-4.5.0/toucan_connectors/micro_strategy/microstrategy.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mongo/mongo-db.png` & `toucan_connectors-4.5.0/toucan_connectors/mongo/mongo-db.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mongo/mongo_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mongo/mongo_translator.py` & `toucan_connectors-4.5.0/toucan_connectors/mongo/mongo_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mssql/mssql.png` & `toucan_connectors-4.5.0/toucan_connectors/mssql/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mssql/mssql_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mssql_TLSv1_0/mssql.png` & `toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mysql/mysql.png` & `toucan_connectors-4.5.0/toucan_connectors/mysql/mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/mysql/mysql_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/redshift/redshift_database_connector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,368 +1,405 @@
-import os
+import logging
+import re
+from contextlib import suppress
 from enum import Enum
-from itertools import groupby as groupby
-from tempfile import NamedTemporaryFile
-from typing import Any, Generator, Optional
+from functools import cached_property
+from typing import Any
 
-import numpy as np
 import pandas as pd
-import pymysql
-from cached_property import cached_property_with_ttl
-from pydantic import Field, SecretStr, constr, create_model, validator
-from pymysql.constants import CR, ER
-
-from toucan_connectors.common import ConnectorStatus, pandas_read_sql
+import redshift_connector
+from pydantic import Field, SecretStr, create_model, root_validator, validator
+from pydantic.types import constr
+
+from toucan_connectors.common import ConnectorStatus
+from toucan_connectors.pagination import build_pagination_info
+from toucan_connectors.redshift.utils import build_database_model_extraction_query, types_map
+from toucan_connectors.sql_query_helper import SqlQueryHelper
 from toucan_connectors.toucan_connector import (
+    DataSlice,
     DiscoverableConnector,
     TableInfo,
     ToucanConnector,
     ToucanDataSource,
-    UnavailableVersion,
-    VersionableEngineConnector,
     strlist_to_enum,
 )
-from toucan_connectors.utils.pem import sanitize_spaces_pem
-
-
-def handle_date_0(df: pd.DataFrame) -> pd.DataFrame:
-    # Mysql driver doesnt translate date '0000-00-00 00:00:00'
-    # to a datetime, so the Series has a 'object' dtype instead of 'datetime'.
-    # This util fixes this behaviour, by replacing it with NaT.
-    return df.replace({'0000-00-00 00:00:00': pd.NaT}).infer_objects()
-
 
-class NoQuerySpecified(Exception):
-    def __init__(self) -> None:
-        super().__init__('no query was specified')
+TABLE_QUERY = """SELECT DISTINCT tablename FROM pg_table_def WHERE schemaname = 'public';"""
 
+DESCRIBE_QUERY = """SELECT * FROM ({column}) AS q LIMIT 0;"""
 
-class MySQLDataSource(ToucanDataSource):
-    """
-    Either `query` or `table` are required, both at the same time are not supported.
-    """
+DEFAULT_DATABASE = 'dev'
 
-    database: str = Field(..., description='The name of the database you want to query')
-    follow_relations: bool | None = Field(
-        None,
-        **{'ui.hidden': True},
-        description='Deprecated, kept for compatibility purpose with old data sources configs',
-    )  # Deprecated
-    table: str = Field(
-        None, **{'ui.hidden': True}
-    )  # To avoid previous config migrations, won't be used
+ORDERED_KEYS = [
+    'type',
+    'name',
+    'host',
+    'port',
+    'default_database',
+    'authentication_method',
+    'user',
+    'password',
+    'cluster_identifier',
+    'db_user',
+    'connect_timeout',
+    'access_key_id',
+    'secret_access_key',
+    'session_token',
+    'profile',
+    'region',
+    'enable_tcp_keepalive',
+]
+
+logger = logging.getLogger(__name__)
+
+
+class AuthenticationMethod(str, Enum):
+    DB_CREDENTIALS: str = 'db_credentials'
+    AWS_CREDENTIALS: str = 'aws_credentials'
+    AWS_PROFILE: str = 'aws_profile'
+
+
+class AuthenticationMethodError(str, Enum):
+    DB_CREDENTIALS: str = f'User & Password are required for {AuthenticationMethod.DB_CREDENTIALS}'
+    AWS_CREDENTIALS: str = f'AccessKeyId, SecretAccessKey & db_user are required for {AuthenticationMethod.AWS_CREDENTIALS}'
+    AWS_PROFILE: str = f'Profile & db_user are required for {AuthenticationMethod.AWS_PROFILE}'
+    UNKNOWN: str = 'Unknown AuthenticationMethod'
+
+
+class RedshiftDataSource(ToucanDataSource):
+    database: str = Field(
+        DEFAULT_DATABASE, description='The name of the database you want to query'
+    )
     query: constr(min_length=1) = Field(
         None,
         description='You can write a custom query against your '
         'database here. It will take precedence over '
-        'the "table" parameter',
+        'the table parameter',
         widget='sql',
     )
-    query_object: dict = Field(
+    query_object: dict[str, Any] = Field(
         None,
-        description='An object describing a simple select query' 'This field is used internally',
+        description='An object describing a simple select query, this field is used internally',
         **{'ui.hidden': True},
     )
     language: str = Field('sql', **{'ui.hidden': True})
 
     @classmethod
-    def get_form(cls, connector: 'MySQLConnector', current_config: dict[str, Any]) -> dict:
+    def get_form(cls, connector: 'RedshiftConnector', current_config: dict[str, Any]):
+        """
+        Method to retrieve the form with a current config
+        Once the connector is set, we are able to give suggestions for the `database` field
+        """
+        default_db = current_config.get('database', DEFAULT_DATABASE)
         return create_model(
             'FormSchema',
-            database=strlist_to_enum('database', connector.available_dbs),
+            database=strlist_to_enum('database', connector.available_dbs, default_db),
             __base__=cls,
         ).schema()
 
 
-_DATABASE_MODEL_EXTRACTION_QUERY = (
-    # table_schema is selected twice because the frontend components needs it but
-    # mysql provides it only for compliance with the SQL-92 standard.
-    # https://dba.stackexchange.com/questions/3774/what-is-the-point-of-the-table-catalog-column-in-information-schema-tables
-    "SELECT t.table_schema AS 'database', t.table_schema AS 'schema', "
-    # Table type and name
-    "CASE WHEN t.table_type = 'BASE TABLE' THEN 'table' ELSE LOWER(t.table_type) END AS table_type, t.table_name, "
-    # Columns from the columns table
-    'c.column_name, c.data_type FROM information_schema.tables t INNER JOIN information_schema.columns c '
-    # Inner join on table name
-    'ON t.table_name = c.table_name '
-    # Filtering on concrete tables/views
-    "WHERE t.table_type in ('BASE TABLE', 'VIEW') AND t.table_schema NOT IN ('mysql', 'information_schema', 'performance_schema', 'sys');"
-)
-
-
-class SSLMode(str, Enum):
-    VERIFY_IDENTITY = 'VERIFY_IDENTITY'
-    VERIFY_CA = 'VERIFY_CA'
-    REQUIRED = 'REQUIRED'
-
-
-class MySQLConnector(ToucanConnector, DiscoverableConnector, VersionableEngineConnector):
-    """
-    Import data from MySQL database.
-    """
-
-    data_source_model: MySQLDataSource
-
-    host: str = Field(
-        ...,
-        description='The domain name (preferred option as more dynamic) or '
-        'the hardcoded IP address of your database server',
-    )
-    port: int = Field(None, description='The listening port of your database server')
-    user: str = Field(..., description='Your login username')
-    password: SecretStr = Field(None, description='Your login password')
-    charset: str = Field(
-        'utf8mb4',
-        title='Charset',
-        description='Character encoding. You should generally let the default "utf8mb4" here.',
-    )
-    connect_timeout: int = Field(
+class RedshiftConnector(ToucanConnector, DiscoverableConnector):
+    data_source_model: RedshiftDataSource
+    authentication_method: AuthenticationMethod = Field(
         None,
-        title='Connection timeout',
-        description='You can set a connection timeout in seconds here, '
-        'i.e. the maximum length of time you want to wait '
-        'for the server to respond. None by default',
+        title='Authentication Method',
+        description='The authentication mechanism that will be used to connect to your redshift data source',
+        **{'ui': {'checkbox': False}},
     )
-    # SSL options
-    ssl_ca: SecretStr = Field(
-        None,
-        description='The CA certificate content in PEM format to use to connect to the MySQL '
-        'server. Equivalent of the --ssl-ca option of the MySQL client',
+    host: str = Field(..., description='The hostname of the Amazon Redshift cluster')
+    port: int = Field(5439, description='The listening port of your Redshift Database')
+    default_database: str = Field(
+        DEFAULT_DATABASE, description='The name of the database instance to connect to'
     )
-    ssl_cert: SecretStr = Field(
-        None,
-        description='The X509 certificate content in PEM format to use to connect to the MySQL '
-        'server. Equivalent of the --ssl-cert option of the MySQL client',
+    user: str | None = Field(
+        None, description='The username to use for authentication with the Amazon Redshift cluster'
     )
-    ssl_key: SecretStr = Field(
-        None,
-        description='The X509 certificate key content in PEM format to use to connect to the MySQL '
-        'server. Equivalent of the --ssl-key option of the MySQL client',
+    password: SecretStr | None = Field(
+        None, description='The password to use for authentication with the Amazon Redshift cluster'
     )
-    ssl_mode: SSLMode = Field(
+
+    db_user: str | None = Field(None, description='The user ID to use with Amazon Redshift')
+    cluster_identifier: str | None = Field(
+        None, description='The cluster identifier of the Amazon Redshift cluster'
+    )
+
+    connect_timeout: int | None = Field(
         None,
-        description='SSL Mode to use to connect to the MySQL server. '
-        'Equivalent of the --ssl-mode option of the MySQL client. Must be set in order to use SSL',
+        title='Connection timeout',
+        description='You can set a connection timeout in seconds here, i.e. the maximum length of '
+        'time you want to wait for the server to respond. None by default',
     )
+    # True by default to match redshift_connector kwargs syntax
+    enable_tcp_keepalive: bool = Field(
+        True,
+        title='Enable TCP keep-alive',
+        description='You may disable TCP keep-alive by unticking this option. Disabling might be '
+        'required for long-running queries or if you are behind a firewall',
+    )
+
+    access_key_id: str | None = Field(None, description='The access key id of your aws account.')
+    secret_access_key: SecretStr | None = Field(
+        None, description='The secret access key of your aws account.'
+    )
+    session_token: str | None = Field(None, description='Your session token')
+    profile: str | None = Field(None, description='AWS profile')
+    region: str | None = Field(None, description='The region in which there is your aws account.')
 
     class Config:
         underscore_attrs_are_private = True
-        keep_untouched = (cached_property_with_ttl,)
+        keep_untouched = (cached_property,)
 
-    @validator('ssl_key')
-    @classmethod
-    def ssl_key_validator(cls, ssl_key: str, values: dict) -> str:
-        ssl_cert = values.get('ssl_cert', None)
-        # if one is present, the other one should be specified
-        if ssl_cert is not None and ssl_key is None:
-            raise ValueError('SSL option "ssl_key" should be specified if "ssl_cert" is provided !')
-        elif ssl_key is not None and ssl_cert is None:
-            raise ValueError('SSL option "ssl_cert" should be specified if "ssl_key" is provided !')
-
-        return ssl_key
-
-    def _sanitize_ssl_params(self) -> dict[str, Any]:
-        params = {}
-        if self.ssl_mode in (SSLMode.VERIFY_CA, SSLMode.VERIFY_IDENTITY):
-
-            for ssl_opt in ('ssl_ca', 'ssl_key', 'ssl_cert'):
-                opt = getattr(self, ssl_opt)
-                if opt is None:
-                    continue
-                secret = opt.get_secret_value()
-                if secret.strip() != '':
-                    params[ssl_opt] = sanitize_spaces_pem(secret)
-        return params
-
-    def _list_db_names(self) -> list[str]:
-        connection = self._connect(cursorclass=None, database=None)
-        # Always add the suggestions for the available databases
-        with connection.cursor() as cursor:
-            cursor.execute('SHOW DATABASES;')
-            res = cursor.fetchall()
-            return [
-                db_name
-                for (db_name,) in res
-                if db_name not in ('information_schema', 'mysql', 'performance_schema')
-            ]
-
-    def _get_project_structure(
-        self, db_name: str | None = None
-    ) -> Generator[TableInfo, None, None]:
-        connection = self._connect(cursorclass=None, database=db_name)
-        # Always add the suggestions for the available databases
-        with connection.cursor() as cursor:
-            cursor.execute(_DATABASE_MODEL_EXTRACTION_QUERY)
-            results = cursor.fetchall()
-
-        column_names = ('database', 'schema', 'table_type', 'table_name', 'columns')
-        # Grouping by DB name, schema name, Table type, Table name
-        for group, grouper in groupby(sorted(results), key=lambda x: x[:4]):
-            col_info = [{'name': x[4], 'type': x[5]} for x in grouper]
-            yield dict(zip(column_names, group + (col_info,)))
+        @staticmethod
+        def schema_extra(schema: dict[str, Any]) -> None:
+            schema['properties'] = {k: schema['properties'][k] for k in ORDERED_KEYS}
 
-    @cached_property_with_ttl(ttl=10)
+    @cached_property
     def available_dbs(self) -> list[str]:
         return self._list_db_names()
 
-    def project_tree(self, db_name: str | None = None) -> list[TableInfo]:
-        return list(self._get_project_structure(db_name=db_name))
-
-    def get_connection_params(
-        self, *, database: str | None = None, cursorclass=pymysql.cursors.DictCursor
-    ):
-        conv = pymysql.converters.conversions.copy()
-        conv[246] = float
-        con_params = {
-            'host': self.host,
-            'user': self.user,
-            'password': self.password.get_secret_value() if self.password else None,
-            'port': self.port,
-            'database': database,
-            'charset': self.charset,
-            'connect_timeout': self.connect_timeout,
-            'conv': conv,
-            'cursorclass': cursorclass,
-        }
-        # remove None values
+    @validator('host')
+    def host_validator(cls, v):
+        return re.sub(r'^https?://', '', v)
+
+    @root_validator
+    def check_requirements(cls, values):
+        mode = values.get('authentication_method')
+        if mode == AuthenticationMethod.DB_CREDENTIALS.value:
+            # TODO: Partial check due to missing context in some operations (Missing: password)
+            user = values.get('user')
+            if user is None:
+                raise ValueError(AuthenticationMethodError.DB_CREDENTIALS.value)
+        elif mode == AuthenticationMethod.AWS_CREDENTIALS.value:
+            # TODO: Partial check due to missing context in some operations (Missing: secret_access_key)
+            access_key_id, db_user = (
+                values.get('access_key_id'),
+                values.get('db_user'),
+            )
+            if access_key_id is None or db_user is None:
+                raise ValueError(AuthenticationMethodError.AWS_CREDENTIALS.value)
+        elif mode == AuthenticationMethod.AWS_PROFILE.value:
+            profile, db_user = (values.get('profile'), values.get('db_user'))
+            if profile is None or db_user is None:
+                raise ValueError(AuthenticationMethodError.AWS_PROFILE.value)
+        else:
+            raise ValueError(AuthenticationMethodError.UNKNOWN.value)
+        return values
+
+    def _get_connection_params(self, database) -> dict[str, Any]:
+        con_params = dict(
+            database=database,
+            host=self.host,
+            port=self.port,
+            timeout=self.connect_timeout,
+            cluster_identifier=self.cluster_identifier,
+            tcp_keepalive=self.enable_tcp_keepalive,
+        )
+        if self.authentication_method == AuthenticationMethod.DB_CREDENTIALS.value:
+            con_params['user'] = self.user
+            con_params['password'] = self.password.get_secret_value() if self.password else None
+        elif self.authentication_method == AuthenticationMethod.AWS_CREDENTIALS.value:
+            con_params['iam'] = True
+            con_params['db_user'] = self.db_user
+            con_params['access_key_id'] = self.access_key_id
+            con_params['secret_access_key'] = (
+                self.secret_access_key.get_secret_value() if self.secret_access_key else None
+            )
+            con_params['session_token'] = self.session_token
+            con_params['region'] = self.region
+        elif self.authentication_method == AuthenticationMethod.AWS_PROFILE.value:
+            con_params['iam'] = True
+            con_params['db_user'] = self.db_user
+            con_params['profile'] = self.profile
+            con_params['region'] = self.region
         return {k: v for k, v in con_params.items() if v is not None}
 
-    def _connect(
-        self, *, database: str | None = None, cursorclass=pymysql.cursors.DictCursor
-    ) -> pymysql.Connection:
-        connection_params = self.get_connection_params(database=database, cursorclass=cursorclass)
-        if self.ssl_mode is not None:
-            connection_params |= {
-                'ssl_disabled': False,
-                # Verify the server's certificate. This one is actually required by pymysql, as no
-                # SSL context will be created otherwise:
-                # https://github.com/PyMySQL/PyMySQL/blob/main/pymysql/connections.py#L266
-                'ssl_verify_cert': True,
-            }
-
-        if self.ssl_mode in (SSLMode.VERIFY_CA, SSLMode.VERIFY_IDENTITY):
-            ssl_params = self._sanitize_ssl_params()
-            ssl_files = []
-            for ssl_opt in ('ssl_ca', 'ssl_key', 'ssl_cert'):
-                if ssl_opt in ssl_params:
-                    ssl_opt_file = NamedTemporaryFile(prefix=ssl_opt, delete=False)
-                    ssl_opt_file.write(ssl_params[ssl_opt].encode())
-                    ssl_opt_file.seek(0)
+    def _get_connection(self, database) -> redshift_connector.Connection:
+        """Establish a connection to an Amazon Redshift cluster."""
+        con = redshift_connector.connect(
+            **self._get_connection_params(
+                database=database if database else None,
+            ),
+        )
+        con.autocommit = True  # see https://stackoverflow.com/q/22019154
+        con.paramstyle = 'pyformat'
+        return con
+
+    def _retrieve_tables(self, database) -> list[str]:
+        with self._get_connection(database=database).cursor() as cursor:
+            cursor.execute(TABLE_QUERY)
+            res = cursor.fetchall()
+        return [table_name for (table_name,) in res]
 
-                    connection_params[ssl_opt] = ssl_opt_file.name
-                    ssl_files.append(ssl_opt_file)
+    def _retrieve_data(
+        self,
+        datasource: RedshiftDataSource,
+        get_row_count: bool = False,
+        offset: int | None = None,
+        limit: int | None = None,
+    ) -> pd.DataFrame:
+        if get_row_count:
+            prepared_query, prepared_query_parameters = SqlQueryHelper.prepare_count_query(
+                datasource.query, datasource.parameters
+            )
+        else:
+            prepared_query, prepared_query_parameters = SqlQueryHelper.prepare_limit_query(
+                datasource.query, datasource.parameters, offset, limit
+            )
+        with self._get_connection(database=datasource.database).cursor() as cursor:
+            cursor.execute(prepared_query, prepared_query_parameters)
+            result: pd.DataFrame = cursor.fetch_dataframe()
+            if result is None:
+                result = pd.DataFrame()
+        return result
+
+    def get_slice(
+        self,
+        data_source: RedshiftDataSource,
+        permissions: dict[str, Any] | None = None,
+        offset: int = 0,
+        limit: int | None = None,
+        get_row_count: bool = False,
+    ) -> DataSlice:
+        """
+        Method to retrieve a part of the data as a pandas dataframe
+        and the total size filtered with permissions
+        - offset is the index of the starting row
+        - limit is the number of pages to retrieve
+        Exemple: if offset = 5 and limit = 10 then 10 results are expected from 6th row
+        """
+        df: pd.DataFrame = self._retrieve_data(data_source, False, offset, limit)
+        total_returned_rows = len(df) if df is not None else 0
 
-            connection_params['ssl_verify_identity'] = self.ssl_mode == SSLMode.VERIFY_IDENTITY
+        run_count_request = get_row_count and SqlQueryHelper.count_query_needed(data_source.query)
 
-            try:
-                connection = pymysql.connect(**connection_params)
-            finally:
-                for ssl_file in ssl_files:
-                    ssl_file.close()
-                    os.unlink(ssl_file.name)  # needed otherwise file is not closed.
-            return connection
-        return pymysql.connect(**connection_params)
+        if run_count_request:
+            df_count: pd.DataFrame = self._retrieve_data(data_source, True)
+            total_rows = (
+                df_count.total_rows[0]
+                if df_count is not None and len(df_count.total_rows) > 0
+                else 0
+            )
+        else:
+            total_rows = total_returned_rows
+
+        return DataSlice(
+            df,
+            pagination_info=build_pagination_info(
+                offset=offset,
+                limit=limit,
+                total_rows=total_rows,
+                retrieved_rows=total_returned_rows,
+            ),
+        )
 
     @staticmethod
-    def _get_details(index: int, status: Optional[bool]):
-        checks = ['Hostname resolved', 'Port opened', 'Host connection', 'Authenticated']
+    def _get_details(index: int, status: bool):
+        checks = [
+            'Hostname resolved',
+            'Port opened',
+            'Authenticated',
+            'Default Database connection',
+        ]
         ok_checks = [(c, True) for i, c in enumerate(checks) if i < index]
         new_check = (checks[index], status)
-        not_validated_checks = [(c, None) for i, c in enumerate(checks) if i > index]
+        not_validated_checks = [(c, False) for i, c in enumerate(checks) if i > index]
         return ok_checks + [new_check] + not_validated_checks
 
     def get_status(self) -> ConnectorStatus:
         # Check hostname
         try:
             self.check_hostname(self.host)
         except Exception as e:
             return ConnectorStatus(status=False, details=self._get_details(0, False), error=str(e))
-
         # Check port
         try:
             self.check_port(self.host, self.port)
         except Exception as e:
             return ConnectorStatus(status=False, details=self._get_details(1, False), error=str(e))
 
-        # Check basic access
+        # Basic db query
         try:
-            self._connect()
-        except pymysql.err.OperationalError as e:
-            error_code = e.args[0]
-
-            # Can't connect to full URI
-            if error_code == CR.CR_CONN_HOST_ERROR:
-                return ConnectorStatus(
-                    status=False, details=self._get_details(2, False), error=e.args[1]
-                )
-
-            # Wrong user/password
-            if error_code == ER.ACCESS_DENIED_ERROR:
-                return ConnectorStatus(
-                    status=False, details=self._get_details(3, False), error=e.args[1]
-                )
+            redshift_connector.connect(
+                **self._get_connection_params(database=self.default_database),
+            )
+        except (Exception, redshift_connector.OperationalError) as e:
+            return ConnectorStatus(status=False, details=self._get_details(3, False), error=str(e))
 
         return ConnectorStatus(status=True, details=self._get_details(3, True), error=None)
 
-    def get_model(self, db_name: str | None = None) -> list[Any]:
-        """Retrieves the database tree structure using current connection"""
-        return DiscoverableConnector.format_db_model(self.project_tree(db_name=db_name))
-
-    @staticmethod
-    def decode_df(df):
-        """
-        Used to change bytes columns to string columns
-        (can be moved to be applied for all connectors if needed)
-        It retrieves all the string columns and converts them all together.
-        The string columns become nan columns so we remove them from the result,
-        we keep the rest and insert it back to the dataframe
-        """
-        str_df = df.select_dtypes([np.object])
-        if str_df.empty:
-            return df
-
-        str_df = str_df.stack().str.decode('utf8').unstack().dropna(axis=1, how='all')
-        for col in str_df.columns:
-            df[col] = str_df[col]
-        return df
-
-    def _retrieve_data(self, datasource):
-        """
-        Transform a table into a DataFrame and recursively merge tables
-        with a foreign key.
-        Returns: DataFrames from config['table'].
-        """
-
-        if not datasource.query or not datasource.query.strip():
-            raise NoQuerySpecified
+    def describe(self, data_source: RedshiftDataSource) -> dict[str, Any]:
+        with self._get_connection(database=data_source.database).cursor() as cursor:
+            cursor.execute(DESCRIBE_QUERY.format(column=data_source.query.replace(';', '')))
+            res = cursor.description
+        return {
+            col[0].decode('utf-8') if isinstance(col[0], bytes) else col[0]: types_map.get(col[1])
+            for col in res
+        }
 
-        connection = self._connect(database=datasource.database)
+    def _db_table_info_rows(self, database: str) -> list[tuple[str, str, str, str]]:
+        with self._get_connection(database).cursor() as cursor:
+            """Get rows of (schema, table name, column name, column type)"""
+            cursor.execute(
+                r"""SELECT "schemaname", "tablename", "column", "type" FROM PG_TABLE_DEF WHERE schemaname = 'public';"""
+            )
+            return cursor.fetchall()
+
+    def _db_tables_info(self, database: str) -> list[tuple[str, str, str, str, str]]:
+        """Get rows of (database, schema, table name, column name, column type)"""
+        table_infos = []
+        for schema, table_name, column_name, column_type in self._db_table_info_rows(database):
+            for row in table_infos[::-1]:
+                if row['schema'] == schema and row['name'] == table_name:
+                    row['columns'].append({'name': column_name, 'type': column_type})
+                    break
+            else:
+                table_infos.append(
+                    {
+                        'database': database,
+                        'schema': schema,
+                        'name': table_name,
+                        'type': 'table',
+                        'columns': [{'name': column_name, 'type': column_type}],
+                    }
+                )
+        return table_infos
 
-        # ----- Prepare -----
-        # As long as frontend builds queries with '"' we need to replace them
-        query = datasource.query.replace('"', '`')
-        MySQLConnector.logger.debug(f'Executing query : {datasource.query}')
-        query_params = datasource.parameters or {}
-
-        df = pandas_read_sql(query, con=connection, params=query_params)
-        df = self.decode_df(df)
-        df = handle_date_0(df)
-        connection.close()
-        return df
+    def get_model(self, db_name: str | None = None) -> list[TableInfo]:
+        """Retrieves the database tree structure using current connection"""
+        tables_info = []
+        dbs = self.available_dbs if db_name is None else [db_name]
+        for db in dbs:
+            with suppress(redshift_connector.OperationalError):
+                tables_info += self._db_tables_info(db)
 
-    def get_engine_version(self) -> tuple:
-        """
-        We try to get the MySQL version by running a query with our connection
-        """
-        connection = pymysql.connect(**self.get_connection_params())
+        return tables_info
 
-        with connection.cursor() as cursor:
-            cursor.execute('SELECT VERSION()')
-            version = cursor.fetchone()
+    def get_model_with_info(self, db_name: str | None = None) -> tuple[list[TableInfo], dict]:
+        """Retrieves the database tree structure using current connection"""
+        databases_tree = []
+        failed_databases = []
+        dbs = self.available_dbs if db_name is None else [db_name]
+        for db in dbs:
             try:
-                return super()._format_version(version['VERSION()'])
-            except (TypeError, KeyError) as exc:
-                raise UnavailableVersion from exc
-
+                databases_tree += self._list_tables_info(db)
+            except redshift_connector.OperationalError:
+                failed_databases.append(db)
+
+        tables_info = DiscoverableConnector.format_db_model(databases_tree)
+        metadata = {}
+        if failed_databases:
+            metadata['info'] = {'Could not reach databases': failed_databases}
+        return (tables_info, metadata)
 
-class InvalidQuery(Exception):
-    """raised when a query is invalid"""
+    def _list_db_names(self) -> list[str]:
+        with self._get_connection(database=self.default_database).cursor() as cursor:
+            # redshift has a weird system db called padb_harvest duplicating the content of 'dev' database
+            # https://bit.ly/3GQJCdy, we have to filter it
+            cursor.execute(
+                """select datname from pg_database where datistemplate = false and datname != 'padb_harvest';"""
+            )
+            return [db_name for (db_name,) in cursor.fetchall()]
+
+    def _list_tables_info(self, database: str) -> list[tuple]:
+        with self._get_cursor(database) as cursor:
+            cursor.execute(build_database_model_extraction_query())
+            return cursor.fetchall()
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/net_explorer/net_explorer.png` & `toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/net_explorer/net_explorer_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/net_explorer/net_explorer_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/oauth2_connector/oauth2connector.py` & `toucan_connectors-4.5.0/toucan_connectors/oauth2_connector/oauth2connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/odata/odata.png` & `toucan_connectors-4.5.0/toucan_connectors/odata/odata.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/odata/odata_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/odata/odata_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/odbc/odbc.png` & `toucan_connectors-4.5.0/toucan_connectors/odbc/odbc.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/odbc/odbc_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/odbc/odbc_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/one_drive/one_drive.png` & `toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/one_drive/one_drive_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/one_drive/one_drive_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/oracle_sql/oracle-sql.png` & `toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle-sql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/oracle_sql/oracle_sql_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/oracle_sql/oracle_sql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/pagination.py` & `toucan_connectors-4.5.0/toucan_connectors/pagination.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/pandas_translator.py` & `toucan_connectors-4.5.0/toucan_connectors/pandas_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/peakina/peakina.png` & `toucan_connectors-4.5.0/toucan_connectors/peakina/peakina.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/postgres/postgres.png` & `toucan_connectors-4.5.0/toucan_connectors/postgres/postgres.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/postgres/postgresql_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/postgres/postgresql_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,24 +197,24 @@
         with connection.cursor() as cursor:
             cursor.execute(f"""SELECT * FROM ({data_source.query.replace(';','')}) AS q LIMIT 0;""")
             res = cursor.description
         return {r.name: types.get(r.type_code) for r in res}
 
     def get_model(self, db_name: str | None = None) -> List[TableInfo]:
         """Retrieves the database tree structure using current connection"""
-        available_dbs = self._list_db_names()
+        available_dbs = self._list_db_names() if db_name is None else [db_name]
         databases_tree = []
         for db in available_dbs:
             with suppress(pgsql.OperationalError):
                 databases_tree += self._list_tables_info(db)
         return DiscoverableConnector.format_db_model(databases_tree)
 
     def get_model_with_info(self, db_name: str | None = None) -> tuple[list[TableInfo], dict]:
         """Retrieves the database tree structure using current connection"""
-        available_dbs = self._list_db_names()
+        available_dbs = self._list_db_names() if db_name is None else [db_name]
         databases_tree = []
         failed_databases = []
         for db in available_dbs:
             try:
                 databases_tree += self._list_tables_info(db)
             except pgsql.OperationalError:
                 failed_databases.append(db)
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/postgres/utils.py` & `toucan_connectors-4.5.0/toucan_connectors/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/query_manager.py` & `toucan_connectors-4.5.0/toucan_connectors/query_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/redshift/redshift.png` & `toucan_connectors-4.5.0/toucan_connectors/redshift/redshift.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/redshift/redshift_database_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake_connector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,403 +1,472 @@
 import logging
-import re
-from contextlib import suppress
+from contextlib import contextmanager, suppress
+from datetime import datetime
 from enum import Enum
-from functools import cached_property
-from typing import Any
+from typing import Any, ContextManager, Generator, Literal, Type, overload
 
+import jwt
 import pandas as pd
-import redshift_connector
-from pydantic import Field, SecretStr, create_model, root_validator, validator
-from pydantic.types import constr
+import requests
+import snowflake
+from jinja2 import Template
+from pydantic import Field, SecretStr, create_model
+from snowflake import connector as sf_connector
+from snowflake.connector import SnowflakeConnection
+from snowflake.connector.cursor import DictCursor as SfDictCursor
 
 from toucan_connectors.common import ConnectorStatus
 from toucan_connectors.pagination import build_pagination_info
-from toucan_connectors.redshift.utils import build_database_model_extraction_query, types_map
+from toucan_connectors.snowflake_common import (
+    build_database_model_extraction_query,
+    type_code_mapping,
+)
 from toucan_connectors.sql_query_helper import SqlQueryHelper
 from toucan_connectors.toucan_connector import (
+    Category,
     DataSlice,
     DiscoverableConnector,
     TableInfo,
     ToucanConnector,
     ToucanDataSource,
     strlist_to_enum,
 )
 
-TABLE_QUERY = """SELECT DISTINCT tablename FROM pg_table_def WHERE schemaname = 'public';"""
-
-DESCRIBE_QUERY = """SELECT * FROM ({column}) AS q LIMIT 0;"""
-
-DEFAULT_DATABASE = 'dev'
-
-ORDERED_KEYS = [
-    'type',
-    'name',
-    'host',
-    'port',
-    'default_database',
-    'authentication_method',
-    'user',
-    'password',
-    'cluster_identifier',
-    'db_user',
-    'connect_timeout',
-    'access_key_id',
-    'secret_access_key',
-    'session_token',
-    'profile',
-    'region',
-    'enable_tcp_keepalive',
-]
-
 logger = logging.getLogger(__name__)
 
+# TODO: Once we remove SnowflakeCommon, directly assign the query block here
+_DB_MODEL_EXTRACTION_QUERY = build_database_model_extraction_query()
+# TODO: Once we remove SnowflakeCommon, declare the mapping here
+_TYPE_CODE_MAPPING = type_code_mapping
 
-class AuthenticationMethod(str, Enum):
-    DB_CREDENTIALS: str = 'db_credentials'
-    AWS_CREDENTIALS: str = 'aws_credentials'
-    AWS_PROFILE: str = 'aws_profile'
-
+_UI_HIDDEN: dict[str, Any] = {'ui.hidden': True}
 
-class AuthenticationMethodError(str, Enum):
-    DB_CREDENTIALS: str = f'User & Password are required for {AuthenticationMethod.DB_CREDENTIALS}'
-    AWS_CREDENTIALS: str = f'AccessKeyId, SecretAccessKey & db_user are required for {AuthenticationMethod.AWS_CREDENTIALS}'
-    AWS_PROFILE: str = f'Profile & db_user are required for {AuthenticationMethod.AWS_PROFILE}'
-    UNKNOWN: str = 'Unknown AuthenticationMethod'
 
+class SnowflakeDataSource(ToucanDataSource['SnowflakeConnector']):
+    database: str = Field(..., description='The name of the database you want to query')
+    warehouse: str | None = Field(None, description='The name of the warehouse you want to query')
 
-class RedshiftDataSource(ToucanDataSource):
-    database: str = Field(
-        DEFAULT_DATABASE, description='The name of the database you want to query'
+    query: str = Field(
+        ..., description='You can write your SQL query here', min_length=1, widget='sql'
     )
-    query: constr(min_length=1) = Field(
-        None,
-        description='You can write a custom query against your '
-        'database here. It will take precedence over '
-        'the table parameter',
-        widget='sql',
-    )
-    query_object: dict[str, Any] = Field(
+
+    # Pydantic sees **_UI_HIDDEN as the third argument (the default factory) and raises an error
+    query_object: dict | None = Field(  # type: ignore[pydantic-field]
         None,
-        description='An object describing a simple select query, this field is used internally',
-        **{'ui.hidden': True},
+        description='An object describing a simple select query'
+        'For example '
+        '{"schema": "SHOW_SCHEMA", "table": "MY_TABLE", "columns": ["col1", "col2"]}'
+        'This field is used internally',
+        **_UI_HIDDEN,
     )
-    language: str = Field('sql', **{'ui.hidden': True})
+    language: str = Field('sql', **_UI_HIDDEN)  # type: ignore[pydantic-field]
 
     @classmethod
-    def get_form(cls, connector: 'RedshiftConnector', current_config: dict[str, Any]):
-        """
-        Method to retrieve the form with a current config
-        Once the connector is set, we are able to give suggestions for the `database` field
-        """
-        default_db = current_config.get('database', DEFAULT_DATABASE)
-        return create_model(
-            'FormSchema',
-            database=strlist_to_enum('database', connector.available_dbs, default_db),
-            __base__=cls,
-        ).schema()
+    def _get_databases(cls, connector: 'SnowflakeConnector'):
+        return connector._get_databases()
+
+    @classmethod
+    def get_form(cls, connector: 'SnowflakeConnector', current_config):
+        constraints: dict[str, Any] = {}
+
+        with suppress(Exception):
+            databases = connector._get_databases()
+            warehouses = connector._get_warehouses()
+            # Restrict some fields to lists of existing counterparts
+            constraints['database'] = strlist_to_enum('database', databases)
+            constraints['warehouse'] = strlist_to_enum('warehouse', warehouses)
+
+        res = create_model('FormSchema', __base__=cls, **constraints).schema()
+        res['properties']['warehouse']['default'] = connector.default_warehouse
+        return res
 
 
-class RedshiftConnector(ToucanConnector, DiscoverableConnector):
-    data_source_model: RedshiftDataSource
+class AuthenticationMethod(str, Enum):
+    PLAIN: str = 'Snowflake (ID + Password)'
+    OAUTH: str = 'oAuth'
+
+
+class AuthenticationMethodValue(str, Enum):
+    PLAIN: str = 'snowflake'
+    OAUTH: str = 'oauth'
+
+
+@contextmanager
+def _snowflake_connection(**args: str | int | None) -> Generator[SnowflakeConnection, None, None]:
+    """Returns a Snowflake connection and automatically closes it."""
+    sf_connector.paramstyle = 'qmark'
+    conn = SnowflakeConnection(**args)
+    try:
+        yield conn
+    finally:
+        # Entire method is already wrapped in a try/except block
+        conn.close()
+
+
+class SnowflakeConnector(ToucanConnector[SnowflakeDataSource], DiscoverableConnector):
+    """
+    Import data from Snowflake data warehouse.
+    """
+
+    _sso_credentials_access: bool = True
+
+    sso_credentials_keeper: Any = None
+    user_tokens_keeper: Any = None
+
+    data_source_model: SnowflakeDataSource
+
+    account: str = Field(
+        ...,
+        description='The full name of your Snowflake account. '
+        'It might require the region and cloud platform where your account is located, '
+        'in the form of: "your_account_name.region_id.cloud_platform". See more details '
+        '<a href="https://docs.snowflake.net/manuals/user-guide/python-connector-api.html#label-account-format-info" target="_blank">here</a>.',
+        placeholder='your_account_name.region_id.cloud_platform',
+    )
+
     authentication_method: AuthenticationMethod = Field(
-        None,
+        AuthenticationMethod.PLAIN,
         title='Authentication Method',
-        description='The authentication mechanism that will be used to connect to your redshift data source',
-        **{'ui': {'checkbox': False}},
-    )
-    host: str = Field(..., description='The hostname of the Amazon Redshift cluster')
-    port: int = Field(5439, description='The listening port of your Redshift Database')
-    default_database: str = Field(
-        DEFAULT_DATABASE, description='The name of the database instance to connect to'
-    )
-    user: str | None = Field(
-        None, description='The username to use for authentication with the Amazon Redshift cluster'
-    )
-    password: SecretStr | None = Field(
-        None, description='The password to use for authentication with the Amazon Redshift cluster'
+        description='The authentication mechanism that will be used to connect to your snowflake data source',
+        ui={'checkbox': False},
     )
 
-    db_user: str | None = Field(None, description='The user ID to use with Amazon Redshift')
-    cluster_identifier: str | None = Field(
-        None, description='The cluster identifier of the Amazon Redshift cluster'
+    user: str = Field(..., description='Your login username')
+    password: SecretStr | None = Field(None, description='Your login password')
+    token_endpoint: str | None = Field(None, description='The token endpoint')
+    token_endpoint_content_type: str = Field(
+        'application/json',
+        description='The content type to use when requesting the token endpoint',
     )
 
-    connect_timeout: int | None = Field(
+    role: str | None = Field(
         None,
-        title='Connection timeout',
-        description='You can set a connection timeout in seconds here, i.e. the maximum length of '
-        'time you want to wait for the server to respond. None by default',
-    )
-    # True by default to match redshift_connector kwargs syntax
-    enable_tcp_keepalive: bool = Field(
-        True,
-        title='Enable TCP keep-alive',
-        description='You may disable TCP keep-alive by unticking this option. Disabling might be '
-        'required for long-running queries or if you are behind a firewall',
+        description='The user role that you want to connect with. '
+        'See more details <a href="https://docs.snowflake.com/en/user-guide/admin-user-management.html#user-roles" target="_blank">here</a>.',
     )
 
-    access_key_id: str | None = Field(None, description='The access key id of your aws account.')
-    secret_access_key: SecretStr | None = Field(
-        None, description='The secret access key of your aws account.'
+    default_warehouse: str | None = Field(
+        None, description='The default warehouse that shall be used for any data source'
     )
-    session_token: str | None = Field(None, description='Your session token')
-    profile: str | None = Field(None, description='AWS profile')
-    region: str | None = Field(None, description='The region in which there is your aws account.')
+    category: Category = Field(Category.SNOWFLAKE, title='category', ui={'checkbox': False})
 
     class Config:
-        underscore_attrs_are_private = True
-        keep_untouched = (cached_property,)
-
         @staticmethod
-        def schema_extra(schema: dict[str, Any]) -> None:
-            schema['properties'] = {k: schema['properties'][k] for k in ORDERED_KEYS}
+        def schema_extra(schema: dict[str, Any], model: Type['SnowflakeConnector']) -> None:
+            ordered_keys = [
+                'type',
+                'name',
+                'account',
+                'authentication_method',
+                'user',
+                'password',
+                'token_endpoint',
+                'token_endpoint_content_type',
+                'role',
+                'default_warehouse',
+                'retry_policy',
+                'secrets_storage_version',
+                'sso_credentials_keeper',
+                'user_tokens_keeper',
+            ]
+            schema['properties'] = {k: schema['properties'][k] for k in ordered_keys}
+
+    @property
+    def access_token(self) -> str | None:
+        return self.user_tokens_keeper and self.user_tokens_keeper.access_token.get_secret_value()
+
+    @property
+    def refresh_token(self) -> str | None:
+        return self.user_tokens_keeper and self.user_tokens_keeper.refresh_token.get_secret_value()
+
+    @property
+    def client_id(self) -> str | None:
+        return self.sso_credentials_keeper and self.sso_credentials_keeper.client_id
+
+    @property
+    def client_secret(self) -> str | None:
+        return (
+            self.sso_credentials_keeper
+            and self.sso_credentials_keeper.client_secret.get_secret_value()
+        )
+
+    @staticmethod
+    def _get_status_details(index: int, status: bool | None) -> list[tuple[str, bool | None]]:
+        checks = ['Connection to Snowflake', 'Default warehouse exists']
+        ok_checks: list[tuple[str, bool | None]] = [
+            (check, True) for i, check in enumerate(checks) if i < index
+        ]
+        new_check = (checks[index], status)
+        not_validated_checks: list[tuple[str, bool | None]] = [
+            (check, None) for i, check in enumerate(checks) if i > index
+        ]
+        return ok_checks + [new_check] + not_validated_checks
 
-    @cached_property
-    def available_dbs(self) -> list[str]:
-        return self._list_db_names()
-
-    @validator('host')
-    def host_validator(cls, v):
-        return re.sub(r'^https?://', '', v)
-
-    @root_validator
-    def check_requirements(cls, values):
-        mode = values.get('authentication_method')
-        if mode == AuthenticationMethod.DB_CREDENTIALS.value:
-            # TODO: Partial check due to missing context in some operations (Missing: password)
-            user = values.get('user')
-            if user is None:
-                raise ValueError(AuthenticationMethodError.DB_CREDENTIALS.value)
-        elif mode == AuthenticationMethod.AWS_CREDENTIALS.value:
-            # TODO: Partial check due to missing context in some operations (Missing: secret_access_key)
-            access_key_id, db_user = (
-                values.get('access_key_id'),
-                values.get('db_user'),
+    def get_status(self) -> ConnectorStatus:
+        try:
+            res = self._get_warehouses(self.default_warehouse)
+            if len(res) == 0:
+                return ConnectorStatus(
+                    status=False,
+                    details=self._get_status_details(1, False),
+                    error=f"The warehouse '{self.default_warehouse}' does not exist.",
+                )
+        except snowflake.connector.errors.OperationalError:
+            # Raised when the provided account does not exists or when the
+            # provided User does not have access to the provided account
+            return ConnectorStatus(
+                status=False,
+                details=self._get_status_details(0, False),
+                error=f"Connection failed for the account '{self.account}', please check the Account field",
             )
-            if access_key_id is None or db_user is None:
-                raise ValueError(AuthenticationMethodError.AWS_CREDENTIALS.value)
-        elif mode == AuthenticationMethod.AWS_PROFILE.value:
-            profile, db_user = (values.get('profile'), values.get('db_user'))
-            if profile is None or db_user is None:
-                raise ValueError(AuthenticationMethodError.AWS_PROFILE.value)
-        else:
-            raise ValueError(AuthenticationMethodError.UNKNOWN.value)
-        return values
+        except snowflake.connector.errors.ForbiddenError:
+            return ConnectorStatus(
+                status=False,
+                details=self._get_status_details(0, False),
+                error=f"Access forbidden, please check that you have access to the '{self.account}' account or try again later.",
+            )
+        except snowflake.connector.errors.ProgrammingError as e:
+            return ConnectorStatus(
+                status=False, details=self._get_status_details(0, False), error=str(e)
+            )
+        except snowflake.connector.errors.DatabaseError:
+            # Raised when the provided User/Password aren't correct
+            return ConnectorStatus(
+                status=False,
+                details=self._get_status_details(0, False),
+                error=f"Connection failed for the user '{self.user}', please check your credentials",
+            )
+
+        return ConnectorStatus(status=True, details=self._get_status_details(1, True), error=None)
+
+    def get_connection_params(self) -> dict[str, str | int]:
+        params: dict[str, str | int] = {
+            'user': Template(self.user).render(),
+            'account': self.account,
+            'authenticator': self.authentication_method,
+            # hard Snowflake params
+            'application': 'ToucanToco',
+            'client_session_keep_alive_heartbeat_frequency': 59,
+            'client_prefetch_threads': 5,
+            'session_id': self.identifier,
+        }
+
+        if params['authenticator'] == AuthenticationMethod.PLAIN and self.password:
+            params['authenticator'] = AuthenticationMethodValue.PLAIN
+            params['password'] = self.password.get_secret_value()
+
+        if self.authentication_method == AuthenticationMethod.OAUTH:
+            if self.access_token is not None:
+                params['token'] = self.access_token
+            params['authenticator'] = AuthenticationMethodValue.OAUTH
 
-    def _get_connection_params(self, database) -> dict[str, Any]:
-        con_params = dict(
-            database=database,
-            host=self.host,
-            port=self.port,
-            timeout=self.connect_timeout,
-            cluster_identifier=self.cluster_identifier,
-            tcp_keepalive=self.enable_tcp_keepalive,
+        if self.role:
+            params['role'] = self.role
+
+        return params
+
+    def _refresh_oauth_token(self):
+        """Regenerates an oauth token.
+
+        Only does so if configuration was provided and if the given token has expired.
+        """
+        if self.token_endpoint and self.refresh_token:
+            try:
+                # Here, we only want to access the expiration date, we don't care if the token is
+                # not valid. The options should be enough according to docs
+                access_token = jwt.decode(
+                    self.access_token,
+                    options={
+                        'verify_signature': False,
+                        'verify_exp': False,
+                        'verify_nbf': False,
+                        'verify_iat': False,
+                        'verify_aud': False,
+                        'verify_iss': False,
+                    },
+                )
+                is_expired = datetime.fromtimestamp(access_token['exp']) < datetime.now()
+            except Exception:
+                is_expired = True
+
+            if is_expired:
+                res = requests.post(
+                    self.token_endpoint,
+                    data={
+                        'grant_type': 'refresh_token',
+                        'client_id': self.client_id,
+                        'client_secret': self.client_secret,
+                        'refresh_token': self.refresh_token,
+                    },
+                    headers={'Content-Type': self.token_endpoint_content_type},
+                )
+                res.raise_for_status()
+
+                self.user_tokens_keeper.update_tokens(
+                    access_token=res.json().get('access_token'),
+                    refresh_token=res.json().get('refresh_token'),
+                )
+
+    def _get_connection(
+        self, database: str | None = None, warehouse: str | None = None
+    ) -> ContextManager[SnowflakeConnection]:
+        if self.authentication_method == AuthenticationMethod.OAUTH:
+            logger.info('Refreshing OAuth token...')
+            self._refresh_oauth_token()
+            logger.info('Done refreshing OAuth token')
+
+        return _snowflake_connection(
+            **self.get_connection_params(), database=database, warehouse=warehouse
         )
-        if self.authentication_method == AuthenticationMethod.DB_CREDENTIALS.value:
-            con_params['user'] = self.user
-            con_params['password'] = self.password.get_secret_value() if self.password else None
-        elif self.authentication_method == AuthenticationMethod.AWS_CREDENTIALS.value:
-            con_params['iam'] = True
-            con_params['db_user'] = self.db_user
-            con_params['access_key_id'] = self.access_key_id
-            con_params['secret_access_key'] = (
-                self.secret_access_key.get_secret_value() if self.secret_access_key else None
-            )
-            con_params['session_token'] = self.session_token
-            con_params['region'] = self.region
-        elif self.authentication_method == AuthenticationMethod.AWS_PROFILE.value:
-            con_params['iam'] = True
-            con_params['db_user'] = self.db_user
-            con_params['profile'] = self.profile
-            con_params['region'] = self.region
-        return {k: v for k, v in con_params.items() if v is not None}
-
-    def _get_connection(self, database) -> redshift_connector.Connection:
-        """Establish a connection to an Amazon Redshift cluster."""
-        con = redshift_connector.connect(
-            **self._get_connection_params(
-                database=database if database else None,
-            ),
+
+    def _set_warehouse(self, data_source: SnowflakeDataSource):
+        return (
+            data_source.copy(update={'warehouse': self.default_warehouse})
+            if not data_source.warehouse
+            else data_source
         )
-        con.autocommit = True  # see https://stackoverflow.com/q/22019154
-        con.paramstyle = 'pyformat'
-        return con
-
-    def _retrieve_tables(self, database) -> list[str]:
-        with self._get_connection(database=database).cursor() as cursor:
-            cursor.execute(TABLE_QUERY)
-            res = cursor.fetchall()
-        return [table_name for (table_name,) in res]
 
-    def _retrieve_data(
+    @overload
+    def _execute_query(
+        self,
+        query: str,
+        parameters: dict | list[str] | None = None,
+        *,
+        warehouse: str | None = None,
+        database: str | None = None,
+        as_df: Literal[True] = ...,
+        snowflake_connection: SnowflakeConnection | None = None,
+    ) -> pd.DataFrame:
+        ...  # pragma: no cover
+
+    @overload
+    def _execute_query(
+        self,
+        query: str,
+        parameters: dict | list[str] | None = None,
+        *,
+        warehouse: str | None = None,
+        database: str | None = None,
+        as_df: Literal[False],
+        snowflake_connection: SnowflakeConnection | None = None,
+    ) -> list[dict]:
+        ...  # pragma: no cover
+
+    def _execute_query(
         self,
-        datasource: RedshiftDataSource,
-        get_row_count: bool = False,
+        query: str,
+        parameters: dict | list[str] | None = None,
+        *,
+        warehouse: str | None = None,
+        database: str | None = None,
+        as_df: bool = True,
+        snowflake_connection: SnowflakeConnection | None = None,
+    ) -> pd.DataFrame | list[dict]:
+        def _execute(conn: SnowflakeConnection) -> pd.DataFrame | list[dict]:
+            curs = conn.cursor(SfDictCursor)
+            query_result = curs.execute(query, parameters)
+            assert query_result is not None
+            # snowflake typing is incomplete for DictCursor
+            results: list[dict] = query_result.fetchall()  # type:ignore[assignment]
+            return pd.DataFrame(results) if as_df else results
+
+        if snowflake_connection is not None:
+            return _execute(snowflake_connection)
+        with self._get_connection(database=database, warehouse=warehouse) as conn:
+            return _execute(conn)
+
+    def _describe_query(self, query: str) -> dict[str, str]:
+        with self._get_connection() as conn:
+            curs = conn.cursor(SfDictCursor)
+            return {r.name: _TYPE_CODE_MAPPING[r.type_code] for r in curs.describe(query)}
+
+    def _get_warehouses(self, warehouse_name: str | None = None) -> list[str]:
+        query = 'SHOW WAREHOUSES'
+        if warehouse_name:
+            query += f" LIKE '{warehouse_name}'"
+
+        result = self._execute_query(query, warehouse=warehouse_name)
+        return result['name'].to_list() if 'name' in result.columns else []
+
+    def _get_databases(self, database_name: str | None = None) -> list[str]:
+        query = 'SHOW DATABASES'
+        if database_name:
+            query += f" LIKE '{database_name}'"
+
+        result = self._execute_query(query, database=database_name)
+        return result['name'].to_list() if 'name' in result.columns else []
+
+    def _fetch_data(
+        self,
+        data_source: SnowflakeDataSource,
         offset: int | None = None,
         limit: int | None = None,
     ) -> pd.DataFrame:
-        if get_row_count:
-            prepared_query, prepared_query_parameters = SqlQueryHelper.prepare_count_query(
-                datasource.query, datasource.parameters
-            )
-        else:
-            prepared_query, prepared_query_parameters = SqlQueryHelper.prepare_limit_query(
-                datasource.query, datasource.parameters, offset, limit
-            )
-        with self._get_connection(database=datasource.database).cursor() as cursor:
-            cursor.execute(prepared_query, prepared_query_parameters)
-            result: pd.DataFrame = cursor.fetch_dataframe()
-            if result is None:
-                result = pd.DataFrame()
-        return result
+        data_source = self._set_warehouse(data_source)
+
+        prepared_query, prepared_params = SqlQueryHelper.prepare_limit_query(
+            data_source.query, data_source.parameters, offset=offset, limit=limit
+        )
+        return self._execute_query(
+            prepared_query,
+            prepared_params,
+            database=data_source.database,
+            warehouse=data_source.warehouse,
+        )
+
+    def _retrieve_data(self, data_source: SnowflakeDataSource) -> pd.DataFrame:
+        return self._fetch_data(data_source)
 
     def get_slice(
         self,
-        data_source: RedshiftDataSource,
-        permissions: dict[str, Any] | None = None,
+        data_source: SnowflakeDataSource,
+        permissions: dict | None = None,
         offset: int = 0,
         limit: int | None = None,
-        get_row_count: bool = False,
+        get_row_count: bool | None = False,
     ) -> DataSlice:
-        """
-        Method to retrieve a part of the data as a pandas dataframe
-        and the total size filtered with permissions
-        - offset is the index of the starting row
-        - limit is the number of pages to retrieve
-        Exemple: if offset = 5 and limit = 10 then 10 results are expected from 6th row
-        """
-        df: pd.DataFrame = self._retrieve_data(data_source, False, offset, limit)
-        total_returned_rows = len(df) if df is not None else 0
-
-        run_count_request = get_row_count and SqlQueryHelper.count_query_needed(data_source.query)
-
-        if run_count_request:
-            df_count: pd.DataFrame = self._retrieve_data(data_source, True)
-            total_rows = (
-                df_count.total_rows[0]
-                if df_count is not None and len(df_count.total_rows) > 0
-                else 0
-            )
-        else:
-            total_rows = total_returned_rows
-
+        # We assume permissions have been applied earlier
+        df = self._fetch_data(data_source, offset=offset, limit=limit)
         return DataSlice(
-            df,
+            df=df,
             pagination_info=build_pagination_info(
-                offset=offset,
-                limit=limit,
-                total_rows=total_rows,
-                retrieved_rows=total_returned_rows,
+                offset=0, limit=limit, total_rows=None, retrieved_rows=len(df)
             ),
         )
 
-    @staticmethod
-    def _get_details(index: int, status: bool):
-        checks = [
-            'Hostname resolved',
-            'Port opened',
-            'Authenticated',
-            'Default Database connection',
-        ]
-        ok_checks = [(c, True) for i, c in enumerate(checks) if i < index]
-        new_check = (checks[index], status)
-        not_validated_checks = [(c, False) for i, c in enumerate(checks) if i > index]
-        return ok_checks + [new_check] + not_validated_checks
-
-    def get_status(self) -> ConnectorStatus:
-        # Check hostname
-        try:
-            self.check_hostname(self.host)
-        except Exception as e:
-            return ConnectorStatus(status=False, details=self._get_details(0, False), error=str(e))
-        # Check port
-        try:
-            self.check_port(self.host, self.port)
-        except Exception as e:
-            return ConnectorStatus(status=False, details=self._get_details(1, False), error=str(e))
+    def describe(self, data_source: SnowflakeDataSource) -> dict[str, str]:
+        return self._describe_query(data_source.query)
 
-        # Basic db query
-        try:
-            redshift_connector.connect(
-                **self._get_connection_params(database=self.default_database),
-            )
-        except (Exception, redshift_connector.OperationalError) as e:
-            return ConnectorStatus(status=False, details=self._get_details(3, False), error=str(e))
-
-        return ConnectorStatus(status=True, details=self._get_details(3, True), error=None)
-
-    def describe(self, data_source: RedshiftDataSource) -> dict[str, Any]:
-        with self._get_connection(database=data_source.database).cursor() as cursor:
-            cursor.execute(DESCRIBE_QUERY.format(column=data_source.query.replace(';', '')))
-            res = cursor.description
+    def _get_unique_datasource_identifier(self, data_source: SnowflakeDataSource) -> dict[str, Any]:
+        prepared_query, prepared_query_parameters = SqlQueryHelper.prepare_query(
+            data_source.query, data_source.parameters
+        )
         return {
-            col[0].decode('utf-8') if isinstance(col[0], bytes) else col[0]: types_map.get(col[1])
-            for col in res
+            'warehouse': data_source.warehouse,
+            'database': data_source.database,
+            'query': prepared_query,
+            'parameters': prepared_query_parameters,
         }
 
-    def _db_table_info_rows(self, database: str) -> list[tuple[str, str, str, str]]:
-        with self._get_connection(database).cursor() as cursor:
-            """Get rows of (schema, table name, column name, column type)"""
-            cursor.execute(
-                r"""SELECT "schemaname", "tablename", "column", "type" FROM PG_TABLE_DEF WHERE schemaname = 'public';"""
-            )
-            return cursor.fetchall()
+    def get_model(self, db_name: str | None = None) -> list[TableInfo]:
+        if db_name is None:
+            databases = self._get_databases()
+        else:
+            databases = [db_name]
 
-    def _db_tables_info(self, database: str) -> list[tuple[str, str, str, str, str]]:
-        """Get rows of (database, schema, table name, column name, column type)"""
-        table_infos = []
-        for schema, table_name, column_name, column_type in self._db_table_info_rows(database):
-            for row in table_infos[::-1]:
-                if row['schema'] == schema and row['name'] == table_name:
-                    row['columns'].append({'name': column_name, 'type': column_type})
-                    break
-            else:
-                table_infos.append(
-                    {
-                        'database': database,
-                        'schema': schema,
-                        'name': table_name,
-                        'type': 'table',
-                        'columns': [{'name': column_name, 'type': column_type}],
-                    }
+        # We need to execute the query for every database in case None is specified
+        values: list[tuple] = []
+        for db in databases:
+            with self._get_connection(database=db) as conn:
+                values.extend(
+                    [
+                        tuple(elem.values())
+                        for elem in self._execute_query(
+                            _DB_MODEL_EXTRACTION_QUERY,
+                            database=db_name,
+                            as_df=False,
+                            snowflake_connection=conn,
+                        )
+                    ]
                 )
-        return table_infos
-
-    def get_model(self, db_name: str | None = None) -> list[TableInfo]:
-        """Retrieves the database tree structure using current connection"""
-        tables_info = []
-        for db in self.available_dbs:
-            with suppress(redshift_connector.OperationalError):
-                tables_info += self._db_tables_info(db)
-
-        return tables_info
-
-    def get_model_with_info(self, db_name: str | None = None) -> tuple[list[TableInfo], dict]:
-        """Retrieves the database tree structure using current connection"""
-        databases_tree = []
-        failed_databases = []
-        for db in self.available_dbs:
-            try:
-                databases_tree += self._list_tables_info(db)
-            except redshift_connector.OperationalError:
-                failed_databases.append(db)
-
-        tables_info = DiscoverableConnector.format_db_model(databases_tree)
-        metadata = {}
-        if failed_databases:
-            metadata['info'] = {'Could not reach databases': failed_databases}
-        return (tables_info, metadata)
-
-    def _list_db_names(self) -> list[str]:
-        with self._get_connection(database=self.default_database).cursor() as cursor:
-            # redshift has a weird system db called padb_harvest duplicating the content of 'dev' database
-            # https://bit.ly/3GQJCdy, we have to filter it
-            cursor.execute(
-                """select datname from pg_database where datistemplate = false and datname != 'padb_harvest';"""
-            )
-            return [db_name for (db_name,) in cursor.fetchall()]
 
-    def _list_tables_info(self, database: str) -> list[tuple]:
-        with self._get_cursor(database) as cursor:
-            cursor.execute(build_database_model_extraction_query())
-            return cursor.fetchall()
+        return self.format_db_model(values)  # type: ignore[arg-type]
```

### Comparing `toucan_connectors-4.4.1/toucan_connectors/redshift/utils.py` & `toucan_connectors-4.5.0/toucan_connectors/redshift/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/salesforce/salesforce-service-cloud.png` & `toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/salesforce/salesforce.jpg` & `toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/salesforce/salesforce_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/salesforce/salesforce_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png` & `toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/salesforce_sandbox/salesforce.jpg` & `toucan_connectors-4.5.0/toucan_connectors/salesforce_sandbox/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/sap_hana/sap-hana.png` & `toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap-hana.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/sap_hana/sap_hana_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/sap_hana/sap_hana_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/share_point/share_point.png` & `toucan_connectors-4.5.0/toucan_connectors/share_point/share_point.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/snowflake/snowflake.png` & `toucan_connectors-4.5.0/toucan_connectors/snowflake/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/snowflake_common.py` & `toucan_connectors-4.5.0/toucan_connectors/snowflake_common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/snowflake_oauth2/snowflake.png` & `toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/soap/helpers.py` & `toucan_connectors-4.5.0/toucan_connectors/soap/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/soap/soap.png` & `toucan_connectors-4.5.0/toucan_connectors/soap/soap.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/soap/soap_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/sql_query_helper.py` & `toucan_connectors-4.5.0/toucan_connectors/sql_query_helper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/toucan_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/toucan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/toucan_toco/toucan.png` & `toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/toucan_toco/toucan_toco_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/toucan_toco/toucan_toco_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/trello/trello.png` & `toucan_connectors-4.5.0/toucan_connectors/trello/trello.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/trello/trello_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/trello/trello_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/utils/pem.py` & `toucan_connectors-4.5.0/toucan_connectors/utils/pem.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/wootric/wootric.png` & `toucan_connectors-4.5.0/toucan_connectors/wootric/wootric.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/toucan_connectors/wootric/wootric_connector.py` & `toucan_connectors-4.5.0/toucan_connectors/wootric/wootric_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.4.1/PKG-INFO` & `toucan_connectors-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: toucan-connectors
-Version: 4.4.1
+Version: 4.5.0
 Summary: Toucan Toco Connectors
 License: BSD
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: adobe
-Provides-Extra: aircall
 Provides-Extra: all
 Provides-Extra: awsathena
 Provides-Extra: azure-mssql
 Provides-Extra: clickhouse
 Provides-Extra: dataiku
 Provides-Extra: elasticsearch
 Provides-Extra: facebook
@@ -23,42 +22,37 @@
 Provides-Extra: google-adwords
 Provides-Extra: google-analytics
 Provides-Extra: google-big-query
 Provides-Extra: google-cloud-mysql
 Provides-Extra: google-my-business
 Provides-Extra: google-sheets
 Provides-Extra: google-spreadsheet
-Provides-Extra: hive
 Provides-Extra: http-api
 Provides-Extra: hubspot
-Provides-Extra: lightspeed
 Provides-Extra: mongo
 Provides-Extra: mssql
 Provides-Extra: mssql-tlsv1-0
 Provides-Extra: mysql
 Provides-Extra: net-explorer
 Provides-Extra: odata
 Provides-Extra: odbc
 Provides-Extra: oracle-sql
 Provides-Extra: postgres
 Provides-Extra: redshift
-Provides-Extra: rok
 Provides-Extra: sap-hana
 Provides-Extra: snowflake
 Provides-Extra: soap
 Provides-Extra: toucan-toco
 Requires-Dist: Authlib (>=1.0.1,<2.0.0)
 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0)
-Requires-Dist: PyHive[hive] (>=0.6.5,<1.0) ; extra == "hive" or extra == "all"
-Requires-Dist: PyJWT (>=1.5.3,<3) ; extra == "rok" or extra == "snowflake" or extra == "all"
+Requires-Dist: PyJWT (>=1.5.3,<3) ; extra == "snowflake" or extra == "all"
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0) ; extra == "google-cloud-mysql" or extra == "mysql" or extra == "all"
 Requires-Dist: adobe-analytics (>=1.2.3,<2.0.0) ; extra == "adobe" or extra == "all"
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0) ; python_version < "3.11"
-Requires-Dist: awswrangler (>=2.15.1,<3.0.0) ; (python_version < "3.11") and (extra == "awsathena" or extra == "all")
-Requires-Dist: bearer (==3.1.0) ; extra == "aircall" or extra == "lightspeed" or extra == "all"
+Requires-Dist: awswrangler (>=3.0.0,<4.0.0) ; extra == "awsathena" or extra == "all"
+Requires-Dist: bearer (==3.1.0) ; extra == "all"
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: clickhouse-driver (>=0.2.3,<1.0) ; extra == "clickhouse" or extra == "all"
 Requires-Dist: cx-Oracle (>=8.3.0,<9.0.0) ; extra == "oracle-sql" or extra == "all"
 Requires-Dist: dataiku-api-client (>=9.0.1,<10.0.0) ; extra == "dataiku" or extra == "all"
 Requires-Dist: elasticsearch (>=7.11.0,<8) ; extra == "elasticsearch" or extra == "all"
 Requires-Dist: facebook-sdk (>=3.1.0,<4.0.0) ; extra == "facebook" or extra == "all"
 Requires-Dist: google-api-python-client (>=2,<3) ; extra == "google-analytics" or extra == "google-my-business" or extra == "google-sheets" or extra == "all"
@@ -67,31 +61,31 @@
 Requires-Dist: gspread (>=5.4.0,<6.0.0) ; extra == "google-spreadsheet" or extra == "all"
 Requires-Dist: hubspot-api-client (>=7.4.0,<8.0.0) ; extra == "hubspot" or extra == "all"
 Requires-Dist: jq (>=1.2.2,<2.0.0)
 Requires-Dist: lxml (>=4.6.5,<5.0.0) ; extra == "redshift" or extra == "soap" or extra == "all"
 Requires-Dist: oauth2client (>=4.1.3,<5.0.0) ; extra == "google-analytics" or extra == "google-spreadsheet" or extra == "all"
 Requires-Dist: oauthlib (==3.2.2) ; extra == "http-api" or extra == "odata" or extra == "all"
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0) ; extra == "net-explorer" or extra == "all"
-Requires-Dist: peakina (>=0.10.0,<0.11.0) ; extra == "all"
+Requires-Dist: peakina (>=0.11.0,<0.12.0) ; extra == "all"
 Requires-Dist: psycopg2 (>=2.7.4,<3.0.0) ; extra == "postgres" or extra == "all"
-Requires-Dist: pyarrow (<11) ; extra == "snowflake" or extra == "all"
+Requires-Dist: pyarrow (<12) ; extra == "snowflake" or extra == "all"
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pyhdb (>=0.3.4,<1.0) ; extra == "sap-hana" or extra == "all"
 Requires-Dist: pymongo (>=3.12.0) ; extra == "mongo" or extra == "all"
 Requires-Dist: pyodbc (>=4,<5) ; extra == "azure-mssql" or extra == "mssql" or extra == "mssql-tlsv1-0" or extra == "all"
 Requires-Dist: python-graphql-client (>=0.4.3,<1.0) ; extra == "github" or extra == "all"
 Requires-Dist: redshift-connector (>=2.0.907,<3.0.0) ; extra == "redshift" or extra == "all"
-Requires-Dist: requests (>=2.28.0,<3.0.0) ; extra == "rok"
+Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: requests-oauthlib (==1.3.1) ; extra == "http-api" or extra == "odata" or extra == "all"
-Requires-Dist: simplejson (>=3.17.6,<4.0.0) ; extra == "rok" or extra == "all"
+Requires-Dist: simplejson (>=3.17.6,<4.0.0) ; extra == "all"
 Requires-Dist: snowflake-connector-python (>=2.7.12,<4.0.0) ; extra == "snowflake" or extra == "all"
 Requires-Dist: tctc-odata (>=0.3,<1.0) ; extra == "odata" or extra == "all"
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: toucan-client (>=1.0.1,<2.0.0) ; extra == "toucan-toco" or extra == "all"
-Requires-Dist: toucan-data-sdk (>=7.4.2,<8.0.0)
+Requires-Dist: toucan-data-sdk (>=7.6.0,<8.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<1.0) ; extra == "http-api" or extra == "all"
 Requires-Dist: zeep (>=4.1.0,<5.0.0) ; extra == "soap" or extra == "all"
 Description-Content-Type: text/markdown
 
 [![Pypi-v](https://img.shields.io/pypi/v/toucan-connectors.svg)](https://pypi.python.org/pypi/toucan-connectors)
 [![Pypi-pyversions](https://img.shields.io/pypi/pyversions/toucan-connectors.svg)](https://pypi.python.org/pypi/toucan-connectors)
 [![Pypi-l](https://img.shields.io/pypi/l/toucan-connectors.svg)](https://pypi.python.org/pypi/toucan-connectors)
@@ -197,30 +191,30 @@
 make test
 ```
 
 Some connectors are tested using mocks (cf. `trello`), others are tested by making calls to data providers (cf. `elasticsearch`) running on the system in docker containers. The required images are in the `tests/docker-compose.yml` file, they need to be pulled (cf. `pytest --pull`) to run the relevant tests.
 
 ## Contributing
 
-This is an open source repository under the [BSD 3-Clause Licence](https://github.com/ToucanToco/toucan-connectors/blob/master/LICENSE). The Toucan Toco tech team are the maintainers of this repository, we welcome contributions. 
+This is an open source repository under the [BSD 3-Clause Licence](https://github.com/ToucanToco/toucan-connectors/blob/master/LICENSE). The Toucan Toco tech team are the maintainers of this repository, we welcome contributions.
 
 At the moment the main use of this code is its integration into Toucan Toco commercially licenced software, as a result our dev and maintenance efforts applied here are mostly driven by Toucan Toco internal priorities.
 
 The starting point of a contribution should be an [Issue](https://github.com/ToucanToco/toucan-connectors/issues), either one you create or an existing one. This allows us (maintainers) to discuss the contribution before it is produced and avoids back and forth in reviews or stalled pull requests.
 
 ### Step 1: Generate base classes and tests files
 
 To generate the connector and test modules from boilerplate, run:
 
 ```
 make new_connector type=mytype
 ```
 
 `mytype` should be the name of a system we would like to build a connector for,
-such as `MySQL` or `Hive` or `Magento`.
+such as `MySQL` or `Magento`.
 
 Open the folder in `tests` for the new connector. You can start writing your tests before implementing it.
 
 Some connectors are tested with calls to the actual data systems that they target,
 for example `elasticsearch`, `mongo`, `mssql`.
 
 Others are tested with mocks of the
```

