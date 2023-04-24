# Comparing `tmp/folio_migration_tools-1.7.9rc2.tar.gz` & `tmp/folio_migration_tools-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folio_migration_tools-1.7.9rc2.tar", max compression
+gzip compressed data, was "folio_migration_tools-1.8.0rc1.tar", max compression
```

## Comparing `folio_migration_tools-1.7.9rc2.tar` & `folio_migration_tools-1.8.0rc1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1072 2022-10-12 06:39:38.400373 folio_migration_tools-1.7.9rc2/LICENSE
--rw-r--r--   0        0        0     4193 2023-03-23 11:06:44.580290 folio_migration_tools-1.7.9rc2/README.md
--rw-r--r--   0        0        0     1680 2023-03-27 18:42:03.467302 folio_migration_tools-1.7.9rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-12 06:39:38.400373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/__init__.py
--rw-r--r--   0        0        0     5474 2023-03-17 11:50:25.858615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/__main__.py
--rw-r--r--   0        0        0    14049 2023-03-17 11:50:25.858615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/circulation_helper.py
--rw-r--r--   0        0        0      227 2022-10-12 06:39:38.400373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/colors.py
--rw-r--r--   0        0        0      648 2022-10-12 06:39:38.400373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/custom_dict.py
--rw-r--r--   0        0        0     2374 2023-01-17 14:16:42.308522 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/custom_exceptions.py
--rw-r--r--   0        0        0     1678 2023-03-17 11:50:25.858615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/extradata_writer.py
--rw-r--r--   0        0        0     6573 2023-03-17 11:50:25.858615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/folder_structure.py
--rw-r--r--   0        0        0     2550 2022-12-15 12:43:40.310709 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/helper.py
--rw-r--r--   0        0        0     7089 2023-03-24 08:26:07.071170 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/holdings_helper.py
--rw-r--r--   0        0        0     2228 2023-03-17 11:50:25.858615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/library_configuration.py
--rw-r--r--   0        0        0    19528 2023-03-27 18:23:56.369019 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapper_base.py
--rw-r--r--   0        0        0        0 2022-10-12 06:39:38.400373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/__init__.py
--rw-r--r--   0        0        0     8051 2023-03-23 11:06:44.580290 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
--rw-r--r--   0        0        0     6359 2023-03-27 11:26:29.099374 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
--rw-r--r--   0        0        0    10035 2023-03-27 18:23:56.369019 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
--rw-r--r--   0        0        0    36223 2023-03-27 11:26:29.099374 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
--rw-r--r--   0        0        0     3548 2023-03-27 11:26:29.099374 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
--rw-r--r--   0        0        0    13946 2023-03-27 11:26:29.099374 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
--rw-r--r--   0        0        0    14579 2023-03-23 11:06:44.580290 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
--rw-r--r--   0        0        0     8795 2022-12-15 12:43:40.310709 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
--rw-r--r--   0        0        0     7726 2023-03-23 11:06:44.580290 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
--rw-r--r--   0        0        0        0 2022-10-12 06:39:38.400373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/__init__.py
--rw-r--r--   0        0        0    33946 2023-03-17 11:50:25.868615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/conditions.py
--rw-r--r--   0        0        0    11297 2022-12-15 12:43:40.310709 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
--rw-r--r--   0        0        0     9394 2023-03-17 11:50:25.868615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
--rw-r--r--   0        0        0   382912 2022-11-21 09:14:52.802243 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
--rw-r--r--   0        0        0    10671 2023-03-27 18:23:56.369019 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
--rw-r--r--   0        0        0     4962 2022-12-15 12:43:40.310709 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
--rw-r--r--   0        0        0     5850 2023-03-27 18:23:56.369019 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
--rw-r--r--   0        0        0    34436 2023-03-27 18:23:56.369019 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
--rw-r--r--   0        0        0    25855 2023-03-27 18:23:56.369019 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
--rw-r--r--   0        0        0    17305 2023-03-27 18:23:56.379021 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
--rw-r--r--   0        0        0     4084 2022-12-15 12:43:40.310709 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_report.py
--rw-r--r--   0        0        0      211 2022-10-12 06:39:38.410373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/__init__.py
--rw-r--r--   0        0        0     3154 2022-12-15 12:43:40.310709 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/authority_transformer.py
--rw-r--r--   0        0        0    26381 2023-03-23 11:06:44.580290 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/batch_poster.py
--rw-r--r--   0        0        0     4650 2023-03-27 18:23:56.379021 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/bibs_transformer.py
--rw-r--r--   0        0        0     5776 2022-12-15 12:43:40.310709 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/courses_migrator.py
--rw-r--r--   0        0        0    19271 2023-03-27 18:23:56.379021 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
--rw-r--r--   0        0        0     6351 2023-03-27 18:23:56.379021 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
--rw-r--r--   0        0        0    14813 2023-03-27 18:23:56.379021 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/items_transformer.py
--rw-r--r--   0        0        0    31931 2023-03-17 11:50:25.868615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/loans_migrator.py
--rw-r--r--   0        0        0    13244 2023-03-17 11:50:25.868615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/migration_task_base.py
--rw-r--r--   0        0        0    10831 2023-03-27 11:26:29.099374 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/orders_transformer.py
--rw-r--r--   0        0        0    14387 2023-03-17 11:50:25.878615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/organization_transformer.py
--rw-r--r--   0        0        0    12990 2023-03-17 11:50:25.878615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/requests_migrator.py
--rw-r--r--   0        0        0     8901 2023-03-17 11:50:25.878615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/reserves_migrator.py
--rw-r--r--   0        0        0     9305 2023-03-17 11:50:25.878615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/user_transformer.py
--rw-r--r--   0        0        0    15098 2023-03-17 11:50:25.878615 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/report_blurbs.py
--rw-r--r--   0        0        0      255 2022-11-22 17:40:18.176802 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/task_configuration.py
--rw-r--r--   0        0        0        0 2022-10-12 06:39:38.410373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/test_infrastructure/__init__.py
--rw-r--r--   0        0        0     5289 2023-03-23 11:06:44.580290 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/test_infrastructure/mocked_classes.py
--rw-r--r--   0        0        0        0 2022-10-12 06:39:38.410373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/__init__.py
--rw-r--r--   0        0        0     5405 2022-10-13 12:04:21.007075 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/legacy_loan.py
--rw-r--r--   0        0        0     6124 2022-11-21 09:14:52.812243 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/legacy_request.py
--rw-r--r--   0        0        0     1839 2022-10-12 06:39:38.410373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/legacy_reserve.py
--rw-r--r--   0        0        0      656 2022-10-12 06:39:38.410373 folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/transaction_result.py
--rw-r--r--   0        0        0     5622 1970-01-01 00:00:00.000000 folio_migration_tools-1.7.9rc2/setup.py
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 folio_migration_tools-1.7.9rc2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-06 22:17:01.793515 folio_migration_tools-1.8.0rc1/LICENSE
+-rw-r--r--   0        0        0     4193 2023-03-21 14:28:28.887645 folio_migration_tools-1.8.0rc1/README.md
+-rw-r--r--   0        0        0     1748 2023-04-21 03:05:13.906897 folio_migration_tools-1.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.810173 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/__init__.py
+-rw-r--r--   0        0        0     5322 2023-04-20 15:39:37.839264 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/__main__.py
+-rw-r--r--   0        0        0    13935 2023-04-19 02:22:09.368441 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/circulation_helper.py
+-rw-r--r--   0        0        0      227 2023-03-06 22:17:01.811146 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/colors.py
+-rw-r--r--   0        0        0      648 2023-03-06 22:17:01.811423 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/custom_dict.py
+-rw-r--r--   0        0        0     2374 2023-03-06 22:17:01.811751 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/custom_exceptions.py
+-rw-r--r--   0        0        0     1678 2023-03-06 22:17:01.812068 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/extradata_writer.py
+-rw-r--r--   0        0        0     6573 2023-03-06 22:17:01.812324 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/folder_structure.py
+-rw-r--r--   0        0        0     2550 2023-03-06 22:17:01.812602 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/helper.py
+-rw-r--r--   0        0        0     7089 2023-03-06 22:17:01.812878 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/holdings_helper.py
+-rw-r--r--   0        0        0     2636 2023-04-18 23:46:20.197850 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/library_configuration.py
+-rw-r--r--   0        0        0    19528 2023-03-27 22:22:56.113076 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapper_base.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.813766 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/__init__.py
+-rw-r--r--   0        0        0     8117 2023-04-19 02:19:29.600062 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py
+-rw-r--r--   0        0        0     6423 2023-04-19 02:19:29.616368 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py
+-rw-r--r--   0        0        0    10081 2023-04-19 02:19:29.618543 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/item_mapper.py
+-rw-r--r--   0        0        0    37072 2023-04-19 02:19:29.621237 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py
+-rw-r--r--   0        0        0     3548 2023-03-24 03:05:35.503768 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py
+-rw-r--r--   0        0        0    14848 2023-04-19 02:22:09.374729 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/order_mapper.py
+-rw-r--r--   0        0        0    14644 2023-04-19 02:22:09.385428 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py
+-rw-r--r--   0        0        0     8795 2023-03-06 22:17:01.816049 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py
+-rw-r--r--   0        0        0     7683 2023-04-19 02:19:29.634576 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/user_mapper.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.816647 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/__init__.py
+-rw-r--r--   0        0        0    34047 2023-04-18 23:46:20.215442 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/conditions.py
+-rw-r--r--   0        0        0    11297 2023-03-06 22:17:01.817193 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py
+-rw-r--r--   0        0        0     9386 2023-04-19 02:22:09.393982 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py
+-rw-r--r--   0        0        0   382912 2023-03-06 22:17:01.818293 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml
+-rw-r--r--   0        0        0    10697 2023-04-23 08:03:03.483979 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py
+-rw-r--r--   0        0        0     4962 2023-03-06 22:17:01.818809 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py
+-rw-r--r--   0        0        0     5850 2023-03-27 22:22:56.116126 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py
+-rw-r--r--   0        0        0    34454 2023-04-17 23:01:11.524015 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py
+-rw-r--r--   0        0        0    25845 2023-04-17 23:01:11.525499 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py
+-rw-r--r--   0        0        0    17417 2023-04-17 23:01:11.530990 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py
+-rw-r--r--   0        0        0     4084 2023-03-06 22:17:01.820137 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_report.py
+-rw-r--r--   0        0        0      211 2023-03-06 22:17:01.820491 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/__init__.py
+-rw-r--r--   0        0        0     4231 2023-04-17 23:01:11.544786 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/authority_transformer.py
+-rw-r--r--   0        0        0    28016 2023-04-21 02:52:45.466270 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/batch_poster.py
+-rw-r--r--   0        0        0     7360 2023-04-19 02:19:29.638089 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/bibs_transformer.py
+-rw-r--r--   0        0        0     5776 2023-03-06 22:17:01.821528 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/courses_migrator.py
+-rw-r--r--   0        0        0    19448 2023-04-17 23:01:11.555968 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py
+-rw-r--r--   0        0        0     9602 2023-04-19 02:19:29.644858 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py
+-rw-r--r--   0        0        0    14990 2023-04-17 23:01:11.562933 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/items_transformer.py
+-rw-r--r--   0        0        0    32162 2023-04-19 02:22:09.411635 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/loans_migrator.py
+-rw-r--r--   0        0        0    13244 2023-03-06 22:17:01.823074 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/migration_task_base.py
+-rw-r--r--   0        0        0    10831 2023-03-24 03:05:35.514754 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/orders_transformer.py
+-rw-r--r--   0        0        0    14387 2023-03-06 22:17:01.823616 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/organization_transformer.py
+-rw-r--r--   0        0        0    12990 2023-03-06 22:17:01.823855 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/requests_migrator.py
+-rw-r--r--   0        0        0     8868 2023-04-19 02:22:09.418100 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/reserves_migrator.py
+-rw-r--r--   0        0        0     9305 2023-03-06 22:17:01.824396 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/user_transformer.py
+-rw-r--r--   0        0        0    15521 2023-04-19 02:19:29.646947 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/report_blurbs.py
+-rw-r--r--   0        0        0      255 2023-03-06 22:17:01.824926 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/task_configuration.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.830348 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/test_infrastructure/__init__.py
+-rw-r--r--   0        0        0     5289 2023-03-24 03:05:35.516008 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/test_infrastructure/mocked_classes.py
+-rw-r--r--   0        0        0        0 2023-03-06 22:17:01.831318 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/__init__.py
+-rw-r--r--   0        0        0     5405 2023-03-06 22:17:01.831654 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/legacy_loan.py
+-rw-r--r--   0        0        0     6124 2023-03-06 22:17:01.831928 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/legacy_request.py
+-rw-r--r--   0        0        0     1839 2023-03-06 22:17:01.832344 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/legacy_reserve.py
+-rw-r--r--   0        0        0      656 2023-03-06 22:17:01.832638 folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/transaction_result.py
+-rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc1/setup.py
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 folio_migration_tools-1.8.0rc1/PKG-INFO
```

### Comparing `folio_migration_tools-1.7.9rc2/LICENSE` & `folio_migration_tools-1.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/README.md` & `folio_migration_tools-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/pyproject.toml` & `folio_migration_tools-1.8.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "folio_migration_tools"
-version = "1.7.9rc2"
+version = "1.8.0rc1"
 description =  "A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP"
 authors = ["Theodor Tolstoy <github.teddes@tolstoy.se>", "Lisa Sjögren", "Brooks Travis"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/FOLIO-FSE/folio_migration_tools"
 repository = "https://github.com/FOLIO-FSE/folio_migration_tools"
 keywords = ["FOLIO", "ILS", "LSP", "Library Systems", "MARC21", "Library data"]
@@ -29,25 +29,25 @@
 
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-folioclient = "^0.43.0"
+folioclient = "^0.50.0rc1"
 pyhumps = "^3.7.3"
 defusedxml = "^0.7.1"
 python-dateutil = "^2.8.2"
 folio-uuid = "^0.2.7"
 pymarc = "^4.2.1"
 pydantic = "^1.10.2"
 argparse-prompt = "^0.0.5"
 deepdiff = "^6.2.3"
-requests = "^2.28.2"
 pyaml = "^21.10.1"
+httpx = "^0.23.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 lxml = "^4.9.1"
 coverage = {extras = ["toml"], version = "^6.5.0"}
 pytest-cov = "^4.0.0"
 black = "^22.10.0"
@@ -59,10 +59,12 @@
 flake8-isort = "^5.0.0"
 flake8-docstrings = "^1.6.0"
 darglint = "^1.8.1"
 sphinx = "^5.3.0"
 sphinx-autodoc-typehints = "^1.19.4"
 myst-parser = "^0.18.1"
 pandas = "^1.5.3"
+types-requests = "^2.28.11.17"
+types-python-dateutil = "^2.8.19.11"
 
 [tool.poetry.extras]
 docs = ["m2r", "sphinx", "sphinx-autodoc-typehints", "sphinx-rtd-theme", "toml"]
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/__main__.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import sys
 
+import httpx
 import humps
-import requests.exceptions
 from argparse_prompt import PromptParser
 from pydantic import ValidationError
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.migration_tasks import *  # noqa: F403, F401
 from folio_migration_tools.migration_tasks import migration_task_base
@@ -98,17 +98,15 @@
                     )
                 print("Halting")
 
             # task_obj.do_work()
             logging.info("Work done. Shutting down")
             sys.exit(0)
             # task_obj.wrap_up()
