# Comparing `tmp/sageworks-0.1.4.tar.gz` & `tmp/sageworks-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.1.4.tar", last modified: Mon Apr 10 15:37:11 2023, max compression
+gzip compressed data, was "sageworks-0.1.4.1.tar", last modified: Sun Apr 23 23:38:24 2023, max compression
```

## Comparing `sageworks-0.1.4.tar` & `sageworks-0.1.4.1.tar`

### file list

```diff
@@ -1,230 +1,266 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.288786 sageworks-0.1.4/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.253556 sageworks-0.1.4/.github/
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.4/.github/dependabot.yml
--rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.4/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.4/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1302 2022-12-06 17:43:49.000000 sageworks-0.1.4/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     6001 2023-04-10 15:37:11.288884 sageworks-0.1.4/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     5264 2023-04-10 15:00:10.000000 sageworks-0.1.4/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.4/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.248042 sageworks-0.1.4/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.253742 sageworks-0.1.4/applications/aws_dashboard/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.254240 sageworks-0.1.4/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12208 2023-04-07 02:17:27.000000 sageworks-0.1.4/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.4/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     1066 2023-04-07 21:10:26.000000 sageworks-0.1.4/applications/aws_dashboard/aws_dashboard.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.255511 sageworks-0.1.4/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.256675 sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/
--rw-r--r--   0 briford    (501) staff       (20)      890 2023-04-07 00:00:26.000000 sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      866 2023-04-07 21:24:49.000000 sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)      890 2023-04-07 00:05:02.000000 sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     1770 2023-04-07 16:07:22.000000 sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/main_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4679 2023-04-07 20:26:10.000000 sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/models_callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.257123 sageworks-0.1.4/applications/aws_dashboard/pages/data/
--rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.4/applications/aws_dashboard/pages/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.4/applications/aws_dashboard/pages/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     1620 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/aws_dashboard/pages/data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)     1413 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/aws_dashboard/pages/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     1510 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/aws_dashboard/pages/feature_sets.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.258085 sageworks-0.1.4/applications/aws_dashboard/pages/layout/
--rw-r--r--   0 briford    (501) staff       (20)     1288 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/aws_dashboard/pages/layout/data_sources_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.4/applications/aws_dashboard/pages/layout/endpoints_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/aws_dashboard/pages/layout/feature_sets_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.4/applications/aws_dashboard/pages/layout/main_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2341 2023-04-09 22:27:31.000000 sageworks-0.1.4/applications/aws_dashboard/pages/layout/models_layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/aws_dashboard/pages/main.py
--rw-r--r--   0 briford    (501) staff       (20)     2517 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/aws_dashboard/pages/models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.258814 sageworks-0.1.4/applications/hello_world/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4/applications/hello_world/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2140 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/hello_world/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.4/applications/hello_world/layout.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.259335 sageworks-0.1.4/applications/model_viewer/
--rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4/applications/model_viewer/callbacks.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.259689 sageworks-0.1.4/applications/model_viewer/data/
--rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.4/applications/model_viewer/data/toy_data.csv
--rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.4/applications/model_viewer/data/toy_scores.json
--rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.4/applications/model_viewer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2500 2023-04-09 21:27:30.000000 sageworks-0.1.4/applications/model_viewer/model_viewer.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.260424 sageworks-0.1.4/applications/web_admin/
--rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.4/applications/web_admin/flask_test.py
--rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.4/applications/web_admin/hello-world-http-test.ini
--rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.4/applications/web_admin/hello-world.ini
--rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.4/applications/web_admin/hello-world.service
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.260665 sageworks-0.1.4/applications/web_admin/nginx_conf/
--rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.4/applications/web_admin/nginx_conf/nginx.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.261546 sageworks-0.1.4/data/
--rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.4/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)      216 2023-04-02 19:30:59.000000 sageworks-0.1.4/data/test_data.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.262349 sageworks-0.1.4/docs/
--rw-r--r--   0 briford    (501) staff       (20)     1770 2023-03-14 15:41:27.000000 sageworks-0.1.4/docs/admin_notes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.267823 sageworks-0.1.4/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.4/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.4/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.4/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.4/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.4/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.4/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.4/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.4/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.4/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.4/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.4/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.4/docs/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.4/docs/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.268657 sageworks-0.1.4/examples/
--rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.4/examples/data_to_data_example.py
--rw-r--r--   0 briford    (501) staff       (20)      121 2023-04-05 21:18:09.000000 sageworks-0.1.4/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.269088 sageworks-0.1.4/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.4/scripts/data_source_tags.py
--rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.4/scripts/list_data_sources.py
--rw-r--r--   0 briford    (501) staff       (20)      527 2023-04-10 15:37:11.289198 sageworks-0.1.4/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1725 2023-04-10 15:37:01.000000 sageworks-0.1.4/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.248715 sageworks-0.1.4/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.269264 sageworks-0.1.4/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)      148 2023-04-02 18:05:33.000000 sageworks-0.1.4/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.269998 sageworks-0.1.4/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.248942 sageworks-0.1.4/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.270089 sageworks-0.1.4/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.4/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.270312 sageworks-0.1.4/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.4/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.249107 sageworks-0.1.4/src/sageworks/algorithms/table/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.270525 sageworks-0.1.4/src/sageworks/algorithms/table/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.4/src/sageworks/algorithms/table/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.271403 sageworks-0.1.4/src/sageworks/algorithms/table/light/
--rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.4/src/sageworks/algorithms/table/light/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.4/src/sageworks/algorithms/table/light/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/algorithms/table/light/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/algorithms/table/light/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.271949 sageworks-0.1.4/src/sageworks/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.4/src/sageworks/artifacts/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.4/src/sageworks/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4087 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/artifacts/artifact.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.272549 sageworks-0.1.4/src/sageworks/artifacts/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/artifacts/data_sources/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7423 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/artifacts/data_sources/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)     1567 2023-04-08 22:38:35.000000 sageworks-0.1.4/src/sageworks/artifacts/data_sources/data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.272907 sageworks-0.1.4/src/sageworks/artifacts/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/artifacts/endpoints/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9539 2023-04-10 01:56:00.000000 sageworks-0.1.4/src/sageworks/artifacts/endpoints/endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.273238 sageworks-0.1.4/src/sageworks/artifacts/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/artifacts/feature_sets/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9909 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/artifacts/feature_sets/feature_set.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.273563 sageworks-0.1.4/src/sageworks/artifacts/models/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/artifacts/models/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4339 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/artifacts/models/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.274023 sageworks-0.1.4/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     6135 2023-04-02 19:53:47.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)     6521 2023-04-09 21:30:08.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.275438 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2269 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     6063 2023-04-02 19:53:47.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     2722 2023-04-02 18:05:33.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     7280 2023-04-09 21:30:08.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3587 2023-04-09 21:30:08.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     2608 2023-04-02 19:53:47.000000 sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.275993 sageworks-0.1.4/src/sageworks/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.4/src/sageworks/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.249759 sageworks-0.1.4/src/sageworks/transforms/data_loaders/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.276248 sageworks-0.1.4/src/sageworks/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)     2785 2023-04-02 19:53:47.000000 sageworks-0.1.4/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.276662 sageworks-0.1.4/src/sageworks/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)     2657 2023-04-09 23:22:33.000000 sageworks-0.1.4/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2558 2023-04-09 23:22:33.000000 sageworks-0.1.4/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.276901 sageworks-0.1.4/src/sageworks/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.276992 sageworks-0.1.4/src/sageworks/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.277095 sageworks-0.1.4/src/sageworks/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.277342 sageworks-0.1.4/src/sageworks/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.277880 sageworks-0.1.4/src/sageworks/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1805 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2336 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.278178 sageworks-0.1.4/src/sageworks/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.278272 sageworks-0.1.4/src/sageworks/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.278445 sageworks-0.1.4/src/sageworks/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.278672 sageworks-0.1.4/src/sageworks/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.279085 sageworks-0.1.4/src/sageworks/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2585 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     2994 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.279215 sageworks-0.1.4/src/sageworks/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.4/src/sageworks/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.250623 sageworks-0.1.4/src/sageworks/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.279305 sageworks-0.1.4/src/sageworks/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.4/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.279521 sageworks-0.1.4/src/sageworks/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.4/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.279780 sageworks-0.1.4/src/sageworks/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7422 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.280319 sageworks-0.1.4/src/sageworks/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.4/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)     4801 2023-04-09 21:15:55.000000 sageworks-0.1.4/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.280655 sageworks-0.1.4/src/sageworks/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4/src/sageworks/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2818 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.281680 sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)     2738 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3137 2023-04-10 02:01:41.000000 sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     2950 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)     8981 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4611 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5039 2023-04-09 22:14:00.000000 sageworks-0.1.4/src/sageworks/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.283454 sageworks-0.1.4/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.4/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3961 2023-04-04 03:03:27.000000 sageworks-0.1.4/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1121 2023-04-05 21:18:09.000000 sageworks-0.1.4/src/sageworks/utils/iso_8601.py
--rw-r--r--   0 briford    (501) staff       (20)     5882 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-02 18:05:33.000000 sageworks-0.1.4/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.4/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.4/src/sageworks/utils/sageworks_sqs.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.283964 sageworks-0.1.4/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)    13175 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/views/artifacts_summary.py
--rw-r--r--   0 briford    (501) staff       (20)     1171 2023-04-05 21:18:09.000000 sageworks-0.1.4/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.286349 sageworks-0.1.4/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      731 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/web_components/box_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.4/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/web_components/feature_details.py
--rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.4/src/sageworks/web_components/feature_importance.py
--rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.4/src/sageworks/web_components/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.4/src/sageworks/web_components/model_data.py
--rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.4/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.4/src/sageworks/web_components/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     1808 2023-04-07 15:59:10.000000 sageworks-0.1.4/src/sageworks/web_components/table.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.269892 sageworks-0.1.4/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     6001 2023-04-10 15:37:11.000000 sageworks-0.1.4/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     7405 2023-04-10 15:37:11.000000 sageworks-0.1.4/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2023-04-10 15:37:11.000000 sageworks-0.1.4/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       92 2023-04-10 15:37:11.000000 sageworks-0.1.4/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2023-04-10 15:37:11.000000 sageworks-0.1.4/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.286585 sageworks-0.1.4/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.287284 sageworks-0.1.4/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1169 2023-04-02 18:05:33.000000 sageworks-0.1.4/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1637 2023-04-09 21:15:55.000000 sageworks-0.1.4/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1095 2023-04-02 18:05:33.000000 sageworks-0.1.4/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.4/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.287700 sageworks-0.1.4/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      347 2023-04-01 21:56:16.000000 sageworks-0.1.4/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      682 2023-04-02 18:05:33.000000 sageworks-0.1.4/tests/aws_account/aws_service_broker_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1575 2023-04-09 22:14:00.000000 sageworks-0.1.4/tests/create_sageworks_objs_for_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-10 15:37:11.288495 sageworks-0.1.4/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      574 2023-04-09 22:14:00.000000 sageworks-0.1.4/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      704 2023-04-09 22:14:00.000000 sageworks-0.1.4/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2023-04-09 22:14:00.000000 sageworks-0.1.4/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      662 2023-04-09 22:14:00.000000 sageworks-0.1.4/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      648 2023-04-09 22:03:48.000000 sageworks-0.1.4/tests/transforms/pandas_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      514 2023-04-09 21:27:16.000000 sageworks-0.1.4/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.186098 sageworks-0.1.4.1/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.125592 sageworks-0.1.4.1/.github/
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-04-03 17:04:32.000000 sageworks-0.1.4.1/.github/dependabot.yml
+-rw-r--r--   0 briford    (501) staff       (20)     1899 2023-03-25 19:33:37.000000 sageworks-0.1.4.1/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      281 2023-03-28 23:51:00.000000 sageworks-0.1.4.1/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2023-02-17 22:10:33.000000 sageworks-0.1.4.1/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1385 2023-04-20 18:56:17.000000 sageworks-0.1.4.1/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     5902 2023-04-23 23:38:24.186185 sageworks-0.1.4.1/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     5163 2023-04-15 19:49:43.000000 sageworks-0.1.4.1/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-04-03 17:04:32.000000 sageworks-0.1.4.1/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.119883 sageworks-0.1.4.1/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.125777 sageworks-0.1.4.1/applications/aws_dashboard/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.126453 sageworks-0.1.4.1/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12208 2023-04-07 02:17:27.000000 sageworks-0.1.4.1/applications/aws_dashboard/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-03-21 14:30:06.000000 sageworks-0.1.4.1/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     1066 2023-04-07 21:10:26.000000 sageworks-0.1.4.1/applications/aws_dashboard/aws_dashboard.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.127837 sageworks-0.1.4.1/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.128955 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/
+-rw-r--r--   0 briford    (501) staff       (20)      928 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      904 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)      928 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     1776 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4717 2023-04-12 21:48:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.129430 sageworks-0.1.4.1/applications/aws_dashboard/pages/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1867 2023-04-08 01:44:28.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-04-05 23:27:13.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     1620 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)     1413 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     1510 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/feature_sets.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.130513 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/
+-rw-r--r--   0 briford    (501) staff       (20)     1288 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/data_sources_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1143 2023-04-09 22:27:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/endpoints_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1286 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/feature_sets_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1584 2023-04-07 15:53:06.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/main_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2341 2023-04-09 22:27:31.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/models_layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/main.py
+-rw-r--r--   0 briford    (501) staff       (20)     2517 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/aws_dashboard/pages/models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.131082 sageworks-0.1.4.1/applications/hello_world/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/hello_world/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2140 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/hello_world/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)     1060 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/hello_world/layout.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.131818 sageworks-0.1.4.1/applications/model_viewer/
+-rw-r--r--   0 briford    (501) staff       (20)     3870 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/model_viewer/callbacks.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.132317 sageworks-0.1.4.1/applications/model_viewer/data/
+-rw-r--r--   0 briford    (501) staff       (20)     1849 2023-03-12 02:23:08.000000 sageworks-0.1.4.1/applications/model_viewer/data/toy_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)      597 2023-03-12 02:23:08.000000 sageworks-0.1.4.1/applications/model_viewer/data/toy_scores.json
+-rw-r--r--   0 briford    (501) staff       (20)     3069 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/model_viewer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2500 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/applications/model_viewer/model_viewer.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.133090 sageworks-0.1.4.1/applications/web_admin/
+-rw-r--r--   0 briford    (501) staff       (20)      213 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/applications/web_admin/flask_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      201 2023-03-03 22:18:34.000000 sageworks-0.1.4.1/applications/web_admin/hello-world-http-test.ini
+-rw-r--r--   0 briford    (501) staff       (20)      235 2023-03-03 22:19:17.000000 sageworks-0.1.4.1/applications/web_admin/hello-world.ini
+-rw-r--r--   0 briford    (501) staff       (20)      399 2023-03-03 22:20:51.000000 sageworks-0.1.4.1/applications/web_admin/hello-world.service
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.133322 sageworks-0.1.4.1/applications/web_admin/nginx_conf/
+-rw-r--r--   0 briford    (501) staff       (20)      486 2023-03-03 22:17:39.000000 sageworks-0.1.4.1/applications/web_admin/nginx_conf/nginx.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.133865 sageworks-0.1.4.1/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3926 2023-04-22 20:31:36.000000 sageworks-0.1.4.1/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-22 20:11:28.000000 sageworks-0.1.4.1/aws_setup/aws_account_check_deep.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.135629 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      960 2023-04-20 18:09:55.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2023-04-20 17:46:12.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.135957 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/sageworks_sandbox/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/sageworks_sandbox/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      503 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/sageworks_sandbox/sageworks_sandbox_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.136237 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.136418 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      549 2023-04-20 17:45:20.000000 sageworks-0.1.4.1/aws_setup/sageworks_sandbox/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.136726 sageworks-0.1.4.1/config/
+-rw-r--r--   0 briford    (501) staff       (20)      148 2023-04-13 17:23:15.000000 sageworks-0.1.4.1/config/sageworks_config.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.138328 sageworks-0.1.4.1/data/
+-rw-r--r--   0 briford    (501) staff       (20)   196156 2023-03-26 18:42:12.000000 sageworks-0.1.4.1/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)      613 2023-04-18 16:23:14.000000 sageworks-0.1.4.1/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-04-19 19:55:29.000000 sageworks-0.1.4.1/data/test_data.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.139164 sageworks-0.1.4.1/docs/
+-rw-r--r--   0 briford    (501) staff       (20)     1770 2023-03-14 15:41:27.000000 sageworks-0.1.4.1/docs/admin_notes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.145110 sageworks-0.1.4.1/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2022-12-06 17:43:49.000000 sageworks-0.1.4.1/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-01-15 22:00:05.000000 sageworks-0.1.4.1/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-03-06 20:35:02.000000 sageworks-0.1.4.1/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-03-06 20:33:32.000000 sageworks-0.1.4.1/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-03-06 20:31:13.000000 sageworks-0.1.4.1/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-03-06 20:40:25.000000 sageworks-0.1.4.1/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-01-15 21:19:16.000000 sageworks-0.1.4.1/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-03-10 19:48:12.000000 sageworks-0.1.4.1/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-01-15 21:23:57.000000 sageworks-0.1.4.1/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-01-12 16:00:43.000000 sageworks-0.1.4.1/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2022-12-06 17:43:49.000000 sageworks-0.1.4.1/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)      667 2023-03-15 14:00:32.000000 sageworks-0.1.4.1/docs/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2023-03-13 14:45:22.000000 sageworks-0.1.4.1/docs/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.145901 sageworks-0.1.4.1/examples/
+-rw-r--r--   0 briford    (501) staff       (20)     1240 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/examples/data_to_data_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.146230 sageworks-0.1.4.1/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   236764 2023-04-20 18:57:28.000000 sageworks-0.1.4.1/notebooks/ML_Pipeline_with_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.152342 sageworks-0.1.4.1/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-04-14 22:52:23.000000 sageworks-0.1.4.1/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-04-14 22:50:14.000000 sageworks-0.1.4.1/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-04-14 23:47:56.000000 sageworks-0.1.4.1/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-04-15 00:30:02.000000 sageworks-0.1.4.1/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-04-15 16:18:02.000000 sageworks-0.1.4.1/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-04-15 16:17:49.000000 sageworks-0.1.4.1/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      173 2023-04-17 20:59:36.000000 sageworks-0.1.4.1/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.153321 sageworks-0.1.4.1/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1373 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/scripts/data_source_tags.py
+-rw-r--r--   0 briford    (501) staff       (20)     1533 2023-04-23 22:12:54.000000 sageworks-0.1.4.1/scripts/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1306 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/scripts/list_data_sources.py
+-rw-r--r--   0 briford    (501) staff       (20)      527 2023-04-23 23:38:24.186503 sageworks-0.1.4.1/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1772 2023-04-23 23:38:12.000000 sageworks-0.1.4.1/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.120819 sageworks-0.1.4.1/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.153493 sageworks-0.1.4.1/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)      853 2023-04-22 21:03:48.000000 sageworks-0.1.4.1/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154218 sageworks-0.1.4.1/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.121028 sageworks-0.1.4.1/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154302 sageworks-0.1.4.1/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-03-05 20:00:31.000000 sageworks-0.1.4.1/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154521 sageworks-0.1.4.1/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-03-05 19:59:59.000000 sageworks-0.1.4.1/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.121187 sageworks-0.1.4.1/src/sageworks/algorithms/table/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154743 sageworks-0.1.4.1/src/sageworks/algorithms/table/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      169 2023-03-05 20:04:10.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.155642 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/
+-rw-r--r--   0 briford    (501) staff       (20)       95 2023-03-05 20:05:08.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1751 2023-04-05 21:18:09.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     9476 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/algorithms/table/light/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.156284 sageworks-0.1.4.1/src/sageworks/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2023-03-05 21:06:58.000000 sageworks-0.1.4.1/src/sageworks/artifacts/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-04-01 03:28:03.000000 sageworks-0.1.4.1/src/sageworks/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4542 2023-04-19 17:15:47.000000 sageworks-0.1.4.1/src/sageworks/artifacts/artifact.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.157134 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7447 2023-04-19 17:02:05.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2000 2023-04-19 17:23:07.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     1625 2023-04-19 17:34:03.000000 sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/data_source_abstract.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.157450 sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9826 2023-04-19 16:14:58.000000 sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.157781 sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    11500 2023-04-19 16:37:35.000000 sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/feature_set.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.158138 sageworks-0.1.4.1/src/sageworks/artifacts/models/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/artifacts/models/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4288 2023-04-19 16:37:35.000000 sageworks-0.1.4.1/src/sageworks/artifacts/models/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.158631 sageworks-0.1.4.1/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     6953 2023-04-14 22:13:26.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)     7200 2023-04-17 17:05:59.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.168627 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-14 19:44:44.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4186 2023-04-14 17:50:25.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     1512 2023-04-19 17:04:31.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     6063 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     2722 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     7280 2023-04-09 21:30:08.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3587 2023-04-09 21:30:08.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     2574 2023-04-22 20:48:49.000000 sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.171275 sageworks-0.1.4.1/src/sageworks/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2023-03-17 17:39:22.000000 sageworks-0.1.4.1/src/sageworks/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.121799 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.171573 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)     3841 2023-04-23 23:15:11.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172302 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)     2997 2023-04-14 22:16:23.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2483 2023-04-19 22:41:04.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4140 2023-04-18 20:16:32.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172682 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172778 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.172867 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:15:48.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.173132 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:16:45.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.173677 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2047 2023-04-19 22:49:17.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2346 2023-04-19 21:48:41.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.173939 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.174057 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.174172 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:14.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.174459 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:14.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175161 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2585 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     3000 2023-04-18 02:49:29.000000 sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175448 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 18:06:15.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.122746 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175571 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2023-03-15 02:18:46.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.175817 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2023-03-15 02:18:46.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.176111 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7866 2023-04-19 18:49:44.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.176643 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)        8 2023-03-25 02:07:31.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)     5179 2023-04-18 16:01:35.000000 sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.177002 sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 15:16:30.000000 sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2818 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.178346 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     2745 2023-04-13 18:18:49.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3144 2023-04-13 18:18:49.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     7073 2023-04-19 22:49:17.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     9472 2023-04-19 16:44:04.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4611 2023-04-19 22:02:24.000000 sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5439 2023-04-19 17:02:05.000000 sageworks-0.1.4.1/src/sageworks/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.180455 sageworks-0.1.4.1/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-03-16 02:34:19.000000 sageworks-0.1.4.1/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3961 2023-04-04 03:03:27.000000 sageworks-0.1.4.1/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     5113 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2023-04-05 21:18:09.000000 sageworks-0.1.4.1/src/sageworks/utils/iso_8601.py
+-rw-r--r--   0 briford    (501) staff       (20)     6168 2023-04-11 20:47:59.000000 sageworks-0.1.4.1/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3618 2023-04-17 19:53:54.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_config.py
+-rw-r--r--   0 briford    (501) staff       (20)     3558 2023-04-12 15:59:21.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)      531 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2209 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/utils/sageworks_sqs.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.180894 sageworks-0.1.4.1/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)    12080 2023-04-19 17:03:51.000000 sageworks-0.1.4.1/src/sageworks/views/artifacts_summary.py
+-rw-r--r--   0 briford    (501) staff       (20)     1296 2023-04-19 17:02:05.000000 sageworks-0.1.4.1/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.182980 sageworks-0.1.4.1/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      731 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/box_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     1661 2023-04-08 01:37:21.000000 sageworks-0.1.4.1/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     1247 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/feature_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      815 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/web_components/feature_importance.py
+-rw-r--r--   0 briford    (501) staff       (20)     1182 2023-04-07 23:04:10.000000 sageworks-0.1.4.1/src/sageworks/web_components/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     1507 2023-04-09 21:30:08.000000 sageworks-0.1.4.1/src/sageworks/web_components/model_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     1703 2023-04-02 19:53:47.000000 sageworks-0.1.4.1/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1551 2023-04-09 21:27:30.000000 sageworks-0.1.4.1/src/sageworks/web_components/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     1808 2023-04-07 15:59:10.000000 sageworks-0.1.4.1/src/sageworks/web_components/table.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.154122 sageworks-0.1.4.1/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     5902 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     8651 2023-04-23 23:38:24.000000 sageworks-0.1.4.1/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)      124 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2023-04-23 23:38:23.000000 sageworks-0.1.4.1/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.183230 sageworks-0.1.4.1/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.184282 sageworks-0.1.4.1/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1169 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1483 2023-04-11 20:37:15.000000 sageworks-0.1.4.1/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1095 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.184713 sageworks-0.1.4.1/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      347 2023-04-12 21:35:42.000000 sageworks-0.1.4.1/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      682 2023-04-02 18:05:33.000000 sageworks-0.1.4.1/tests/aws_account/aws_service_broker_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     3341 2023-04-19 17:23:07.000000 sageworks-0.1.4.1/tests/create_sageworks_objs_for_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2023-04-23 23:38:24.185813 sageworks-0.1.4.1/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      574 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      704 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      662 2023-04-09 22:14:00.000000 sageworks-0.1.4.1/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      648 2023-04-09 22:03:48.000000 sageworks-0.1.4.1/tests/transforms/pandas_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      729 2023-04-13 21:22:54.000000 sageworks-0.1.4.1/tox.ini
```

### Comparing `sageworks-0.1.4/.gitignore` & `sageworks-0.1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/LICENSE` & `sageworks-0.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/Makefile` & `sageworks-0.1.4.1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 	@echo "test - run tests quickly with the default Python"
 	@echo "test-all - run tests on every Python version with tox"
 	@echo "coverage - check code coverage quickly with the default Python"
 	@echo "docs - generate Sphinx HTML documentation, including API docs"
 	@echo "release - package and upload a release"
 	@echo "sdist - package"
 