-    except requests.exceptions.SSLError:
-        print("\nSSL error. Are you connected to the Internet and the VPN?")
-    except requests.exceptions.ConnectionError as connection_error:
+    except httpx.HTTPError as connection_error:
         print(
             f"\nConnection Error when connecting to {connection_error.request.url}. "
             "Are you connectet to the Internet/VPN? Do you need to update DNS settings?"
         )
         sys.exit(1)
     except FileNotFoundError as fnf_error:
         print(f"\n{fnf_error.strerror}: {fnf_error.filename}")
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/circulation_helper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/circulation_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import copy
 import json
 import logging
 import re
 import time
 from typing import Set
 
-import requests
+import httpx
 from folioclient import FolioClient
-from requests import HTTPError
+from httpx import HTTPError
 
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.migration_report import MigrationReport
 from folio_migration_tools.report_blurbs import Blurbs
 from folio_migration_tools.transaction_migration.legacy_loan import LegacyLoan
 from folio_migration_tools.transaction_migration.legacy_request import LegacyRequest
 from folio_migration_tools.transaction_migration.transaction_result import (
@@ -137,17 +137,15 @@
             if legacy_loan.patron_barcode in self.missing_patron_barcodes:
                 error_message = "Patron barcode already detected as missing"
                 logging.error(
                     f"{error_message} Patron barcode: {legacy_loan.patron_barcode} "
                     f"Item Barcode:{legacy_loan.item_barcode}"
                 )
                 return TransactionResult(False, False, "", error_message, error_message)
-            req = requests.post(
-                url, headers=self.folio_client.okapi_headers, data=json.dumps(data)
-            )
+            req = httpx.post(url, headers=self.folio_client.okapi_headers, json=data)
             if req.status_code == 422:
                 error_message_from_folio = json.loads(req.text)["errors"][0]["message"]
                 stat_message = error_message_from_folio
                 error_message = error_message_from_folio
                 if "has the item status" in error_message_from_folio:
                     stat_message = re.findall(
                         r"(?<=has the item status\s).*(?=\sand cannot be checked out)",
@@ -240,28 +238,28 @@
             )
 
     @staticmethod
     def create_request(
         folio_client: FolioClient, legacy_request: LegacyRequest, migration_report: MigrationReport
     ):
         try:
-            path = "/circulation/requests"
+            path = "/circulation/httpx"
             url = f"{folio_client.okapi_url}{path}"
             data = legacy_request.serialize()
             data["requestProcessingParameters"] = {
                 "overrideBlocks": {
                     "itemNotLoanableBlock": {
                         "dueDate": legacy_request.request_expiration_date.isoformat()
                     },
                     "patronBlock": {},
                     "itemLimitBlock": {},
                     "comment": "Migrated from legacy system",
                 }
             }
-            req = requests.post(url, headers=folio_client.okapi_headers, data=json.dumps(data))
+            req = httpx.post(url, headers=folio_client.okapi_headers, json=data)
             logging.debug(f"POST {req.status_code}\t{url}\t{json.dumps(data)}")
             if str(req.status_code) == "422":
                 message = json.loads(req.text)["errors"][0]["message"]
                 logging.error(f"{message}")
                 migration_report.add_general_statistics(message)
                 return False
             else:
@@ -307,17 +305,15 @@
         try:
             loan_to_put = copy.deepcopy(loan)
             del loan_to_put["metadata"]
             loan_to_put["dueDate"] = extension_due_date.isoformat()
             loan_to_put["loanDate"] = extend_out_date.isoformat()
             url = f"{folio_client.okapi_url}/circulation/loans/{loan_to_put['id']}"
 
-            req = requests.put(
-                url, headers=folio_client.okapi_headers, data=json.dumps(loan_to_put)
-            )
+            req = httpx.put(url, headers=folio_client.okapi_headers, json=loan_to_put)
             logging.info(
                 "%s\tPUT Extend loan %s to %s\t %s",
                 req.status_code,
                 loan_to_put["id"],
                 loan_to_put["dueDate"],
                 url,
             )
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/custom_dict.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/custom_dict.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/custom_exceptions.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/extradata_writer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/extradata_writer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/folder_structure.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/folder_structure.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/helper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/holdings_helper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/holdings_helper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapper_base.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapper_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/courses_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         if user := self.user_cache.get(instructor["userId"], {}):
             instructor["userId"] = user.get("id", "")
             instructor["barcode"] = user.get("barcode", "")
             instructor["patronGroup"] = user.get("patronGroup", "")
         else:
             del instructor["userId"]
 
-    def get_prop(self, legacy_item, folio_prop_name, index_or_id):
+    def get_prop(self, legacy_item, folio_prop_name, index_or_id, schema_default_value):
         if folio_prop_name == "courselisting.termId":
             return self.get_mapped_ref_data_value(
                 self.terms_map,
                 legacy_item,
                 folio_prop_name,
                 index_or_id,
                 False,
@@ -153,15 +153,17 @@
             return self.get_mapped_ref_data_value(
                 self.departments_map,
                 legacy_item,
                 folio_prop_name,
                 index_or_id,
                 False,
             )
-        elif mapped_value := super().get_prop(legacy_item, folio_prop_name, index_or_id):
+        elif mapped_value := super().get_prop(
+            legacy_item, folio_prop_name, index_or_id, schema_default_value
+        ):
             return mapped_value
         else:
             self.migration_report.add(Blurbs.UnmappedProperties, f"{folio_prop_name}")
             return ""
 
     def get_composite_course_schema(self) -> Dict[str, Any]:
         if self:
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/holdings_mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,25 +51,27 @@
                 "/call-number-types",
                 "callNumberTypes",
                 call_number_type_map,
                 "name",
                 Blurbs.CallNumberTypeMapping,
             )
 
-    def get_prop(self, legacy_item, folio_prop_name, index_or_id):
-        mapped_value = super().get_prop(legacy_item, folio_prop_name, index_or_id)
-
+    def get_prop(self, legacy_item, folio_prop_name, index_or_id, schema_default_value):
         if folio_prop_name == "permanentLocationId":
             return self.get_location_id(legacy_item, index_or_id, folio_prop_name)
-        elif folio_prop_name == "callNumber":
-            return self.get_call_number(mapped_value)
         elif folio_prop_name == "callNumberTypeId":
             return self.get_call_number_type_id(legacy_item, folio_prop_name, index_or_id)
         elif folio_prop_name.startswith("statisticalCodeIds"):
             return self.get_statistical_code(legacy_item, folio_prop_name, index_or_id)
+
+        mapped_value = super().get_prop(
+            legacy_item, folio_prop_name, index_or_id, schema_default_value
+        )
+        if folio_prop_name == "callNumber":
+            return self.get_call_number(mapped_value)
         elif folio_prop_name == "instanceId":
             return self.get_instance_ids(mapped_value, index_or_id)
         elif mapped_value:
             return mapped_value
         else:
             self.migration_report.add(Blurbs.UnmappedProperties, f"{folio_prop_name}")
             return ""
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/item_mapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/item_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,25 +58,24 @@
                 self.folio_client,
                 "/loan-types",
                 "loantypes",
                 temporary_loan_type_mapping,
                 "name",
                 Blurbs.TemporaryLoanTypeMapping,
             )
+        self.temp_location_mapping = None
         if temporary_location_mapping:
             self.temp_location_mapping = RefDataMapping(
                 self.folio_client,
                 "/locations",
                 "locations",
                 temporary_location_mapping,
                 "code",
                 Blurbs.TemporaryLocationMapping,
             )