-clean: clean-build clean-pyc
+clean: clean-build clean-pyc clean-misc
 
 clean-build:
 	find . -name 'build' -exec rm -rf {} +
 	find . -name '_build' -exec rm -rf {} +
 	find . -name 'dist' -exec rm -rf {} +
 	find . -name '*.egg-info' -exec rm -rf {} +
 	find . -name '*.tar.gz' -exec rm -rf {} +
@@ -25,19 +25,22 @@
 	find . -name '__pycache__' -exec rm -rf {} +
 
 clean-pyc:
 	find . -name '*.pyc' -exec rm -rf {} +
 	find . -name '*.pyo' -exec rm -rf {} +
 	find . -name '*~' -exec rm -rf {} +
 
+clean-misc:
+	find . -name '.ipynb_checkpoints' -exec rm -rf {} +
+
 lint:
-	flake8 src tests
+	flake8 src/sageworks tests
 
 test:
-	py.test
+	tox
 
 test-all:
 	tox
 
 release: clean
 	python setup.py sdist upload
 	python setup.py bdist_wheel upload
```

### Comparing `sageworks-0.1.4/PKG-INFO` & `sageworks-0.1.4.1/Readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,20 @@
-Metadata-Version: 2.1
-Name: sageworks
-Version: 0.1.4
-Summary: SageWorks: An easy to use WorkBench for creating and deploying SageMaker Models
-Home-page: https://github.com/SuperCowPowers/sageworks
-Author: SuperCowPowers LLC
-Author-email: support@supercowpowers.com
-License: MIT
-Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img align="left" src="docs/images/scp.png" width="180">
 
 # SageWorks<sup><i>TM</i></sup>
 
 #### SageWorks: The scientist's workbench powered by AWS® for scalability, flexibility, and security.
 
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
 <img src="docs/images/sageworks_concepts.png">
 
 ### Full SageWorks OverView
 [SageWorks Architected FrameWork](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing)
 
-### Getting Started Video Demo
-[SageWorks Getting Started](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) This video is an informal screen capture + chatting while I'm coding. The video demonstrates creating an entire AWS ML Pipeline, from data ingestion, to feature sets, to models and endpoints.
-
-
 
 ## Why SageWorks?
 
 <img align="right" src="docs/images/graph_representation.png" width="300">
 
 - The AWS SageMaker® ecosystem is **awesome** but has a large number of services with significant complexity
 - SageWorks provides **rapid prototyping** through easy to use **classes** and **transforms**
@@ -49,27 +27,26 @@
 
 **Single pane of glass** visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
 
 <img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