-        else:
-            self.temp_location_mapping = None
 
         if item_statuses_map:
             self.setup_status_mapping(item_statuses_map)
         if call_number_type_map:
             self.call_number_mapping = RefDataMapping(
                 self.folio_client,
                 "/call-number-types",
@@ -144,16 +143,15 @@
                 sys.exit(1)
             else:
                 self.status_mapping = {
                     v["legacy_code"]: v["folio_name"] for v in item_statuses_map
                 }
         logging.info(json.dumps(statuses, indent=True))
 
-    def get_prop(self, legacy_item, folio_prop_name, index_or_id):
-        mapped_value = super().get_prop(legacy_item, folio_prop_name, index_or_id)
+    def get_prop(self, legacy_item, folio_prop_name, index_or_id, schema_default_value):
 
         if folio_prop_name == "permanentLocationId":
             return self.get_mapped_ref_data_value(
                 self.location_mapping,
                 legacy_item,
                 folio_prop_name,
                 index_or_id,
@@ -181,27 +179,14 @@
                 folio_prop_name,
                 index_or_id,
             )
         elif folio_prop_name == "itemLevelCallNumberTypeId":
             return self.get_item_level_call_number_type_id(
                 legacy_item, folio_prop_name, index_or_id
             )
-        elif folio_prop_name == "status.name":
-            return self.transform_status(mapped_value)
-        elif folio_prop_name == "barcode":
-            barcode = mapped_value
-            if barcode.strip() and barcode in self.unique_barcodes:
-                Helper.log_data_issue(index_or_id, "Duplicate barcode", mapped_value)
-                self.migration_report.add_general_statistics("Duplicate barcodes")
-                return f"{barcode}-{uuid4()}"
-            else:
-                if barcode.strip():
-                    self.unique_barcodes.add(barcode)
-                return barcode
-
         elif folio_prop_name == "status.date":
             return datetime.now(timezone.utc).isoformat()
         elif folio_prop_name == "temporaryLoanTypeId":
             ltid = self.get_mapped_ref_data_value(
                 self.temp_loan_type_mapping,
                 legacy_item,
                 folio_prop_name,
@@ -221,14 +206,30 @@
                 legacy_item, folio_prop_name, index_or_id
             )
             self.migration_report.add(
                 Blurbs.StatisticalCodeMapping,
                 f"{folio_prop_name} -> {statistical_code_id}",
             )
             return statistical_code_id
+
+        mapped_value = super().get_prop(
+            legacy_item, folio_prop_name, index_or_id, schema_default_value
+        )
+        if folio_prop_name == "status.name":
+            return self.transform_status(mapped_value)
+        elif folio_prop_name == "barcode":
+            barcode = mapped_value
+            if barcode.strip() and barcode in self.unique_barcodes:
+                Helper.log_data_issue(index_or_id, "Duplicate barcode", mapped_value)
+                self.migration_report.add_general_statistics("Duplicate barcodes")
+                return f"{barcode}-{uuid4()}"
+            else:
+                if barcode.strip():
+                    self.unique_barcodes.add(barcode)
+                return barcode
         elif folio_prop_name == "holdingsRecordId":
             if mapped_value in self.holdings_id_map:
                 return self.holdings_id_map[mapped_value][1]
             elif f"{self.bib_id_template}{mapped_value}" in self.holdings_id_map:
                 return self.holdings_id_map[f"{self.bib_id_template}{mapped_value}"][1]
             self.migration_report.add_general_statistics(
                 "Records failed because of failed holdings",
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/mapping_file_mapper_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
         return [
             k["folio_field"]
             for k in the_map["data"]
             if (
                 k["legacy_field"] not in empty_vals
                 # and k["folio_field"] != "legacyIdentifier"
                 or k.get("value", "") not in empty_vals
+                or isinstance(k.get("value", ""), bool)
             )
         ]
 
     @staticmethod
     def get_mapped_legacy_properties_from_map(the_map):
         return [
             k["legacy_field"].strip()
@@ -235,15 +236,15 @@
             )
         self.migration_report.add(
             Blurbs.StatisticalCodeMapping,
             "Mapping not setup",
         )
         return ""
 
-    def get_prop(self, legacy_object, folio_prop_name, index_or_id):
+    def get_prop(self, legacy_object, folio_prop_name, index_or_id, schema_default_value):
         legacy_item_keys = self.mapped_from_legacy_data.get(folio_prop_name, [])
         map_entries = list(
             MappingFileMapperBase.get_map_entries_by_folio_prop_name(
                 folio_prop_name, self.record_map["data"]
             )
         )
         if not any(map_entries):
@@ -253,17 +254,25 @@
             return " ".join(
                 MappingFileMapperBase.get_legacy_value(
                     legacy_object, map_entry, self.migration_report, index_or_id
                 )
                 for map_entry in map_entries
             ).strip()
         else:
-            return MappingFileMapperBase.get_legacy_value(
+            legacy_value = MappingFileMapperBase.get_legacy_value(
                 legacy_object, map_entries[0], self.migration_report, index_or_id
             )
+            if legacy_value or isinstance(legacy_value, bool):
+                return legacy_value
+            else:
+                self.migration_report.add(
+                    Blurbs.FolioDefaultValuesAdded,
+                    f"{schema_default_value} added to {folio_prop_name}",
+                )
+                return schema_default_value
 
     def do_map(
         self,
         legacy_object,
         index_or_id: str,
         object_type: FOLIONamespaces,
         accept_duplicate_ids=False,
@@ -303,15 +312,19 @@
                         legacy_object,
                         schema_property_name,
                         schema_property["items"]["properties"],
                         folio_object,
                         index_or_id,
                         schema_property["items"].get("required", []),
                     )
-                elif schema_property["items"].get("type", "") == "string":
+                    self.validate_object_items_in_array(
+                        folio_object, schema_property_name, schema_property
+                    )
+
+                elif schema_property["items"].get("type", "") in ["string", "number", "integer"]:
                     self.map_string_array_props(
                         legacy_object,
                         schema_property_name,
                         folio_object,
                         index_or_id,
                     )
                 else:
@@ -345,14 +358,15 @@
                 Blurbs.DefaultValuesAdded,
                 f"{value_mapped_value} added to {mapping_file_entry.get('folio_field', '')}",
             )
             return value_mapped_value
 
         # Value mapped from the Legacy field(s)
         value = legacy_object.get(mapping_file_entry["legacy_field"], "")
+
         if value and mapping_file_entry.get("rules", {}).get("replaceValues", {}):
             if replaced_val := mapping_file_entry["rules"]["replaceValues"].get(value, ""):
                 migration_report.add(
                     Blurbs.FieldMappingDetails,
                     (
                         f"Replaced {value} in {mapping_file_entry['legacy_field']} "
                         f"with {replaced_val}"
@@ -425,30 +439,39 @@
                     legacy_object,
                     f"{schema_property_name}.{child_property_name}",
                     child_property["items"]["properties"],
                     folio_object,
                     index_or_id,
                     [],
                 )
-            elif (
-                child_property.get("type", "") == "array"
-                and child_property.get("items", {}).get("type", "") == "string"
-            ):
+                self.validate_object_items_in_array(
+                    legacy_object,
+                    child_property_name,
+                    child_property["items"]["properties"],
+                )
+
+            elif child_property.get("type", "") == "array" and child_property.get("items", {}).get(
+                "type", ""
+            ) in ["string", "number", "integer"]:
                 self.map_string_array_props(
                     legacy_object,
                     f"{schema_property_name}.{child_property_name}",
                     folio_object,
                     index_or_id,
                 )
-            elif child_property.get("type", "") == "string":
+            elif child_property.get("type", "") in ["string", "number", "integer"]:
                 path = sub_prop_path.split("].")[-1]
-                if p := self.get_prop(legacy_object, sub_prop_path, index_or_id):
+                if p := self.get_prop(
+                    legacy_object, sub_prop_path, index_or_id, child_property.get("default", "")
+                ):
                     set_deep(folio_object, f"{path}", p)
                 # temp_object[child_property_name] = p
-            elif p := self.get_prop(legacy_object, sub_prop_path, index_or_id):
+            elif p := self.get_prop(
+                legacy_object, sub_prop_path, index_or_id, child_property.get("default", "")
+            ):
                 set_deep(folio_object, sub_prop_path, p)
         if temp_object:
             set_deep(folio_object, schema_property_name, temp_object)
             # folio_object[schema_property_name] = temp_object
 
     def map_objects_array_props(
         self,
@@ -474,15 +497,20 @@
                     (k, p)
                     for k, p in sub_properties.items()
                     if not p.get("folio:isVirtual", False)
                 ):
                     prop_path = f"{prop_name}[{i}].{sub_prop_name}"
                     if prop_path in self.folio_keys:
                         # We have reached the end of the prop path?
-                        res = self.get_prop(legacy_object, prop_path, index_or_id)
+                        res = self.get_prop(
+                            legacy_object,
+                            prop_path,
+                            index_or_id,
+                            sub_properties[sub_prop_name].get("default", ""),
+                        )
                         self.report_legacy_mapping(
                             self.legacy_basic_property(prop_path), True, True
                         )
 
                         if (
                             isinstance(res, str)
                             and self.library_configuration.multi_field_delimiter in res
@@ -505,19 +533,25 @@
                             folio_object,
                             index_or_id,
                             [],
                         )
                     elif (
                         sub_prop_name in sub_properties
                         and sub_properties[sub_prop_name].get("type", "") == "array"
-                        and sub_properties[sub_prop_name]["items"].get("type", "") == "string"
+                        and sub_properties[sub_prop_name]["items"].get("type", "")
+                        in ["string", "number", "integer"]
                     ):
                         # We have not reached the end of the prop path
                         for array_path in [p for p in self.folio_keys if p.startswith(prop_path)]:
-                            res = self.get_prop(legacy_object, array_path, index_or_id)
+                            res = self.get_prop(
+                                legacy_object,
+                                array_path,
+                                index_or_id,
+                                sub_properties[sub_prop_name].get("default", ""),
+                            )
                             self.validate_enums(
                                 res, sub_prop, sub_prop_name, index_or_id, required
                             )
                             if res or isinstance(res, bool):
                                 self.add_values_to_string_array(
                                     sub_prop_name,
                                     temp_object,
@@ -527,45 +561,24 @@
 
                     elif sub_prop.get("type", "") == "object" and "properties" in sub_prop:
                         self.map_object_props(
                             legacy_object, prop_path, sub_prop, temp_object, index_or_id, 0
                         )
             i = i + 1
 
-            if temp_object != {} and all(
-                temp_object.get(r) or (isinstance(temp_object.get(r), bool)) for r in required
-            ):
-                if any(multi_field_props):
-                    resulting_array.extend(
-                        self.split_obj_by_delim(
-                            self.library_configuration.multi_field_delimiter,
-                            temp_object,
-                            multi_field_props,
-                        )
+            if any(multi_field_props):
+                resulting_array.extend(
+                    self.split_obj_by_delim(
+                        self.library_configuration.multi_field_delimiter,
+                        temp_object,
+                        multi_field_props,
                     )
-                else:
-                    resulting_array.append(temp_object)
-
-            elif any(
-                (
-                    v
-                    for k, v in temp_object.items()
-                    if not self.is_uuid(v) and not isinstance(v, bool)
-                )
-            ):
-                self.migration_report.add(
-                    Blurbs.IncompleteSubPropertyRemoved,
-                    f"{prop_name}",
                 )
-                # Helper.log_data_issue(
-                #     f"{prop_name}",
-                #     f"Sub-property {sub_prop} removed as it is missing required fields:"
-                #     f"{required}",
-                #     temp_object,
-                # )
+            else:
+                resulting_array.append(temp_object)
 
         if any(resulting_array):
             set_deep2(folio_object, prop_name, resulting_array)
 
     @staticmethod
     def split_obj_by_delim(delimiter: str, folio_obj: dict, delimited_props: List[str]):
         non_split_props = [(k, v) for k, v in folio_obj.items() if k not in delimited_props]
@@ -583,15 +596,15 @@
             r.update(non_split_props)
         return res
 
     def map_string_array_props(self, legacy_object, prop, folio_object, index_or_id):
         keys_to_map = [k for k in self.folio_keys if k.startswith(prop)]
         for prop_name in keys_to_map:
             if prop_name in self.folio_keys and self.has_property(legacy_object, prop_name):
-                if mapped_prop := self.get_prop(legacy_object, prop_name, index_or_id):
+                if mapped_prop := self.get_prop(legacy_object, prop_name, index_or_id, ""):
                     self.add_values_to_string_array(
                         prop,
                         folio_object,
                         mapped_prop,
                         self.library_configuration.multi_field_delimiter,
                     )
                 self.report_legacy_mapping(self.legacy_basic_property(prop_name), True, True)
@@ -615,30 +628,27 @@
             # No values in array previously
             set_deep(folio_object, prop, [mapped_prop_value])
 
     def map_basic_props(
         self, legacy_object, property_name, folio_object, index_or_id, schema_property
     ):
         if self.has_basic_property(legacy_object, property_name):  # is there a match in the csv?
-            if mapped_prop := self.get_prop(legacy_object, property_name, index_or_id):
+            mapped_prop = self.get_prop(
+                legacy_object, property_name, index_or_id, schema_property.get("default", "")
+            )
+            if mapped_prop or isinstance(mapped_prop, bool):
                 self.validate_enums(
                     mapped_prop,
                     schema_property,
                     property_name,
                     index_or_id,
                     self.schema.get("required", []),
                 )
                 folio_object[property_name] = mapped_prop
             self.report_legacy_mapping(self.legacy_basic_property(property_name), True, True)
-        elif "default" in schema_property:
-            folio_object[property_name] = schema_property["default"]
-            self.migration_report.add(
-                Blurbs.DefaultValuesAdded,
-                f"From Schema: {property_name} -> {schema_property['default']}",
-            )
 
     @staticmethod
     def _get_delimited_file_reader(source_file, file_name: Path):
         """
             First, let's count:
             * The total number of rows in the source file
             * The total number of empty rows in the source file
@@ -695,25 +705,17 @@
 
     def has_basic_property(self, legacy_object, folio_prop_name):
         if folio_prop_name not in self.folio_keys:
             return False
         if folio_prop_name in self.mapped_from_values:
             return True
         legacy_mappings = self.legacy_record_mappings.get(folio_prop_name, [])
-        return (
-            any(legacy_mappings)
-            and any(legacy_mapping not in empty_vals for legacy_mapping in legacy_mappings)
-            and any(
-                legacy_object.get(legacy_mapping["legacy_field"], "")
-                or (
-                    "fallback_legacy_field" in legacy_mapping
-                    and legacy_object.get(legacy_mapping["fallback_legacy_field"], "")
-                )
-                for legacy_mapping in legacy_mappings
-            )
+
+        return any(legacy_mappings) and any(
+            legacy_mapping not in empty_vals for legacy_mapping in legacy_mappings
         )
 
     @staticmethod
     def get_map_entries_by_folio_prop_name(folio_prop_name, data):
         return (
             k
             for k in data
@@ -810,14 +812,32 @@
         """
         try:
             uuid.UUID(str(value))
         except ValueError:
             return False
         return True
 
+    def validate_object_items_in_array(self, folio_object, schema_property_name, schema_property):
+        valid_array_objects = []
+        for item in folio_object.get(schema_property_name, []):
+            if all(
+                item.get(r) or (isinstance(item.get(r), bool))
+                for r in schema_property["items"].get("required", [])
+            ):
+                valid_array_objects.append(item)
+            else:
+                self.migration_report.add(
+                    Blurbs.IncompleteSubPropertyRemoved,
+                    f"{schema_property_name}",
+                )
+        if valid_array_objects:
+            folio_object[schema_property_name] = valid_array_objects
+        else:
+            folio_object.pop(schema_property_name, [])
+
 
 def skip_property(property_name, property):
     return bool(
         property_name in ["metadata", "id", "type", "lastCheckIn"]
         or property_name.startswith("effective")
         or property.get("folio:isVirtual", False)
         or property.get("description", "") == "Deprecated"
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/notes_mapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/order_mapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/order_mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import os
 import re
 import sys
 import urllib.parse
 import uuid
 
-import requests
+import httpx
 from folio_uuid.folio_uuid import FOLIONamespaces
 from folioclient import FolioClient
-from requests.exceptions import HTTPError
+from httpx import HTTPError
 
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
     MappingFileMapperBase,
 )
 from folio_migration_tools.mapping_file_transformation.notes_mapper import NotesMapper
@@ -58,49 +58,69 @@
             "/orders/acquisition-methods",
             "acquisitionMethods",
             acquisition_method_map,
             "value",
             Blurbs.AcquisitionMethodMapping,
         )
         logging.info("Init done")
+        self.location_mapping = RefDataMapping(
+            self.folio_client,
+            "/locations",
+            "locations",
+            location_map,
+            "code",
+            Blurbs.OrderLineLocationMapping,
+        )
 
         self.folio_client: FolioClient = folio_client
         self.notes_mapper: NotesMapper = NotesMapper(
             library_configuration,
             self.folio_client,
             composite_order_map,
             FOLIONamespaces.note,
             True,
         )
         self.notes_mapper.migration_report = self.migration_report
 
-    def get_prop(self, legacy_order, folio_prop_name: str, index_or_id):
-        mapped_value = super().get_prop(legacy_order, folio_prop_name, index_or_id)
+    def get_prop(self, legacy_order, folio_prop_name: str, index_or_id, schema_default_value):
         if folio_prop_name.endswith(".acquisitionMethod"):
             mapped_val = self.acquisitions_methods_mapping.get_ref_data_mapping(legacy_order)
             return mapped_val["folio_id"]
 
-        elif folio_prop_name == "vendor":
+        elif re.compile(r"compositePoLines\[(\d+)\]\.id").fullmatch(folio_prop_name):
+            return str(uuid.uuid4())
+
+        elif re.compile(r"notes\[\d+\]\.").match(folio_prop_name):
+            return ""
+
+        mapped_value = super().get_prop(
+            legacy_order, folio_prop_name, index_or_id, schema_default_value
+        )
+
+        if folio_prop_name.endswith(".locationId"):
+            return self.get_mapped_ref_data_value(
+                self.location_mapping,
+                legacy_order,
+                folio_prop_name,
+                index_or_id,
+                True,
+            )
+
+        if folio_prop_name == "vendor":
             if mapped_value in self.vendor_code_map:
                 self.migration_report.add_general_statistics(
                     "Successfully matched Vendor against code"
                 )
                 return self.vendor_code_map[mapped_value]
             else:
                 self.migration_report.add_general_statistics("Orders without assigned vendor")
                 Helper.log_data_issue(
                     index_or_id, "Vendor code not found among migrated Organizations", mapped_value
                 )
 
-        elif re.compile("compositePoLines\[(\d+)\]\.id").fullmatch(folio_prop_name):
-            return str(uuid.uuid4())
-
-        elif re.compile(r"notes\[\d+\]\.").match(folio_prop_name):
-            return ""
-
         elif folio_prop_name.endswith(".instanceId"):
             if mapped_value in self.instance_id_map:
                 self.migration_report.add_general_statistics(
                     "Instance ID mapped from previously migrated bib records"
                 )
                 return self.instance_id_map.get(mapped_value)[1]
             else:
@@ -162,23 +182,28 @@
             # raml_utils_sha = next((item["sha"] for item in submodules
             # if item["path"] == "raml-utils"))
 
             acq_models_path = (
                 f"{github_path}/{owner}/acq-models/{acq_models_sha}/{module}/schemas/"
             )
 
-            req = requests.get(f"{acq_models_path}/{object}.json", headers=github_headers)
+            req = httpx.get(
+                f"{acq_models_path}/{object}.json",
+                headers=github_headers,
+                follow_redirects=True,
+                timeout=None,
+            )
             req.raise_for_status()
 
             object_schema = json.loads(req.text)
 
             return CompositeOrderMapper.build_extended_object(
                 object_schema, acq_models_path, github_headers
             )
-        except requests.exceptions.HTTPError as http_error:
+        except httpx.HTTPError as http_error:
             logging.critical(f"Halting! \t{http_error}")
             sys.exit(2)
 
         except json.decoder.JSONDecodeError as json_error:
             logging.critical(json_error)
             sys.exit(2)
 
@@ -200,34 +225,36 @@
 
         """
 
         github_path = "https://api.github.com/repos"
 
         # Get metadata for the latest release
         latest_release_path = f"{github_path}/{owner}/{repo}/releases/latest"
-        req = requests.get(f"{latest_release_path}", headers=github_headers)
+        req = httpx.get(
+            f"{latest_release_path}", headers=github_headers, follow_redirects=True, timeout=None
+        )
         req.raise_for_status()
         latest_release = json.loads(req.text)
 
         # Get the tag assigned to the latest release
         release_tag = latest_release["tag_name"]
         logging.info(f"Using schemas from latest {repo} release: {release_tag}")
 
         # Get the tree for the latest release
         tree_path = f"{github_path}/{owner}/{repo}/git/trees/{release_tag}"
-        req = requests.get(tree_path, headers=github_headers)
+        req = httpx.get(tree_path, headers=github_headers, follow_redirects=True, timeout=None)
         req.raise_for_status()
         release_tree = json.loads(req.text)
 
         # Loop through the tree to get the sha of the folder with path "ramls"
         ramls_sha = next((item["sha"] for item in release_tree["tree"] if item["path"] == "ramls"))
 
         # Get the tree for the ramls folder
         ramls_path = f"{github_path}/{owner}/{repo}/git/trees/{ramls_sha}"
-        req = requests.get(ramls_path, headers=github_headers)
+        req = httpx.get(ramls_path, headers=github_headers, follow_redirects=True, timeout=None)
         req.raise_for_status()
         ramls_tree = json.loads(req.text)
 
         # Loop through the tree to get the sha of submodules
         submodules = [item for item in ramls_tree["tree"] if item["mode"] == "160000"]
 
         return submodules
@@ -332,25 +359,29 @@
             u1 = urllib.parse.urlparse(submodule_path)
             schema_url = urllib.parse.urljoin(u1.geturl(), property["$ref"])
             if schema_url.endswith("tags.schema"):
                 schema_url = f"{base_raml}schemas/tags.schema"
             if schema_url.endswith("metadata.schema"):
                 schema_url = f"{base_raml}schemas/metadata.schema"
 
-            req = requests.get(schema_url, headers=github_headers)
+            req = httpx.get(
+                schema_url, headers=github_headers, follow_redirects=True, timeout=None
+            )
             req.raise_for_status()
             return dict(property, **json.loads(req.text))
         except Exception as ee:
             logging.error(ee)
             return {}
 
     @staticmethod
     def inject_items_schema_by_ref(submodule_path, github_headers, property: dict):
         try:
             u1 = urllib.parse.urlparse(submodule_path)
             schema_url = urllib.parse.urljoin(u1.geturl(), property["items"]["$ref"])
-            req = requests.get(schema_url, headers=github_headers)
+            req = httpx.get(
+                schema_url, headers=github_headers, follow_redirects=True, timeout=None
+            )
             req.raise_for_status()
             return dict(property["items"], **json.loads(req.text))
         except Exception as ee:
             logging.error(ee)
             return {}
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/organization_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import logging
 import os
 import re
 import sys
 
-import requests
+import httpx
 from folio_uuid.folio_uuid import FOLIONamespaces
 from folioclient import FolioClient
-from requests.exceptions import HTTPError
 
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.mapping_file_transformation.mapping_file_mapper_base import (
     MappingFileMapperBase,
 )
 from folio_migration_tools.mapping_file_transformation.notes_mapper import NotesMapper
 from folio_migration_tools.mapping_file_transformation.ref_data_mapping import (
@@ -62,15 +61,15 @@
             organization_map,
             FOLIONamespaces.note,
             True,
         )
         self.notes_mapper.migration_report = self.migration_report
 
     # Commence the mapping work
-    def get_prop(self, legacy_organization, folio_prop_name, index_or_id):
+    def get_prop(self, legacy_organization, folio_prop_name, index_or_id, schema_default_value):
         value_tuple = (
             legacy_organization,
             index_or_id,
             folio_prop_name,
         )
 
         # Perfrom reference data mappings
@@ -103,15 +102,17 @@
             )
 
         elif re.compile("interfaces\[(\d+)\]\.interfaceCredential.interfaceId").fullmatch(
             folio_prop_name
         ):
             return "replace_with_interface_id"
 
-        return super().get_prop(legacy_organization, folio_prop_name, index_or_id)
+        return super().get_prop(
+            legacy_organization, folio_prop_name, index_or_id, schema_default_value
+        )
 
     def set_up_reference_data_mapping(
         self,
         organization_types_map,
         address_categories_map,
         email_categories_map,
         phone_categories_map,
@@ -203,27 +204,27 @@
 
             # # TODO Maybe - fetch raml_utils schemas if deemed necessary
             # raml_utils_sha = next((item["sha"] for item in submodules
             # if item["path"] == "raml-utils"))
 
             acq_models_path = f"{github_path}/{owner}/acq-models/{acq_models_sha}/{module}/schemas"
 
-            req = requests.get(f"{acq_models_path}/{object}.json", headers=github_headers)
+            req = httpx.get(f"{acq_models_path}/{object}.json", headers=github_headers)
             req.raise_for_status()
 
             object_schema = json.loads(req.text)
 
             # Fetch referenced schemas
             extended_object_schema = OrganizationMapper.build_extended_object(
                 object_schema, acq_models_path, github_headers
             )
 
             return extended_object_schema
 
-        except requests.exceptions.HTTPError as http_error:
+        except httpx.HTTPError as http_error:
             logging.critical(f"Halting! \t{http_error}")
             sys.exit(2)
 
         except json.decoder.JSONDecodeError as json_error:
             logging.critical(json_error)
             sys.exit(2)
 
@@ -243,34 +244,34 @@
             _type_: _description_
         """
 
         github_path = "https://api.github.com/repos"
 
         # Get metadata for the latest release
         latest_release_path = f"{github_path}/{owner}/{repo}/releases/latest"
-        req = requests.get(f"{latest_release_path}", headers=github_headers)
+        req = httpx.get(f"{latest_release_path}", headers=github_headers, timeout=None)
         req.raise_for_status()
         latest_release = json.loads(req.text)
 
         # Get the tag assigned to the latest release
         release_tag = latest_release["tag_name"]
         logging.info(f"Using schemas from latest {repo} release: {release_tag}")
 
         # Get the tree for the latest release
         tree_path = f"{github_path}/{owner}/{repo}/git/trees/{release_tag}"
-        req = requests.get(tree_path, headers=github_headers)
+        req = httpx.get(tree_path, headers=github_headers, timeout=None)
         req.raise_for_status()
         release_tree = json.loads(req.text)
 
         # Loop through the tree to get the sha of the folder with path "ramls"
         ramls_sha = next((item["sha"] for item in release_tree["tree"] if item["path"] == "ramls"))
 
         # Get the tree for the ramls folder
         ramls_path = f"{github_path}/{owner}/{repo}/git/trees/{ramls_sha}"
-        req = requests.get(ramls_path, headers=github_headers)
+        req = httpx.get(ramls_path, headers=github_headers, timeout=None)
         req.raise_for_status()
         ramls_tree = json.loads(req.text)
 
         # Loop through the tree to get the sha of submodules
         submodules = [item for item in ramls_tree["tree"] if item["mode"] == "160000"]
 
         return submodules
@@ -351,35 +352,35 @@
                 # Handle object properties
                 elif property_level1.get("type") == "object" and property_level1.get("$ref"):
                     logging.info("Fecthing referenced schema for object %s", property_name_level1)
 
                     ref_object = property_level1["$ref"]
                     schema_url = f"{submodule_path}/{ref_object}"
 
-                    req = requests.get(schema_url, headers=github_headers)
+                    req = httpx.get(schema_url, headers=github_headers, timeout=None)
                     req.raise_for_status()
 
                     property_level1 = dict(property_level1, **json.loads(req.text))
 
                 elif property_level1.get("type") == "array" and property_level1.get("items").get(
                     "$ref"
                 ):
                     ref_object = property_level1["items"]["$ref"]
                     schema_url = f"{submodule_path}/{ref_object}"
 
-                    req = requests.get(schema_url, headers=github_headers)
+                    req = httpx.get(schema_url, headers=github_headers, timeout=None)
                     req.raise_for_status()
 
                     property_level1["items"] = dict(
                         property_level1["items"], **json.loads(req.text)
                     )
 
             return object_schema
 
-        except HTTPError as he:
+        except httpx.HTTPError as he:
             logging.error(he)
 
     @staticmethod
     def fetch_additional_schema(folio_object):
         additional_schema = OrganizationMapper.get_latest_acq_schemas_from_github(
             "folio-org", "mod-organizations-storage", "mod-orgs", folio_object
         )
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/ref_data_mapping.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/mapping_file_transformation/user_mapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/mapping_file_transformation/user_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import csv
 import json
 import logging
 import sys
-from datetime import datetime
-from datetime import timezone
 
 from dateutil.parser import parse
 from folio_uuid.folio_namespaces import FOLIONamespaces
 from folioclient import FolioClient
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
@@ -124,16 +122,18 @@
         for idx, row in enumerate(reader):
             if len(row.keys()) < 3:
                 raise TransformationProcessError(
                     idx, "something is wrong source file row", json.dumps(row)
                 )
             yield row
 
-    def get_prop(self, legacy_user, folio_prop_name, index_or_id):
-        mapped_value = super().get_prop(legacy_user, folio_prop_name, index_or_id)
+    def get_prop(self, legacy_user, folio_prop_name, index_or_id, schema_default_value):
+        mapped_value = super().get_prop(
+            legacy_user, folio_prop_name, index_or_id, schema_default_value
+        )
         if folio_prop_name == "personal.addresses.id":
             return ""
         elif folio_prop_name == "patronGroup":
             if self.groups_mapping:
                 return self.get_mapped_name(
                     self.groups_mapping,
                     legacy_user,
@@ -157,23 +157,24 @@
             )
         elif folio_prop_name in ["expirationDate", "enrollmentDate", "personal.dateOfBirth"]:
             return self.get_parsed_date(mapped_value, folio_prop_name)
         return mapped_value
 
     def get_parsed_date(self, mapped_value, folio_prop_name: str):
         try:
+            if not mapped_value.strip():
+                return ""
             format_date = parse(mapped_value, fuzzy=True)
-            fmt_string = f"{folio_prop_name}: {mapped_value} -> {format_date.isoformat()}"
             return format_date.isoformat()
         except Exception as ee:
             v = mapped_value
             logging.error(f"{folio_prop_name} {v} could not be parsed: {ee}")
-            fmt_string = f"Parsing error! {folio_prop_name}: {v}. NOW() was returned"
+            fmt_string = f"Parsing error! {folio_prop_name}: {v}. The empty string was returned"
             self.migration_report.add(Blurbs.DateTimeConversions, fmt_string)
-            return datetime.now(timezone.utc).isoformat()
+            return ""
 
     def setup_groups_mapping(self, groups_map):
         if groups_map:
             self.groups_mapping = RefDataMapping(
                 self.folio_client,
                 "/groups",
                 "usergroups",
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/conditions.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,20 @@
         logging.info(f"{len(self.statistical_codes)} \tstatistical_codes")
 
         # Raise for empty settings
         if not self.folio.class_types:
             raise TransformationProcessError("", "No class_types in FOLIO")
 
     def setup_reference_data_for_auth(self):
-        if self.folio_release not in [FolioRelease.morning_glory, FolioRelease.lotus]:
+        if self.folio_release not in [
+            FolioRelease.orchid,
+            FolioRelease.nolana,
+            FolioRelease.morning_glory,
+            FolioRelease.lotus,
+        ]:
             self.authority_source_files = list(
                 self.folio.folio_get_all(
                     "/authority-source-files", "authoritySourceFiles", self.folio.cql_all, 1000
                 )
             )
             logging.info(f"{len(self.authority_source_files)} \tAuthority source files")
         self.authority_note_types = list(
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/holdings_statementsparser.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/hrid_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 from typing import Set
 
-import requests
+import httpx
 from folio_uuid import FOLIONamespaces
 from folioclient import FolioClient
 from pymarc import Field
 from pymarc import Record
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.helper import Helper
@@ -21,19 +21,19 @@
         folio_client: FolioClient,
         handling: HridHandling,
         migration_report: MigrationReport,
         deactivate035_from001: bool,
     ):
         self.unique_001s: Set[str] = set()
         self.deactivate035_from001: bool = deactivate035_from001
-        hrid_path = "/hrid-settings-storage/hrid-settings"
+        self.hrid_path = "/hrid-settings-storage/hrid-settings"
         self.folio_client: FolioClient = folio_client
         self.handling: HridHandling = handling
         self.migration_report: MigrationReport = migration_report
-        self.hrid_settings = self.folio_client.folio_get_single_object(hrid_path)
+        self.hrid_settings = self.folio_client.folio_get_single_object(self.hrid_path)
         self.instance_hrid_prefix = self.hrid_settings["instances"]["prefix"]
         self.instance_hrid_counter = self.hrid_settings["instances"]["startNumber"]
         self.holdings_hrid_prefix = self.hrid_settings["holdings"]["prefix"]
         self.holdings_hrid_counter = self.hrid_settings["holdings"]["startNumber"]
         self.items_hrid_prefix = self.hrid_settings["items"]["prefix"]
         self.items_hrid_counter = self.hrid_settings["items"]["startNumber"]
         self.common_retain_leading_zeroes: bool = self.hrid_settings["commonRetainLeadingZeroes"]
@@ -152,17 +152,17 @@
                 logging.info("NOT POSTing HRID settings, since did not change.")
                 return
 
             self.hrid_settings["instances"]["startNumber"] = self.instance_hrid_counter
             self.hrid_settings["holdings"]["startNumber"] = self.holdings_hrid_counter
             self.hrid_settings["items"]["startNumber"] = self.items_hrid_counter
             url = self.folio_client.okapi_url + self.hrid_path
-            resp = requests.put(
+            resp = httpx.put(
                 url,
-                data=json.dumps(self.hrid_settings),
+                json=self.hrid_settings,
                 headers=self.folio_client.okapi_headers,
             )
             resp.raise_for_status()
             logging.info("%s Successfully set HRID settings.", resp.status_code)
             a = self.folio_client.folio_get_single_object(self.hrid_path)
             logging.info("Current hrid settings: %s", json.dumps(a, indent=4))
         except Exception:
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/loc_language_codes.xml`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/marc_file_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                         and folio_rec.get("formerIds", "")
                     ):
                         self.mapper.remove_from_id_map(folio_rec.get("formerIds", []))
 
     def save_srs_record(
         self,
         marc_record: Record,
-        file_def,
+        file_def: FileDefinition,
         folio_rec,
         legacy_ids: List[str],
         object_type: FOLIONamespaces,
     ):
         if not self.mapper.task_configuration.create_source_records:
             return
         if object_type in [FOLIONamespaces.holdings]:
@@ -151,15 +151,15 @@
         self.mapper.save_source_record(
             self.srs_records_file,
             self.object_type,
             self.mapper.folio_client,
             marc_record,
             folio_rec,
             legacy_ids,
-            file_def.suppressed,
+            file_def.discovery_suppressed,
         )
         self.mapper.migration_report.add_general_statistics("SRS records written to disk")
 
     def add_mapped_location_code_to_record(self, marc_record, folio_rec):
         location_code = next(
             (
                 location["code"]
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/marc_reader_wrapper.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_authorities.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,16 +509,16 @@
     ):
         entity_mapping = mapping["entity"]
         e_parent = entity_mapping[0]["target"].split(".")[0]
         if mapping.get("entityPerRepeatedSubfield", False):
             for temp_field in self.grouped(marc_field):
                 entity = self.create_entity(entity_mapping, temp_field, e_parent, legacy_ids)
                 if entity and (
-                    (type(entity) is dict and all(entity.values()))
-                    or (type(entity) is list and all(entity))
+                    (isinstance(entity, dict) and all(entity.values()))
+                    or (isinstance(entity, list) and all(entity))
                 ):
                     self.add_entity_to_record(entity, e_parent, folio_record, self.schema)
         else:
             if mapping.get("ignoreSubsequentSubfields", False):
                 marc_field = self.remove_repeated_subfields(marc_field)
             entity = self.create_entity(entity_mapping, marc_field, e_parent, legacy_ids)
             if e_parent in ["precedingTitles", "succeedingTitles"]:
@@ -546,15 +546,15 @@
                 )
                 # Experimental
                 # self.add_entity_to_record(entity, e_parent, rec, self.schema)
 
     def handle_suppression(
         self, folio_record, file_def: FileDefinition, only_discovery_suppress: bool = False
     ):
-        folio_record["discoverySuppress"] = file_def.suppressed
+        folio_record["discoverySuppress"] = file_def.discovery_suppressed
         self.migration_report.add(
             Blurbs.Suppression,
             f'Suppressed from discovery = {folio_record["discoverySuppress"]}',
         )
         if not only_discovery_suppress:
             folio_record["staffSuppress"] = file_def.staff_suppressed
             self.migration_report.add(
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_bibs.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                 self.migration_report.add(
                     Blurbs.HoldingsGenerationFromBibs,
                     "Records without 852s but with 86X",
                 )
 
     def wrap_up(self):
         logging.info("Mapper wrapping up")
-        if not self.task_configuration.never_update_hrid_settings:
+        if self.task_configuration.update_hrid_settings:
             self.hrid_handler.store_hrid_settings()
 
     def get_instance_type_id(self, marc_record, legacy_id):
         return_id = ""
 
         def get_folio_id_by_name(f336a: str):
             match_template = f336a.lower().replace(" ", "")
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/marc_rules_transformation/rules_mapper_holdings.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,17 +249,20 @@
             TransformationRecordFailedError: _description_
         """
         self.set_holdings_type(marc_record, folio_holding, legacy_ids)
         self.set_default_call_number_type_if_empty(folio_holding)
         self.pick_first_location_if_many(folio_holding, legacy_ids)
         self.parse_coded_holdings_statements(marc_record, folio_holding, legacy_ids)
         HoldingsHelper.handle_notes(folio_holding)
-        self.hrid_handler.handle_hrid(
-            FOLIONamespaces.holdings, folio_holding, marc_record, legacy_ids
-        )
+        if self.task_configuration.create_source_records:
+            self.hrid_handler.handle_hrid(
+                FOLIONamespaces.holdings, folio_holding, marc_record, legacy_ids
+            )
+        else:
+            del folio_holding["hrid"]
         if not folio_holding.get("instanceId", ""):
             raise TransformationRecordFailedError(
                 "".join(folio_holding.get("formerIds", [])),
                 "Missing instance ids. Something is wrong.",
                 "",
             )
         self.handle_suppression(folio_holding, file_def, True)
@@ -310,15 +313,15 @@
                     )
             except TransformationFieldMappingError as tfme:
                 Helper.log_data_issue(tfme.index_or_id, tfme.message, tfme.data_value)
                 self.migration_report.add(Blurbs.FieldMappingErrors, tfme.message)
 
     def wrap_up(self):
         logging.info("Mapper wrapping up")
-        if not self.task_configuration.never_update_hrid_settings:
+        if self.task_configuration.update_hrid_settings:
             if self.task_configuration.create_source_records:
                 self.hrid_handler.store_hrid_settings()
             else:
                 logging.info("NOT storing HRID settings since that is managed by FOLIO")
 
     def fetch_holdings_schema(self, folio_client: FolioClient):
         logging.info("Fetching HoldingsRecord schema...")
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_report.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_report.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/authority_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/authority_transformer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from typing import Annotated
 from typing import List
-from typing import Optional
 
 from folio_uuid.folio_namespaces import FOLIONamespaces
 from pydantic import Field
 
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import IlsFlavour
@@ -18,26 +17,62 @@
 )
 from folio_migration_tools.migration_tasks.migration_task_base import MigrationTaskBase
 from folio_migration_tools.task_configuration import AbstractTaskConfiguration
 
 
 class AuthorityTransformer(MigrationTaskBase):
     class TaskConfiguration(AbstractTaskConfiguration):
-        name: Annotated[str, Field(description=("Name of this task"))]
+        name: Annotated[
+            str,
+            Field(
+                description=(
+                    "Name of this migration task. The name is being used to call the specific "
+                    "task, and to distinguish tasks of similar types"
+                )
+            ),
+        ]
         migration_task_type: Annotated[
-            str, Field(description=("The string represenation of this class. Do not set"))
+            str,
+            Field(
+                title="Migration task type",
+                description=("The type of migration task you want to perform"),
+            ),
         ]
         files: Annotated[
             List[FileDefinition],
-            Field(description=("List of MARC21 files with authority records")),
+            Field(
+                title="Source files", description=("List of MARC21 files with authority records")
+            ),
+        ]
+        ils_flavour: Annotated[
+            IlsFlavour,
+            Field(
+                title="ILS flavour", description="The type of ILS you are migrating records from."
+            ),
         ]
-        ils_flavour: IlsFlavour
-        tags_to_delete: Optional[List[str]] = []
+        tags_to_delete: Annotated[
+            List[str],
+            Field(
+                title="Tags to delete from MARC record",
+                description=(
+                    "Tags in the incoming MARC authority that the process should remove "
+                    "before adding them into FOLIO. These tags will be used in the "
+                    "transformation before getting removed."
+                ),
+            ),
+        ] = []
         create_source_records: Annotated[
-            bool, Field(description="Controls wheter or not to retain the MARC records in SRS.")
+            bool,
+            Field(
+                title="Create source records",
+                description=(
+                    "Controls wheter or not to retain the MARC records in "
+                    "Source Record Storage."
+                ),
+            ),
         ] = True
 
     @staticmethod
     def get_object_type() -> FOLIONamespaces:
         return FOLIONamespaces.authorities
 
     def __init__(
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/batch_poster.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/batch_poster.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import traceback
 from datetime import datetime
 from typing import Annotated
 from typing import List
 from uuid import uuid4
 
-import requests
+import httpx
 from folio_uuid.folio_namespaces import FOLIONamespaces
 from pydantic import Field
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.custom_exceptions import TransformationRecordFailedError
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
@@ -99,75 +99,81 @@
         self.failed_batches = 0
         self.users_created = 0
         self.users_updated = 0
         self.users_per_group: dict = {}
         self.failed_fields: set = set()
         self.num_failures = 0
         self.num_posted = 0
+        self.okapi_headers = self.folio_client.okapi_headers
+        self.http_client = None
 
     def do_work(self):
-        try:
-            batch = []
-            if self.task_configuration.object_type == "SRS":
-                self.create_snapshot()
-            with open(self.folder_structure.failed_recs_path, "w") as failed_recs_file:
-                for file_def in self.task_configuration.files:
-                    path = self.folder_structure.results_folder / file_def.file_name
-                    with open(path) as rows:
-                        logging.info("Running %s", path)
-                        last_row = ""
-                        for self.processed, row in enumerate(rows, start=1):
-                            last_row = row
-                            if row.strip():
-                                try:
-                                    if self.task_configuration.object_type == "Extradata":
-                                        self.post_extra_data(row, self.processed, failed_recs_file)
-                                    elif not self.api_info["is_batch"]:
-                                        self.post_single_records(
-                                            row, self.processed, failed_recs_file
+        with httpx.Client(timeout=None, headers=self.folio_client.okapi_headers) as httpx_client:
+            self.http_client = httpx_client
+            try:
+                batch = []
+                if self.task_configuration.object_type == "SRS":
+                    self.create_snapshot()
+                with open(self.folder_structure.failed_recs_path, "w") as failed_recs_file:
+                    for file_def in self.task_configuration.files:
+                        path = self.folder_structure.results_folder / file_def.file_name
+                        with open(path) as rows:
+                            logging.info("Running %s", path)
+                            last_row = ""
+                            for self.processed, row in enumerate(rows, start=1):
+                                last_row = row
+                                if row.strip():
+                                    try:
+                                        if self.task_configuration.object_type == "Extradata":
+                                            self.post_extra_data(
+                                                row, self.processed, failed_recs_file
+                                            )
+                                        elif not self.api_info["is_batch"]:
+                                            self.post_single_records(
+                                                row, self.processed, failed_recs_file
+                                            )
+                                        else:
+                                            batch = self.post_record_batch(
+                                                batch, failed_recs_file, row
+                                            )
+                                    except UnicodeDecodeError as unicode_error:
+                                        self.handle_unicode_error(unicode_error, last_row)
+                                    except TransformationProcessError as tpe:
+                                        self.handle_generic_exception(
+                                            tpe,
+                                            last_row,
+                                            batch,
+                                            self.processed,
+                                            failed_recs_file,
                                         )
-                                    else:
-                                        batch = self.post_record_batch(
-                                            batch, failed_recs_file, row
+                                        logging.critical("Halting %s", tpe)
+                                        print(f"\n\t{tpe.message}")
+                                        sys.exit(1)
+                                    except TransformationRecordFailedError as exception:
+                                        self.handle_generic_exception(
+                                            exception,
+                                            last_row,
+                                            batch,
+                                            self.processed,
+                                            failed_recs_file,
                                         )
-                                except UnicodeDecodeError as unicode_error:
-                                    self.handle_unicode_error(unicode_error, last_row)
-                                except TransformationProcessError as tpe:
-                                    self.handle_generic_exception(
-                                        tpe,
-                                        last_row,
-                                        batch,
-                                        self.processed,
-                                        failed_recs_file,
-                                    )
-                                    logging.critical("Halting %s", tpe)
-                                    print(f"\n\t{tpe.message}")
-                                    sys.exit(1)
-                                except TransformationRecordFailedError as exception:
-                                    self.handle_generic_exception(
-                                        exception,
-                                        last_row,
-                                        batch,
-                                        self.processed,
-                                        failed_recs_file,
-                                    )
-                                    batch = []
-
-                if self.task_configuration.object_type != "Extradata" and any(batch):
-                    try:
-                        self.post_batch(batch, failed_recs_file, self.processed)
-                    except Exception as exception:
-                        self.handle_generic_exception(
-                            exception, last_row, batch, self.processed, failed_recs_file
-                        )
-                logging.info("Done posting %s records. ", (self.processed))
-        except Exception as ee:
-            if self.task_configuration.object_type == "SRS":
-                self.commit_snapshot()
-            raise ee
+                                        batch = []
+
+                    if self.task_configuration.object_type != "Extradata" and any(batch):
+                        try:
+                            self.post_batch(batch, failed_recs_file, self.processed)
+                        except Exception as exception:
+                            self.handle_generic_exception(
+                                exception, last_row, batch, self.processed, failed_recs_file
+                            )
+                    logging.info("Done posting %s records. ", (self.processed))
+            except Exception as ee:
+                if self.task_configuration.object_type == "SRS":
+                    self.commit_snapshot()
+                raise ee
 
     def post_record_batch(self, batch, failed_recs_file, row):
         json_rec = json.loads(row.split("\t")[-1])
         if (
             self.task_configuration.object_type in ["Instances", "Holdings", "Items"]
             and not self.task_configuration.use_safe_inventory_endpoints
         ):
@@ -230,17 +236,20 @@
             logging.info(
                 "%s records posted successfully. %s failed",
                 self.num_posted,
                 self.num_failures,
             )
 
     def post_objects(self, url, body):
-        return requests.post(
-            url, headers=self.folio_client.okapi_headers, data=body.encode("utf-8")
-        )
+        if self.http_client and not self.http_client.is_closed:
+            return self.http_client.post(url, data=body.encode("utf-8"))
+        else:
+            return httpx.post(
+                url, headers=self.okapi_headers, data=body.encode("utf-8"), timeout=None
+            )
 
     def handle_generic_exception(self, exception, last_row, batch, num_records, failed_recs_file):
         logging.error("%s", exception)
         self.migration_report.add(Blurbs.Details, "Generic exceptions (see log for details)")
         # logging.error("Failed row: %s", last_row)
         self.failed_batches += 1
         self.num_failures += len(batch)
@@ -379,17 +388,20 @@
         url = self.folio_client.okapi_url + path
         if self.api_info["object_name"] == "users":
             payload = {self.api_info["object_name"]: list(batch), "totalRecords": len(batch)}
         elif self.api_info["total_records"]:
             payload = {"records": list(batch), "totalRecords": len(batch)}
         else:
             payload = {self.api_info["object_name"]: batch}
-        return requests.post(
-            url, data=json.dumps(payload), headers=self.folio_client.okapi_headers
-        )
+        if self.http_client and not self.http_client.is_closed:
+            return self.http_client.post(url, data=json.dumps(payload))
+        else:
+            return httpx.post(
+                url, headers=self.okapi_headers, data=json.dumps(payload), timeout=None
+            )
 
     def wrap_up(self):
         logging.info("Done. Wrapping up")
         self.extradata_writer.flush()
         if self.task_configuration.object_type == "SRS":
             self.commit_snapshot()
         if self.task_configuration.object_type != "Extradata":
@@ -461,40 +473,49 @@
         snapshot = {
             "jobExecutionId": self.snapshot_id,
             "status": "PARSING_IN_PROGRESS",
             "processingStartedDate": datetime.utcnow().isoformat(timespec="milliseconds"),
         }
         try:
             url = f"{self.folio_client.okapi_url}/source-storage/snapshots"
-            res = requests.post(
-                url, data=json.dumps(snapshot), headers=self.folio_client.okapi_headers
-            )
+            if self.http_client and not self.http_client.is_closed:
+                res = self.http_client.post(url, data=json.dumps(snapshot))
+            else:
+                res = httpx.post(
+                    url, headers=self.okapi_headers, data=json.dumps(snapshot), timeout=None
+                )
             res.raise_for_status()
             logging.info("Posted Snapshot to FOLIO: %s", json.dumps(snapshot, indent=4))
             get_url = f"{self.folio_client.okapi_url}/source-storage/snapshots/{self.snapshot_id}"
             getted = False
             while not getted:
                 logging.info("Sleeping while waiting for the snapshot to get created")
                 time.sleep(5)
-                res = requests.get(get_url, headers=self.folio_client.okapi_headers)
+                if self.http_client and not self.http_client.is_closed:
+                    res = self.http_client.get(get_url)
+                else:
+                    res = httpx.get(get_url, headers=self.okapi_headers, timeout=None)
                 if res.status_code == 200:
                     getted = True
                 else:
                     logging.info(res.status_code)
         except Exception:
             logging.exception("Could not post the snapshot")
             sys.exit(1)
 
     def commit_snapshot(self):
         snapshot = {"jobExecutionId": self.snapshot_id, "status": "COMMITTED"}
         try:
             url = f"{self.folio_client.okapi_url}/source-storage/snapshots/{self.snapshot_id}"
-            res = requests.put(
-                url, data=json.dumps(snapshot), headers=self.folio_client.okapi_headers
-            )
+            if self.http_client and not self.http_client.is_closed:
+                res = self.http_client.put(url, data=json.dumps(snapshot))
+            else:
+                res = httpx.put(
+                    url, headers=self.okapi_headers, data=json.dumps(snapshot), timeout=None
+                )
             res.raise_for_status()
             logging.info("Posted Committed snapshot to FOLIO: %s", json.dumps(snapshot, indent=4))
         except Exception:
             logging.exception(
                 "Could not commit snapshot with id %s. Post this to /source-storage/snapshots/%s:",
                 self.snapshot_id,
                 self.snapshot_id,
@@ -568,14 +589,21 @@
         "Organizations": {
             "object_name": "",
             "api_endpoint": "/organizations/organizations",
             "is_batch": False,
             "total_records": False,
             "addSnapshotId": False,
         },
+        "Orders": {
+            "object_name": "",
+            "api_endpoint": "/orders/composite-orders",
+            "is_batch": False,
+            "total_records": False,
+            "addSnapshotId": False,
+        },
     }
 
     try:
         return choices[object_type]
     except KeyError:
         key_string = ",".join(choices.keys())
         logging.error(f"Wrong type. Only one of {key_string} are allowed")
@@ -625,13 +653,13 @@
     suffix_index = 0
     while size > 1024 and suffix_index < 4:
         suffix_index += 1  # increment the index of the suffix
         size = size / 1024.0  # apply the division
     return "%.*f%s" % (precision, size, suffixes[suffix_index])
 
 
-def get_req_size(response):
+def get_req_size(response: httpx.Response):
     size = response.request.method
-    size += response.request.url
+    size += str(response.request.url)
     size += "\r\n".join(f"{k}{v}" for k, v in response.request.headers.items())
-    size += response.request.body or []
+    size += response.request.content.decode("utf-8") or ""
     return get_human_readable(len(size.encode("utf-8")))
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/bibs_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/bibs_transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 from typing import Annotated
 from typing import List
-from typing import Optional
 
 from folio_uuid.folio_namespaces import FOLIONamespaces
 from pydantic import Field
 
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import HridHandling
@@ -19,57 +18,135 @@
 )
 from folio_migration_tools.migration_tasks.migration_task_base import MigrationTaskBase
 from folio_migration_tools.task_configuration import AbstractTaskConfiguration
 
 
 class BibsTransformer(MigrationTaskBase):
     class TaskConfiguration(AbstractTaskConfiguration):
-        name: str
-        add_administrative_notes_with_legacy_ids: Annotated[
-            bool,
+        name: Annotated[
+            str,
             Field(
                 description=(
-                    "If set to true, an Administrative note will be added to the records "
-                    "containing the legacy ID. Use this in order to protect the values from "
-                    "getting overwritten by overlays,"
-                ),
+                    "Name of this migration task. The name is being used to call the specific "
+                    "task, and to distinguish tasks of similar types"
+                )
             ),
-        ] = True
-        migration_task_type: str
-        hrid_handling: Optional[HridHandling] = HridHandling.default
-        deactivate035_from001: Optional[bool] = False
-        files: List[FileDefinition]
-        ils_flavour: IlsFlavour
+        ]
+        migration_task_type: Annotated[
+            str,
+            Field(
+                title="Migration task type",
+                description=("The type of migration task you want to perform."),
+            ),
+        ]
+        files: Annotated[
+            List[FileDefinition],
+            Field(
+                title="Source files",
+                description=("List of MARC21 files with bibliographic records."),
+            ),
+        ]
+        ils_flavour: Annotated[
+            IlsFlavour,
+            Field(
+                title="ILS flavour", description="The type of ILS you are migrating records from."
+            ),
+        ]
         custom_bib_id_field: Annotated[
             str,
             Field(
+                title="Custom BIB ID field",
                 description=(
                     'A string representing a MARC field with optional subfield indicated by a "$" '
                     '(eg. "991$a") from which to draw legacy Bib ID. Use this in combination '
                     'with `ilsFlavour: "custom"`. Defaults to "001", and is ignored for all other '
                     "ilsFlavours."
-                )
+                ),
             ),
         ] = "001"
-        tags_to_delete: Optional[List[str]] = []
-        reset_hrid_settings: Optional[bool] = False
-        never_update_hrid_settings: Optional[bool] = False
+        add_administrative_notes_with_legacy_ids: Annotated[
+            bool,
+            Field(
+                title="Add administrative notes with legacy IDs",
+                description=(
+                    "If set to true, an Administrative note will be added to the records "
+                    "containing the legacy ID. Use this in order to protect the values from "
+                    "getting overwritten by overlays,"
+                ),
+            ),
+        ] = True
+        tags_to_delete: Annotated[
+            List[str],
+            Field(
+                title="Tags to delete from MARC record",
+                description=(
+                    "Tags in the incoming MARC authority that the process should remove "
+                    "before adding them into FOLIO. These tags will be used in the "
+                    "transformation before getting removed."
+                ),
+            ),
+        ] = []
         create_source_records: Annotated[
-            bool, Field(description="Controls wheter or not to retain the MARC records in SRS.")
+            bool,
+            Field(
+                title="Create source records",
+                description=(
+                    "Controls wheter or not to retain the MARC records in "
+                    "Source Record Storage."
+                ),
+            ),
         ] = True
         parse_cataloged_date: Annotated[
             bool,
             Field(
                 title="Parse cataloged date",
                 description=(
                     "Parse fields mapped to catalogedDate into a FOLIO accepted date string using "
                     "dateutil.parser. Verify results carefully when using"
                 ),
             ),
         ] = False
+        hrid_handling: Annotated[
+            HridHandling,
+            Field(
+                title="HRID Handling",
+                description=(
+                    "Setting to default will make FOLIO generate HRIDs and move the existing "
+                    "001:s into a 035, concatenated with the 003. Choosing preserve001 means "
+                    "the 001:s will remain in place, and that they will also become the HRIDs"
+                ),
+            ),
+        ] = HridHandling.default
+        reset_hrid_settings: Annotated[
+            bool,
+            Field(
+                title="Reset HRID settings",
+                description=(
+                    "Setting to true means the task will "
+                    "reset the HRID counters for this particular record type"
+                ),
+            ),
+        ] = False
+        update_hrid_settings: Annotated[
+            bool,
+            Field(
+                title="Update HRID settings",
+                description="At the end of the run, update FOLIO with the HRID settings",
+            ),
+        ] = True
+        deactivate035_from001: Annotated[
+            bool,
+            Field(
+                title="Create 035 from 001 and 003",
+                description=(
+                    "This deactivates the FOLIO default functionality of moving the previous 001 "
+                    "into a 035, prefixed with the value from 003"
+                ),
+            ),
+        ] = False
 
     @staticmethod
     def get_object_type() -> FOLIONamespaces:
         return FOLIONamespaces.instances
 
     def __init__(
         self,
@@ -82,15 +159,15 @@
         self.check_source_files(
             self.folder_structure.legacy_records_folder, self.task_configuration.files
         )
         self.mapper = BibsRulesMapper(self.folio_client, library_config, self.task_configuration)
         self.bib_ids: set = set()
         if (
             self.task_configuration.reset_hrid_settings
-            and not self.task_configuration.never_update_hrid_settings
+            and self.task_configuration.update_hrid_settings
         ):
             self.mapper.hrid_handler.reset_instance_hrid_counter()
         logging.info("Init done")
 
     def do_work(self):
         self.do_work_marc_transformer()
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/courses_migrator.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/courses_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/holdings_csv_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,21 @@
         call_number_type_map_file_name: Optional[str]
         holdings_merge_criteria: Optional[list[str]] = [
             "instanceId",
             "permanentLocationId",
             "callNumber",
         ]
         reset_hrid_settings: Optional[bool] = False
-        never_update_hrid_settings: Optional[bool] = False
+        update_hrid_settings: Annotated[
+            bool,
+            Field(
+                title="Update HRID settings",
+                description="At the end of the run, update FOLIO with the HRID settings",
+            ),
+        ] = True
 
     @staticmethod
     def get_object_type() -> FOLIONamespaces:
         return FOLIONamespaces.holdings
 
     def __init__(
         self,
@@ -131,15 +137,15 @@
                     )
 
             else:
                 logging.info("No file of legacy holdings setup.")
 
             if (
                 self.task_configuration.reset_hrid_settings
-                and not self.task_configuration.never_update_hrid_settings
+                and self.task_configuration.update_hrid_settings
             ):
                 hrid_handler = HRIDHandler(
                     self.folio_client, HridHandling.default, self.mapper.migration_report, True
                 )
                 hrid_handler.reset_holdings_hrid_counter()
 
         except HTTPError as http_error:
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/holdings_marc_transformer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 '''Main "script."'''
 import csv
 import logging
 from typing import Annotated
 from typing import List
-from typing import Optional
 
 from folio_uuid.folio_namespaces import FOLIONamespaces
 from pydantic import Field
 
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
@@ -18,24 +17,57 @@
 )
 from folio_migration_tools.migration_tasks.migration_task_base import MigrationTaskBase
 from folio_migration_tools.task_configuration import AbstractTaskConfiguration
 
 
 class HoldingsMarcTransformer(MigrationTaskBase):
     class TaskConfiguration(AbstractTaskConfiguration):
-        name: str
-        legacy_id_marc_path: str
-        deduplicate_holdings_statements: Optional[bool] = True
-        migration_task_type: str
-        hrid_handling: Optional[HridHandling] = HridHandling.default
-        deactivate035_from001: Optional[bool] = False
-        files: List[FileDefinition]
-        location_map_file_name: str
-        default_call_number_type_name: str
-        fallback_holdings_type_id: str
+        name: Annotated[
+            str,
+            Field(
+                description=(
+                    "Name of this migration task. The name is being used to call the specific "
+                    "task, and to distinguish tasks of similar types"
+                )
+            ),
+        ]
+        migration_task_type: Annotated[
+            str,
+            Field(
+                title="Migration task type",
+                description=("The type of migration task you want to perform"),
+            ),
+        ]
+        files: Annotated[
+            List[FileDefinition],
+            Field(
+                title="Source files", description=("List of MARC21 files with holdings records")
+            ),
+        ]
+        hrid_handling: Annotated[
+            HridHandling,
+            Field(
+                title="HRID Handling",
+                description=(
+                    "Setting to default will make FOLIO generate HRIDs and move the existing "
+                    "001:s into a 035, concatenated with the 003. Choosing preserve001 means "
+                    "the 001:s will remain in place, and that they will also become the HRIDs"
+                ),
+            ),
+        ] = HridHandling.default
+        deactivate035_from001: Annotated[
+            bool,
+            Field(
+                title="Create 035 from 001 and 003",
+                description=(
+                    "This deactivates the FOLIO default functionality of moving the previous 001 "
+                    "into a 035, prefixed with the value from 003"
+                ),
+            ),
+        ] = False
         holdings_type_uuid_for_boundwiths: Annotated[
             str,
             Field(
                 title="Holdings Type for Boundwith Holdings",
                 description=(
                     "UUID for a Holdings type (set in Settings->Inventory) "
                     "for Bound-with Holdings)"
@@ -49,18 +81,81 @@
                 description=(
                     "Path to a file outlining Boundwith relationships, in the style of Voyager."
                     " A TSV file with MFHD_ID and BIB_ID headers and values"
                 ),
             ),
         ] = ""
         create_source_records: Annotated[
-            bool, Field(description="Controls wheter or not to retain the MARC records in SRS.")
+            bool,
+            Field(
+                title="Create source records",
+                description=(
+                    "Controls wheter or not to retain the MARC records in "
+                    "Source Record Storage."
+                ),
+            ),
+        ] = True
+        update_hrid_settings: Annotated[
+            bool,
+            Field(
+                title="Update HRID settings",
+                description="At the end of the run, update FOLIO with the HRID settings",
+            ),
+        ] = True
+        reset_hrid_settings: Annotated[
+            bool,
+            Field(
+                title="Reset HRID settings",
+                description=(
+                    "Setting to true means the task will "
+                    "reset the HRID counters for this particular record type"
+                ),
+            ),
+        ] = False
+        legacy_id_marc_path: Annotated[
+            str,
+            Field(
+                title="Path to legacy id in the records",
+                description=(
+                    "The path to the field where the legacy id is located. "
+                    "Example syntax: '001' or '951$c'"
+                ),
+            ),
+        ]
+        deduplicate_holdings_statements: Annotated[
+            bool,
+            Field(
+                title="Deduplicate holdings statements",
+                description=(
+                    "If set to False, duplicate holding statements within the same record will "
+                    "remain in place"
+                ),
+            ),
         ] = True
-        reset_hrid_settings: Optional[bool] = False
-        never_update_hrid_settings: Optional[bool] = False
+        location_map_file_name: Annotated[
+            str,
+            Field(
+                title="Path to location map file",
+                description="Must be a TSV file located in the mapping_files folder",
+            ),
+        ]
+        default_call_number_type_name: Annotated[
+            str,
+            Field(
+                title="Default callnumber type name",
+                description="The name of the callnumber type that will be used as fallback",
+            ),
+        ]
+        fallback_holdings_type_id: Annotated[
+            str,
+            Field(
+                title="Fallback holdings type id",
+                description="The UUID of the Holdings type that will be used for unmapped values",
+            ),
+        ]
 
     @staticmethod
     def get_object_type() -> FOLIONamespaces:
         return FOLIONamespaces.holdings
 
     def __init__(
         self,
@@ -126,15 +221,15 @@
             self.task_config,
             self.library_configuration,
             self.instance_id_map,
             self.boundwith_relationship_map,
         )
         if (
             self.task_configuration.reset_hrid_settings
-            and not self.task_configuration.never_update_hrid_settings
+            and self.task_configuration.update_hrid_settings
         ):
             self.mapper.hrid_handler.reset_holdings_hrid_counter()
         logging.info("%s Instance ids in map", len(self.instance_id_map))
         logging.info("Init done")
 
     def do_work(self):
         self.do_work_marc_transformer()
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/items_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/items_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,21 @@
         material_types_map_file_name: str
         loan_types_map_file_name: str
         temp_loan_types_map_file_name: Optional[str] = ""
         statistical_codes_map_file_name: Optional[str] = ""
         item_statuses_map_file_name: str
         call_number_type_map_file_name: str
         reset_hrid_settings: Optional[bool] = False
-        never_update_hrid_settings: Optional[bool] = False
+        update_hrid_settings: Annotated[
+            bool,
+            Field(
+                title="Update HRID settings",
+                description="At the end of the run, update FOLIO with the HRID settings",
+            ),
+        ] = True
         boundwith_relationship_file_path: Annotated[
             str,
             Field(
                 title="Boundwith relationship file path",
                 description=(
                     "Path to a file outlining Boundwith relationships, in the style of Voyager."
                     " A TSV file with MFHD_ID and BIB_ID headers and values"
@@ -181,15 +187,15 @@
             temporary_loan_type_mapping,
             temporary_location_mapping,
             self.library_configuration,
             self.boundwith_relationship_map,
         )
         if (
             self.task_configuration.reset_hrid_settings
-            and not self.task_configuration.never_update_hrid_settings
+            and self.task_configuration.update_hrid_settings
         ):
             hrid_handler = HRIDHandler(
                 self.folio_client, HridHandling.default, self.mapper.migration_report, True
             )
             hrid_handler.reset_item_hrid_counter()
 
         logging.info("Init done")
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/loans_migrator.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/loans_migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import traceback
 from datetime import datetime
 from datetime import timedelta
 from typing import Optional
 from urllib.error import HTTPError
 from zoneinfo import ZoneInfo
 
-import requests
+import httpx
 from dateutil import parser as du_parser
 from folio_uuid.folio_namespaces import FOLIONamespaces
 
 from folio_migration_tools.circulation_helper import CirculationHelper
 from folio_migration_tools.helper import Helper
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
@@ -148,34 +148,39 @@
             for i in range(10, 0, -1):
                 sys.stdout.write("Pausing for {:02d} seconds. Press Ctrl+C to exit...\r".format(i))
                 time.sleep(1)
         else:
             logging.info("SMTP connection is disabled...")
 
     def do_work(self):
-        logging.info("Starting")
-        starting_index = (
-            self.task_configuration.starting_row - 1
-            if self.task_configuration.starting_row > 0
-            else 0
-        )
-        if self.task_configuration.starting_row > 1:
-            logging.info(f"Skipping {(starting_index)} records")
-        for num_loans, legacy_loan in enumerate(self.valid_legacy_loans[starting_index:], start=1):
-            t0_migration = time.time()
-            self.migration_report.add_general_statistics("Processed pre-validated loans")
-            try:
-                self.checkout_single_loan(legacy_loan)
-            except Exception as ee:
-                logging.exception(
-                    f"Error in row {num_loans}  Item barcode: {legacy_loan.item_barcode} "
-                    f"Patron barcode: {legacy_loan.patron_barcode} {ee}"
-                )
-            if num_loans % 25 == 0:
-                logging.info(f"{timings(self.t0, t0_migration, num_loans)} {num_loans}")
+        with httpx.Client(
+            timeout=None, headers=self.folio_client.okapi_headers
+        ) as self.http_client:
+            logging.info("Starting")
+            starting_index = (
+                self.task_configuration.starting_row - 1
+                if self.task_configuration.starting_row > 0
+                else 0
+            )
+            if self.task_configuration.starting_row > 1:
+                logging.info(f"Skipping {(starting_index)} records")
+            for num_loans, legacy_loan in enumerate(
+                self.valid_legacy_loans[starting_index:], start=1
+            ):
+                t0_migration = time.time()
+                self.migration_report.add_general_statistics("Processed pre-validated loans")
+                try:
+                    self.checkout_single_loan(legacy_loan)
+                except Exception as ee:
+                    logging.exception(
+                        f"Error in row {num_loans}  Item barcode: {legacy_loan.item_barcode} "
+                        f"Patron barcode: {legacy_loan.patron_barcode} {ee}"
+                    )
+                if num_loans % 25 == 0:
+                    logging.info(f"{timings(self.t0, t0_migration, num_loans)} {num_loans}")
 
     def checkout_single_loan(self, legacy_loan: LegacyLoan):
         """Checks a legacy loan out. Retries once if it fails.
 
         Args:
             legacy_loan (LegacyLoan): The Legacy loan
         """
@@ -452,18 +457,18 @@
         try:
             loan_to_put = copy.deepcopy(folio_loan)
             del loan_to_put["metadata"]
             loan_to_put["dueDate"] = due_date.isoformat()
             loan_to_put["loanDate"] = out_date.isoformat()
             loan_to_put["renewalCount"] = renewal_count
             url = f"{self.folio_client.okapi_url}/circulation/loans/{loan_to_put['id']}"
-            req = requests.put(
+            req = self.http_client.put(
                 url,
                 headers=self.folio_client.okapi_headers,
-                data=json.dumps(loan_to_put),
+                json=loan_to_put,
             )
             if req.status_code == 422:
                 error_message = json.loads(req.text)["errors"][0]["message"]
                 s = f"Update open loan error: {error_message} {req.status_code}"
                 self.migration_report.add(Blurbs.Details, s)
                 logging.error(s)
                 return False
@@ -533,15 +538,15 @@
             )
 
     def set_item_status(self, legacy_loan: LegacyLoan):
         try:
             # Get Item by barcode, update status.
             item_path = f'item-storage/items?query=(barcode=="{legacy_loan.item_barcode}")'
             item_url = f"{self.folio_client.okapi_url}/{item_path}"
-            resp = requests.get(item_url, headers=self.folio_client.okapi_headers)
+            resp = self.http_client.get(item_url, headers=self.folio_client.okapi_headers)
             resp.raise_for_status()
             data = resp.json()
             folio_item = data["items"][0]
             folio_item["status"]["name"] = legacy_loan.next_item_status
             if self.update_item(folio_item):
                 self.migration_report.add(
                     Blurbs.Details,
@@ -586,33 +591,33 @@
 
     def update_user(self, user):
         url = f'/users/{user["id"]}'
         self.folio_put_post(url, user, "PUT", "Update user")
 
     def get_user_by_barcode(self, barcode):
         url = f'{self.folio_client.okapi_url}/users?query=(barcode=="{barcode}")'
-        resp = requests.get(url, headers=self.folio_client.okapi_headers)
+        resp = self.http_client.get(url, headers=self.folio_client.okapi_headers)
         resp.raise_for_status()
         data = resp.json()
         return data["users"][0]
 
     def folio_put_post(self, url, data_dict, verb, action_description=""):
         full_url = f"{self.folio_client.okapi_url}{url}"
         try:
             if verb == "PUT":
-                resp = requests.put(
+                resp = self.http_client.put(
                     full_url,
                     headers=self.folio_client.okapi_headers,
-                    data=json.dumps(data_dict),
+                    json=data_dict,
                 )
             elif verb == "POST":
-                resp = requests.post(
+                resp = self.http_client.post(
                     full_url,
                     headers=self.folio_client.okapi_headers,
-                    data=json.dumps(data_dict),
+                    json=data_dict,
                 )
             else:
                 raise Exception("Bad verb")
             if resp.status_code == 422:
                 error_message = json.loads(resp.text)["errors"][0]["message"]
                 logging.error(error_message)
                 self.migration_report.add(
@@ -639,16 +644,16 @@
             return False
 
     def change_due_date(self, folio_loan, legacy_loan):
         try:
             api_path = f"{folio_loan['id']}/change-due-date"
             api_url = f"{self.folio_client.okapi_url}/circulation/loans/{api_path}"
             body = {"dueDate": du_parser.isoparse(str(legacy_loan.due_date)).isoformat()}
-            req = requests.post(
-                api_url, headers=self.folio_client.okapi_headers, data=json.dumps(body)
+            req = self.http_client.post(
+                api_url, headers=self.folio_client.okapi_headers, json=body
             )
             if req.status_code == 422:
                 error_message = json.loads(req.text)["errors"][0]["message"]
                 self.migration_report.add(
                     Blurbs.Details, f"Change due date error: {error_message}"
                 )
                 logging.info(
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/migration_task_base.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/migration_task_base.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/orders_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/orders_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/organization_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/organization_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/requests_migrator.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/requests_migrator.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/reserves_migrator.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/reserves_migrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import sys
 import time
 import traceback
 from typing import Dict
 from urllib.error import HTTPError
 
-import requests
+import httpx
 from folio_uuid.folio_namespaces import FOLIONamespaces
 
 from folio_migration_tools.custom_dict import InsensitiveDictReader
 from folio_migration_tools.custom_exceptions import TransformationProcessError
 from folio_migration_tools.library_configuration import FileDefinition
 from folio_migration_tools.library_configuration import LibraryConfiguration
 from folio_migration_tools.migration_report import MigrationReport
@@ -162,24 +162,24 @@
             logging.critical("Halting...")
             sys.exit(1)
 
     def folio_put_post(self, url, data_dict, verb, action_description=""):
         full_url = f"{self.folio_client.okapi_url}{url}"
         try:
             if verb == "PUT":
-                resp = requests.put(
+                resp = httpx.put(
                     full_url,
                     headers=self.folio_client.okapi_headers,
-                    data=json.dumps(data_dict),
+                    json=data_dict,
                 )
             elif verb == "POST":
-                resp = requests.post(
+                resp = httpx.post(
                     full_url,
                     headers=self.folio_client.okapi_headers,
-                    data=json.dumps(data_dict),
+                    json=data_dict,
                 )
             else:
                 raise TransformationProcessError("Bad verb supplied. This is a code issue.")
             if resp.status_code == 422:
                 error_message = json.loads(resp.text)["errors"][0]["message"]
                 logging.error(error_message)
                 self.migration_report.add(
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/migration_tasks/user_transformer.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/migration_tasks/user_transformer.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/report_blurbs.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/report_blurbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,16 +164,20 @@
     LegacyLocationCodes = ("Legacy location codes", "")
     Locations = (
         "Locations - Unmapped legacy codes",
         "",
     )
     UserGroupMapping = ("User group mapping", "")
     DefaultValuesAdded = (
-        "Default values added",
-        "The values below was added to all records from the value field in the mapping file instead of coming from the source records",
+        "Default values from mapping added",
+        "The values below were added to all records from the 'value' field in the mapping file, overriding any mapped values from the source data.",
+    )
+    FolioDefaultValuesAdded = (
+        "FOLIO default values added",
+        "The below FOLIO default values were added to records that had no mapped value in the source data.",
     )
     UsersPerPatronType = ("Users per patron type", "")
     MappedLocations = ("Mapped Locations", "")
     Leader06 = ("Leader 06 (Holdings type)", "")
     Section3 = ("__Section 3: items", "The entries below seem to be related to items")
     Exceptions = ("Exceptions", "")
     HridHandling = (
@@ -233,14 +237,18 @@
         'Most language codes in MARC records come from this list: https://www.loc.gov/marc/languages/, But other codes are allowed. The controlled vocabulary needs to be stated in $2 and this is where the information in this list comes from. The mapping tools can not currently handle other language codes, and so cannot FOLIO. <br/>One solution is to migrate the codes into a string or/and replace the language code with the parent language (these languages are usually subgroups of other languages). Many times, these records already have the "super-language" recorded as well. The data will remain in the MARC records.',
     )
     FailedFiles = ("Failed files", "")
     BoundWithMappings = ("Bound-with mapping", "")
     TemporaryLocationMapping = ("Temporary location mapping", "")
     TemporaryLoanTypeMapping = ("Temporary Loan type mapping", "")
     PermanentLoanTypeMapping = ("Permanent Loan type mapping", "")
+    OrderLineLocationMapping = (
+        "Order line location mapping",
+        "This is the holdings location for for the order line (used to create holdings records if settings are configured to do so)",
+    )
     StatisticalCodeMapping = ("Statistical code mapping", "")
     HoldingsRecordIdMapping = ("Holdings IDs mapped", "")
     UnmappedProperties = ("Unmapped properties", "")
     StatusMapping = ("Status mapping", "")
     ReferenceDataMapping = ("Reference Data Mapping", "")
     FieldMappingErrors = ("Field mapping errors", "")
     AddedValueFromParameter = ("Added value from parameter since value is empty", "")
```

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/test_infrastructure/mocked_classes.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/test_infrastructure/mocked_classes.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/legacy_loan.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/legacy_loan.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/legacy_request.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/legacy_request.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/legacy_reserve.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/legacy_reserve.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/src/folio_migration_tools/transaction_migration/transaction_result.py` & `folio_migration_tools-1.8.0rc1/src/folio_migration_tools/transaction_migration/transaction_result.py`

 * *Files identical despite different names*

### Comparing `folio_migration_tools-1.7.9rc2/setup.py` & `folio_migration_tools-1.8.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 {'': ['*']}
 
 install_requires = \
 ['argparse-prompt>=0.0.5,<0.0.6',
  'deepdiff>=6.2.3,<7.0.0',
  'defusedxml>=0.7.1,<0.8.0',
  'folio-uuid>=0.2.7,<0.3.0',
- 'folioclient>=0.43.0,<0.44.0',
+ 'folioclient>=0.50.0rc1,<0.51.0',
+ 'httpx>=0.23.3,<0.24.0',
  'pyaml>=21.10.1,<22.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pyhumps>=3.7.3,<4.0.0',
  'pymarc>=4.2.1,<5.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'requests>=2.28.2,<3.0.0']
+ 'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'folio-migration-tools',
-    'version': '1.7.9rc2',
+    'version': '1.8.0rc1',
     'description': 'A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP',
     'long_description': '# FOLIO Migration Tools\n![example workflow](https://github.com/FOLIO-FSE/MARC21-To-FOLIO/actions/workflows/python-app.yml/badge.svg)[![codecov](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools/branch/main/graph/badge.svg?token=ZQL5ILWWGT)](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools)   [![readthedocs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://folio-migration-tools.readthedocs.io/)\n\nA toolkit that enables you to migrate data over from a legacy ILS system into [FOLIO LSP](https://www.folio.org/)\n\n# What is it good for?\nFOLIO Migration tools enables you to migrate libraries with the most common ILS:s over to FOLIO without data losses or any major data transformation tasks. \nThe tools transforms and loads the data providing you and the library with good actionable logs and data cleaning task lists together with the migrated data.\n\n## What data does it cover?\nFOLIO Migration Tools currently covers the following data sets:\n* Catalog (Inventory and SRS in FOLIO terminology)\n* Circulation transactions (Open loans and requests)\n* Users/Patrons (In FOLIO, these share the same app/database)\n* Courses and Reserves (Course reserves)\n* Organizations (Vendor records)\n* Orders (limited support)\n\n### What additional functionality is on the roadmap?\nThis is the loose roadmap, in order of most likely implementations first\n* ERM-related objects\n* Financial records\n\n### Can I use the tools for ongoing imports and integrations?\nThe tools are primarliy maintained for performing initial data migrations. We recommend that you use native FOLIO functionality for ongoing loads where possible. \nIn theory, these tools can be used for ongoing patron loads from systems like Banner, Workday, or PeopleSoft. But we recommend you to weigh your options carefully before going down this path. \n\n# Contributing\nWant to contribute? Read the [CONTRIBUTING.MD](https://github.com/FOLIO-FSE/folio_migration_tools/blob/main/CONTRIBUTING.md)\n\n# Found an issue?\nReport it on the [Github Issue tracker](https://github.com/FOLIO-FSE/folio_migration_tools/issues)\n\nThe scripts requires a FOLIO tenant with reference data properly set up. The script will throw messages telling what reference data is missing.\n# Installing\nMake sure you are running Python 3.9 or above. \n## 1. Using pip and venv\n### 2.1. Create and activate a [virtual environment](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment)   \n```   \npython -m venv ./.venv     # Creates a virtual env in the current folder\nsource .venv/bin/activate  # Activates the venv    \n```\n### 2. Install using pip: \n```\npython -m pip install folio_migration_tools\n```\n### 3. Test the installation by showing the help pages \n```   \npython -m folio_migration_tools -h\n```    \n\n## 2. Using pipenv\n### 1. Run\n```   \npipenv install folio-migration-tools\n```   \n### 2. Test the installation by showing the help pages\n```  \npipenv run python3 -m folio_migration_tools -h\n```  \n\n# FOLIO migration process\nThis repo plays the main part in a process using a collection of tools. The process itself is documented in more detail, including example configuration files, at [this template repository](https://github.com/FOLIO-FSE/migration_repo_template)\nIn order to perform migrations according to this process, you need the following:\n* An Installation of [FOLIO Migration Tools](https://pypi.org/project/folio-migration-tools/). Installation instructions above.\n* A clone, or a separate repo created from [migration_repo_template](https://github.com/FOLIO-FSE/migration_repo_template)\n* Access to the [Data mapping file creator](https://data-mapping-file-creator.folio.ebsco.com/data_mapping_creation) web tool\n* A FOLIO tenant running the latest or the second latest version of FOLIO\n\n\n\n# Running the scripts\nFor information on syntax, what files are needed and produced by the toolkit, refer to the documentation and example files in the [template repository](https://github.com/FOLIO-FSE/migration_repo_template). We are building out the docs section in this repository as well:[Documentation](https://folio-migration-tools.readthedocs.io/en/latest/)\n¨\n',
     'author': 'Theodor Tolstoy',
     'author_email': 'github.teddes@tolstoy.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FOLIO-FSE/folio_migration_tools',
```

### Comparing `folio_migration_tools-1.7.9rc2/PKG-INFO` & `folio_migration_tools-1.8.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folio-migration-tools
-Version: 1.7.9rc2
+Version: 1.8.0rc1
 Summary: A tool allowing you to migrate data from legacy ILS:s (Library systems) into FOLIO LSP
 Home-page: https://github.com/FOLIO-FSE/folio_migration_tools
 License: MIT
 Keywords: FOLIO,ILS,LSP,Library Systems,MARC21,Library data
 Author: Theodor Tolstoy
 Author-email: github.teddes@tolstoy.se
 Requires-Python: >=3.9,<4.0
@@ -14,21 +14,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: argparse-prompt (>=0.0.5,<0.0.6)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: folio-uuid (>=0.2.7,<0.3.0)
-Requires-Dist: folioclient (>=0.43.0,<0.44.0)
+Requires-Dist: folioclient (>=0.50.0rc1,<0.51.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: pyaml (>=21.10.1,<22.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.3,<4.0.0)
 Requires-Dist: pymarc (>=4.2.1,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/FOLIO-FSE/folio_migration_tools
 Description-Content-Type: text/markdown
 
 # FOLIO Migration Tools
 ![example workflow](https://github.com/FOLIO-FSE/MARC21-To-FOLIO/actions/workflows/python-app.yml/badge.svg)[![codecov](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools/branch/main/graph/badge.svg?token=ZQL5ILWWGT)](https://codecov.io/gh/FOLIO-FSE/folio_migration_tools)   [![readthedocs](https://readthedocs.org/projects/docs/badge/?version=latest)](https://folio-migration-tools.readthedocs.io/)
 
 A toolkit that enables you to migrate data over from a legacy ILS system into [FOLIO LSP](https://www.folio.org/)
```