-## Installation
-```
-pip install sageworks
-```
-
-### Gettting Started
-SageWorks has a large number of classes and components, the best place to get started is our [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) and [SageWorks Wiki](https://github.com/SuperCowPowers/sageworks/wiki) for developers wanting to try out the Python API. 
 
-Video: [SageWorks Getting Started](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) shows an informal screen capture + chatting while I'm coding. The video demonstrates creating an entire AWS ML Pipeline, from data ingestion, to feature sets, to models and endpoints.
+## Getting Started
+- [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
+- [Initial Setup and Installation](https://github.com/SuperCowPowers/sageworks/wiki/Initial-Setup-and-Installation) for initial AWS/config/repository set up. 
+- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
+- [Coding with SageWorks Video](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
+- Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
-You can also join us on Discord <https://discord.gg/WHAJuz8sw8> for questions and advice on using SageWorks within your organization.
+### SageWorks Analysis Notebooks
+- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from Start to Finish
 
-### SageWorks Zen``
+### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
 - SageWorks Classes encapsulate, organize, and manage sets of AWS® Services.
 - **Heavy** transforms typically use **[AWS Athena](https://aws.amazon.com/athena/)** or **[Apache Spark](https://spark.apache.org/)** (AWS Glue/EMR Serverless).
 - **Light** transforms will typically use **[Pandas](https://pandas.pydata.org/)**.
 - Heavy and Light transforms both update **AWS Artifacts** (collections of AWS Services).
 - **Quick prototypes** are typically built with the **light path** and then flipped to the **heavy path** as the system matures and usage grows.
```

### Comparing `sageworks-0.1.4/applications/aws_dashboard/assets/custom.css` & `sageworks-0.1.4.1/applications/aws_dashboard/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/aws_dashboard.py` & `sageworks-0.1.4.1/applications/aws_dashboard/aws_dashboard.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/data_sources_callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,9 +13,10 @@
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_data_sources_table(app: Dash, sageworks_artifacts: ArtifactsSummary):
     @app.callback(Output("DATA_SOURCES_DETAILS", "data"), Input("data-sources-updater", "n_intervals"))
     def data_sources_update(n):
         print("Calling DataSources Refresh...")
+        sageworks_artifacts.refresh()
         data_sources = sageworks_artifacts.data_sources_summary()
         return data_sources.to_dict("records")
```

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/endpoints_callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,9 +13,10 @@
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_endpoints_table(app: Dash, sageworks_artifacts: ArtifactsSummary):
     @app.callback(Output("ENDPOINTS_DETAILS", "data"), Input("endpoints-updater", "n_intervals"))
     def data_sources_update(n):
         print("Calling FeatureSets Refresh...")
+        sageworks_artifacts.refresh()
         endpoints = sageworks_artifacts.endpoints_summary()
         return endpoints.to_dict("records")
```

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/feature_sets_callbacks.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,9 +13,10 @@
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_feature_sets_table(app: Dash, sageworks_artifacts: ArtifactsSummary):
     @app.callback(Output("FEATURE_SETS_DETAILS", "data"), Input("feature-sets-updater", "n_intervals"))
     def data_sources_update(n):
         print("Calling FeatureSets Refresh...")
+        sageworks_artifacts.refresh()
         feature_sets = sageworks_artifacts.feature_sets_summary()
         return feature_sets.to_dict("records")
```

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/main_callbacks.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/main_callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 # SageWorks Imports
 from sageworks.views.artifacts_summary import ArtifactsSummary
 
 # Cheese Sauce
 all_data = None
 
 
-def update_last_updated(app: Dash, artifacts_summary: ArtifactsSummary):
+def update_last_updated(app: Dash, sageworks_artifacts: ArtifactsSummary):
     @app.callback(Output("last-updated", "children"), Input("main-updater", "n_intervals"))
     def time_updated(n):
         global all_data
         print("Calling ALL Artifact Refresh...")
-        artifacts_summary.refresh()
-        all_data = artifacts_summary.view_data()
+        sageworks_artifacts.refresh()
+        all_data = sageworks_artifacts.view_data()
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_artifact_tables(app: Dash):
     @app.callback(Output("INCOMING_DATA", "data"), Input("main-updater", "n_intervals"))
     def incoming_data_update(n):
         incoming_data = all_data["INCOMING_DATA"]
```

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/callbacks/models_callbacks.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/callbacks/models_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         return datetime.now().strftime("Last Updated: %Y-%m-%d %H:%M:%S")
 
 
 def update_models_table(app: Dash, sageworks_artifacts: ArtifactsSummary):
     @app.callback(Output("models_table", "data"), Input("models-updater", "n_intervals"))
     def data_sources_update(n):
         print("Calling DataSources Refresh...")
+        sageworks_artifacts.refresh()
         models = sageworks_artifacts.models_summary()
         return models.to_dict("records")
 
 
 # Highlights the selected row in the table
 def table_row_select(app: Dash, table_name: str):
     @app.callback(
```

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/data/toy_data.csv` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/data/toy_scores.json` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/data_sources.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/data_sources.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/endpoints.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/feature_sets.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/feature_sets.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/layout/data_sources_layout.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/data_sources_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/layout/endpoints_layout.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/endpoints_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/layout/feature_sets_layout.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/feature_sets_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/layout/main_layout.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/main_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/layout/models_layout.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/layout/models_layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/main.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/main.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/aws_dashboard/pages/models.py` & `sageworks-0.1.4.1/applications/aws_dashboard/pages/models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/hello_world/callbacks.py` & `sageworks-0.1.4.1/applications/hello_world/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/hello_world/hello_world.py` & `sageworks-0.1.4.1/applications/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/hello_world/layout.py` & `sageworks-0.1.4.1/applications/hello_world/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/model_viewer/callbacks.py` & `sageworks-0.1.4.1/applications/model_viewer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/model_viewer/data/toy_data.csv` & `sageworks-0.1.4.1/applications/model_viewer/data/toy_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/model_viewer/data/toy_scores.json` & `sageworks-0.1.4.1/applications/model_viewer/data/toy_scores.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/model_viewer/layout.py` & `sageworks-0.1.4.1/applications/model_viewer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/applications/model_viewer/model_viewer.py` & `sageworks-0.1.4.1/applications/model_viewer/model_viewer.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/data/abalone.csv` & `sageworks-0.1.4.1/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/admin_notes.md` & `sageworks-0.1.4.1/docs/admin_notes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/big_spider.png` & `sageworks-0.1.4.1/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/graph_representation.png` & `sageworks-0.1.4.1/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/powered_aws_dark_blue.png` & `sageworks-0.1.4.1/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/powered_aws_transparent.png` & `sageworks-0.1.4.1/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/powered_aws_white.png` & `sageworks-0.1.4.1/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.1.4.1/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/sageworks.png` & `sageworks-0.1.4.1/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/sageworks_concepts.png` & `sageworks-0.1.4.1/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/scp.png` & `sageworks-0.1.4.1/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/scp_labs.png` & `sageworks-0.1.4.1/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/images/small_spider.png` & `sageworks-0.1.4.1/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/sageworks_classes_concepts.md` & `sageworks-0.1.4.1/docs/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/docs/scp_consulting.md` & `sageworks-0.1.4.1/docs/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/examples/data_to_data_example.py` & `sageworks-0.1.4.1/examples/data_to_data_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/scripts/data_source_tags.py` & `sageworks-0.1.4.1/scripts/data_source_tags.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/scripts/list_data_sources.py` & `sageworks-0.1.4.1/scripts/list_data_sources.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/setup.cfg` & `sageworks-0.1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/setup.py` & `sageworks-0.1.4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,47 +2,48 @@
 """Setup.py for SageWorks: Sagemaker Workbench"""
 
 import os
 import glob
 
 from setuptools import setup, find_packages
 
-readme = open("README.md").read()
+readme = open("Readme.md").read()
 
 
 # Data and Example Files
 def get_files(dir_name):
     """Simple directory walker"""
     return [(os.path.join(".", d), [os.path.join(d, f) for f in files]) for d, _, files in os.walk(dir_name)]
 
 
 setup(
     name="sageworks",
     # use_scm_version=True,
-    version="0.1.4",
+    version="0.1.4.1",
     description="SageWorks: An easy to use WorkBench for creating and deploying SageMaker Models",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SuperCowPowers LLC",
     author_email="support@supercowpowers.com",
     url="https://github.com/SuperCowPowers/sageworks",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[os.path.splitext(os.path.basename(path))[0] for path in glob.glob("src/*.py")],
     include_package_data=True,
     data_files=get_files("data") + get_files("examples"),
     install_requires=[
         "boto3",
-        "awswrangler",
+        "awswrangler >= 3.0.0",
         "sagemaker >= 2.143",
         "pandas",
         "scikit-learn",
         "redis",
         "dash",
         "dash-bootstrap-components",
+        "dash-bootstrap-templates",
     ],
     license="MIT",
     keywords="SageMaker, Machine Learning, AWS, Python, Utilities",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
```

### Comparing `sageworks-0.1.4/src/sageworks/algorithms/table/light/data_source_eda.py` & `sageworks-0.1.4.1/src/sageworks/algorithms/table/light/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/algorithms/table/light/feature_spider.py` & `sageworks-0.1.4.1/src/sageworks/algorithms/table/light/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/algorithms/table/light/row_tagger.py` & `sageworks-0.1.4.1/src/sageworks/algorithms/table/light/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/artifacts/Readme.md` & `sageworks-0.1.4.1/src/sageworks/artifacts/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/artifacts/artifact.py` & `sageworks-0.1.4.1/src/sageworks/artifacts/artifact.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,45 +3,50 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 import logging
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 from sageworks.aws_service_broker.aws_service_broker import AWSServiceBroker
+from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
 
 # Setup Logging
 logging_setup()
 
 
 class Artifact(ABC):
     """Artifact: Abstract Base Class for all Artifact classes in SageWorks.
     Artifacts simply reflect and aggregate one or more AWS Services"""
 
     # Class attributes
     log = logging.getLogger(__name__)
 
     # Set up our Boto3 and SageMaker Session and SageMaker Client
-    boto_session = AWSAccountClamp().boto_session()
-    sm_session = AWSAccountClamp().sagemaker_session()
-    sm_client = AWSAccountClamp().sagemaker_client()
+    aws_account_clamp = AWSAccountClamp()
+    boto_session = aws_account_clamp.boto_session()
+    sm_session = aws_account_clamp.sagemaker_session(boto_session)
+    sm_client = aws_account_clamp.sagemaker_client(boto_session)
+    aws_region = aws_account_clamp.region()
 
     # AWSServiceBroker pulls and collects metadata from a bunch of AWS Services
-    aws_meta = AWSServiceBroker()
+    aws_broker = AWSServiceBroker()
+
+    # Grab our SageWorksConfig for S3 Buckets and other SageWorks specific settings
+    sageworks_config = SageWorksConfig()
+    data_catalog_db = "sageworks"
+    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
+    data_source_s3_path = sageworks_bucket + "/data-sources"
+    feature_sets_s3_path = sageworks_bucket + "/feature-sets"
 
     def __init__(self, uuid):
         """Artifact Initialization"""
         self.uuid = uuid
         self.log = logging.getLogger(__name__)
 
-        # FIXME: We should have this come from AWS or Config
-        self.data_catalog_db = "sageworks"
-        self.data_source_s3_path = "s3://scp-sageworks-artifacts/data-sources"
-        self.feature_sets_s3_path = "s3://scp-sageworks-artifacts/feature-sets"
-
     @abstractmethod
     def check(self) -> bool:
         """Does the Artifact exist? Can we connect to it?"""
         pass
 
     @abstractmethod
     def details(self) -> dict:
@@ -70,46 +75,49 @@
 
     @abstractmethod
     def aws_url(self):
         """AWS console/web interface for this artifact"""
         pass
 
     @abstractmethod
-    def meta(self):
+    def aws_meta(self):
         """Get the full AWS metadata for this artifact"""
         pass
 
     @abstractmethod
     def delete(self):
         """Delete this artifact including all related AWS objects"""
         pass
 
+    def set_tags(self, tag):
+        """Set the tags for this artifact"""
+        self.log.error("set_tags: functionality needs to be added!")
+
     @staticmethod
     def aws_tags_to_dict(aws_tags):
         """AWS Tags are in an odd format, so convert to regular dictionary"""
         return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
 
     def sageworks_meta(self):
-        """Get the SageWorks specific metadata for this Artifact"""
+        """Get the SageWorks specific metadata for this Artifact
+        Note: This functionality will work for FeatureSets, Models, and Endpoints
+        but not for DataSources. DataSources need to overwrite this method
+        """
         aws_arn = self.arn()
         self.log.info(f"Retrieving SageWorks Metadata for Artifact: {aws_arn}...")
         aws_tags = self.sm_session.list_tags(aws_arn)
         meta = self.aws_tags_to_dict(aws_tags)
         return meta
 
     def sageworks_tags(self):
         """Get the tags for this artifact"""
         combined_tags = self.sageworks_meta().get("sageworks_tags", "")
         tags = combined_tags.split(":")
         return tags
 
-    def add_tag(self, tag):
-        """Add a tag to this artifact"""
-        self.log.error("add_tag: functionality needs to be added!")
-
     def summary(self) -> dict:
         """This is generic summary information for all Artifacts. If you
         want to get more detailed information, call the details() method
         which is implemented by the specific Artifact class"""
         return {
             "uuid": self.uuid,
             "aws_arn": self.arn(),
```

### Comparing `sageworks-0.1.4/src/sageworks/artifacts/data_sources/athena_source.py` & `sageworks-0.1.4.1/src/sageworks/artifacts/data_sources/athena_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """AthenaSource: SageWorks Data Source accessible through Athena"""
 import pandas as pd
 import awswrangler as wr
 from datetime import datetime
 
 # SageWorks Imports
-from sageworks.artifacts.data_sources.data_source import DataSource
+from sageworks.artifacts.data_sources.data_source_abstract import DataSourceAbstract
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
-from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 
 
-class AthenaSource(DataSource):
+class AthenaSource(DataSourceAbstract):
     """AthenaSource: SageWorks Data Source accessible through Athena
 
     Common Usage:
         my_data = AthenaSource(data_uuid, database="sageworks")
         my_data.summary()
         my_data.details()
         df = my_data.query(f"select * from {data_uuid} limit 5")
@@ -30,27 +29,27 @@
         # Call superclass init
         super().__init__(data_uuid)
 
         self.data_catalog_db = database
         self.table_name = data_uuid
 
         # Grab an AWS Metadata Broker object and pull information for Data Sources
-        self.catalog_meta = self.aws_meta.get_metadata(ServiceCategory.DATA_CATALOG)[self.data_catalog_db].get(
+        self.catalog_meta = self.aws_broker.get_metadata(ServiceCategory.DATA_CATALOG)[self.data_catalog_db].get(
             self.table_name
         )
 
         # All done
         print(f"AthenaSource Initialized: {self.data_catalog_db}.{self.table_name}")
 
     def check(self) -> bool:
         """Validation Checks for this Data Source"""
 
         # We're we able to pull AWS Metadata for this table_name?"""
         if self.catalog_meta is None:
-            self.log.critical(f"AthenaSource.check() {self.table_name} not found in SageWorks Metadata!")
+            self.log.info(f"AthenaSource.check() {self.table_name} not found in SageWorks Metadata...")
             return False
         return True
 
     def deep_check(self) -> bool:
         """These are more comprehensive checks for this Data Source (may take a LONG TIME)"""
 
         # Can we run an Athena Test Query
@@ -60,37 +59,37 @@
         except Exception as exc:
             self.log.critical(f"Athena Test Query Failed: {exc}")
             return False
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         # Grab our SageWorks Role Manager, get our AWS account id, and region for ARN creation
-        account_id = AWSAccountClamp().account_id()
-        region = AWSAccountClamp().region()
+        account_id = self.aws_account_clamp.account_id()
+        region = self.aws_account_clamp.region()
         arn = f"arn:aws:glue:{region}:{account_id}:table/{self.data_catalog_db}/{self.table_name}"
         return arn
 
     def sageworks_meta(self):
         """Get the SageWorks specific metadata for this Artifact"""
         params = self.catalog_meta.get("Parameters", {})
         return {key: value for key, value in params.items() if "sageworks" in key}
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         size_in_bytes = sum(wr.s3.size_objects(self.s3_storage_location(), boto3_session=self.boto_session).values())
         size_in_mb = size_in_bytes / 1_000_000
         return size_in_mb
 
-    def meta(self):
+    def aws_meta(self):
         """Get the full AWS metadata for this artifact"""
         return self.catalog_meta
 
     def aws_url(self):
         """The AWS URL for looking at/querying this data source"""
-        return "https://us-west-2.console.aws.amazon.com/athena/home"
+        return f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
 
     def created(self) -> datetime:
         """Return the datetime when this artifact was created"""
         return self.catalog_meta["CreateTime"]
 
     def modified(self) -> datetime:
         """Return the datetime when this artifact was last modified"""
@@ -161,16 +160,17 @@
 
     # Verify that the Athena Data Source exists
     assert my_data.check()
 
     # What's my SageWorks UUID
     print(f"UUID: {my_data.uuid}")
 
-    # What's my AWS ARN
+    # What's my AWS ARN and URL
     print(f"AWS ARN: {my_data.arn()}")
+    print(f"AWS URL: {my_data.aws_url()}")
 
     # Get the S3 Storage for this Data Source
     print(f"S3 Storage: {my_data.s3_storage_location()}")
 
     # What's the size of the data?
     print(f"Size of Data (MB): {my_data.size()}")
```

### Comparing `sageworks-0.1.4/src/sageworks/artifacts/endpoints/endpoint.py` & `sageworks-0.1.4.1/src/sageworks/artifacts/endpoints/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Endpoint: SageWorks Endpoint Class"""
+import sys
 from datetime import datetime
 import botocore
 import pandas as pd
 import numpy as np
 from io import StringIO
 
 from sklearn.metrics import mean_absolute_error, r2_score, mean_squared_error
@@ -24,35 +25,36 @@
         my_endpoint = Endpoint(endpoint_uuid)
         prediction_df = my_endpoint.predict(test_df)
         metrics = my_endpoint.performance_metrics(target_column, prediction_df)
         for metric, value in metrics.items():
             print(f"{metric}: {value:0.3f}")
     """
 
-    def __init__(self, endpoint_uuid):
+    def __init__(self, endpoint_uuid, exit_on_error=True):
         """Endpoint Initialization
 
         Args:
             endpoint_uuid (str): Name of Endpoint in SageWorks
         """
         # Call SuperClass Initialization
         super().__init__(endpoint_uuid)
 
         # Grab an AWS Metadata Broker object and pull information for Endpoints
         self.endpoint_name = endpoint_uuid
-        self.endpoint_meta = self.aws_meta.get_metadata(ServiceCategory.ENDPOINTS).get(self.endpoint_name)
+        self.endpoint_meta = self.aws_broker.get_metadata(ServiceCategory.ENDPOINTS).get(self.endpoint_name)
         self.endpoint_return_columns = None
+        self.exit_on_error = exit_on_error
 
         # All done
         self.log.info(f"Endpoint Initialized: {self.endpoint_name}")
 
     def check(self) -> bool:
         """Does the feature_set_name exist in the AWS Metadata?"""
         if self.endpoint_meta is None:
-            self.log.critical(f"Endpoint.check() {self.endpoint_name} not found in AWS Metadata!")
+            self.log.info(f"Endpoint.check() {self.endpoint_name} not found in AWS Metadata!")
             return False
         return True
 
     def predict(self, feature_df: pd.DataFrame) -> pd.DataFrame:
         """Run inference/prediction on the given Feature DataFrame
         Args:
             feature_df (pd.DataFrame): DataFrame to run predictions on (must have superset of features)
@@ -115,14 +117,19 @@
             self.endpoint_return_columns = results_df.columns.tolist()
 
             # Return the results dataframe
             return results_df
 
         except botocore.exceptions.ClientError as err:
             if err.response["Error"]["Code"] == "ModelError":  # Model Error
+                # Report the error
+                self.log.critical(f"Endpoint prediction error: {err.response.get('Message')}")
+                if self.exit_on_error:
+                    sys.exit(1)
+
                 # Base case: DataFrame with 1 Row
                 if len(feature_df) == 1:
                     # If we don't have ANY known good results we're kinda screwed
                     if not self.endpoint_return_columns:
                         raise err
 
                     # Construct an Error DataFrame (one row of NaNs in the return columns)
@@ -149,25 +156,25 @@
             error_df[column] = df[column].values
         return error_df
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def meta(self):
+    def aws_meta(self):
         """Get the metadata for this artifact"""
         return self.endpoint_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         return self.endpoint_meta["EndpointArn"]
 
     def aws_url(self):
         """The AWS URL for looking at/querying this data source"""
-        return "https://us-west-2.console.aws.amazon.com/athena/home"
+        return f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
 
     def created(self) -> datetime:
         """Return the datetime when this artifact was created"""
         return self.endpoint_meta["CreationTime"]
 
     def modified(self) -> datetime:
         """Return the datetime when this artifact was last modified"""
```

### Comparing `sageworks-0.1.4/src/sageworks/artifacts/feature_sets/feature_set.py` & `sageworks-0.1.4.1/src/sageworks/artifacts/feature_sets/feature_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import awswrangler as wr
 
 from sagemaker.feature_store.feature_group import FeatureGroup
 from sagemaker.feature_store.feature_store import FeatureStore
 
 # SageWorks Imports
 from sageworks.artifacts.artifact import Artifact
+from sageworks.artifacts.data_sources.data_source import DataSource
 from sageworks.artifacts.data_sources.athena_source import AthenaSource
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 
 
 class FeatureSet(Artifact):
     """FeatureSet: SageWorks Feature Set accessible through Athena
 
@@ -31,93 +32,97 @@
             feature_uuid (str): Name of Feature Set in SageWorks Metadata.
         """
         # Call superclass init
         super().__init__(feature_uuid)
 
         # Grab an AWS Metadata Broker object and pull information for Feature Sets
         self.feature_set_name = feature_uuid
-        self.feature_meta = self.aws_meta.get_metadata(ServiceCategory.FEATURE_STORE).get(self.feature_set_name)
+        self.feature_meta = self.aws_broker.get_metadata(ServiceCategory.FEATURE_STORE).get(self.feature_set_name)
         if self.feature_meta is None:
-            self.log.warning(f"Could not find feature set {self.feature_set_name} within current visibility scope")
-            self.athena_source = None
+            self.log.info(f"Could not find feature set {self.feature_set_name} within current visibility scope")
+            self.data_source = None
             return
         else:
             self.record_id = self.feature_meta["RecordIdentifierFeatureName"]
             self.event_time = self.feature_meta["EventTimeFeatureName"]
 
             # Pull Athena and S3 Storage information from metadata
             self.athena_database = self.feature_meta["sageworks"].get("athena_database")
             self.athena_table = self.feature_meta["sageworks"].get("athena_table")
             self.s3_storage = self.feature_meta["sageworks"].get("s3_storage")
 
-            # Creat our internal AthenaSource
-            self.athena_source = AthenaSource(self.athena_table, self.athena_database)
+            # Creat our internal DataSource (hardcoded to Athena for now)
+            self.data_source = AthenaSource(self.athena_table, self.athena_database)
 
         # Spin up our Feature Store
         self.feature_store = FeatureStore(self.sm_session)
 
         # All done
         self.log.info(f"FeatureSet Initialized: {self.feature_set_name}")
 
     def check(self) -> bool:
         """Does the feature_set_name exist in the AWS Metadata?"""
         if self.feature_meta is None:
-            self.log.critical(f"FeatureSet.check() {self.feature_set_name} not found in AWS Metadata!")
+            self.log.info(f"FeatureSet.check() {self.feature_set_name} not found in AWS Metadata!")
             return False
         return True
 
-    def meta(self) -> dict:
+    def aws_meta(self) -> dict:
         """Get the full AWS metadata for this artifact"""
         return self.feature_meta
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for this artifact"""
         return self.feature_meta["FeatureGroupArn"]
 
     def size(self) -> float:
-        """Return the size of the internal AthenaSource in MegaBytes"""
-        return self.athena_source.size()
+        """Return the size of the internal DataSource in MegaBytes"""
+        return self.data_source.size()
 
     def column_names(self) -> list[str]:
-        """Return the column names of the internal AthenaSource"""
-        return self.athena_source.column_names()
+        """Return the column names of the Feature Set"""
+        return list(self.column_details().keys())
 
     def column_types(self) -> list[str]:
-        """Return the column types of the internal AthenaSource"""
-        return self.athena_source.column_types()
+        """Return the column types of the Feature Set"""
+        return list(self.column_details().values())
 
-    def column_details(self) -> list[str]:
-        """Return the column types of the internal AthenaSource"""
-        return self.athena_source.column_details()
+    def column_details(self) -> dict:
+        """Return the column details of the Feature Set"""
+        return {item["FeatureName"]: item["FeatureType"] for item in self.feature_meta["FeatureDefinitions"]}
 
     def num_columns(self) -> int:
-        """Return the number of columns of the internal AthenaSource"""
+        """Return the number of columns of the Feature Set"""
         return len(self.column_names())
 
     def num_rows(self) -> int:
-        """Return the number of rows of the internal AthenaSource"""
-        return self.athena_source.num_rows()
+        """Return the number of rows of the internal DataSource"""
+        return self.data_source.num_rows()
 
     def query(self, query: str) -> pd.DataFrame:
-        """Return the number of rows of the internal AthenaSource"""
-        return self.athena_source.query(query)
+        """Query the internal DataSource"""
+        return self.data_source.query(query)
 
     def aws_url(self):
         """The AWS URL for looking at/querying this data source"""
-        return "https://us-west-2.console.aws.amazon.com/athena/home"
+        return f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
 
     def created(self) -> datetime:
         """Return the datetime when this artifact was created"""
         return self.feature_meta["CreationTime"]
 
     def modified(self) -> datetime:
         """Return the datetime when this artifact was last modified"""
         # Note: We can't currently figure out how to this from AWS Metadata
         return self.feature_meta["CreationTime"]
 
+    def get_data_source(self) -> DataSource:
+        """Return the underlying DataSource object"""
+        return self.data_source
+
     def get_feature_store(self) -> FeatureStore:
         """Return the underlying AWS FeatureStore object. This can be useful for more advanced usage
         with create_dataset() such as Joins and time ranges and a host of other options
         See: https://docs.aws.amazon.com/sagemaker/latest/dg/feature-store-create-a-dataset.html
         """
         return self.feature_store
 
@@ -164,29 +169,57 @@
             f"        ORDER BY {self.event_time} desc, api_invocation_time DESC, write_time DESC) AS row_num "
             f'        FROM "{self.athena_table}") '
             "    WHERE row_num = 1 and  NOT is_deleted;"
         )
         return query
 
     def details(self) -> dict:
-        """Additional Details about this FeatureSet"""
-        details = self.summary()
-        # Fill in more details here if needed
-        return details
+        """Additional Details about this FeatureSet
+        Returns:
+            dict: A dictionary of details about this FeatureSet
+        Notes:
+            - num_columns
+            - num_rows
+            - column_details
+            - storage_type ('athena' or 'rds')
+            - storage_uuid
+
+        Drill Down:
+        You can use the fs.get_data_source().details() method to get additional
+        details on the underlying DataSource object.
+        """
+        # Include the summary information in the details
+        fs_details = self.summary()
+
+        # Number of Columns
+        fs_details["num_columns"] = self.num_columns()
+
+        # Number of Rows
+        fs_details["num_rows"] = self.num_rows()
+
+        # Column Details
+        fs_details["column_details"] = self.column_details()
+
+        # Underlying Storage Details
+        fs_details["storage_type"] = "athena"  # TODO: Add RDS support
+        fs_details["storage_uuid"] = self.data_source.uuid
+
+        # Return the details
+        return fs_details
 
     def delete(self):
         """Delete the Feature Set: Feature Group, Catalog Table, and S3 Storage Objects"""
 
         # Delete the Feature Group and ensure that it gets deleted
         remove_fg = FeatureGroup(name=self.feature_set_name, sagemaker_session=self.sm_session)
         remove_fg.delete()
         self.ensure_feature_group_deleted(remove_fg)
 
-        # Delete our underlying AthenaSource (Data Catalog Table and S3 Storage Objects)
-        self.athena_source.delete()
+        # Delete our underlying DataSource (Data Catalog Table and S3 Storage Objects)
+        self.data_source.delete()
 
         # Feature Sets can often have a lot of cruft so delete the entire bucket/prefix
         s3_delete_path = self.feature_sets_s3_path + f"/{self.feature_set_name}"
         self.log.info(f"Deleting S3 Storage Objects {s3_delete_path}")
         wr.s3.delete_objects(s3_delete_path, boto3_session=self.boto_session)
 
     def ensure_feature_group_deleted(self, feature_group):
@@ -201,22 +234,25 @@
                     break
                 else:
                     raise error
             time.sleep(1)
         self.log.info(f"FeatureSet {feature_group.name} successfully deleted")
 
 
-# Simple test of the FeatureSet functionality
-def test():
-    """Test for FeatureSet Class"""
+if __name__ == "__main__":
+    """Exercise for FeatureSet Class"""
+    from pprint import pprint
 
     # Grab a FeatureSet object and pull some information from it
     my_features = FeatureSet("test_feature_set")
 
     # Call the various methods
+    # What's my AWS ARN and URL
+    print(f"AWS ARN: {my_features.arn()}")
+    print(f"AWS URL: {my_features.aws_url()}")
 
     # Let's do a check/validation of the feature set
     print(f"Feature Set Check: {my_features.check()}")
 
     # How many rows and columns?
     num_rows = my_features.num_rows()
     num_columns = my_features.num_columns()
@@ -226,14 +262,25 @@
     columns = my_features.column_names()
     print(columns)
 
     # Get the metadata and tags associated with this feature set
     print(f"SageWorks Meta: {my_features.sageworks_meta()}")
     print(f"SageWorks Tags: {my_features.sageworks_tags()}")
 
+    # Get a summary for this Feature Set
+    print("\nSummary:")
+    pprint(my_features.summary())
+
+    # Get the details for this Feature Set
+    print("\nDetails:")
+    details = my_features.details()
+    pprint(details)
+
+    # Now do deep dive on storage
+    if details["storage_type"] == "athena":
+        storage = my_features.get_data_source()
+        print("\nStorage Details:")
+        pprint(storage.details())
+
     # Now delete the AWS artifacts associated with this Feature Set
     # print('Deleting SageWorks Feature Set...')
     # my_features.delete()
-
-
-if __name__ == "__main__":
-    test()
```

### Comparing `sageworks-0.1.4/src/sageworks/artifacts/models/model.py` & `sageworks-0.1.4.1/src/sageworks/artifacts/models/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,36 +23,36 @@
             model_uuid (str): Name of Model in SageWorks.
         """
         # Call SuperClass Initialization
         super().__init__(model_uuid)
 
         # Grab an AWS Metadata Broker object and pull information for Models
         self.model_name = model_uuid
-        self.model_meta = self.aws_meta.get_metadata(ServiceCategory.MODELS).get(self.model_name)
+        self.model_meta = self.aws_broker.get_metadata(ServiceCategory.MODELS).get(self.model_name)
         if self.model_meta is None:
             self.log.warning(f"Could not find model {self.model_name} within current visibility scope")
         else:
             self.latest_model = self.model_meta[0]
             self.description = self.latest_model["ModelPackageDescription"]
 
         # All done
         self.log.info(f"Model Initialized: {self.model_name}")
 
     def check(self) -> bool:
         """Does the model metadata exist in the AWS Metadata?"""
         if self.model_meta is None:
-            self.log.critical(f"Model.check() {self.model_name} not found in AWS Metadata!")
+            self.log.info(f"Model.check() {self.model_name} not found in AWS Metadata!")
             return False
         return True
 
     def size(self) -> float:
         """Return the size of this data in MegaBytes"""
         return 0.0
 
-    def meta(self):
+    def aws_meta(self):
         """Get the metadata for this artifact"""
         return self.latest_model
 
     def arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for the Model Package Group"""
         return self.group_arn()
 
@@ -62,15 +62,15 @@
 
     def model_arn(self) -> str:
         """AWS ARN (Amazon Resource Name) for the Model Package Group"""
         return self.latest_model["ModelPackageArn"]
 
     def aws_url(self):
         """The AWS URL for looking at/querying this data source"""
-        return "https://us-west-2.console.aws.amazon.com/athena/home"
+        return f"https://{self.aws_region}.console.aws.amazon.com/athena/home"
 
     def created(self) -> datetime:
         """Return the datetime when this artifact was created"""
         return self.latest_model["CreationTime"]
 
     def modified(self) -> datetime:
         """Return the datetime when this artifact was last modified"""
@@ -97,17 +97,16 @@
             self.sm_client.delete_model_package(ModelPackageName=model["ModelPackageArn"])
 
         # Now delete the Model Package Group
         self.log.info(f"Deleting Model Group {self.model_name}...")
         self.sm_client.delete_model_package_group(ModelPackageGroupName=self.model_name)
 
 
-# Simple test of the Model functionality
-def test():
-    """Test for Model Class"""
+if __name__ == "__main__":
+    """Exercise the Model Class"""
 
     # Grab a Model object and pull some information from it
     my_model = Model("abalone-regression")
 
     # Call the various methods
 
     # Let's do a check/validation of the Model
@@ -121,11 +120,7 @@
     print(f"Tags: {my_model.sageworks_tags()}")
 
     # Get creation time
     print(f"Created: {my_model.created()}")
 
     # Delete the Model
     # my_model.delete()
-
-
-if __name__ == "__main__":
-    test()
```

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,37 @@
-"""AWSAccountClamp provides logic/functionality over the set of AWS IAM Services"""
+"""AWSAccountClamp provides logic/functionality over a set of AWS IAM Services"""
 import sys
 import boto3
 from botocore.exceptions import ClientError, UnauthorizedSSOTokenError
+from botocore.credentials import RefreshableCredentials
+from botocore.session import get_session
 from sagemaker.session import Session as SageSession
-import argparse
+from datetime import timedelta
 import logging
 
 # SageWorks Imports
+from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
 
 # Setup Logging
 logging_setup()
 
 
 class AWSAccountClamp:
-    def __init__(self, role_name="SageWorks-ExecutionRole"):
-        """AWSAccountClamp provides logic/functionality over the set of AWS IAM Services"""
+    def __init__(self):
+        """AWSAccountClamp provides logic/functionality over a set of AWS IAM Services"""
         self.log = logging.getLogger(__file__)
-        self.role_name = role_name
-
-    def check(self):
-        """Check if the AWS Account Clamp is 100% 'locked in'
-        - Check the current AWS Identity (Print it out)
-        - See if we can 'assume-role' for the SageWorks-ExecutionRole
-        - Test out S3 Access (with boto_session)
-        - Test out SageMaker Access (with sm_session)
-        - Test out SageMake Client (with sm_client)
-        """
-        self.log.info("\n*** AWS Identity Check ***")
-        self.check_aws_identity()
-        self.log.info("Identity Check Success...")
-
-        self.log.info("\n*** AWS Assume SageWorks-ExecutionRole Check ***")
-        my_boto_session = self.boto_session()
-        self.log.info("Assume Role Success...")
 
-        self.log.info("\n*** AWS S3 Access Check ***")
-        s3 = my_boto_session.client("s3")
-        results = s3.list_buckets()
-        for bucket in results["Buckets"]:
-            self.log.info(f"\t{bucket['Name']}")
-
-        self.log.info("\n*** AWS Sagemaker Session/Client Check ***")
-        sm_client = self.sagemaker_client()
-        self.log.info(sm_client.list_feature_groups()["FeatureGroupSummaries"])
-
-        self.log.info("\n*** AWS Sagemaker Session/Client Check ***")
-        sm_client = self.sagemaker_client()
-        self.log.info(sm_client.list_feature_groups()["FeatureGroupSummaries"])
+        # Grab the AWS Role Name from the SageWorks Config
+        config = SageWorksConfig()
+        role_name = config.get_config_value("SAGEWORKS_AWS", "SAGEWORKS_ROLE")
+        self.role_name = role_name
 
-        self.log.info("\nAWS Account Clamp: AOK!")
+        # The default AWS Assume Role TTL is 1 hour, so we'll set our TTL to 50 minutes
+        self.session_time_delta = timedelta(minutes=50)
 
     def check_aws_identity(self) -> bool:
         """Check the AWS Identity currently active"""
         # Check AWS Identity Token
         sts = boto3.client("sts")
         try:
             identity = sts.get_caller_identity()
@@ -63,89 +41,125 @@
             self.log.info(f"Region: {self.region()}")
             return True
         except (ClientError, UnauthorizedSSOTokenError) as exc:
             self.log.critical("AWS Identity Check Failure: Check AWS_PROFILE and/or Renew SSO Token...")
             self.log.critical(exc)
             sys.exit(1)  # FIXME: Longer term we probably want to raise exc and have caller catch it
 
+    def check_app_config(self, boto_session: boto3.Session) -> bool:
+        """Check if the AWS AppConfig Service is enabled"""
+        # FIXME: This will be enabled later
+        return True
+        appconfig = boto_session.client("appconfig")
+        try:
+            appconfig.list_applications()
+            return True
+        except (ClientError, UnauthorizedSSOTokenError) as exc:
+            self.log.critical("AWS AppConfig Check Failure: Check AWS_PROFILE and/or Renew SSO Token...")
+            self.log.critical(exc)
+            sys.exit(1)
+
+    def check_s3_access(self, boto_session: boto3.Session) -> bool:
+        s3 = boto_session.client("s3")
+        results = s3.list_buckets()
+        for bucket in results["Buckets"]:
+            self.log.info(f"\t{bucket['Name']}")
+        return True
+
     def is_sageworks_role(self) -> bool:
         """Check if the current AWS Identity is the SageWorks Role"""
         sts = boto3.client("sts")
         try:
-            if "SageWorks-ExecutionRole" in sts.get_caller_identity()["Arn"]:
+            if self.role_name in sts.get_caller_identity()["Arn"]:
                 return True
         except (ClientError, UnauthorizedSSOTokenError) as exc:
             self.log.critical("SageWorks Role Check Failure: Check AWS_PROFILE and/or Renew SSO Token...")
             self.log.critical(exc)
             sys.exit(1)  # FIXME: Longer term we probably want to raise exc and have caller catch it
 
     def sageworks_execution_role_arn(self):
         """Get the SageWorks Execution Role"""
+        iam = boto3.client("iam")
         try:
-            iam = boto3.client("iam")
             role_arn = iam.get_role(RoleName=self.role_name)["Role"]["Arn"]
             return role_arn
         except iam.exceptions.NoSuchEntityException as exc:
             self.log.critical(f"Could Not Find Role {self.role_name}")
             self.log.critical(exc)
             sys.exit(1)  # FIXME: Longer term we probably want to raise exc and have caller catch it
         except UnauthorizedSSOTokenError as exc:
             self.log.critical("SageWorks Role Check Failure: Check AWS_PROFILE and/or Renew SSO Token...")
             self.log.critical(exc)
             sys.exit(1)  # FIXME: Longer term we probably want to raise exc and have caller catch it
 
+    def _session_credentials(self):
+        """Internal: Set up our AWS Session credentials for automatic refresh"""
+
+        # Assume the SageWorks Execution Role and then pull the credentials
+        self.log.debug("Assuming the SageWorks Execution Role and Refreshing Credentials...")
+        sts = boto3.Session().client("sts")
+        response = sts.assume_role(
+            RoleArn=self.sageworks_execution_role_arn(),
+            RoleSessionName="sageworks-execution-role-session",
+        ).get("Credentials")
+        credentials = {
+            "access_key": response.get("AccessKeyId"),
+            "secret_key": response.get("SecretAccessKey"),
+            "token": response.get("SessionToken"),
+            "expiry_time": response.get("Expiration").isoformat(),
+        }
+        self.log.debug(f"Credentials Refreshed: Expires at {credentials['expiry_time']}")
+        return credentials
+
     def boto_session(self):
-        """Create a sageworks session using sts.assume_role(sageworks_execution_role)"""
+        """Create a *refreshable* AWS/boto session so that clients don't get TOKEN timeouts"""
 
-        # First check if we have already assumed the SageWorks Execution Role
+        # If we're already using the SageWorks Execution Role, then we don't need refreshable credentials
         if self.is_sageworks_role():
             return boto3.Session()
 
-        # Okay we need to assume the SageWorks Execution Role and Return a boto3 session
-        session = boto3.Session()
-        sts = session.client("sts")
-        response = sts.assume_role(
-            RoleArn=self.sageworks_execution_role_arn(),
-            RoleSessionName="sageworks-execution-role-session",
-        )
-        new_session = boto3.Session(
-            aws_access_key_id=response["Credentials"]["AccessKeyId"],
-            aws_secret_access_key=response["Credentials"]["SecretAccessKey"],
-            aws_session_token=response["Credentials"]["SessionToken"],
+        # Get our refreshable credentials
+        refreshable_credentials = RefreshableCredentials.create_from_metadata(
+            metadata=self._session_credentials(),
+            refresh_using=self._session_credentials,
+            method="sts-assume-role",
         )
-        return new_session
 
-    def sagemaker_session(self):
-        """Create a sageworks SageMaker session using sts.assume_role(sageworks_execution_role)"""
-        return SageSession(boto_session=self.boto_session())
-
-    def sagemaker_client(self):
-        """Create a sageworks SageMaker client using sts.assume_role(sageworks_execution_role)"""
-        return self.sagemaker_session().boto_session.client("sagemaker")
+        # Attach the refreshable credentials to a generic boto3 session
+        session = get_session()
+        session._credentials = refreshable_credentials
+
+        # Create a new boto3 session using the refreshable credentials
+        refreshable_session = boto3.Session(botocore_session=session)
+        return refreshable_session
+
+    def sagemaker_session(self, session: boto3.Session = None):
+        """Create a sageworks SageMaker session (using our boto3 refreshable session)"""
+        session = session or self.boto_session()
+        return SageSession(boto_session=session)
+
+    def sagemaker_client(self, session: boto3.Session = None):
+        """Create a sageworks SageMaker client (using our boto3 refreshable session)"""
+        session = session or self.boto_session()
+        return session.client("sagemaker")
 
     @staticmethod
     def account_id():
         """Get the AWS AccountID"""
         return boto3.client("sts").get_caller_identity()["Account"]
 
     def region(self):
         """Get the AWS AccountID"""
         return self.boto_session().region_name
 
 
 if __name__ == "__main__":
     """Exercise the AWS Account Clamp Class"""
 
-    # Collect args from the command line
-    parser = argparse.ArgumentParser()
-    args, commands = parser.parse_known_args()
-
-    # Check for unknown args
-    if commands:
-        print("Unrecognized args: %s" % commands)
-        sys.exit(1)
+    # Import the Check Class to test this class :)
+    from sageworks.aws_service_broker.aws_account_check import AWSAccountCheck
 
     # Create the class
-    aws_clamp = AWSAccountClamp()
+    aws_account_check = AWSAccountCheck()
 
     # Check that out AWS Account Clamp is working AOK
-    aws_clamp.check()
+    aws_account_check.check()
```

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # SageWorks Imports
 from sageworks.utils.redis_cache import RedisCache
 from sageworks.aws_service_broker.aws_service_connectors.s3_bucket import S3Bucket
 from sageworks.aws_service_broker.aws_service_connectors.data_catalog import DataCatalog
 from sageworks.aws_service_broker.aws_service_connectors.feature_store import FeatureStore
 from sageworks.aws_service_broker.aws_service_connectors.model_registry import ModelRegistry
 from sageworks.aws_service_broker.aws_service_connectors.endpoints import Endpoints
+from sageworks.aws_service_broker.aws_service_connectors.artifact_info import ArtifactInfo
+from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
 
 # Setup Logging
 logging_setup()
 
 
 # Enumerated types for SageWorks Meta Requests
@@ -46,35 +48,39 @@
         return cls.instance
 
     @classmethod
     def __class_init__(cls, database_scope):
         """AWSServiceBroker pulls and collects metadata from a bunch of AWS Services"""
         cls.log = logging.getLogger(__file__)
 
-        # FIXME: This should be pulled from a config file
-        cls.incoming_data_bucket = "s3://scp-sageworks-artifacts/incoming-data"
+        # Grab our SageWorksConfig for S3 Buckets and other SageWorks specific settings
+        sageworks_config = SageWorksConfig()
+        sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
+        cls.incoming_data_bucket = sageworks_bucket + "/incoming-data"
 
         # SageWorks category mapping to AWS Services
         # - incoming_data = S3
         # - data_sources = Data Catalog, Athena
         # - feature_sets = Data Catalog, Athena, Feature Store
         # - models = Model Registry
         # - endpoints = Sagemaker Endpoints, Model Monitors
 
         # Pull in AWS Service Connectors
         cls.incoming_data = S3Bucket(cls.incoming_data_bucket)
         cls.data_catalog = DataCatalog(database_scope)
         cls.feature_store = FeatureStore()
         cls.model_registry = ModelRegistry()
         cls.endpoints = Endpoints()
+        cls.artifact_info = ArtifactInfo()
+
         # Model Monitors
 
         # Redis Cache for Metadata
         cls.meta_cache = RedisCache()
-        cls.fresh_cache = RedisCache(expire=5, postfix=":fresh")
+        cls.fresh_cache = RedisCache(expire=10, postfix=":fresh")
         cls.open_threads = []
 
         # This connection map sets up the connector objects for each category of metadata
         # Note: Even though this seems confusing, it makes other code WAY simpler
         cls.connection_map = {
             ServiceCategory.INCOMING_DATA: cls.incoming_data,
             ServiceCategory.DATA_CATALOG: cls.data_catalog,
@@ -128,16 +134,18 @@
             return cls.meta_cache.get(category)
 
         # If the metadata is fresh, just return it
         cls.log.info(f"Metadata for {category} is fresh!")
         return cls.meta_cache.get(category)
 
     @classmethod
-    def get_all_metadata(cls) -> dict:
+    def get_all_metadata(cls, warn=True) -> dict:
         """Pull the metadata for ALL the Service Categories"""
+        if warn:
+            cls.log.warning("Getting ALL AWS Metadata: You should call get_metadata() with specific categories")
         return {_category: cls.get_metadata(_category) for _category in ServiceCategory}
 
     @classmethod
     def wait_for_refreshes(cls) -> None:
         """Wait for any open threads to finish"""
         for thread in cls.open_threads:
             thread.join()
@@ -165,9 +173,13 @@
         print(f"{my_category}:")
         pprint(aws_broker.get_metadata(my_category))
 
     # Get the Metadata for ALL the categories
     # NOTE: There should be NO Refreshes in the logs
     pprint(aws_broker.get_all_metadata())
 
+    # Get S3 object sizes
+    incoming_data_size = aws_broker.artifact_info.s3_object_sizes(aws_broker.incoming_data.bucket)
+    print(f"Incoming Data Size: {incoming_data_size} MB")
+
     # Wait for any open threads to finish
     aws_broker.wait_for_refreshes()
```

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Connector: Abstract Base Class for pulling/refreshing AWS Service metadata"""
 from abc import ABC, abstractmethod
 
-import time
 import logging
 from typing import final
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 from sageworks.utils.sageworks_logging import logging_setup
 
@@ -14,34 +13,18 @@
 
 
 class Connector(ABC):
     # Class attributes
     log = logging.getLogger(__name__)
 
     # Set up our Boto3 and SageMaker Session and SageMaker Client
-    boto_session = AWSAccountClamp().boto_session()
-    sm_session = AWSAccountClamp().sagemaker_session()
-    sm_client = AWSAccountClamp().sagemaker_client()
-
-    # Set up the token refresh time
-    refresh_minutes = 45
-    token_refresh_time = time.time() + (refresh_minutes * 60)
-
-    @classmethod
-    def refresh_class_aws_sessions(cls):
-        """Class method to refresh our AWS Sessions/Tokens"""
-        now = time.time()
-        if now > cls.token_refresh_time:
-            cls.log.info(f"Current Refresh Time: {cls.token_refresh_time}")
-            cls.token_refresh_time = now + (cls.refresh_minutes * 60)
-            cls.log.info(f"New Refresh Time: {cls.token_refresh_time}")
-            cls.log.info("Refreshing AWS SSO Token...")
-            cls.boto_session = AWSAccountClamp().boto_session()
-            cls.sm_session = AWSAccountClamp().sagemaker_session()
-            cls.sm_client = AWSAccountClamp().sagemaker_client()
+    aws_account_clamp = AWSAccountClamp()
+    boto_session = aws_account_clamp.boto_session()
+    sm_session = aws_account_clamp.sagemaker_session(boto_session)
+    sm_client = aws_account_clamp.sagemaker_client(boto_session)
 
     def __init__(self):
         """Connector: Abstract Base Class for pulling/refreshing AWS Service metadata"""
         self.log = logging.getLogger(__name__)
 
     @abstractmethod
     def check(self) -> bool:
@@ -52,16 +35,15 @@
     def refresh_impl(self):
         """Abstract Method: Implement the AWS Service Data Refresh"""
         pass
 
     @final
     def refresh(self) -> bool:
         """Refresh data/metadata associated with this service"""
-        # Check if it's time to Refresh our AWS/SSO Token
-        Connector.refresh_class_aws_sessions()
+        # We could do something here to refresh the AWS Session or whatever
 
         # Call the subclass Refresh method
         return self.refresh_impl()
 
     @abstractmethod
     def metadata(self) -> dict:
         """Return all the metadata for this service"""
```

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.1.4.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """S3Bucket: Class to retrieve object/file information from an AWS S3 Bucket"""
-import sys
-import argparse
 import awswrangler as wr
 
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_service_connectors.connector import Connector
 
 
@@ -46,33 +44,27 @@
 
     def file_info(self, file: str) -> dict:
         """Get additional info about this specific file"""
         return self.s3_bucket_data[file]
 
 
 if __name__ == "__main__":
+    """Exercises the S3Bucket Class"""
     from pprint import pprint
+    from sageworks.utils.sageworks_config import SageWorksConfig
 
-    # Collect args from the command line
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--bucket",
-        type=str,
-        default="s3://scp-sageworks-artifacts/incoming-data",
-        help="AWS S3 Bucket",
-    )
-    args, commands = parser.parse_known_args()
-
-    # Check for unknown args
-    if commands:
-        print("Unrecognized args: %s" % commands)
-        sys.exit(1)
-
-    # Create the class and get the AWS Data Catalog database info
-    s3_bucket = S3Bucket(args.bucket)
+    # Grab out incoming data bucket for something to test with
+    sageworks_config = SageWorksConfig()
+    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
+    incoming_data_bucket = sageworks_bucket + "/incoming-data"
+
+    # Create the class and check the functionality
+    s3_bucket = S3Bucket(incoming_data_bucket)
+    s3_bucket.check()
+    s3_bucket.refresh()
 
     # List files in the bucket
     print(f"{s3_bucket.bucket}")
     for file_name in s3_bucket.file_names():
         print(f"\t{file_name}")
 
     # Get additional info for a specific file
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/Readme.md` & `sageworks-0.1.4.1/src/sageworks/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/json_to_data_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,64 @@
-"""S3HeavyToDataSource: Class to move HEAVY S3 Files into a SageWorks DataSource"""
-import awswrangler as wr
-import json
+"""JSONToDataSource: Class to move local JSON Files into a SageWorks DataSource"""
+import os
+import pandas as pd
 
 # Local imports
 from sageworks.transforms.transform import Transform, TransformInput, TransformOutput
-from sageworks.artifacts.data_sources.athena_source import AthenaSource
+from sageworks.transforms.pandas_transforms.pandas_to_data import PandasToData
 
 
-# FIXME: This class is not funny implemented. It will be a glue jobs that uses SPARK to convert
-#        CSV to Parquet in a scalable way and then populate the AWS Data Catalog with the information
+class JSONToDataSource(Transform):
+    """JSONToDataSource: Class to move local JSON Files into a SageWorks DataSource
 
+    Common Usage:
+        json_to_data = JSONToDataSource(json_file_path, data_uuid)
+        json_to_data.set_output_tags(["abalone", "json", "whatever"])
+        json_to_data.transform()
+    """
 
-class S3HeavyToDataSource(Transform):
-    def __init__(self, input_uuid, output_uuid):
-        """S3HeavyToDataSource: Class to move HEAVY S3 Files into a SageWorks DataSource"""
+    def __init__(self, json_file_path: str, data_uuid: str):
+        """JSONToDataSource: Class to move local JSON Files into a SageWorks DataSource"""
 
         # Call superclass init
-        super().__init__(input_uuid, output_uuid)
+        super().__init__(json_file_path, data_uuid)
 
         # Set up all my instance attributes
-        self.input_type = TransformInput.S3_OBJECT
+        self.input_type = TransformInput.LOCAL_FILE
         self.output_type = TransformOutput.DATA_SOURCE
 
     def transform_impl(self, overwrite: bool = True):
-        """Convert the CSV data into Parquet Format in the SageWorks S3 Bucket, and
+        """Convert the local JSON file into Parquet Format in the SageWorks Data Sources Bucket, and
         store the information about the data to the AWS Data Catalog sageworks database"""
 
-        # Add some tags here
-        tags = ["sageworks", "public"]
+        # Report the transformation initiation
+        json_file = os.path.basename(self.input_uuid)
+        self.log.info(f"Starting {json_file} -->  DataSource: {self.output_uuid}...")
+
+        # Read in the Local JSON as a Pandas DataFrame
+        df = pd.read_json(self.input_uuid, lines=True)
+
+        # Use the SageWorks Pandas to Data Source class
+        pandas_to_data = PandasToData(self.output_uuid)
+        pandas_to_data.set_input(df)
+        pandas_to_data.set_output_tags(self.output_tags)
+        pandas_to_data.add_output_meta(self.output_meta)
+        pandas_to_data.transform()
 
-        # Read in the S3 CSV as a Pandas DataFrame
-        df = wr.s3.read_csv(self.input_uuid, low_memory=False, boto3_session=self.boto_session)
-
-        # Create the Output Parquet file S3 Storage Path
-        s3_storage_path = f"{self.data_source_s3_path}/{self.output_uuid}"
-
-        # Write out the DataFrame to Parquet/DataStore/Athena
-        wr.s3.to_parquet(
-            df,
-            path=s3_storage_path,
-            dataset=True,
-            mode="overwrite",
-            database=self.data_catalog_db,
-            table=self.output_uuid,
-            description=f"SageWorks data source: {self.output_uuid}",
-            filename_prefix=f"{self.output_uuid}_",
-            parameters={"tags": json.dumps(tags)},
-            boto3_session=self.boto_session,
-            partition_cols=None,
-        )  # FIXME: Have some logic around partition columns
+        # Report the transformation results
+        self.log.info(f"{json_file} -->  DataSource: {self.output_uuid} Complete!")
 
 
 if __name__ == "__main__":
-    """Exercise the S3HeavyToDataSource Class"""
-    import pandas as pd
+    """Exercise the JSONToDataSource Class"""
+    import sys
+    from pathlib import Path
+
+    # Get the path to the dataset in the repository data directory
+    data_path = str(Path(sys.modules["sageworks"].__file__).parent.parent.parent / "data" / "test_data.json")
 
     # Create my Data Loader
-    output_uuid = "test_heavy_data"
-    my_loader = S3HeavyToDataSource("s3://scp-sageworks-artifacts/incoming-data/abalone.csv", output_uuid)
+    my_loader = JSONToDataSource(data_path, "test_data_json")
+    my_loader.set_output_tags("test:small")
 
     # Store this data as a SageWorks DataSource
     my_loader.transform()
-
-    # Grab the output and query it for a dataframe
-    output = AthenaSource(output_uuid)
-    df = output.query(f"select * from {output_uuid} limit 5")
-
-    # Setup Pandas output options
-    pd.set_option("display.max_colwidth", 15)
-    pd.set_option("display.max_columns", 15)
-    pd.set_option("display.width", 1000)
-
-    # Show the dataframe
-    print(df)
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CSVToDataSource: Class to move local CSV Files into a SageWorks DataSource"""
+import os
 import pandas as pd
 from pandas.errors import ParserError
 
 # Local imports
 from sageworks.transforms.transform import Transform, TransformInput, TransformOutput
 from sageworks.transforms.pandas_transforms.pandas_to_data import PandasToData
 
@@ -12,15 +13,15 @@
 
     Common Usage:
         csv_to_data = CSVToDataSource(csv_file_path, data_uuid)
         csv_to_data.set_output_tags(["abalone", "csv", "whatever"])
         csv_to_data.transform()
     """
 
-    def __init__(self, csv_file_path, data_uuid):
+    def __init__(self, csv_file_path: str, data_uuid: str):
         """CSVToDataSource: Class to move local CSV Files into a SageWorks DataSource"""
 
         # Call superclass init
         super().__init__(csv_file_path, data_uuid)
 
         # Set up all my instance attributes
         self.input_type = TransformInput.LOCAL_FILE
@@ -28,40 +29,47 @@
 
     def convert_columns_to_datetime(self, df: pd.DataFrame) -> pd.DataFrame:
         """Try to automatically convert object columns to datetime columns"""
         for c in df.columns[df.dtypes == "object"]:  # Look at the object columns
             try:
                 df[c] = pd.to_datetime(df[c])
             except (ParserError, ValueError):
-                self.log.info(f"Column {c} could not be converted to datetime...")
+                self.log.debug(f"Column {c} could not be converted to datetime...")
         return df
 
     def transform_impl(self, overwrite: bool = True):
         """Convert the local CSV file into Parquet Format in the SageWorks Data Sources Bucket, and
         store the information about the data to the AWS Data Catalog sageworks database"""
 
+        # Report the transformation initiation
+        csv_file = os.path.basename(self.input_uuid)
+        self.log.info(f"Starting {csv_file} -->  DataSource: {self.output_uuid}...")
+
         # Read in the Local CSV as a Pandas DataFrame
         df = pd.read_csv(self.input_uuid, low_memory=False)
         df = self.convert_columns_to_datetime(df)
 
         # Use the SageWorks Pandas to Data Source class
         pandas_to_data = PandasToData(self.output_uuid)
         pandas_to_data.set_input(df)
         pandas_to_data.set_output_tags(self.output_tags)
         pandas_to_data.add_output_meta(self.output_meta)
         pandas_to_data.transform()
 
+        # Report the transformation results
+        self.log.info(f"{csv_file} -->  DataSource: {self.output_uuid} Complete!")
+
 
 if __name__ == "__main__":
     """Exercise the CSVToDataSource Class"""
     import sys
     from pathlib import Path
 
     # Get the path to the dataset in the repository data directory
-    data_path = Path(sys.modules["sageworks"].__file__).parent.parent.parent / "data" / "test_data.csv"
+    data_path = str(Path(sys.modules["sageworks"].__file__).parent.parent.parent / "data" / "test_data.csv")
 
     # Create my Data Loader
     my_loader = CSVToDataSource(data_path, "test_data")
     my_loader.set_output_tags("test:small")
 
     # Store this data as a SageWorks DataSource
     my_loader.transform()
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.1.4.1/src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,97 @@
 """S3ToDataSourceLight: Class to move LIGHT S3 Files into a SageWorks DataSource"""
 import awswrangler as wr
+import pandas as pd
+from pandas.errors import ParserError
 
 # Local imports
 from sageworks.transforms.transform import Transform, TransformInput, TransformOutput
 from sageworks.transforms.pandas_transforms.pandas_to_data import PandasToData
 
 
 class S3ToDataSourceLight(Transform):
     """S3ToDataSourceLight: Class to move LIGHT S3 Files into a SageWorks DataSource
 
     Common Usage:
-        s3_to_data = S3ToDataSourceLight(s3_path, data_uuid)
+        s3_to_data = S3ToDataSourceLight(s3_path, data_uuid, datatype="csv/json")
         s3_to_data.set_output_tags(["abalone", "whatever"])
         s3_to_data.transform()
     """
 
-    def __init__(self, s3_path, data_uuid):
-        """S3ToDataSourceLight Initialization"""
+    def __init__(self, s3_path: str, data_uuid: str, datatype: str = "csv"):
+        """S3ToDataSourceLight Initialization
+        Args:
+            s3_path (str): The S3 Path to the file to be transformed
+            data_uuid (str): The UUID of the SageWorks DataSource to be created
+            datatype (str): The datatype of the file to be transformed (defaults to "csv")
+        """
 
         # Call superclass init
         super().__init__(s3_path, data_uuid)
 
         # Set up all my instance attributes
         self.input_type = TransformInput.S3_OBJECT
         self.output_type = TransformOutput.DATA_SOURCE
+        self.datatype = datatype
 
     def input_size_mb(self) -> int:
         """Get the size of the input S3 object in MBytes"""
         size_in_bytes = wr.s3.size_objects(self.input_uuid, boto3_session=self.boto_session)[self.input_uuid]
         size_in_mb = round(size_in_bytes / 1_000_000)
         return size_in_mb
 
+    def convert_object_columns(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Try to automatically convert object columns to datetime columns"""
+        for c in df.columns[df.dtypes == "object"]:  # Look at the object columns
+            try:
+                df[c] = pd.to_datetime(df[c])
+            except (ParserError, ValueError, TypeError):
+                self.log.debug(f"Column {c} could not be converted to datetime...")
+
+                # Now try to convert object to string
+                try:
+                    df[c] = df[c].astype(str)
+                except (ParserError, ValueError, TypeError):
+                    self.log.info(f"Column {c} could not be converted to string...")
+        return df
+
     def transform_impl(self, overwrite: bool = True):
         """Convert the CSV data into Parquet Format in the SageWorks Data Sources Bucket, and
         store the information about the data to the AWS Data Catalog sageworks database"""
 
         # Sanity Check for S3 Object size
         object_megabytes = self.input_size_mb()
         if object_megabytes > 100:
             self.log.error(f"S3 Object too big ({object_megabytes} MBytes): Use the S3ToDataSourceHeavy class!")
             return
 
         # Read in the S3 CSV as a Pandas DataFrame
-        df = wr.s3.read_csv(self.input_uuid, low_memory=False, boto3_session=self.boto_session)
+        if self.datatype == "csv":
+            df = wr.s3.read_csv(self.input_uuid, low_memory=False, boto3_session=self.boto_session)
+        else:
+            df = wr.s3.read_json(self.input_uuid, lines=True, boto3_session=self.boto_session)
+
+        # Convert object columns before sending to SageWorks Data Source
+        df = self.convert_object_columns(df)
 
         # Use the SageWorks Pandas to Data Source class
         pandas_to_data = PandasToData(self.output_uuid)
         pandas_to_data.set_input(df)
         pandas_to_data.set_output_tags(self.output_tags)
         pandas_to_data.add_output_meta(self.output_meta)
         pandas_to_data.transform()
 
 
 if __name__ == "__main__":
     """Exercise the S3ToDataSourceLight Class"""
+    from sageworks.utils.sageworks_config import SageWorksConfig
 
     # Create my Data Loader
-    input_path = "s3://scp-sageworks-artifacts/incoming-data/aqsol_public_data.csv"
+    sageworks_config = SageWorksConfig()
+    sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
+    input_path = sageworks_bucket + "/incoming-data/aqsol_public_data.csv"
     output_uuid = "aqsol_data"
     my_loader = S3ToDataSourceLight(input_path, output_uuid)
     my_loader.set_output_tags(["aqsol", "public"])
 
     # Store this data as a SageWorks DataSource
     my_loader.transform()
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/data_to_data/light/clean_data.py` & `sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/clean_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def __init__(self, input_data_uuid: str, output_data_uuid: str):
         """CleanData Initialization"""
 
         # Call superclass init
         super().__init__(input_data_uuid, output_data_uuid)
 
-    def transform_impl(self, drop_na="any"):
+    def transform_impl(self, drop_na="any", **kwargs):
         """Simple Clean Data, will improve later"""
 
         """
         Notes for later:
         Cleaning data typically involves two phases: Identification and Remediation.
 
         - Identification
@@ -45,7 +45,13 @@
 if __name__ == "__main__":
     """Exercise the CleanData Class"""
 
     # Create the class with inputs and outputs and invoke the transform
     input_uuid = "test_data"
     output_uuid = "test_data_clean"
     CleanData(input_uuid, output_uuid).transform(drop_na="any")
+
+    input_uuid = "test_data_json"
+    output_uuid = "test_data_json_clean"
+    data_to_data = CleanData(input_uuid, output_uuid)
+    data_to_data.set_output_tags(["test", "json", "clean"])
+    data_to_data.transform(drop_na="any")
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.1.4.1/src/sageworks/transforms/data_to_data/light/data_to_data_light.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """Base Class is simply an identity transform"""
         self.output_df = self.input_df
 
     def post_transform(self, **kwargs):
         """At this point the output DataFrame should be populated, so publish it as a DataSource"""
 
         # Now publish to the output location
-        output_data_source = PandasToData(self.output_uuid)
+        output_data_source = PandasToData(self.output_uuid, **kwargs)
         output_data_source.set_input(self.output_df)
         output_data_source.set_output_tags(self.output_tags)
         output_data_source.add_output_meta(self.output_meta)
         output_data_source.transform()
 
 
 if __name__ == "__main__":
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py` & `sageworks-0.1.4.1/src/sageworks/transforms/data_to_features/light/rdkit_descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # Turn off warnings for RDKIT (revisit this)
         RDLogger.DisableLog("rdApp.*")
 
     def transform_impl(self, **kwargs):
         """Compute a Feature Set based on RDKit Descriptors"""
 
         # Note: The parent class manages the input_df and output_df
-        #       So we simply need to grab the input and produce the output
+        #       So we simply need to grab the input_df and produce the output_df
 
         # Remove all the dataframe columns except for ID and SMILES
         self.output_df = self.input_df[["id", "smiles", "solubility"]]
 
         # Compute/add all the RDKIT Descriptors
         self.output_df = self.compute_rdkit_descriptors()
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/features_to_model/features_to_model.py` & `sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/features_to_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,32 @@
 
 
 class FeaturesToModel(Transform):
     """FeaturesToModel: Train/Create a Model from a FeatureSet
 
     Common Usage:
         to_model = FeaturesToModel(feature_uuid, model_uuid)
-        to_model.set_output_tags(["aqsol", "public", "whatever"])
-        to_model.transform(target="solubility", input_feature_list=<features>,
-                           model_type="regression/classification", delete_existing=True/False)
+        to_model.set_output_tags(["abalone", "public", "whatever"])
+        to_model.transform(target="class_number_of_rings", description="Abalone Regression Model".
+                           input_feature_list=<features>, model_type="regression/classification",
+                           delete_existing=True/False)
     """
 
     def __init__(self, feature_uuid: str, model_uuid: str):
         """FeaturesToModel Initialization"""
 
         # Call superclass init
         super().__init__(feature_uuid, model_uuid)
 
         # Set up all my instance attributes
         self.input_type = TransformInput.FEATURE_SET
         self.output_type = TransformOutput.MODEL
         self.estimator = None
         self.model_script_dir = None
+        self.model_description = None
 
     def generate_model_script(self, target: str, feature_list: list[str], model_type: str) -> str:
         """Fill in the model template with specific target and feature_list
         Args:
             target (str): Column name of the target variable
             feature_list (list[str]): A list of columns for the features
             model_type (str): regression or classification
@@ -59,38 +61,47 @@
         xgb_script = xgb_script.replace("{{model_type}}", model_type)
 
         # Now write out the generated model script and return the name
         with open(output_path, "w") as fp:
             fp.write(xgb_script)
         return script_name
 
-    def transform_impl(self, target, input_feature_list=None, model_type="regression", delete_existing=True):
+    def transform_impl(self, target, description, feature_list=None, model_type="regression", delete_existing=True):
         """Generic Features to Model: Note you should create a new class and inherit from
-        this one to include specific logic for your Feature Set/Model"""
+        this one to include specific logic for your Feature Set/Model
+        Args:
+            target (str): Column name of the target variable
+            description (str): Description of the model
+            feature_list (list[str]): A list of columns for the features
+            model_type (str): regression or classification
+            delete_existing (bool): Delete the existing model if it exists
+        """
+        # Set our model description
+        self.model_description = description
 
         # Get our Feature Set and create an S3 CSV Training dataset
         feature_set = FeatureSet(self.input_uuid)
         s3_training_path = feature_set.create_s3_training_data()
         self.log.info(f"Created new training data {s3_training_path}...")
 
-        # Did they specify a feature list?
-        if input_feature_list:
-            feature_list = input_feature_list
-
-        # Try to figure out features with this logic
-        # - Don't include id, event_time columns
-        # - Don't include AWS generated columns (e.g. write_time, api_invocation_time, is_deleted)
-        # - Don't include any columns that are of type string
-        # - The rest of the columns are assumed to be features
-        else:
-            self.log.warning("Guessing at the feature list, please specify a feature list!")
+        # If they didn't specify a feature list, try to guess it
+        if feature_list is None:
+            # Try to figure out features with this logic
+            # - Don't include id, event_time, __index_level_0__, or training columns
+            # - Don't include AWS generated columns (e.g. write_time, api_invocation_time, is_deleted)
+            # - Don't include the target columns
+            # - Don't include any columns that are of type string or timestamp
+            # - The rest of the columns are assumed to be features
+            self.log.warning("Guessing at the feature list, HIGHLY SUGGESTED to specify an explicit feature list!")
             all_columns = feature_set.column_names()
             filter_list = [
                 "id",
                 "event_time",
+                "__index_level_0__",
+                "training",
                 "write_time",
                 "api_invocation_time",
                 "is_deleted",
             ] + [target]
             feature_list = [c for c in all_columns if c not in filter_list]
 
             # Now remove any string or datetime columns from the Feature List
@@ -153,28 +164,20 @@
             model_package_group_name=self.output_uuid,
             framework_version="1.0.1",
             content_types=["text/csv"],
             response_types=["text/csv"],
             inference_instances=["ml.t2.medium"],
             transform_instances=["ml.m5.large"],
             approval_status="Approved",
-            description="Test Model: AQSol Regression",
+            description=self.model_description,
         )
 
 
 if __name__ == "__main__":
     """Exercise the FeaturesToModel Class"""
 
     # Create the class with inputs and outputs and invoke the transform
-    """
     input_uuid = "abalone_feature_set"
     output_uuid = "abalone-regression"
     to_model = FeaturesToModel(input_uuid, output_uuid)
     to_model.set_output_tags(["abalone", "public"])
     to_model.transform(target="class_number_of_rings")
-    """
-
-    input_uuid = "aqsol_feature_set"
-    output_uuid = "aqsol-regression"
-    to_model = FeaturesToModel(input_uuid, output_uuid)
-    to_model.set_output_tags(["aqsol", "public"])
-    to_model.transform(target="solubility", model_type="regression")
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.1.4.1/src/sageworks/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files 7% similar despite different names*

```diff
@@ -37,16 +37,23 @@
     # Combine files and read them all into a single pandas dataframe
     all_df = pd.concat([pd.read_csv(file, engine="python") for file in training_files])
 
     # Features/Target output
     print(f"Target: {target}")
     print(f"Features: {str(feature_list)}")
 
-    # Now Split based on training Split
-    df_train, df_val = train_test_split(all_df, test_size=validation_split)
+    # Does the dataframe have a training column?
+    if 'training' in all_df.columns:
+        print("Found training column, splitting data based on training column")
+        df_train = all_df[all_df['training'] == 1]
+        df_val = all_df[all_df['training'] == 0]
+    else:
+        # Just do a random training Split
+        print("No training column found, splitting data with random state=42")
+        df_train, df_val = train_test_split(all_df, test_size=validation_split, random_state=42)
     print(f'FIT/TRAIN: {df_train.shape}')
     print(f'VALIDATiON: {df_val.shape}')
 
     # Now spin up our XGB Model
     if model_type == 'classifier':
         xgb_model = xgb.XGBClassifier()
     else:
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.1.4.1/src/sageworks/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/data_to_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         my_df = data_to_df.get_output()
     """
 
     def __init__(self, input_uuid: str):
         """DataToPandas Initialization"""
 
         # Call superclass init
-        super().__init__(input_uuid, None)
+        super().__init__(input_uuid, "DataFrame")
 
         # Set up all my instance attributes
         self.input_type = TransformInput.DATA_SOURCE
         self.output_type = TransformOutput.PANDAS_DF
         self.output_df = None
         self.transform_run = False
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/features_to_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         my_df = feature_to_df.get_output()
     """
 
     def __init__(self, feature_set_name: str):
         """FeaturesToPandas Initialization"""
 
         # Call superclass init
-        super().__init__(input_uuid=feature_set_name, output_uuid=None)
+        super().__init__(input_uuid=feature_set_name, output_uuid="DataFrame")
 
         # Set up all my instance attributes
         self.input_type = TransformInput.FEATURE_SET
         self.output_type = TransformOutput.PANDAS_DF
         self.output_df = None
         self.transform_run = False
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_to_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """PandasToFeatures: Class to publish a Pandas DataFrame into a FeatureSet (Athena/FeatureStore)"""
 from datetime import datetime, timezone
 import pandas as pd
+import numpy as np
 import time
 import botocore
 from sagemaker.feature_store.feature_group import FeatureGroup
 
 # Local imports
 from sageworks.utils.iso_8601 import datetime_to_iso8601
 from sageworks.transforms.transform import Transform
@@ -21,73 +22,73 @@
         to_features.transform(delete_existing=True/False)
     """
 
     def __init__(self, output_uuid: str):
         """PandasToFeatures Initialization"""
 
         # Call superclass init
-        super().__init__(None, output_uuid)
+        super().__init__("DataFrame", output_uuid)
 
         # Set up all my instance attributes
-        self.input_df = None
         self.id_column = None
         self.event_time_column = None
+        self.output_df = None
 
     def set_input(self, input_df: pd.DataFrame, id_column=None, event_time_column=None):
         """Set the Input DataFrame for this Transform"""
         self.id_column = id_column
         self.event_time_column = event_time_column
-        self.input_df = input_df
+        self.output_df = input_df.copy()
 
     def _ensure_id_column(self):
         """Internal: AWS Feature Store requires an Id field for all data store"""
-        if self.id_column is None or self.id_column not in self.input_df.columns:
-            if "id" not in self.input_df.columns:
+        if self.id_column is None or self.id_column not in self.output_df.columns:
+            if "id" not in self.output_df.columns:
                 self.log.info("Generating an id column before FeatureSet Creation...")
-                self.input_df["id"] = self.input_df.index
+                self.output_df["id"] = self.output_df.index
             self.id_column = "id"
 
     def _ensure_event_time(self):
         """Internal: AWS Feature Store requires an event_time field for all data stored"""
-        if self.event_time_column is None or self.event_time_column not in self.input_df.columns:
+        if self.event_time_column is None or self.event_time_column not in self.output_df.columns:
             current_datetime = datetime.now(timezone.utc)
             self.log.info("Generating an event_time column before FeatureSet Creation...")
             self.event_time_column = "event_time"
-            self.input_df[self.event_time_column] = pd.Series([current_datetime] * len(self.input_df))
+            self.output_df[self.event_time_column] = pd.Series([current_datetime] * len(self.output_df))
 
         # The event_time_column is defined so lets make sure it the right type for Feature Store
-        if pd.api.types.is_datetime64_any_dtype(self.input_df[self.event_time_column]):
+        if pd.api.types.is_datetime64_any_dtype(self.output_df[self.event_time_column]):
             self.log.info(f"Converting {self.event_time_column} to ISOFormat Date String before FeatureSet Creation...")
 
             # Convert the datetime DType to ISO-8601 string
-            self.input_df[self.event_time_column] = self.input_df[self.event_time_column].map(datetime_to_iso8601)
-            self.input_df[self.event_time_column] = self.input_df[self.event_time_column].astype(pd.StringDtype())
+            self.output_df[self.event_time_column] = self.output_df[self.event_time_column].map(datetime_to_iso8601)
+            self.output_df[self.event_time_column] = self.output_df[self.event_time_column].astype(pd.StringDtype())
 
     def _convert_objs_to_string(self):
         """Internal: AWS Feature Store doesn't know how to store object dtypes, so convert to String"""
-        for col in self.input_df:
-            if pd.api.types.is_object_dtype(self.input_df[col].dtype):
-                self.input_df[col] = self.input_df[col].astype(pd.StringDtype())
+        for col in self.output_df:
+            if pd.api.types.is_object_dtype(self.output_df[col].dtype):
+                self.output_df[col] = self.output_df[col].astype(pd.StringDtype())
 
     # Helper Methods
     def categorical_converter(self):
         """Convert object and string types to Categorical"""
         categorical_columns = []
-        for feature, dtype in self.input_df.dtypes.items():
+        for feature, dtype in self.output_df.dtypes.items():
             print(feature, dtype)
             if dtype in ["object", "string"] and feature not in [self.event_time_column, self.id_column]:
-                unique_values = self.input_df[feature].nunique()
+                unique_values = self.output_df[feature].nunique()
                 print(f"Unique Values = {unique_values}")
                 if unique_values < 5:
                     print(f"Converting object column {feature} to categorical")
-                    self.input_df[feature] = self.input_df[feature].astype("category")
+                    self.output_df[feature] = self.output_df[feature].astype("category")
                     categorical_columns.append(feature)
 
         # Now convert Categorical Types to One Hot Encoding
-        self.input_df = pd.get_dummies(self.input_df, columns=categorical_columns)
+        self.output_df = pd.get_dummies(self.output_df, columns=categorical_columns)
 
     @staticmethod
     def convert_nullable_types(df: pd.DataFrame) -> pd.DataFrame:
         """Convert the new Pandas 'nullable types' since AWS SageMaker code doesn't currently support them
         See: https://github.com/aws/sagemaker-python-sdk/pull/3740"""
         for column in list(df.select_dtypes(include=[pd.Int64Dtype]).columns):
             df[column] = df[column].astype("int64")
@@ -103,32 +104,39 @@
         self._ensure_id_column()
         self._ensure_event_time()
 
         # Convert object and string types to Categorical
         self.categorical_converter()
 
         # Convert Int64 and Float64 types (see: https://github.com/aws/sagemaker-python-sdk/pull/3740)
-        self.input_df = self.convert_nullable_types(self.input_df)
+        self.output_df = self.convert_nullable_types(self.output_df)
+
+        # FeatureSet Internal Storage (Athena) will convert columns names to lowercase, so we need
+        # to make sure that the column names are lowercase to match and avoid downstream issues
+        self.output_df.columns = self.output_df.columns.str.lower()
+
+        # Mark 80% of the data as training and 20% as validation/test
+        self.output_df["training"] = np.random.binomial(size=len(self.output_df), n=1, p=0.8)
 
         # Do we want to delete the existing FeatureSet?
         if delete_existing:
             try:
                 delete_fs = FeatureSet(self.output_uuid)
                 if delete_fs.check():
                     delete_fs.delete()
             except botocore.exceptions.ClientError as exc:
                 self.log.info(f"FeatureSet {self.output_uuid} doesn't exist...")
                 self.log.info(exc)
 
         # Create a Feature Group and load our Feature Definitions
         my_feature_group = FeatureGroup(name=self.output_uuid, sagemaker_session=self.sm_session)
-        my_feature_group.load_feature_definitions(data_frame=self.input_df)
+        my_feature_group.load_feature_definitions(data_frame=self.output_df)
 
         # Create the Output Parquet file S3 Storage Path for this Feature Set
-        s3_storage_path = f"{self.feature_set_s3_path}/{self.output_uuid}"
+        s3_storage_path = f"{self.feature_sets_s3_path}/{self.output_uuid}"
 
         # Data Catalog Config
         # FIXME: AWS wants to put Feature Groups into the 'sagemaker_features' database
         #        and a random table name. We can overwrite these but then the AWS Glue
         #        Catalog Table isn't automatically created.
         """
         my_config = DataCatalogConfig(table_name=self.output_uuid,
@@ -151,15 +159,15 @@
             # disable_glue_table_creation=True
         )
 
         # Ensure/wait for the feature group to be created
         self.ensure_feature_group_created(my_feature_group)
 
         # Now we actually push the data into the Feature Group
-        my_feature_group.ingest(self.input_df, max_processes=4)
+        my_feature_group.ingest(self.output_df, max_processes=4)
 
     def ensure_feature_group_created(self, feature_group):
         status = feature_group.describe().get("FeatureGroupStatus")
         while status == "Creating":
             self.log.info("FeatureSet being Created...")
             time.sleep(5)
             status = feature_group.describe().get("FeatureGroupStatus")
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/pandas_transforms/pandas_utils.py` & `sageworks-0.1.4.1/src/sageworks/transforms/pandas_transforms/pandas_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Setup Logging
 logging_setup()
 log = logging.getLogger(__name__)
 
 
 def get_percent_nan(df):
-    log.info("Dataframe ({:d} rows)".format(len(df)))
+    log.info("DataFrame ({:d} rows)".format(len(df)))
     s = df.isna().mean().round(3) * 100.0
     s.name = "percent_nan"
     return s
 
 
 def unique(df):
     s = df.nunique()
```

### Comparing `sageworks-0.1.4/src/sageworks/transforms/transform.py` & `sageworks-0.1.4.1/src/sageworks/transforms/transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from enum import Enum, auto
 from typing import final
 import logging
 import awswrangler as wr
 
 # SageWorks Imports
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
+from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
 
 # Setup Logging
 logging_setup()
 
 
 class TransformInput(Enum):
@@ -38,52 +39,55 @@
     ENDPOINT = auto()
 
 
 class Transform(ABC):
     """Transform: Base Class for all transforms within SageWorks. Inherited Classes
     must implement the abstract transform_impl() method"""
 
-    def __init__(self, input_uuid: str | None, output_uuid: str | None):
+    def __init__(self, input_uuid: str, output_uuid: str):
         """Transform Initialization"""
 
         self.log = logging.getLogger(__name__)
         self.input_type = None
         self.output_type = None
         self.output_tags = ""
-        self.input_uuid = input_uuid
-        self.output_uuid = output_uuid
-        self.output_meta = {'sageworks_input': self.input_uuid}
+        self.input_uuid = str(input_uuid)  # Occasionally we get a pathlib.Path object
+        self.output_uuid = str(output_uuid)  # Occasionally we get a pathlib.Path object
+        self.output_meta = {"sageworks_input": self.input_uuid}
 
-        # FIXME: We should have this come from AWS or Config
+        # Grab our SageWorksConfig for S3 Buckets and other SageWorks specific settings
+        sageworks_config = SageWorksConfig()
         self.data_catalog_db = "sageworks"
-        self.data_source_s3_path = "s3://scp-sageworks-artifacts/data-sources"
-        self.feature_set_s3_path = "s3://scp-sageworks-artifacts/feature-sets"
+        sageworks_bucket = sageworks_config.get_config_value("SAGEWORKS_AWS", "S3_BUCKET")
+        self.data_source_s3_path = sageworks_bucket + "/data-sources"
+        self.feature_sets_s3_path = sageworks_bucket + "/feature-sets"
 
         # Grab a SageWorks Role ARN, Boto3, SageMaker Session, and SageMaker Client
-        self.sageworks_role_arn = AWSAccountClamp().sageworks_execution_role_arn()
-        self.boto_session = AWSAccountClamp().boto_session()
-        self.sm_session = AWSAccountClamp().sagemaker_session()
-        self.sm_client = AWSAccountClamp().sagemaker_client()
+        self.aws_account_clamp = AWSAccountClamp()
+        self.sageworks_role_arn = self.aws_account_clamp.sageworks_execution_role_arn()
+        self.boto_session = self.aws_account_clamp.boto_session()
+        self.sm_session = self.aws_account_clamp.sagemaker_session(self.boto_session)
+        self.sm_client = self.aws_account_clamp.sagemaker_client(self.boto_session)
 
         # Make sure the AWS data catalog database exists
         self.ensure_aws_catalog_db(self.data_catalog_db)
         self.ensure_aws_catalog_db("sagemaker_featurestore")
 
     @abstractmethod
     def transform_impl(self, **kwargs):
         """Abstract Method: Implement the Transformation from Input to Output"""
         pass
 
     def pre_transform(self, **kwargs):
         """Perform any Pre-Transform operations"""
-        self.log.info("Pre-Transform...")
+        self.log.debug("Pre-Transform...")
 
     def post_transform(self, **kwargs):
         """Perform any Post-Transform operations"""
-        self.log.info("Post-Transform...")
+        self.log.debug("Post-Transform...")
 
     def set_output_tags(self, tags: list | str):
         """Set the tags that will be associated with the output object
         Args:
             tags (list | str): The list of tags or a ':' separated string of tags"""
         if isinstance(tags, list):
             self.output_tags = ":".join(tags)
```

### Comparing `sageworks-0.1.4/src/sageworks/utils/cache.py` & `sageworks-0.1.4.1/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.1.4.1/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/utils/iso_8601.py` & `sageworks-0.1.4.1/src/sageworks/utils/iso_8601.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/utils/redis_cache.py` & `sageworks-0.1.4.1/src/sageworks/utils/redis_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import redis
 import logging
 from datetime import datetime, date
 
 # Local Imports
 from sageworks.utils.iso_8601 import datetime_to_iso8601, iso8601_to_datetime
+from sageworks.utils.sageworks_config import SageWorksConfig
 from sageworks.utils.sageworks_logging import logging_setup
 
 # Setup Logging
 logging_setup()
 
 
 class RedisCache:
@@ -24,18 +25,19 @@
          > None
          redis_cache.clear()
     """
 
     # Setup logger (class attribute)
     log = logging.getLogger(__name__)
 
-    # FIXME: Get these from SageWorks configuration
-    host = "localhost"
-    port = 6379
-    password = None
+    # Grab our SageWorksConfig for SageWorks specific settings
+    sageworks_config = SageWorksConfig()
+    host = sageworks_config.get_config_value("SAGEWORKS_REDIS", "HOST")
+    port = sageworks_config.get_config_value("SAGEWORKS_REDIS", "PORT")
+    password = sageworks_config.get_config_value("SAGEWORKS_REDIS", "PASSWORD") or None
 
     # Open the Redis connection (class object)
     log.info(f"Opening Redis connection to: {host}:{port}...")
     redis_db = redis.Redis(host, port=port, password=password, charset="utf-8", decode_responses=True, db=0)
     try:
         redis_db.ping()
         log.info(f"Redis connection success: {host}:{port}...")
```

### Comparing `sageworks-0.1.4/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.1.4.1/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class SageWorksEventBridge:
     def __init__(self, bus_name="sageworks"):
         """SageWorksEventBridge: Class for publishing events to AWS EventBridge"""
         self.log = logging.getLogger(__name__)
         self.event_bus = bus_name
 
-        # Grab a SageWorks Session (this allows us to assume the SageWorks-ExecutionRole)
+        # Grab a SageWorks Session (this allows us to assume the SageWorks ExecutionRole)
         self.boto_session = AWSAccountClamp().boto_session()
 
         # Get our AWS EventBridge Client
         self.event_bridge = self.boto_session.client("events")
 
     def create_artifact(self, uuid: str, artifact_type: ArtifactType):
         event = {
```

### Comparing `sageworks-0.1.4/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.1.4.1/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.1.4.1/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/views/artifacts_summary.py` & `sageworks-0.1.4.1/src/sageworks/views/artifacts_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,59 @@
 """ArtifactsSummary pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
 import sys
 import argparse
-import awswrangler as wr
 import pandas as pd
 
 # SageWorks Imports
 from sageworks.views.view import View
-from sageworks.utils.cache import Cache
 from sageworks.aws_service_broker.aws_service_broker import ServiceCategory
 from sageworks.aws_service_broker.aws_account_clamp import AWSAccountClamp
 
 
 class ArtifactsSummary(View):
     def __init__(self):
         """ArtifactsSummary pulls All the metadata from the AWS Service Broker and organizes/summarizes it"""
         # Call SuperClass Initialization
         super().__init__()
 
         # Get AWS Service information for ALL the categories (data_source, feature_set, endpoints, etc)
-        self.service_info = self.aws_broker.get_all_metadata()
-        self.sm_session = AWSAccountClamp().sagemaker_session()
+        self.aws_artifact_data = self.aws_broker.get_all_metadata()
+        self.aws_account_clamp = AWSAccountClamp()
 
-        # Summary data for ALL the AWS Services
-        self.summary_data = {}
-
-        # S3 Object Size Cache
-        self.size_cache = Cache(expire=60)
+        # Get a handle to the AWS Artifact Information class
+        self.artifact_info = self.aws_broker.artifact_info
 
     def check(self) -> bool:
         """Can we connect to this view/service?"""
         return True  # I'm great, thx for asking
 
     def refresh(self):
         """Refresh data/metadata associated with this view"""
-        self.service_info = self.aws_broker.get_all_metadata()
-
-    def s3_objects_size(self, s3_path) -> bool:
-        """Return the size of this data in MegaBytes"""
-        size_in_mb = self.size_cache.get(s3_path)
-        if size_in_mb is None:
-            self.log.info(f"Computing S3 Object sizes: {s3_path}...")
-            size_in_bytes = sum(wr.s3.size_objects(s3_path, boto3_session=self.boto_session).values())
-            size_in_mb = f"{ (size_in_bytes/1_000_000):.1f}"
-            self.size_cache.set(s3_path, size_in_mb)
-        return size_in_mb
-
-    @staticmethod
-    def aws_tags_to_dict(aws_tags):
-        """AWS Tags are in an odd format, so convert to regular dictionary"""
-        return {item["Key"]: item["Value"] for item in aws_tags if "sageworks" in item["Key"]}
-
-    def artifact_meta(self, aws_arn):
-        """Get the Metadata for this Artifact"""
-        meta = self.size_cache.get(aws_arn)
-        if meta is None:
-            self.log.info(f"Retrieving Artifact Tags, Metadata, and S3 Object Size: {aws_arn}...")
-            aws_tags = self.sm_session.list_tags(aws_arn)
-            meta = self.aws_tags_to_dict(aws_tags)
-            self.size_cache.set(aws_arn, meta)
-        return meta
+        self.aws_artifact_data = self.aws_broker.get_all_metadata()
 
     def view_data(self) -> dict:
         """Get all the data that's useful for this view
 
         Returns:
-            dict: Dictionary of Pandas Dataframes, i.e. {'INCOMING_DATA', pd.DataFrame}
+            dict: Dictionary of Pandas Dataframes, e.g. {'INCOMING_DATA': pd.DataFrame, ...}
         """
 
         # We're filling in Summary Data for all the AWS Services
-        self.log.warning("Refreshing ALL AWS Service Broker Metadata...")
-        self.summary_data["INCOMING_DATA"] = self.incoming_data_summary()
-        self.summary_data["DATA_SOURCES"] = self.data_sources_summary()
-        self.summary_data["FEATURE_SETS"] = self.feature_sets_summary()
-        self.summary_data["MODELS"] = self.models_summary()
-        self.summary_data["ENDPOINTS"] = self.endpoints_summary()
-        return self.summary_data
+        summary_data = {
+            "INCOMING_DATA": self.incoming_data_summary(),
+            "DATA_SOURCES": self.data_sources_summary(),
+            "FEATURE_SETS": self.feature_sets_summary(),
+            "MODELS": self.models_summary(),
+            "ENDPOINTS": self.endpoints_summary(),
+        }
+        return summary_data
 
     def incoming_data_summary(self):
         """Get summary data about data in the incoming-data S3 Bucket"""
-        data = self.service_info[ServiceCategory.INCOMING_DATA]
+        data = self.aws_artifact_data[ServiceCategory.INCOMING_DATA]
         data_summary = []
         for name, info in data.items():
             # Get the size of the S3 Storage Object(s)
             size = info.get("ContentLength") / 1_000_000
             summary = {
                 "Name": name,
                 "Size(MB)": f"{size:.1f}",
@@ -95,34 +66,37 @@
             }
             data_summary.append(summary)
 
         return pd.DataFrame(data_summary)
 
     def data_sources_summary(self):
         """Get summary data about the SageWorks DataSources"""
-        data = self.service_info[ServiceCategory.DATA_CATALOG]
+        data = self.aws_artifact_data[ServiceCategory.DATA_CATALOG]
         data_summary = []
-        for name, info in data["sageworks"].items():  # Just the sageworks database (not sagemaker_featurestore)
-            # Get the size of the S3 Storage Object(s)
-            size = self.s3_objects_size(info["StorageDescriptor"]["Location"])
-            summary = {
-                "Name": self.hyperlinks(name, "data_sources"),
-                "Ver": info.get("VersionId", "-"),
-                "Size(MB)": size,
-                "Catalog DB": info.get("DatabaseName", "-"),
-                # 'Created': self.datetime_string(info.get('CreateTime')),
-                "Modified": self.datetime_string(info.get("UpdateTime")),
-                "Num Columns": self.num_columns(info),
-                "DataLake": info.get("IsRegisteredWithLakeFormation", "-"),
-                "Tags": info.get("Parameters", {}).get("sageworks_tags", "-"),
-                "Input": str(
-                    info.get("Parameters", {}).get("sageworks_input", "-"),
-                ),
-            }
-            data_summary.append(summary)
+
+        # Get the SageWorks DataSources
+        if "sageworks" in data:
+            for name, info in data["sageworks"].items():  # Just the sageworks database (not sagemaker_featurestore)
+                # Get the size of the S3 Storage Object(s)
+                size = self.artifact_info.s3_object_sizes(info["StorageDescriptor"]["Location"])
+                summary = {
+                    "Name": self.hyperlinks(name, "data_sources"),
+                    "Ver": info.get("VersionId", "-"),
+                    "Size(MB)": size,
+                    "Catalog DB": info.get("DatabaseName", "-"),
+                    # 'Created': self.datetime_string(info.get('CreateTime')),
+                    "Modified": self.datetime_string(info.get("UpdateTime")),
+                    "Num Columns": self.num_columns(info),
+                    "DataLake": info.get("IsRegisteredWithLakeFormation", "-"),
+                    "Tags": info.get("Parameters", {}).get("sageworks_tags", "-"),
+                    "Input": str(
+                        info.get("Parameters", {}).get("sageworks_input", "-"),
+                    ),
+                }
+                data_summary.append(summary)
 
         # Make sure we have data else return just the column names
         if data_summary:
             return pd.DataFrame(data_summary)
         else:
             columns = [
                 "Name",
@@ -133,32 +107,31 @@
                 "Num Columns",
                 "DataLake",
                 "Tags",
                 "Input",
             ]
             return pd.DataFrame(columns=columns)
 
-    @staticmethod
-    def hyperlinks(name, detail_type):
-        athena_url = "https://us-west-2.console.aws.amazon.com/athena/home"
+    def hyperlinks(self, name, detail_type):
+        athena_url = f"https://{self.aws_account_clamp.region()}.console.aws.amazon.com/athena/home"
         link = f"<a href='{detail_type}' target='_blank'>{name}</a>"
         link += f" [<a href='{athena_url}' target='_blank'>query</a>]"
         return link
 
     def feature_sets_summary(self):
         """Get summary data about the SageWorks FeatureSets"""
-        data = self.service_info[ServiceCategory.FEATURE_STORE]
+        data = self.aws_artifact_data[ServiceCategory.FEATURE_STORE]
         data_summary = []
         for feature_group, group_info in data.items():
             # Get the tags for this Feature Group
             arn = group_info["FeatureGroupArn"]
-            sageworks_meta = self.artifact_meta(arn)
+            sageworks_meta = self.artifact_info.get_sagemaker_obj_info(arn)
 
             # Get the size of the S3 Storage Object(s)
-            size = self.s3_objects_size(group_info["OfflineStoreConfig"]["S3StorageConfig"]["S3Uri"])
+            size = self.artifact_info.s3_object_sizes(group_info["OfflineStoreConfig"]["S3StorageConfig"]["S3Uri"])
             summary = {
                 "Feature Group": self.hyperlinks(group_info["FeatureGroupName"], "feature_sets"),
                 # 'Status': group_info['FeatureGroupStatus'],
                 "Size(MB)": size,
                 "Catalog DB": group_info["OfflineStoreConfig"].get("DataCatalogConfig", {}).get("Database", "-"),
                 "Athena Table": group_info["OfflineStoreConfig"].get("DataCatalogConfig", {}).get("TableName", "-"),
                 # 'ID/EventTime': f"{group_info['RecordIdentifierFeatureName']}/{group_info['EventTimeFeatureName']}",
@@ -183,28 +156,28 @@
                 "Tags",
                 "Input",
             ]
             return pd.DataFrame(columns=columns)
 
     def models_summary(self, concise=False):
         """Get summary data about the SageWorks Models"""
-        data = self.service_info[ServiceCategory.MODELS]
+        data = self.aws_artifact_data[ServiceCategory.MODELS]
         model_summary = []
         for model_group, model_list in data.items():
             # Special Case for Model Groups without any Models
             if not model_list:
                 summary = {"Model Group": model_group}
                 model_summary.append(summary)
                 continue
 
             # Get Summary information for each model in the model_list
             for model in model_list:
                 # Get the tags for this Model Group
                 model_group_arn = model["ModelPackageGroupArn"]
-                sageworks_meta = self.artifact_meta(model_group_arn)
+                sageworks_meta = self.artifact_info.get_sagemaker_obj_info(model_group_arn)
 
                 # Do they want the full details or just the concise summary?
                 if concise:
                     summary = {
                         "Model Group": self.hyperlinks(model["ModelPackageGroupName"], "models"),
                         "Description": model["ModelPackageDescription"],
                         "Created": self.datetime_string(model.get("CreationTime")),
@@ -236,22 +209,22 @@
                 "Tags",
                 "Input",
             ]
             return pd.DataFrame(columns=columns)
 
     def endpoints_summary(self):
         """Get summary data about the SageWorks Endpoints"""
-        data = self.service_info[ServiceCategory.ENDPOINTS]
+        data = self.aws_artifact_data[ServiceCategory.ENDPOINTS]
         data_summary = []
 
         # Get Summary information for each endpoint
         for endpoint, endpoint_info in data.items():
             # Get the tags for this Model Group
             endpoint_arn = endpoint_info["EndpointArn"]
-            sageworks_meta = self.artifact_meta(endpoint_arn)
+            sageworks_meta = self.artifact_info.get_sagemaker_obj_info(endpoint_arn)
 
             summary = {
                 "Name": self.hyperlinks(endpoint_info["EndpointName"], "endpoints"),
                 "Status": endpoint_info["EndpointStatus"],
                 "Created": self.datetime_string(endpoint_info.get("CreationTime")),
                 # "Modified": self.datetime_string(endpoint_info.get("LastModifiedTime")),
                 "DataCapture": str(endpoint_info.get("DataCaptureConfig", {}).get("EnableCapture", "False")),
```

### Comparing `sageworks-0.1.4/src/sageworks/views/view.py` & `sageworks-0.1.4.1/src/sageworks/views/view.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 class View(ABC):
     def __init__(self):
         """View: View in the database sense: Pulls from the AWS Service Broker and does slice and dice"""
         self.log = logging.getLogger(__name__)
 
         # Grab an AWS Metadata Broker object for pulling AWS Service information
         self.aws_broker = AWSServiceBroker()
-        self.boto_session = AWSAccountClamp().boto_session()
+        self.aws_account_clamp = AWSAccountClamp()
+        self.boto_session = self.aws_account_clamp.boto_session()
+        self.sm_session = self.aws_account_clamp.sagemaker_session()
 
     @abstractmethod
     def check(self) -> bool:
         """Can we connect to this view/service?"""
         pass
 
     @abstractmethod
```

### Comparing `sageworks-0.1.4/src/sageworks/web_components/box_plot.py` & `sageworks-0.1.4.1/src/sageworks/web_components/box_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.1.4.1/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/feature_details.py` & `sageworks-0.1.4.1/src/sageworks/web_components/feature_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/feature_importance.py` & `sageworks-0.1.4.1/src/sageworks/web_components/feature_importance.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/histogram.py` & `sageworks-0.1.4.1/src/sageworks/web_components/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/line_chart.py` & `sageworks-0.1.4.1/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/model_data.py` & `sageworks-0.1.4.1/src/sageworks/web_components/model_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/model_details.py` & `sageworks-0.1.4.1/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/scatter_plot.py` & `sageworks-0.1.4.1/src/sageworks/web_components/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks/web_components/table.py` & `sageworks-0.1.4.1/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.1.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: SageWorks: An easy to use WorkBench for creating and deploying SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 3 - Alpha
@@ -25,18 +25,14 @@
 SageWorks is a medium granularity framework that manages and aggregates AWS® Services into classes and concepts. When you use SageWorks you think about **DataSources**, **FeatureSets**, **Models**, and **Endpoints**. Underneath the hood those classes handle all the details around updating and managing a **complex set of AWS Services**. All the power and none of the pain so that your team can **Do Science Faster!**
 
 <img src="docs/images/sageworks_concepts.png">
 
 ### Full SageWorks OverView
 [SageWorks Architected FrameWork](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing)
 
-### Getting Started Video Demo
-[SageWorks Getting Started](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) This video is an informal screen capture + chatting while I'm coding. The video demonstrates creating an entire AWS ML Pipeline, from data ingestion, to feature sets, to models and endpoints.
-
-
 
 ## Why SageWorks?
 
 <img align="right" src="docs/images/graph_representation.png" width="300">
 
 - The AWS SageMaker® ecosystem is **awesome** but has a large number of services with significant complexity
 - SageWorks provides **rapid prototyping** through easy to use **classes** and **transforms**
@@ -49,27 +45,26 @@
 
 **Single pane of glass** visibility into the AWS Services that underpin the SageWorks Classes. We can see that SageWorks automatically tags and tracks the inputs of all artifacts providing 'data provenance' for all steps in the AWS modeling pipeline.
 
 <img width="1000" alt="Screenshot 2023-03-31 at 2 16 36 PM" src="https://user-images.githubusercontent.com/4806709/229222245-59e342c1-7254-47de-a453-268448643143.png">
 
 <i><b> Clearly illustrated:</b> SageWorks provides intuitive and transparent visibility into the full pipeline of your AWS Sagemaker Deployments.</i>
 
-## Installation
-```
-pip install sageworks
-```
-
-### Gettting Started
-SageWorks has a large number of classes and components, the best place to get started is our [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) and [SageWorks Wiki](https://github.com/SuperCowPowers/sageworks/wiki) for developers wanting to try out the Python API. 
 
-Video: [SageWorks Getting Started](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) shows an informal screen capture + chatting while I'm coding. The video demonstrates creating an entire AWS ML Pipeline, from data ingestion, to feature sets, to models and endpoints.
+## Getting Started
+- [SageWorks Overview](https://docs.google.com/presentation/d/1ZiSy4ulEx5gfNQS76yRv8vgkehJ9gXRJ1PulutLKzis/edit?usp=sharing) Slides that cover and illustrate the SageWorks Modeling Pipeline.
+- [Initial Setup and Installation](https://github.com/SuperCowPowers/sageworks/wiki/Initial-Setup-and-Installation) for initial AWS/config/repository set up. 
+- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from start to finish.
+- [Coding with SageWorks Video](https://drive.google.com/file/d/1iO7IuQtTYdx4BtQjxv9lI1aVJ2ZcAo43/view?usp=sharing) Informal coding + chatting while building a full ML pipeline.
+- Join our [Discord](https://discord.gg/WHAJuz8sw8) for questions and advice on using SageWorks within your organization.
 
-You can also join us on Discord <https://discord.gg/WHAJuz8sw8> for questions and advice on using SageWorks within your organization.
+### SageWorks Analysis Notebooks
+- [SageWorks Pipeline](https://nbviewer.jupyter.org/github/SuperCowPowers/sageworks/blob/main/notebooks/ML_Pipeline_with_SageWorks.ipynb) Building an AWS® ML Pipeline from Start to Finish
 
-### SageWorks Zen``
+### SageWorks Zen
 - The AWS SageMaker® set of services is vast and **complex**.
 - SageWorks Classes encapsulate, organize, and manage sets of AWS® Services.
 - **Heavy** transforms typically use **[AWS Athena](https://aws.amazon.com/athena/)** or **[Apache Spark](https://spark.apache.org/)** (AWS Glue/EMR Serverless).
 - **Light** transforms will typically use **[Pandas](https://pandas.pydata.org/)**.
 - Heavy and Light transforms both update **AWS Artifacts** (collections of AWS Services).
 - **Quick prototypes** are typically built with the **light path** and then flipped to the **heavy path** as the system matures and usage grows.
```

### Comparing `sageworks-0.1.4/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.1.4.1/src/sageworks.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -38,16 +38,32 @@
 applications/model_viewer/data/toy_data.csv
 applications/model_viewer/data/toy_scores.json
 applications/web_admin/flask_test.py
 applications/web_admin/hello-world-http-test.ini
 applications/web_admin/hello-world.ini
 applications/web_admin/hello-world.service
 applications/web_admin/nginx_conf/nginx.conf
+aws_setup/aws_account_check.py
+aws_setup/aws_account_check_deep.py
+aws_setup/sageworks_sandbox/.gitignore
+aws_setup/sageworks_sandbox/README.md
+aws_setup/sageworks_sandbox/app.py
+aws_setup/sageworks_sandbox/cdk.json
+aws_setup/sageworks_sandbox/requirements-dev.txt
+aws_setup/sageworks_sandbox/requirements.txt
+aws_setup/sageworks_sandbox/source.bat
+aws_setup/sageworks_sandbox/sageworks_sandbox/__init__.py
+aws_setup/sageworks_sandbox/sageworks_sandbox/sageworks_sandbox_stack.py
+aws_setup/sageworks_sandbox/tests/__init__.py
+aws_setup/sageworks_sandbox/tests/unit/__init__.py
+aws_setup/sageworks_sandbox/tests/unit/test_sageworks_sandbox_stack.py
+config/sageworks_config.ini
 data/abalone.csv
 data/test_data.csv
+data/test_data.json
 docs/admin_notes.md
 docs/sageworks_classes_concepts.md
 docs/scp_consulting.md
 docs/images/big_spider.png
 docs/images/graph_representation.png
 docs/images/powered_aws_dark_blue.png
 docs/images/powered_aws_transparent.png
@@ -55,15 +71,23 @@
 docs/images/powered_aws_with_tm_grey.png
 docs/images/sageworks.png
 docs/images/sageworks_concepts.png
 docs/images/scp.png
 docs/images/scp_labs.png
 docs/images/small_spider.png
 examples/data_to_data_example.py
+notebooks/ML_Pipeline_with_SageWorks.ipynb
+notebooks/images/athena_query_aqsol.png
+notebooks/images/aws_dashboard_aqsol.png
+notebooks/images/dashboard_aqsol_features.png
+notebooks/images/model_screenshot.png
+notebooks/images/sageworks_concepts.png
+notebooks/images/scp_labs.png
 scripts/data_source_tags.py
+scripts/generate_jsonl_data.py
 scripts/list_data_sources.py
 src/sageworks/__init__.py
 src/sageworks.egg-info/PKG-INFO
 src/sageworks.egg-info/SOURCES.txt
 src/sageworks.egg-info/dependency_links.txt
 src/sageworks.egg-info/requires.txt
 src/sageworks.egg-info/top_level.txt
@@ -77,34 +101,37 @@
 src/sageworks/algorithms/table/light/row_tagger.py
 src/sageworks/artifacts/Readme.md
 src/sageworks/artifacts/__init__.py
 src/sageworks/artifacts/artifact.py
 src/sageworks/artifacts/data_sources/__init__.py
 src/sageworks/artifacts/data_sources/athena_source.py
 src/sageworks/artifacts/data_sources/data_source.py
+src/sageworks/artifacts/data_sources/data_source_abstract.py
 src/sageworks/artifacts/endpoints/__init__.py
 src/sageworks/artifacts/endpoints/endpoint.py
 src/sageworks/artifacts/feature_sets/__init__.py
 src/sageworks/artifacts/feature_sets/feature_set.py
 src/sageworks/artifacts/models/__init__.py
 src/sageworks/artifacts/models/model.py
 src/sageworks/aws_service_broker/aws_account_clamp.py
 src/sageworks/aws_service_broker/aws_service_broker.py
 src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+src/sageworks/aws_service_broker/aws_service_connectors/artifact_info.py
 src/sageworks/aws_service_broker/aws_service_connectors/connector.py
 src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
 src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
 src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
 src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
 src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
 src/sageworks/transforms/Readme.md
 src/sageworks/transforms/__init__.py
 src/sageworks/transforms/transform.py
 src/sageworks/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
 src/sageworks/transforms/data_loaders/light/csv_to_data_source.py
+src/sageworks/transforms/data_loaders/light/json_to_data_source.py
 src/sageworks/transforms/data_loaders/light/s3_to_data_source_light.py
 src/sageworks/transforms/data_to_data/__init__.py
 src/sageworks/transforms/data_to_data/heavy/__init__.py
 src/sageworks/transforms/data_to_data/heavy/emr/Readme.md
 src/sageworks/transforms/data_to_data/heavy/glue/Readme.md
 src/sageworks/transforms/data_to_data/light/__init__.py
 src/sageworks/transforms/data_to_data/light/clean_data.py
@@ -131,14 +158,15 @@
 src/sageworks/transforms/pandas_transforms/pandas_to_features.py
 src/sageworks/transforms/pandas_transforms/pandas_utils.py
 src/sageworks/utils/__init__.py
 src/sageworks/utils/cache.py
 src/sageworks/utils/df_to_endpoint.py
 src/sageworks/utils/iso_8601.py
 src/sageworks/utils/redis_cache.py
+src/sageworks/utils/sageworks_config.py
 src/sageworks/utils/sageworks_event_bridge.py
 src/sageworks/utils/sageworks_logging.py
 src/sageworks/utils/sageworks_sqs.py
 src/sageworks/views/artifacts_summary.py
 src/sageworks/views/view.py
 src/sageworks/web_components/box_plot.py
 src/sageworks/web_components/confusion_matrix.py
```

### Comparing `sageworks-0.1.4/tests/artifacts/data_source_tests.py` & `sageworks-0.1.4.1/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/artifacts/endpoint_tests.py` & `sageworks-0.1.4.1/tests/artifacts/endpoint_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Tests for the Endpoint functionality"""
-import pandas as pd
 
 # SageWorks Imports
 from sageworks.artifacts.endpoints.endpoint import Endpoint
 
 
 def test():
     """Simple test of the Endpoint functionality"""
-    from sageworks.transforms.pandas_transforms.features_to_pandas import (
-        FeaturesToPandas,
-    )
-    from sklearn.metrics import mean_absolute_error, r2_score, mean_squared_error
-    from math import sqrt
+    from sageworks.transforms.pandas_transforms.features_to_pandas import FeaturesToPandas
 
     # Grab an Endpoint object and pull some information from it
-    my_endpoint = Endpoint("abalone-regression-endpoint")
+    my_endpoint = Endpoint("abalone-regression-end")
 
     # Call the various methods
 
     # Let's do a check/validation of the Endpoint
     assert my_endpoint.check()
 
     # Creation/Modification Times
@@ -40,14 +35,14 @@
 
     # Okay now run inference against our Features DataFrame
     result_df = my_endpoint.predict(feature_df)
     print(result_df)
 
     # Compute performance metrics for our test predictions
     target_column = "class_number_of_rings"
-    metrics = my_endpoint.performance_metrics(target_column, prediction_df)
+    metrics = my_endpoint.performance_metrics(target_column, result_df)
     for metric, value in metrics.items():
         print(f"{metric}: {value:0.3f}")
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `sageworks-0.1.4/tests/artifacts/feature_set_tests.py` & `sageworks-0.1.4.1/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/artifacts/model_tests.py` & `sageworks-0.1.4.1/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.1.4.1/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/transforms/data_to_data_tests.py` & `sageworks-0.1.4.1/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/transforms/data_to_features_tests.py` & `sageworks-0.1.4.1/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/transforms/features_to_model_tests.py` & `sageworks-0.1.4.1/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.1.4.1/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.1.4/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.1.4.1/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

