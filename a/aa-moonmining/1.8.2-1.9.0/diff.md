# Comparing `tmp/aa-moonmining-1.8.2.tar.gz` & `tmp/aa_moonmining-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-moonmining-1.8.2.tar", last modified: Sun Mar 12 01:09:34 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa-moonmining-1.8.2.tar` & `aa_moonmining-1.9.0.tar`

### file list

```diff
@@ -1,138 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.687550 aa-moonmining-1.8.2/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2021-04-17 14:42:21.000000 aa-moonmining-1.8.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      245 2022-06-18 12:28:04.000000 aa-moonmining-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13777 2023-03-12 01:09:34.687550 aa-moonmining-1.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12847 2023-01-31 14:30:00.000000 aa-moonmining-1.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.659550 aa-moonmining-1.8.2/aa_moonmining.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13777 2023-03-12 01:09:34.000000 aa-moonmining-1.8.2/aa_moonmining.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5324 2023-03-12 01:09:34.000000 aa-moonmining-1.8.2/aa_moonmining.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 01:09:34.000000 aa-moonmining-1.8.2/aa_moonmining.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-03-12 01:09:34.000000 aa-moonmining-1.8.2/aa_moonmining.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-12 01:09:34.000000 aa-moonmining-1.8.2/aa_moonmining.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.663550 aa-moonmining-1.8.2/moonmining/
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11200 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2022-05-02 19:27:04.000000 aa-moonmining-1.8.2/moonmining/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-03-01 14:57:54.000000 aa-moonmining-1.8.2/moonmining/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      882 2022-04-29 20:58:52.000000 aa-moonmining-1.8.2/moonmining/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2022-04-30 19:15:04.000000 aa-moonmining-1.8.2/moonmining/core.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1005 2021-04-08 21:36:41.000000 aa-moonmining-1.8.2/moonmining/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.655550 aa-moonmining-1.8.2/moonmining/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.663550 aa-moonmining-1.8.2/moonmining/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      102 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2022-04-21 18:53:34.000000 aa-moonmining-1.8.2/moonmining/management/commands/moonmining_calculate_all.py
--rw-rw-rw-   0 root         (0) root         (0)     7966 2022-04-21 12:11:35.000000 aa-moonmining-1.8.2/moonmining/management/commands/moonmining_import_moons.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2022-04-21 18:53:34.000000 aa-moonmining-1.8.2/moonmining/management/commands/moonmining_load_eve.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2021-04-27 13:31:36.000000 aa-moonmining-1.8.2/moonmining/management/commands/moonstuff_export_moons.py
--rw-rw-rw-   0 root         (0) root         (0)    14268 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.667550 aa-moonmining-1.8.2/moonmining/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    17813 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2663 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/migrations/0002_add_mining_ledger.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/migrations/0003_mining_ledger_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/migrations/0004_add_permission_moon_ledgers.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/migrations/0005_make_pricing_more_flexible.py
--rw-rw-rw-   0 root         (0) root         (0)     1705 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/migrations/0006_add_labels.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    56187 2022-06-17 10:12:15.000000 aa-moonmining-1.8.2/moonmining/models.py
--rw-rw-rw-   0 root         (0) root         (0)      245 2022-06-17 10:12:15.000000 aa-moonmining-1.8.2/moonmining/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.655550 aa-moonmining-1.8.2/moonmining/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.655550 aa-moonmining-1.8.2/moonmining/static/moonmining/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.667550 aa-moonmining-1.8.2/moonmining/static/moonmining/css/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/css/extractions.css
--rw-rw-rw-   0 root         (0) root         (0)     1306 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/css/moonmining.css
--rw-rw-rw-   0 root         (0) root         (0)      495 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/css/moons.css
--rw-rw-rw-   0 root         (0) root         (0)     2812 2022-04-25 19:46:29.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/css/reports.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.667550 aa-moonmining-1.8.2/moonmining/static/moonmining/img/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.655550 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.655550 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.667550 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5573 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3250 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js
--rw-rw-rw-   0 root         (0) root         (0)     2529 2022-04-25 15:42:22.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js
--rw-rw-rw-   0 root         (0) root         (0)      384 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)      384 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-rw-rw-   0 root         (0) root         (0)   881820 2022-12-13 18:26:47.000000 aa-moonmining-1.8.2/moonmining/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     6423 2023-01-31 14:30:00.000000 aa-moonmining-1.8.2/moonmining/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.655550 aa-moonmining-1.8.2/moonmining/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.667550 aa-moonmining-1.8.2/moonmining/templates/moonmining/
--rw-rw-rw-   0 root         (0) root         (0)      350 2021-04-14 20:53:10.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/_generic_modal_page.html
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-04-25 15:42:22.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/base.html
--rw-rw-rw-   0 root         (0) root         (0)     6204 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/extractions.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.671550 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/
--rw-rw-rw-   0 root         (0) root         (0)      358 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/base.html
--rw-rw-rw-   0 root         (0) root         (0)     1080 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/content_base.html
--rw-rw-rw-   0 root         (0) root         (0)      290 2021-04-14 20:53:10.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/extraction_details.html
--rw-rw-rw-   0 root         (0) root         (0)      315 2021-04-14 20:53:10.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/extraction_ledger.html
--rw-rw-rw-   0 root         (0) root         (0)      247 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/loader_body.html
--rw-rw-rw-   0 root         (0) root         (0)      260 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/moon_details.html
--rw-rw-rw-   0 root         (0) root         (0)      185 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/upload_survey.html
--rw-rw-rw-   0 root         (0) root         (0)     8751 2022-04-25 15:42:22.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/moons.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.675550 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/
--rw-rw-rw-   0 root         (0) root         (0)      175 2021-04-14 20:53:10.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1999 2022-04-28 19:20:34.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_details_head.html
--rw-rw-rw-   0 root         (0) root         (0)      559 2022-04-22 19:18:28.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_details_head_base.html
--rw-rw-rw-   0 root         (0) root         (0)     1851 2022-04-21 12:11:35.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_details_products.html
--rw-rw-rw-   0 root         (0) root         (0)     2246 2021-04-27 13:31:36.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger.html
--rw-rw-rw-   0 root         (0) root         (0)     2141 2021-05-19 19:09:43.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger_characters.html
--rw-rw-rw-   0 root         (0) root         (0)      885 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger_head.html
--rw-rw-rw-   0 root         (0) root         (0)     2582 2022-04-21 18:53:34.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html
--rw-rw-rw-   0 root         (0) root         (0)      859 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extractions_tab.html
--rw-rw-rw-   0 root         (0) root         (0)     3020 2022-04-20 13:19:41.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/global_js.html
--rw-rw-rw-   0 root         (0) root         (0)      624 2021-04-04 20:37:35.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/location.html
--rw-rw-rw-   0 root         (0) root         (0)     2337 2021-05-19 19:16:24.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/menu.html
--rw-rw-rw-   0 root         (0) root         (0)      162 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/moon_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1349 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/moon_details_moon.html
--rw-rw-rw-   0 root         (0) root         (0)     2313 2022-04-28 19:34:11.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/moon_details_products.html
--rw-rw-rw-   0 root         (0) root         (0)     1002 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/moons_tab.html
--rw-rw-rw-   0 root         (0) root         (0)      968 2022-04-25 19:46:29.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html
--rw-rw-rw-   0 root         (0) root         (0)     1066 2022-04-22 18:35:46.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/reports_owned_value_tab.html
--rw-rw-rw-   0 root         (0) root         (0)     1624 2021-04-18 19:55:44.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/reports_user_mining_tab.html
--rw-rw-rw-   0 root         (0) root         (0)      736 2021-11-03 17:21:52.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html
--rw-rw-rw-   0 root         (0) root         (0)      487 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/upload_survey.html
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-04-26 17:34:16.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/value_estimate_legend.html
--rw-rw-rw-   0 root         (0) root         (0)    10057 2022-04-25 19:46:29.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/reports.html
--rw-rw-rw-   0 root         (0) root         (0)     1041 2021-04-14 20:53:10.000000 aa-moonmining-1.8.2/moonmining/templates/moonmining/tests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.675550 aa-moonmining-1.8.2/moonmining/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2022-04-21 18:53:34.000000 aa-moonmining-1.8.2/moonmining/templatetags/moonmining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.675550 aa-moonmining-1.8.2/moonmining/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2022-04-29 23:40:25.000000 aa-moonmining-1.8.2/moonmining/tests/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-03-12 00:42:07.000000 aa-moonmining-1.8.2/moonmining/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2022-04-21 12:11:35.000000 aa-moonmining-1.8.2/moonmining/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     4258 2022-04-28 19:20:34.000000 aa-moonmining-1.8.2/moonmining/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2021-04-06 23:55:07.000000 aa-moonmining-1.8.2/moonmining/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     8354 2022-04-30 19:15:04.000000 aa-moonmining-1.8.2/moonmining/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     7242 2022-04-29 23:40:25.000000 aa-moonmining-1.8.2/moonmining/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    47353 2022-07-21 18:47:00.000000 aa-moonmining-1.8.2/moonmining/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1611 2021-04-14 20:53:10.000000 aa-moonmining-1.8.2/moonmining/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)    27002 2022-05-03 14:13:21.000000 aa-moonmining-1.8.2/moonmining/tests/test_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 01:09:34.687550 aa-moonmining-1.8.2/moonmining/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      173 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3687 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/allianceauth.json
--rw-rw-rw-   0 root         (0) root         (0)     1340 2022-04-29 18:02:47.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/create_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)    29013 2022-04-30 19:15:04.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/esi.json
--rw-rw-rw-   0 root         (0) root         (0)     1373 2021-05-19 18:05:31.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/esi_client_stub.py
--rw-rw-rw-   0 root         (0) root         (0)  1283587 2022-04-29 18:02:47.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/eveuniverse.json
--rw-rw-rw-   0 root         (0) root         (0)    17156 2022-07-21 18:47:00.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2022-05-02 19:27:04.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/generate_many_moons.py
--rw-rw-rw-   0 root         (0) root         (0)    99565 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/generate_moons.json
--rw-rw-rw-   0 root         (0) root         (0)     6596 2022-05-02 19:27:04.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/generate_moons.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/load_allianceauth.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-01-02 17:40:06.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/load_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)    50000 2022-04-25 19:46:29.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/moon_ids.csv
--rw-rw-rw-   0 root         (0) root         (0)      525 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/moon_survey_input_2.txt
--rw-rw-rw-   0 root         (0) root         (0)      335 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/moon_survey_input_3.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2021-04-05 13:43:19.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/moons_for_import.csv
--rw-rw-rw-   0 root         (0) root         (0)      779 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/notification_details.py
--rw-rw-rw-   0 root         (0) root         (0)     4033 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/notifications_full.json
--rw-rw-rw-   0 root         (0) root         (0)      436 2021-04-04 20:01:33.000000 aa-moonmining-1.8.2/moonmining/tests/testdata/survey_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2022-04-25 15:42:22.000000 aa-moonmining-1.8.2/moonmining/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    38790 2022-04-26 17:34:16.000000 aa-moonmining-1.8.2/moonmining/views.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-12 01:09:34.687550 aa-moonmining-1.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1606 2023-01-31 14:30:00.000000 aa-moonmining-1.8.2/setup.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/__init__.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/admin.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/app_settings.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/apps.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/auth_hooks.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/constants.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/core.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/forms.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/helpers.py
+-rw-r--r--   0        0        0    14543 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/managers.py
+-rw-r--r--   0        0        0    57269 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/models.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/providers.py
+-rw-r--r--   0        0        0   881820 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/swagger.json
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tasks.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/urls.py
+-rw-r--r--   0        0        0    39111 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/views.py
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/django.pot
+-rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19962 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    20049 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonmining_calculate_all.py
+-rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonmining_import_moons.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonmining_load_eve.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonstuff_export_moons.py
+-rw-r--r--   0        0        0    17813 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0003_mining_ledger_reports.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0004_add_permission_moon_ledgers.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0005_make_pricing_more_flexible.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0006_add_labels.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0007_add_localization.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/__init__.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/extractions.css
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/global.css
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/moonmining.css
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/moons.css
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/reports.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/_generic_modal_page.html
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/base.html
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/extractions.html
+-rw-r--r--   0        0        0     8913 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/moons.html
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/reports.html
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/tests.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/base.html
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/content_base.html
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/extraction_details.html
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/extraction_ledger.html
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/loader_body.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/moon_details.html
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/upload_survey.html
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details.html
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head.html
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head_base.html
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_products.html
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger.html
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_characters.html
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_head.html
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extractions_tab.html
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/global_js.html
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/location.html
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/menu.html
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details.html
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_moon.html
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_products.html
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moons_tab.html
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_owned_value_tab.html
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_user_mining_tab.html
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/upload_survey.html
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/value_estimate_legend.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templatetags/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templatetags/moonmining.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/helpers.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_admin.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_commands.py
+-rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_core.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_helpers.py
+-rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_integration.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_managers.py
+-rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_models.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_templatetags.py
+-rw-r--r--   0        0        0    27002 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_views.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/allianceauth.json
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/esi.json
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0  1283587 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    17156 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/factories.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/generate_many_moons.py
+-rw-r--r--   0        0        0    99565 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.json
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/load_allianceauth.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moon_ids.csv
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moon_survey_input_2.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moon_survey_input_3.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moons_for_import.csv
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/notification_details.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/notifications_full.json
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/survey_data.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tools/drop_tables.sql
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tools/esi_notes.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/LICENSE
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/README.md
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/PKG-INFO
```

### Comparing `aa-moonmining-1.8.2/LICENSE` & `aa_moonmining-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/PKG-INFO` & `aa_moonmining-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: aa-moonmining
-Version: 1.8.2
+Version: 1.9.0
 Summary: Alliance Auth app for tracking moon extractions and scouting new moons.
-Home-page: https://gitlab.com/ErikKalkoken/aa-moonmining
-Author: Erik Kalkoken
-Author-email: kaloken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-moonmining
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-moonmining
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-moonmining/-/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-moonmining/-/issues
+Author-email: Erik Kalkoken <kaloken87@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.8
+Requires-Python: >=3.8
+Requires-Dist: allianceauth-app-utils>=1.14.2
+Requires-Dist: allianceauth>=3
+Requires-Dist: django-bootstrap-form
+Requires-Dist: django-datatables-view>=1.20
+Requires-Dist: django-eveuniverse>=0.18
+Requires-Dist: django-navhelper
+Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Moon Mining
 
 An Alliance Auth app for tracking moon extractions and scouting new moons.
 
 [![release](https://img.shields.io/pypi/v/aa-moonmining?label=release)](https://pypi.org/project/aa-moonmining/)
 [![python](https://img.shields.io/pypi/pyversions/aa-moonmining)](https://pypi.org/project/aa-moonmining/)
@@ -164,15 +172,15 @@
 > **Note**<br>You can monitor the progress on by looking at how many tasks are running on the dashboard.
 
 ### Step 6 - Load prices from ESI
 
 In order to get the current prices from ESI initially, please run the following command (assuming the name of your Auth installation is `myauth`):
 
 ```bash
-celery -A myauth call moonmining.tasks.run_calculated_properties_update
+python manage.py moonmining_calculate_all
 ```
 
 Please wait until the loading is complete before continuing.
 
 > **Hint**<br>You can monitor the loading progress on the dashboard. As long as the Task Queue shows more than 0 tasks the process is most likely still ongoing.
 
 ### Step 7 - Update EVE Online API Application
@@ -189,30 +197,36 @@
 
 Congratulations! You are now ready to use Moon Mining!
 
 ## User Manual
 
 ### Pricing
 
-The app uses average market prices as basis for all price calculations. Average market prices are same prices that you also see in the Eve client e.g. for the mining ledger or fitting costs. These can be slightly different from Jita prices, since they are represent an average accross all of New Eden, not just Jita / The Forge.
+The app uses average market prices as basis for all price calculations. Average market prices are same prices that you also see in the Eve client e.g. for the mining ledger or fitting costs. These can be slightly different from Jita prices, since they are represent an average across all of New Eden, not just Jita / The Forge.
 
 The calculation of ore prices can be done in two different ways.
 
 ### Default ore pricing
 
-The default ore pricing uses the average market prices directly to calculate ore prices. This is the same approach that the Eve client uses in the minning ledger or when scheduling an extraction. So the main benefit of this approach that you will see the same prices in-game and in the app.
+The default ore pricing uses the average market prices directly to calculate ore prices. This is the same approach that the Eve client uses in the mining ledger or when scheduling an extraction. So the main benefit of this approach that you will see the same prices in-game and in the app.
 
 ### Reprocess ore pricing
 
 The disadvantage of this approach is that average market prices for ores are not always accurate. Ores are rarely sold directly on the market, instead most people of refining their ores and selling the refined materials instead. This is because they have they are much smaller in volume making them easier to transport. The total value of the refined materials is also often higher then the value of the ore.
 
-Therefore you can also chose to use refined ore pricing. This will give you more occurate prices, but the values will be very different from what you may be used to see in the Eve client. For this approach the app calculates the price for a unit of ore as the sum total of it's refined materials. For the materials again the average market price is used.
+Therefore you can also chose to use refined ore pricing. This will give you more accurate prices, but the values will be very different from what you may be used to see in the Eve client. For this approach the app calculates the price for a unit of ore as the sum total of it's refined materials. For the materials again the average market price is used.
 
 Please see the settings `MOONMINING_USE_REPROCESS_PRICING` and `MOONMINING_REPROCESSING_YIELD` for configuring the ore pricing approach.
 
+After you changed the settings for price calculation, you please restart your AA services so that the changes to your settings become effective. Next please run the following command to recalculate all prices:
+
+```bash
+python manage.py moonmining_calculate_all
+```
+
 >**Note**<br>You can see the current prices used for all ores in the app in the ore prices report.
 
 ### Labels
 
 To help with organizing your moons you can label them. For example you might have some of your moons rented out to a third party. Just add a label "Rented out to X" to those moons and the moons and related extractions will show that label allowing you to quickly recognize which are related to your renters.
 
 Labels are created on the admin site under Label and can then be assigned under Moon.
@@ -271,9 +285,7 @@
 
 - Q: How are the prices and values of ores calculated?
 - A: All ore prices are **average prices** (not Jita prices), which are the current average price of an item accross all of New Eden and the same that the in-game client is showing, e.g. for price estimates when scheduling an extraction.
 
 ## History
 
 This project started as a fork from [aa-moonstuff](https://gitlab.com/colcrunch/aa-moonstuff) in 2019, but as diverged heavily since then through two major iterations. The first iteration was called Moon Planner and used internally. It had a very different data model build upon [allianceauth-evesde](https://gitlab.com/ErikKalkoken/allianceauth-evesde). The current version is the second iteration and is build upon [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse). Nevertheless, we like to take the opportunity to thank @colcrunch for providing a great starting point with moonstuff.
-
-
```

### Comparing `aa-moonmining-1.8.2/README.md` & `aa_moonmining-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 > **Note**<br>You can monitor the progress on by looking at how many tasks are running on the dashboard.
 
 ### Step 6 - Load prices from ESI
 
 In order to get the current prices from ESI initially, please run the following command (assuming the name of your Auth installation is `myauth`):
 
 ```bash
-celery -A myauth call moonmining.tasks.run_calculated_properties_update
+python manage.py moonmining_calculate_all
 ```
 
 Please wait until the loading is complete before continuing.
 
 > **Hint**<br>You can monitor the loading progress on the dashboard. As long as the Task Queue shows more than 0 tasks the process is most likely still ongoing.
 
 ### Step 7 - Update EVE Online API Application
@@ -164,30 +164,36 @@
 
 Congratulations! You are now ready to use Moon Mining!
 
 ## User Manual
 
 ### Pricing
 
-The app uses average market prices as basis for all price calculations. Average market prices are same prices that you also see in the Eve client e.g. for the mining ledger or fitting costs. These can be slightly different from Jita prices, since they are represent an average accross all of New Eden, not just Jita / The Forge.
+The app uses average market prices as basis for all price calculations. Average market prices are same prices that you also see in the Eve client e.g. for the mining ledger or fitting costs. These can be slightly different from Jita prices, since they are represent an average across all of New Eden, not just Jita / The Forge.
 
 The calculation of ore prices can be done in two different ways.
 
 ### Default ore pricing
 
-The default ore pricing uses the average market prices directly to calculate ore prices. This is the same approach that the Eve client uses in the minning ledger or when scheduling an extraction. So the main benefit of this approach that you will see the same prices in-game and in the app.
+The default ore pricing uses the average market prices directly to calculate ore prices. This is the same approach that the Eve client uses in the mining ledger or when scheduling an extraction. So the main benefit of this approach that you will see the same prices in-game and in the app.
 
 ### Reprocess ore pricing
 
 The disadvantage of this approach is that average market prices for ores are not always accurate. Ores are rarely sold directly on the market, instead most people of refining their ores and selling the refined materials instead. This is because they have they are much smaller in volume making them easier to transport. The total value of the refined materials is also often higher then the value of the ore.
 
-Therefore you can also chose to use refined ore pricing. This will give you more occurate prices, but the values will be very different from what you may be used to see in the Eve client. For this approach the app calculates the price for a unit of ore as the sum total of it's refined materials. For the materials again the average market price is used.
+Therefore you can also chose to use refined ore pricing. This will give you more accurate prices, but the values will be very different from what you may be used to see in the Eve client. For this approach the app calculates the price for a unit of ore as the sum total of it's refined materials. For the materials again the average market price is used.
 
 Please see the settings `MOONMINING_USE_REPROCESS_PRICING` and `MOONMINING_REPROCESSING_YIELD` for configuring the ore pricing approach.
 
+After you changed the settings for price calculation, you please restart your AA services so that the changes to your settings become effective. Next please run the following command to recalculate all prices:
+
+```bash
+python manage.py moonmining_calculate_all
+```
+
 >**Note**<br>You can see the current prices used for all ores in the app in the ore prices report.
 
 ### Labels
 
 To help with organizing your moons you can label them. For example you might have some of your moons rented out to a third party. Just add a label "Rented out to X" to those moons and the moons and related extractions will show that label allowing you to quickly recognize which are related to your renters.
 
 Labels are created on the admin site under Label and can then be assigned under Moon.
```

### Comparing `aa-moonmining-1.8.2/moonmining/admin.py` & `aa_moonmining-1.9.0/moonmining/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.contrib import admin
 from django.core.exceptions import ObjectDoesNotExist
+from django.utils.translation import gettext_lazy as _
 
 from . import tasks
 from .models import (
     EveOreType,
     EveOreTypeExtras,
     Extraction,
     ExtractionProduct,
@@ -36,15 +37,15 @@
         qs = super().get_queryset(request)
         return qs.select_related("extras", "eve_group")
 
     @admin.display(ordering="extras__current_price")
     def _current_price(self, obj):
         try:
             return f"{obj.extras.current_price:,.2f}"
-        except ObjectDoesNotExist:
+        except (ObjectDoesNotExist, TypeError):
             return None
 
     @admin.display(ordering="eve_group__name")
     def _group(self, obj):
         return str(obj.eve_group)
 
     @admin.display(ordering="extras__pricing_method")
@@ -70,22 +71,25 @@
     list_display = ("chunk_arrival_at", "status", "_owner", "refinery", "_ledger")
     ordering = ("-chunk_arrival_at",)
     list_filter = ("chunk_arrival_at", "status", "refinery__owner", "refinery")
     search_fields = ("refinery__moon__eve_moon__name",)
     inlines = [ExtractionProductAdmin]
     actions = ["update_calculated_properties"]
 
-    @admin.display(description="Update calculated properties for selected extrations.")
+    @admin.display(
+        description=_("Update calculated properties for selected extractions.")
+    )
     def update_calculated_properties(self, request, queryset):
         num = 0
         for obj in queryset:
             tasks.update_extraction_calculated_properties.delay(extraction_pk=obj.pk)
             num += 1
         self.message_user(
-            request, f"Started updating calculated properties for {num} extractions."
+            request,
+            _("Started updating calculated properties for %d extractions." % num),
         )
 
     def _owner(self, obj):
         return obj.refinery.owner
 
     @admin.display(boolean=True)
     def _ledger(self, obj):
@@ -131,16 +135,16 @@
 
 class MoonHasRefineryFilter(admin.SimpleListFilter):
     title = "has refinery"
     parameter_name = "has_refinery"
 
     def lookups(self, request, model_admin):
         return (
-            ("yes", "Yes"),
-            ("no", "No"),
+            ("yes", _("Yes")),
+            ("no", _("No")),
         )
 
     def queryset(self, request, queryset):
         """Return the filtered queryset"""
         if self.value() == "yes":
             return queryset.filter(refinery__isnull=False)
         elif self.value() == "no":
@@ -246,35 +250,35 @@
     def _refinery(self, obj) -> str:
         return obj.refinery.name
 
     @admin.display(ordering="refinery__owner__name")
     def _owner(self, obj) -> str:
         return obj.refinery.owner.name
 
-    @admin.display(description="Update calculated properties for selected moons.")
+    @admin.display(description=_("Update calculated properties for selected moons."))
     def update_calculated_properties(self, request, queryset):
         num = 0
         for obj in queryset:
             tasks.update_moon_calculated_properties.delay(moon_pk=obj.pk)
             num += 1
         self.message_user(
-            request, f"Started updating calculated properties for {num} moons."
+            request, _("Started updating calculated properties for %d moons." % num)
         )
 
     @admin.display(
-        description=("Update products from latest extraction for selected moons.")
+        description=_("Update products from latest extraction for selected moons.")
     )
     def update_products_from_latest_extraction(self, request, queryset):
         num = 0
         for obj in queryset:
             tasks.update_moon_products_from_latest_extraction.delay(moon_pk=obj.pk)
             num += 1
         self.message_user(
             request,
-            f"Started updating products from latest extractions for {num} moons.",
+            _("Started updating products from latest extractions for %d moons." % num),
         )
 
 
 @admin.register(Notification)
 class NotificationAdmin(admin.ModelAdmin):
     list_display = (
         "notification_id",
@@ -313,27 +317,27 @@
     )
     actions = ["update_owner"]
 
     @admin.display(ordering="corporation__alliance__alliance_name")
     def _alliance(self, obj):
         return obj.corporation.alliance
 
-    @admin.display(description="Update selected owners from ESI")
+    @admin.display(description=_("Update selected owners from ESI"))
     def update_owner(self, request, queryset):
         for obj in queryset:
             tasks.update_owner.delay(obj.pk)
-            text = f"Started updating owner: {obj}. "
+            text = _("Started updating owner %s." % obj)
             self.message_user(request, text)
 
     def has_add_permission(self, request):
         return False
 
     def get_readonly_fields(self, request, obj=None):
         if obj:  # editing an existing object
-            return self.readonly_fields + (
+            return tuple(self.readonly_fields) + (
                 "corporation",
                 "character_ownership",
                 "last_update_at",
                 "last_update_ok",
             )
         return self.readonly_fields
 
@@ -364,13 +368,15 @@
         return False
 
     def has_add_permission(self, request):
         return False
 
     actions = ["update_mining_ledger"]
 
-    @admin.display(description="Update mining ledger for selected refineries from ESI")
+    @admin.display(
+        description=_("Update mining ledger for selected refineries from ESI")
+    )
     def update_mining_ledger(self, request, queryset):
         for obj in queryset:
             tasks.update_mining_ledger_for_refinery.delay(obj.id)
-            text = f"Started updating mining ledger: {obj}. "
+            text = _("Started updating mining ledger %s." % obj)
             self.message_user(request, text)
```

### Comparing `aa-moonmining-1.8.2/moonmining/app_settings.py` & `aa_moonmining-1.9.0/moonmining/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/auth_hooks.py` & `aa_moonmining-1.9.0/moonmining/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/constants.py` & `aa_moonmining-1.9.0/moonmining/constants.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/core.py` & `aa_moonmining-1.9.0/moonmining/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime as dt
 from dataclasses import dataclass
 from enum import IntEnum, auto
-from typing import List
+from typing import List, Optional
 
 from . import helpers
 
 
 @dataclass
 class CalculatedExtraction:
     """An extraction calculated from moon mining notifications."""
@@ -15,23 +15,23 @@
         CANCELED = auto()
         READY = auto()
         COMPLETED = auto()
         UNDEFINED = auto()
 
     refinery_id: int
     status: Status
-    auto_fracture_at: dt.datetime = None
-    canceled_at: dt.datetime = None
-    canceled_by: int = None
-    chunk_arrival_at: dt.datetime = None
-    fractured_at: dt.datetime = None
-    fractured_by: int = None
-    products: List["CalculatedExtractionProduct"] = None
-    started_at: dt.datetime = None
-    started_by: int = None
+    auto_fracture_at: Optional[dt.datetime] = None
+    canceled_at: Optional[dt.datetime] = None
+    canceled_by: Optional[int] = None
+    chunk_arrival_at: Optional[dt.datetime] = None
+    fractured_at: Optional[dt.datetime] = None
+    fractured_by: Optional[int] = None
+    products: Optional[List["CalculatedExtractionProduct"]] = None
+    started_at: Optional[dt.datetime] = None
+    started_by: Optional[int] = None
 
     def __post_init__(self):
         self.refinery_id = int(self.refinery_id)
         self.status = self.Status(self.status)
         if self.started_at:
             self.started_at = helpers.round_seconds(self.started_at)
         if self.chunk_arrival_at:
@@ -58,14 +58,16 @@
     ) -> List["CalculatedMoonProduct"]:
         """List of products with estimated amounts."""
         duration_in_days = self.duration.total_seconds() / (60 * 60 * 24)
         if duration_in_days <= 0:
             raise ValueError("Can not estimate products without duration.")
         max_volume = duration_in_days * volume_per_day
         correction_factor = max(1, self.total_volume() / max_volume)
+        if not self.products:
+            return []
         products = [
             CalculatedMoonProduct(
                 ore_type_id=product.ore_type_id,
                 amount=product.calculated_share(duration_in_days, volume_per_day)
                 / correction_factor,
             )
             for product in self.products
```

### Comparing `aa-moonmining-1.8.2/moonmining/helpers.py` & `aa_moonmining-1.9.0/moonmining/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return {k: elem.value for k, elem in cls.__members__.items()}
 
 
 class HttpResponseUnauthorized(HttpResponse):
     status_code = 401
 
 
-def eveentity_get_or_create_esi_safe(id):
+def eve_entity_get_or_create_esi_safe(id):
     """Get or Create EveEntity with given ID safely and return it. Else return None."""
     if id:
         try:
             entity, _ = EveEntity.objects.get_or_create_esi(id=id)
             return entity
         except OSError:
             pass
```

### Comparing `aa-moonmining-1.8.2/moonmining/management/commands/moonmining_calculate_all.py` & `aa_moonmining-1.9.0/moonmining/management/commands/moonmining_calculate_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def handle(self, *args, **options):
         moon_count = Moon.objects.count()
         extractions_count = Extraction.objects.count()
         self.stdout.write(
             f"Updating calculated properties for {moon_count} moons "
             f"and {extractions_count} extractions. This can take a while."
         )
-        self.stdout.write()
+        self.stdout.write("")
         user_input = get_input("Are you sure you want to proceed? (Y/n)?")
 
         if user_input.lower() != "n":
             tasks.run_calculated_properties_update.delay()
             self.stdout.write(self.style.SUCCESS("Update started."))
         else:
             self.stdout.write(self.style.WARNING("Aborted"))
```

### Comparing `aa-moonmining-1.8.2/moonmining/management/commands/moonmining_import_moons.py` & `aa_moonmining-1.9.0/moonmining/management/commands/moonmining_import_moons.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/management/commands/moonmining_load_eve.py` & `aa_moonmining-1.9.0/moonmining/management/commands/moonmining_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/management/commands/moonstuff_export_moons.py` & `aa_moonmining-1.9.0/moonmining/management/commands/moonstuff_export_moons.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/managers.py` & `aa_moonmining-1.9.0/moonmining/managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from collections import namedtuple
-from typing import Tuple
+from typing import List, Optional, Tuple
 
 from django.contrib.auth.models import User
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models, transaction
 from django.db.models import ExpressionWrapper, F, FloatField, IntegerField, Sum
 from django.db.models.functions import Coalesce
 from django.utils.timezone import now
+from django.utils.translation import gettext_lazy as _
 from eveuniverse.managers import EveTypeManager
 from eveuniverse.models import EveMoon
 
 from allianceauth.notifications import notify
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from . import __title__
 from .app_settings import (
     MOONMINING_REPROCESSING_YIELD,
     MOONMINING_USE_REPROCESS_PRICING,
 )
 from .constants import EveCategoryId
 from .core import CalculatedExtraction
-from .helpers import eveentity_get_or_create_esi_safe
+from .helpers import eve_entity_get_or_create_esi_safe
 
 MAX_THREAD_WORKERS = 20
 BULK_BATCH_SIZE = 500
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 SurveyProcessResult = namedtuple(
     "SurveyProcessResult", ["moon_name", "success", "error_name"]
@@ -39,15 +40,15 @@
             super()
             .get_queryset()
             .select_related("eve_group")
             .filter(published=True)
             .filter(eve_group__eve_category_id=EveCategoryId.ASTEROID)
         )
 
-    def update_current_prices(self, use_process_pricing: bool = None):
+    def update_current_prices(self, use_process_pricing: Optional[bool] = None):
         """Update current prices for all ores."""
         from .models import EveOreTypeExtras
 
         if use_process_pricing is None:
             use_process_pricing = MOONMINING_USE_REPROCESS_PRICING
 
         for obj in self.filter(published=True).select_related("market_price"):
@@ -99,15 +100,15 @@
             "refinery__owner__corporation",
             "refinery__owner__corporation__alliance",
             "label",
         )
 
 
 class MoonManagerBase(models.Manager):
-    def update_moons_from_survey(self, scans: str, user: User = None) -> bool:
+    def update_moons_from_survey(self, scans: str, user: Optional[User] = None) -> bool:
         """Update moons from survey input.
 
         Args:
             scans: raw text input from user containing moon survey data
             user: (optional) user who submitted the data
         """
         surveys, error_name = self._parse_scans(scans)
@@ -133,66 +134,68 @@
                 line = line.strip("\r").split("\t")
                 lines_.append(line)
             lines = lines_
 
             # Find all groups of scans.
             if len(lines[0]) == 0 or lines[0][0] == "Moon":
                 lines = lines[1:]
-            sublists = []
+            sub_lists = []
             for line in lines:
                 # Find the lines that start a scan
                 if line[0] == "":
                     pass
                 else:
-                    sublists.append(lines.index(line))
+                    sub_lists.append(lines.index(line))
 
             # Separate out individual surveys
-            for i in range(len(sublists)):
+            for i in range(len(sub_lists)):
                 # The First List
                 if i == 0:
-                    if i + 2 > len(sublists):
-                        surveys.append(lines[sublists[i] :])
+                    if i + 2 > len(sub_lists):
+                        surveys.append(lines[sub_lists[i] :])
                     else:
-                        surveys.append(lines[sublists[i] : sublists[i + 1]])
+                        surveys.append(lines[sub_lists[i] : sub_lists[i + 1]])
                 else:
-                    if i + 2 > len(sublists):
-                        surveys.append(lines[sublists[i] :])
+                    if i + 2 > len(sub_lists):
+                        surveys.append(lines[sub_lists[i] :])
                     else:
-                        surveys.append(lines[sublists[i] : sublists[i + 1]])
+                        surveys.append(lines[sub_lists[i] : sub_lists[i + 1]])
 
-        except Exception as ex:
+        except (TypeError, ValueError, KeyError, AttributeError, IndexError) as ex:
             logger.warning(
                 "An issue occurred while trying to parse the surveys", exc_info=True
             )
             error_name = type(ex).__name__
 
         else:
             error_name = ""
         return surveys, error_name
 
-    def _process_surveys(self, surveys: list, user: User) -> Tuple[list, bool]:
+    def _process_surveys(
+        self, surveys: list, user: Optional[User]
+    ) -> Tuple[List[SurveyProcessResult], bool]:
         from .models import EveOreType, MoonProduct
 
         overall_success = True
         process_results = list()
         for survey in surveys:
             moon_name = ""
             try:
                 moon_name = survey[0][0]
                 moon_id = survey[1][6]
-                eve_moon, _ = EveMoon.objects.get_or_create_esi(id=moon_id)
-                moon, _ = self.get_or_create(eve_moon=eve_moon)
+                eve_moon = EveMoon.objects.get_or_create_esi(id=moon_id)[0]
+                moon = self.get_or_create(eve_moon=eve_moon)[0]
                 moon_products = list()
                 survey = survey[1:]
                 for product_data in survey:
                     # Trim off the empty index at the front
                     product_data = product_data[1:]
-                    ore_type, _ = EveOreType.objects.get_or_create_esi(
-                        id=product_data[2]
-                    )
+                    ore_type = EveOreType.objects.get_or_create_esi(id=product_data[2])[
+                        0
+                    ]
                     moon_products.append(
                         MoonProduct(
                             moon=moon, amount=product_data[1], ore_type=ore_type
                         )
                     )
                 moon.update_products(moon_products, updated_by=user)
                 logger.info("Added moon survey for %s", moon.name)
@@ -214,15 +217,18 @@
                     moon_name=moon_name, success=success, error_name=error_name
                 )
             )
         return process_results, overall_success
 
     @staticmethod
     def _send_survey_process_report_to_user(
-        process_results: list, error_name: str, user: User, success: bool
+        process_results: Optional[List[SurveyProcessResult]],
+        error_name: str,
+        user: User,
+        success: bool,
     ) -> bool:
         message = "We have completed processing your moon survey input:\n\n"
         if process_results:
             for num, process_result in enumerate(process_results):
                 moon_name = process_result.moon_name
                 if process_result.success:
                     status = "OK"
@@ -235,16 +241,17 @@
                     num + 1, moon_name, status, error_name
                 )
         else:
             message += "\nProcessing failed"
 
         notify(
             user=user,
-            title="Moon survey input processing results: {}".format(
-                "OK" if success else "FAILED"
+            title=_(
+                "Moon survey input processing results: %s"
+                % ("OK" if success else "FAILED")
             ),
             message=message,
             level="success" if success else "danger",
         )
         return success
 
 
@@ -316,39 +323,39 @@
             return False
 
         needs_update = False
         if calculated.canceled_at and not extraction.canceled_at:
             extraction.canceled_at = calculated.canceled_at
             needs_update = True
         if calculated.canceled_by and not extraction.canceled_by:
-            extraction.canceled_by = eveentity_get_or_create_esi_safe(
+            extraction.canceled_by = eve_entity_get_or_create_esi_safe(
                 calculated.canceled_by
             )
             needs_update = True
         if calculated.canceled_by and not extraction.canceled_by:
-            extraction.canceled_by = eveentity_get_or_create_esi_safe(
+            extraction.canceled_by = eve_entity_get_or_create_esi_safe(
                 calculated.canceled_by
             )
             needs_update = True
         if calculated.fractured_by and not extraction.fractured_by:
-            extraction.fractured_by = eveentity_get_or_create_esi_safe(
+            extraction.fractured_by = eve_entity_get_or_create_esi_safe(
                 calculated.fractured_by
             )
             needs_update = True
         if calculated.fractured_at and not extraction.fractured_at:
             extraction.fractured_at = calculated.fractured_at
             needs_update = True
         if self.model.Status.from_calculated(calculated) != extraction.status:
             extraction.status = self.model.Status.from_calculated(calculated)
             needs_update = True
             status_changed = True
         else:
             status_changed = False
         if calculated.started_by and not extraction.started_by:
-            extraction.started_by = eveentity_get_or_create_esi_safe(
+            extraction.started_by = eve_entity_get_or_create_esi_safe(
                 calculated.started_by
             )
             needs_update = True
         updated = False
         if needs_update:
             extraction.save()
             updated = True
```

### Comparing `aa-moonmining-1.8.2/moonmining/migrations/0001_initial.py` & `aa_moonmining-1.9.0/moonmining/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/migrations/0002_add_mining_ledger.py` & `aa_moonmining-1.9.0/moonmining/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/migrations/0003_mining_ledger_reports.py` & `aa_moonmining-1.9.0/moonmining/migrations/0003_mining_ledger_reports.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/migrations/0004_add_permission_moon_ledgers.py` & `aa_moonmining-1.9.0/moonmining/migrations/0004_add_permission_moon_ledgers.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/migrations/0005_make_pricing_more_flexible.py` & `aa_moonmining-1.9.0/moonmining/migrations/0005_make_pricing_more_flexible.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/migrations/0006_add_labels.py` & `aa_moonmining-1.9.0/moonmining/migrations/0006_add_labels.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/models.py` & `aa_moonmining-1.9.0/moonmining/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models, transaction
 from django.db.models import F, Sum, Value
 from django.db.models.functions import Coalesce
 from django.utils.functional import cached_property, classproperty
 from django.utils.html import format_html
 from django.utils.timezone import now
+from django.utils.translation import gettext_lazy as _
 from esi.models import Token
 from eveuniverse.models import EveEntity, EveMoon, EveSolarSystem, EveType
 
 from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.eveonline.models import EveCorporationInfo
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.allianceauth import notify_admins_throttled
@@ -85,45 +86,45 @@
         }
 
 
 class OreRarityClass(models.IntegerChoices):
     """Rarity class of an ore"""
 
     NONE = 0, ""
-    R4 = 4, "R 4"
-    R8 = 8, "R 8"
-    R16 = 16, "R16"
-    R32 = 32, "R32"
-    R64 = 64, "R64"
+    R4 = 4, _("R 4")
+    R8 = 8, _("R 8")
+    R16 = 16, _("R16")
+    R32 = 32, _("R32")
+    R64 = 64, _("R64")
 
     @property
     def bootstrap_tag_html(self) -> str:
         map_rarity_to_type = {
             self.R4: BootstrapStyle.PRIMARY,
             self.R8: BootstrapStyle.INFO,
             self.R16: BootstrapStyle.SUCCESS,
             self.R32: BootstrapStyle.WARNING,
             self.R64: BootstrapStyle.DANGER,
         }
         try:
             return bootstrap_label_html(
-                f"R{self.value}", label=map_rarity_to_type[self.value]
+                f"R{self.value}", label=map_rarity_to_type[self].value
             )
         except KeyError:
             return ""
 
     @classmethod
     def from_eve_group_id(cls, eve_group_id: int) -> "OreRarityClass":
         """Create object from eve group ID"""
         map_group_2_rarity = {
-            EveGroupId.UBIQUITOUS_MOON_ASTEROIDS: cls.R4,
-            EveGroupId.COMMON_MOON_ASTEROIDS: cls.R8,
-            EveGroupId.UNCOMMON_MOON_ASTEROIDS: cls.R16,
-            EveGroupId.RARE_MOON_ASTEROIDS: cls.R32,
-            EveGroupId.EXCEPTIONAL_MOON_ASTEROIDS: cls.R64,
+            EveGroupId.UBIQUITOUS_MOON_ASTEROIDS.value: cls.R4,
+            EveGroupId.COMMON_MOON_ASTEROIDS.value: cls.R8,
+            EveGroupId.UNCOMMON_MOON_ASTEROIDS.value: cls.R16,
+            EveGroupId.RARE_MOON_ASTEROIDS.value: cls.R32,
+            EveGroupId.EXCEPTIONAL_MOON_ASTEROIDS.value: cls.R64,
         }
         try:
             return map_group_2_rarity[eve_group_id]
         except KeyError:
             return cls.NONE
 
     @classmethod
@@ -131,28 +132,28 @@
         """Create object from eve type"""
         return cls.from_eve_group_id(eve_type.eve_group_id)
 
 
 class OreQualityClass(models.TextChoices):
     """Quality class of an ore"""
 
-    UNDEFINED = "UN", "(undefined)"
-    REGULAR = "RE", "regular"
-    IMPROVED = "IM", "improved"
-    EXCELLENT = "EX", "excellent"
+    UNDEFINED = "UN", _("undefined")
+    REGULAR = "RE", _("regular")
+    IMPROVED = "IM", _("improved")
+    EXCELLENT = "EX", _("excellent")
 
     @property
     def bootstrap_tag_html(self) -> str:
         """Return bootstrap tag."""
         map_quality_to_label_def = {
             self.IMPROVED: {"text": "+15%", "label": BootstrapStyle.SUCCESS},
             self.EXCELLENT: {"text": "+100%", "label": BootstrapStyle.WARNING},
         }
         try:
-            label_def = map_quality_to_label_def[self.value]
+            label_def = map_quality_to_label_def[self]
             return bootstrap_label_html(label_def["text"], label=label_def["label"])
         except KeyError:
             return ""
 
     @classmethod
     def from_eve_type(cls, eve_type: EveType) -> "OreQualityClass":
         """Create object from given eve type."""
@@ -175,26 +176,22 @@
 
 class EveOreType(EveType):
     """Subset of EveType for all ore types.
 
     Ensures TYPE_MATERIALS and DOGMAS is always enabled and allows adding methods to types.
     """
 
-    URL_PROFILE_TYPE = "https://www.kalkoken.org/apps/eveitems/"
-
     class Meta:
         proxy = True
+        verbose_name = _("ore type")
+        verbose_name_plural = _("ore types")
 
     objects = EveOreTypeManger()
 
     @property
-    def profile_url(self) -> str:
-        return f"{self.URL_PROFILE_TYPE}?typeId={self.id}"
-
-    @property
     def icon_url_32(self) -> str:
         return self.icon_url(32)
 
     @property
     def rarity_class(self) -> OreRarityClass:
         return OreRarityClass.from_eve_type(self)
 
@@ -204,23 +201,25 @@
 
     @cached_property
     def price(self) -> float:
         """Return calculated price estimate in ISK per unit."""
         result = self.extras.current_price
         return result if result is not None else 0.0
 
-    def price_by_volume(self, volume: int) -> float:
+    def price_by_volume(self, volume: int) -> Optional[float]:
         """Return calculated price estimate in ISK for volume in m3."""
-        return self.price_by_units(volume / self.volume)
+        return self.price_by_units(int(volume // self.volume)) if self.volume else None
 
     def price_by_units(self, units: int) -> float:
         """Return calculated price estimate in ISK for units."""
         return self.price * units
 
-    def calc_refined_value_per_unit(self, reprocessing_yield: float = None) -> float:
+    def calc_refined_value_per_unit(
+        self, reprocessing_yield: Optional[float] = None
+    ) -> float:
         """Calculate the refined total value per unit and return it."""
         if not reprocessing_yield:
             reprocessing_yield = MOONMINING_REPROCESSING_YIELD
         units = 10000
         r_units = units / 100
         value = 0
         for type_material in self.materials.select_related(
@@ -245,68 +244,72 @@
         return enabled_sections
 
 
 class EveOreTypeExtras(models.Model):
     """Extra fields for an EveOreType, e.g. for pricing calculations."""
 
     class PricingMethod(models.TextChoices):
-        UNKNOWN = "UN", "Unknown"
-        EVE_CLIENT = "EC", "Eve client"
-        REPROCESSED_MATERIALS = "RP", "Reprocessed materials"
+        UNKNOWN = "UN", _("Undefined")
+        EVE_CLIENT = "EC", _("Eve client")
+        REPROCESSED_MATERIALS = "RP", _("Reprocessed materials")
 
     ore_type = models.OneToOneField(
         EveOreType, on_delete=models.CASCADE, related_name="extras"
     )
     current_price = models.FloatField(
         default=None,
         null=True,
-        help_text="price used all price calculations with this type",
+        help_text=_("Price used by all price calculations with this type"),
     )
     pricing_method = models.CharField(
         max_length=2, choices=PricingMethod.choices, default=PricingMethod.UNKNOWN
     )
 
+    class Meta:
+        verbose_name = _("ore type extra")
+        verbose_name_plural = _("ore type extras")
+
     def __str__(self) -> str:
         return str(self.ore_type)
 
 
 class Extraction(models.Model):
     """A mining extraction."""
 
     class Status(models.TextChoices):
-        STARTED = "ST", "started"  # has been started
-        CANCELED = "CN", "canceled"  # has been canceled
-        READY = "RD", "ready"  # has finished extraction and is ready to be fractured
-        COMPLETED = "CP", "completed"  # has been fractured
-        UNDEFINED = "UN", "undefined"  # unclear status
+        STARTED = "ST", _("started")  # has been started
+        CANCELED = "CN", _("canceled")  # has been canceled
+        READY = "RD", _("ready")  # has finished extraction and is ready to be fractured
+        COMPLETED = "CP", _("completed")  # has been fractured
+        UNDEFINED = "UN", _("undefined")  # unclear status
 
         @property
         def bootstrap_tag_html(self) -> str:
             map_to_type = {
                 self.STARTED: BootstrapStyle.SUCCESS,
                 self.CANCELED: BootstrapStyle.DANGER,
                 self.READY: BootstrapStyle.WARNING,
                 self.COMPLETED: BootstrapStyle.PRIMARY,
                 self.UNDEFINED: "",
             }
             try:
-                return bootstrap_label_html(self.label, label=map_to_type[self.value])
+                return bootstrap_label_html(self.label, label=map_to_type[self].value)
             except KeyError:
                 return ""
 
         @property
-        def to_notification_type(self) -> str:
+        def to_notification_type(self) -> NotificationType:
             map_to_type = {
                 self.STARTED: NotificationType.MOONMINING_EXTRACTION_STARTED,
                 self.CANCELED: NotificationType.MOONMINING_EXTRACTION_CANCELLED,
                 self.READY: NotificationType.MOONMINING_EXTRACTION_FINISHED,
                 self.COMPLETED: NotificationType.MOONMINING_LASER_FIRED,
             }
             try:
-                return map_to_type[self.value]
+                return map_to_type[self]
             except KeyError:
                 raise ValueError("Invalid status for notification type") from None
 
         @classproperty
         def considered_active(cls):
             return [cls.STARTED, cls.READY]
 
@@ -328,76 +331,79 @@
             except KeyError:
                 return cls.UNDEFINED
 
     # PK
     refinery = models.ForeignKey(
         "Refinery", on_delete=models.CASCADE, related_name="extractions"
     )
-    started_at = models.DateTimeField(help_text="when this extraction was started")
-    # TODO: Add db_index
+    started_at = models.DateTimeField(
+        db_index=True, help_text=_("When this extraction was started")
+    )
     # normal properties
     auto_fracture_at = models.DateTimeField(
-        help_text="when this extraction will be automatically fractured",
+        help_text=_("When this extraction will be automatically fractured"),
     )
     canceled_at = models.DateTimeField(
-        null=True, default=None, help_text="when this extraction was canceled"
+        null=True, default=None, help_text=_("When this extraction was canceled")
     )
     canceled_by = models.ForeignKey(
         EveEntity,
         on_delete=models.SET_DEFAULT,
         null=True,
         default=None,
         related_name="+",
-        help_text="Eve character who canceled this extraction",
+        help_text=_("Eve character who canceled this extraction"),
     )
     chunk_arrival_at = models.DateTimeField(
-        db_index=True, help_text="when this extraction is ready to be fractured"
+        db_index=True, help_text=_("When this extraction is ready to be fractured")
     )
     fractured_at = models.DateTimeField(
-        null=True, default=None, help_text="when this extraction was fractured"
+        null=True, default=None, help_text=_("When this extraction was fractured")
     )
     fractured_by = models.ForeignKey(
         EveEntity,
         on_delete=models.SET_DEFAULT,
         null=True,
         default=None,
         related_name="+",
-        help_text="Eve character who fractured this extraction (if any)",
+        help_text=_("Eve character who fractured this extraction (if any)"),
     )
     is_jackpot = models.BooleanField(
         default=None,
         null=True,
-        help_text="Whether this is a jackpot extraction (calculated)",
+        help_text=_("Whether this is a jackpot extraction (calculated)"),
     )
     started_by = models.ForeignKey(
         EveEntity,
         on_delete=models.SET_DEFAULT,
         null=True,
         default=None,
         related_name="+",
-        help_text="Eve character who started this extraction",
+        help_text=_("Eve character who started this extraction"),
     )
     status = models.CharField(
         max_length=2, choices=Status.choices, default=Status.UNDEFINED, db_index=True
     )
     value = models.FloatField(
         null=True,
         default=None,
         validators=[MinValueValidator(0.0)],
-        help_text="Estimated value of this extraction (calculated)",
+        help_text=_("Estimated value of this extraction (calculated)"),
     )
 
     objects = ExtractionManager()
 
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["refinery", "started_at"], name="functional_pk_extraction"
             )
         ]
+        verbose_name = _("extraction")
+        verbose_name_plural = _("extractions")
 
     def __str__(self) -> str:
         return f"{self.refinery} - {self.started_at} - {self.status}"
 
     @property
     def duration(self) -> dt.timedelta:
         """Duration of this extraction."""
@@ -451,28 +457,29 @@
             * F("volume")
             / F("ore_type__volume"),
             output_field=models.FloatField(),
         )
 
     def calc_is_jackpot(self) -> Optional[bool]:
         """Calculate if extraction is jackpot and return result.
-        Return None if extraction has no products"""
+        Return None if extraction has no products.
+        """
         try:
             products_qualities = [
                 product.ore_type.quality_class == OreQualityClass.EXCELLENT
                 for product in self.products.select_related("ore_type").all()
             ]
         except (ObjectDoesNotExist, AttributeError):
             return None
         else:
             if not products_qualities:
                 return None
             return all(products_qualities)
 
-    def update_calculated_properties(self) -> float:
+    def update_calculated_properties(self) -> None:
         """Update calculated properties for this extraction."""
         self.value = self.calc_value()
         self.is_jackpot = self.calc_is_jackpot()
         self.save()
 
     def to_calculated_extraction(self) -> CalculatedExtraction:
         """Generate a calculated extraction from this extraction."""
@@ -538,48 +545,54 @@
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["extraction", "ore_type"],
                 name="functional_pk_extractionproduct",
             )
         ]
+        verbose_name = _("extraction product")
+        verbose_name_plural = _("extractions products")
 
     def __str__(self) -> str:
         return f"{self.extraction} - {self.ore_type}"
 
 
 class Label(models.Model):
     """A custom label for structuring moons."""
 
     class Style(models.TextChoices):
-        DARK_BLUE = "primary", "dark blue"
-        GREEN = "success", "green"
-        GREY = "default", "grey"
-        LIGHT_BLUE = "info", "light blue"
-        ORANGE = "warning", "orange"
-        RED = "danger", "red"
+        DARK_BLUE = "primary", _("dark blue")
+        GREEN = "success", _("green")
+        GREY = "default", _("grey")
+        LIGHT_BLUE = "info", _("light blue")
+        ORANGE = "warning", _("orange")
+        RED = "danger", _("red")
 
         @property
         def bootstrap_style(self) -> str:
             map_to_type = {
                 self.DARK_BLUE: BootstrapStyle.PRIMARY,
                 self.GREEN: BootstrapStyle.SUCCESS,
                 self.LIGHT_BLUE: BootstrapStyle.INFO,
                 self.ORANGE: BootstrapStyle.WARNING,
                 self.RED: BootstrapStyle.DANGER,
             }
             try:
-                return map_to_type[self.value]
+                return map_to_type[self].value
             except KeyError:
                 return BootstrapStyle.DEFAULT
 
     description = models.TextField(default="", blank=True)
     name = models.CharField(max_length=100, unique=True)
     style = models.CharField(max_length=16, choices=Style.choices, default=Style.GREY)
 
+    class Meta:
+        verbose_name = _("label")
+        verbose_name_plural = _("labels")
+
     def __str__(self) -> str:
         return self.name
 
     @property
     def tag_html(self) -> str:
         label_style = self.Style(self.style).bootstrap_style
         return bootstrap_label_html(self.name, label=label_style)
@@ -605,32 +618,32 @@
 class MiningLedgerRecord(models.Model):
     """A recorded mining activity in the vicinity of a refinery."""
 
     refinery = models.ForeignKey(
         "Refinery",
         on_delete=models.CASCADE,
         related_name="mining_ledger",
-        help_text="Refinery this mining activity was observed at",
+        help_text=_("Refinery this mining activity was observed at"),
     )
-    day = models.DateField(help_text="last_updated in ESI", db_index=True)
+    day = models.DateField(db_index=True, help_text=_("last_updated in ESI"))
     character = models.ForeignKey(
         EveEntity,
         on_delete=models.CASCADE,
         related_name="+",
-        help_text="character that did the mining",
+        help_text=_("character that did the mining"),
     )
     ore_type = models.ForeignKey(
         EveOreType, on_delete=models.CASCADE, related_name="mining_ledger"
     )
     # regular
     corporation = models.ForeignKey(
         EveEntity,
         on_delete=models.CASCADE,
         related_name="+",
-        help_text="corporation of the character at time data was recorded",
+        help_text=_("corporation of the character at time data was recorded"),
     )
     quantity = models.PositiveBigIntegerField()
     user = models.ForeignKey(
         User,
         on_delete=models.CASCADE,
         default=None,
         null=True,
@@ -642,54 +655,59 @@
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["refinery", "day", "character", "ore_type"],
                 name="functional_pk_mining_activity",
             )
         ]
+        verbose_name = _("ledger record")
+        verbose_name_plural = _("ledger records")
 
 
 class Moon(models.Model):
     """Known moon through either survey data or anchored refinery.
 
-    "Head" model for many of the other models
+    "Head" model for many of the other models.
     """
 
     # pk
     eve_moon = models.OneToOneField(
-        EveMoon, on_delete=models.CASCADE, primary_key=True, related_name="known_moon"
+        EveMoon, on_delete=models.CASCADE, primary_key=True, related_name="+"
     )
-    # TODO: Remove "related_name"
     # regular
     label = models.ForeignKey(
         Label, on_delete=models.SET_DEFAULT, default=None, null=True
     )
     products_updated_at = models.DateTimeField(
-        null=True, default=None, help_text="Time the last moon survey was uploaded"
+        null=True, default=None, help_text=_("Time the last moon survey was uploaded")
     )
     products_updated_by = models.ForeignKey(
         User,
         on_delete=models.SET_DEFAULT,
         null=True,
         default=None,
-        help_text="User who uploaded the last moon survey",
+        help_text=_("User who uploaded the last moon survey"),
     )
     rarity_class = models.PositiveIntegerField(
         choices=OreRarityClass.choices, default=OreRarityClass.NONE
     )
     value = models.FloatField(
         null=True,
         default=None,
         validators=[MinValueValidator(0.0)],
         db_index=True,
-        help_text="Calculated value estimate",
+        help_text=_("Calculated value estimate"),
     )
 
     objects = MoonManager()
 
+    class Meta:
+        verbose_name = _("moon")
+        verbose_name_plural = _("moons")
+
     def __str__(self):
         return self.name
 
     @property
     def name(self) -> str:
         return self.eve_moon.name.replace("Moon ", "")
 
@@ -762,15 +780,15 @@
     def update_calculated_properties(self):
         """Update all calculated properties for this moon."""
         self.value = self.calc_value()
         self.rarity_class = self.calc_rarity_class()
         self.save()
 
     def update_products(
-        self, moon_products: List["MoonProduct"], updated_by: User = None
+        self, moon_products: List["MoonProduct"], updated_by: Optional[User] = None
     ) -> None:
         """Update products of this moon."""
         with transaction.atomic():
             self.products.all().delete()
             MoonProduct.objects.bulk_create(moon_products, batch_size=500)
         self.products_updated_at = now()
         self.products_updated_by = updated_by
@@ -800,29 +818,29 @@
             ]
             self.update_products(moon_products)
             return True
         return False
 
     def update_products_from_latest_extraction(
         self, overwrite_survey: bool = False
-    ) -> bool:
+    ) -> Optional[bool]:
         try:
             extraction = self.refinery.extractions.order_by("-started_at").first()
         except ObjectDoesNotExist:
             return None
         if not extraction:
             return None
         calculated_extraction = extraction.to_calculated_extraction()
         return self.update_products_from_calculated_extraction(
             calculated_extraction, overwrite_survey=overwrite_survey
         )
 
 
 class MoonProduct(models.Model):
-    """A product of a moon, i.e. a specifc ore."""
+    """A product of a moon, i.e. a specific ore."""
 
     moon = models.ForeignKey(Moon, on_delete=models.CASCADE, related_name="products")
     ore_type = models.ForeignKey(EveOreType, on_delete=models.CASCADE, related_name="+")
 
     amount = models.FloatField(
         validators=[MinValueValidator(0.0), MaxValueValidator(1.0)]
     )
@@ -832,14 +850,16 @@
 
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["moon", "ore_type"], name="functional_pk_moonproduct"
             )
         ]
+        verbose_name = _("moon product")
+        verbose_name_plural = _("moons products")
 
     @property
     def amount_percent(self) -> float:
         """Return the amount of this product as percent"""
         return self.amount * 100
 
 
@@ -847,56 +867,58 @@
     """An EVE Online notification about structures."""
 
     # pk
     owner = models.ForeignKey(
         "Owner",
         on_delete=models.CASCADE,
         related_name="notifications",
-        help_text="Corporation that received this notification",
+        help_text=_("Corporation that received this notification"),
     )
     notification_id = models.PositiveBigIntegerField(verbose_name="id")
     # regular
     created = models.DateTimeField(
         null=True,
         default=None,
-        help_text="Date when this notification was first received from ESI",
+        help_text=_("Date when this notification was first received from ESI"),
     )
     details = models.JSONField(default=dict)
     notif_type = models.CharField(
         max_length=100,
         default="",
         db_index=True,
         verbose_name="type",
-        help_text="type of this notification as reported by ESI",
+        help_text=_("type of this notification as reported by ESI"),
     )
     is_read = models.BooleanField(
         null=True,
         default=None,
-        help_text="True when this notification has read in the eve client",
+        help_text=_("True when this notification has read in the eve client"),
     )
     last_updated = models.DateTimeField(
-        help_text="Date when this notification has last been updated from ESI"
+        help_text=_("Date when this notification has last been updated from ESI")
     )
     sender = models.ForeignKey(
         EveEntity, on_delete=models.CASCADE, null=True, default=None, related_name="+"
     )
     timestamp = models.DateTimeField(db_index=True)
 
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["owner", "notification_id"], name="functional_pk_notification"
             )
         ]
+        verbose_name = _("notification")
+        verbose_name_plural = _("notifications")
 
     def __str__(self) -> str:
         return str(self.notification_id)
 
     def __repr__(self) -> str:
-        return "%s(notification_id=%d, owner='%s', notif_type='%s')" % (
+        return "%s(notification_id=%s, owner='%s', notif_type='%s')" % (
             self.__class__.__name__,
             self.notification_id,
             self.owner,
             self.notif_type,
         )
 
     def to_calculated_extraction(self) -> CalculatedExtraction:
@@ -953,41 +975,41 @@
 class Owner(models.Model):
     """A EVE Online corporation owning refineries."""
 
     ESI_SERVICE_NAME_MOON_DRILLING = "Moon Drilling"
 
     # pk
     corporation = models.OneToOneField(
-        EveCorporationInfo,
-        on_delete=models.CASCADE,
-        primary_key=True,
-        related_name="mining_corporation",
+        EveCorporationInfo, on_delete=models.CASCADE, primary_key=True, related_name="+"
     )
-    # TODO: remove "mining_corporation"
     # regular
     character_ownership = models.ForeignKey(
         CharacterOwnership,
         on_delete=models.SET_DEFAULT,
         default=None,
         null=True,
         related_name="+",
-        help_text="character used to sync this corporation from ESI",
+        help_text=_("Character used to sync this corporation from ESI"),
     )
     is_enabled = models.BooleanField(
         default=True,
         db_index=True,
-        help_text="disabled corporations are excluded from the update process",
+        help_text=_("Disabled corporations are excluded from the update process"),
     )
     last_update_at = models.DateTimeField(
-        null=True, default=None, help_text="time of last successful update"
+        null=True, default=None, help_text=_("Time of last successful update")
     )
     last_update_ok = models.BooleanField(
-        null=True, default=None, help_text="True if the last update was successful"
+        null=True, default=None, help_text=_("True if the last update was successful")
     )
 
+    class Meta:
+        verbose_name = _("owner")
+        verbose_name_plural = _("owners")
+
     def __str__(self):
         return self.name
 
     @property
     def name(self) -> str:
         alliance_ticker_str = (
             f" [{self.corporation.alliance.alliance_ticker}]"
@@ -1026,15 +1048,15 @@
             raise Token.DoesNotExist(f"{self}: No valid token found.")
         return token
 
     def update_refineries_from_esi(self):
         """Update all refineries from ESI."""
         logger.info("%s: Updating refineries...", self)
         refineries = self._fetch_refineries_from_esi()
-        for structure_id, _ in refineries.items():
+        for structure_id in refineries.keys():
             try:
                 self._update_or_create_refinery_from_esi(structure_id)
             except OSError as exc:
                 exc_name = type(exc).__name__
                 msg = (
                     f"{self}: Failed to fetch refinery with ID {structure_id} from ESI"
                 )
@@ -1094,20 +1116,20 @@
                 "owner": self,
             },
         )
         if not refinery.moon:
             refinery.update_moon_from_structure_info(structure_info)
         return True
 
-    def fetch_notifications_from_esi(self) -> bool:
-        """fetches notification for the current owners and proceses them"""
+    def fetch_notifications_from_esi(self) -> None:
+        """fetches notification for the current owners and process them"""
         notifications = self._fetch_moon_notifications_from_esi()
         self._store_notifications(notifications)
 
-    def _fetch_moon_notifications_from_esi(self) -> dict:
+    def _fetch_moon_notifications_from_esi(self) -> List[dict]:
         """Fetch all notifications from ESI for current owner."""
         logger.info("%s: Fetching notifications from ESI...", self)
         all_notifications = (
             esi.client.Character.get_characters_character_id_notifications(
                 character_id=self.character_ownership.character.character_id,
                 token=self.fetch_token().valid_access_token(),
             ).results()
@@ -1148,15 +1170,15 @@
             text = notification["text"] if "text" in notification else None
             is_read = notification["is_read"] if "is_read" in notification else None
             new_notification_objects.append(
                 Notification(
                     notification_id=notification["notification_id"],
                     owner=self,
                     created=now(),
-                    details=yaml.safe_load(text),
+                    details=yaml.safe_load(text) if text else {},
                     is_read=is_read,
                     last_updated=now(),
                     # at least one type has a trailing white space
                     # which we need to remove
                     notif_type=notification["type"].strip(),
                     sender=sender,
                     timestamp=notification["timestamp"],
@@ -1227,17 +1249,16 @@
         for refinery in self.refineries.all():
             updated_count = 0
             extraction = None
             notifications_for_refinery = self.notifications.filter(
                 details__structureID=refinery.id
             )
             if not refinery.moon and notifications_for_refinery.exists():
-                """Update the refinery's moon from notification in case
-                it was not found by nearest_celestial.
-                """
+                # Update the refinery's moon from notification in case
+                # it was not found by nearest_celestial.
                 notif = notifications_for_refinery.first()
                 refinery.update_moon_from_eve_id(notif.details["moonID"])
             for notif in notifications_for_refinery.order_by("timestamp"):
                 if notif.notif_type == NotificationType.MOONMINING_EXTRACTION_STARTED:
                     extraction = notif.to_calculated_extraction()
                     if refinery.moon.update_products_from_calculated_extraction(
                         extraction,
@@ -1357,34 +1378,38 @@
     eve_type = models.ForeignKey(EveType, on_delete=models.CASCADE, related_name="+")
     moon = models.OneToOneField(
         Moon,
         on_delete=models.SET_DEFAULT,
         default=None,
         null=True,
         related_name="refinery",
-        help_text="The moon this refinery is anchored at (if any)",
+        help_text=_("The moon this refinery is anchored at (if any)"),
     )
     name = models.CharField(max_length=150, db_index=True)
     owner = models.ForeignKey(
         Owner,
         on_delete=models.CASCADE,
         related_name="refineries",
-        help_text="Corporation that owns this refinery",
+        help_text=_("Corporation that owns this refinery"),
     )
     ledger_last_update_at = models.DateTimeField(
-        null=True, default=None, help_text="last successful update of mining ledger"
+        null=True, default=None, help_text=_("last successful update of mining ledger")
     )
     ledger_last_update_ok = models.BooleanField(
         null=True,
         default=None,
-        help_text="True if the last update of the mining ledger was successful",
+        help_text=_("True if the last update of the mining ledger was successful"),
     )
 
     objects = RefineryManager()
 
+    class Meta:
+        verbose_name = _("refinery")
+        verbose_name_plural = _("refineries")
+
     def __str__(self):
         return self.name
 
     def name_html(self) -> str:
         return format_html("{}<br>{}", self.name, self.owner.name)
 
     def update_moon_from_structure_info(self, structure_info: dict) -> bool:
@@ -1429,15 +1454,15 @@
             token=self.owner.fetch_token().valid_access_token(),
         ).results()
         logger.info(
             "%s: Received %d mining observer records from ESI", self, len(records)
         )
         # preload all missing ore types
         EveOreType.objects.bulk_get_or_create_esi(
-            ids={record["type_id"] for record in records}
+            ids=[record["type_id"] for record in records]
         )
         character_2_user = {
             obj[0]: obj[1]
             for obj in CharacterOwnership.objects.values_list(
                 "character__character_id",
                 "user_id",
             )
```

### Comparing `aa-moonmining-1.8.2/moonmining/static/moonmining/css/global.css` & `aa_moonmining-1.9.0/moonmining/static/moonmining/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/static/moonmining/css/moonmining.css` & `aa_moonmining-1.9.0/moonmining/static/moonmining/css/moonmining.css`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif` & `aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif` & `aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js` & `aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js` & `aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/swagger.json` & `aa_moonmining-1.9.0/moonmining/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tasks.py` & `aa_moonmining-1.9.0/moonmining/tasks.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/base.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/base.html`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/extractions.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/extractions.html`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     <div class="panel panel-default panel-tabs">
         <div class="panel-body">
             <div class="tab-content">
                 {% include "moonmining/partials/extractions_tab.html" with category=ExtractionsCategory.UPCOMING %}
                 {% include "moonmining/partials/extractions_tab.html" with category=ExtractionsCategory.PAST %}
             </div>
             {% include 'moonmining/partials/value_estimate_legend.html' %}
-            <p class="text-muted">All times displayed are EVE/UTC • Extractions will be shown on the upcoming tab until {{ stale_hours }} hours after their ready time.</p>
+            <p class="text-muted">
+                {% blocktranslate %}All times displayed are EVE/UTC{% endblocktranslate %} •
+                {% blocktranslate %}Extractions will be shown on the upcoming tab until {{ stale_hours }} hours after their ready time.{% endblocktranslate %}
+            </p>
         </div>
     </div>
 
     <!-- Modals -->
     {% include "moonmining/modals/base.html" with modal_id="modalMoonDetails" modal_content_id="modalMoonDetailsContent" %}
     {% include "moonmining/modals/base.html" with modal_id="modalExtractionDetails" modal_content_id="modalExtractionDetailsContent" %}
     {% include "moonmining/modals/base.html" with modal_id="modalExtractionLedger" modal_content_id="modalExtractionLedgerContent" modal_size="modal-xl" %}
@@ -81,39 +84,39 @@
                     { "orderable": false, "targets": [ 7 ] },
                     { "visible": false, "targets": [ 8, 9, 10, 11, 12, 13, 14 ] },
                 ],
                 filterDropDown: {
                     columns: [
                         {
                             idx: 9,
-                            title: "Alliance"
+                            title: "{% translate 'Alliance' %}"
                         },
                         {
                             idx: 8,
-                            title: "Corporation"
+                            title: "{% translate 'Corporation' %}"
                         },
                         {
                             idx: 12,
-                            title: "Region"
+                            title: "{% translate 'Region' %}"
                         },
                         {
                             idx: 13,
-                            title: "Constellation"
+                            title: "{% translate 'Constellation' %}"
                         },
                         {
                             idx: 14,
-                            title: "Rarity"
+                            title: "{% translate 'Rarity' %}"
                         },
                         {
                             idx: 11,
-                            title: "Moon"
+                            title: "{% translate 'Moon' %}"
                         },
                         {
                             idx: 10,
-                            title: "Status"
+                            title: "{% translate 'Status' %}"
                         }
                     ],
                     bootstrap: true,
                     autoSize: false
                 },
                 footerCallback: function (row, data, start, end, display) {
                     var api = this.api(), data;
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/modals/content_base.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/content_base.html`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 
         <div class="modal-body">
             {% include modal_body_url %}
         </div>
 
         <div class="modal-footer">
             {% if new_page_url %}
-                <a class="btn btn-default pull-left" href="{{ new_page_url }}?new_page=yes" target="_blank" title="Open in new tab">
+                <a  class="btn btn-default pull-left"
+                    href="{{ new_page_url }}?new_page=yes"
+                    target="_blank"
+                    title="{% translate 'Open in new tab' %}">
                     <i class="far fa-window-restore"></i>
                 </a>
             {% endif %}
             <button type="button" class="btn btn-default" data-dismiss="modal">
                 {% translate 'Close' %}
             </button>
         </div>
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/moons.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/moons.html`

 * *Files 3% similar despite different names*

```diff
@@ -100,55 +100,55 @@
                     { "orderable": false, "targets": [ 4, 6 ] },
                     { "visible": false, "targets": [ 7, 8, 9, 10, 11, 12, 13, 14, 15 ] },
                 ],
                 filterDropDown: {
                     columns: [
                         {
                             idx: 10,
-                            title: "Alliance",
+                            title: "{% translate 'Alliance' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 9,
-                            title: "Corporation",
+                            title: "{% translate 'Corporation' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 15,
-                            title: "Region",
+                            title: "{% translate 'Region' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 13,
-                            title: "Constellation",
+                            title: "{% translate 'Constellation' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 7,
-                            title: "System",
+                            title: "{% translate 'System' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 11,
-                            title: "Rarity",
+                            title: "{% translate 'Rarity' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 14,
-                            title: "Label",
+                            title: "{% translate 'Label' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 8,
-                            title: "Refinery?",
+                            title: "{% translate 'Refinery?' %}",
                             maxWidth: "10em"
                         },
                         {
                             idx: 12,
-                            title: "Extraction?",
+                            title: "{% translate 'Extraction?' %}",
                             maxWidth: "10em"
                         }
                     ],
                     bootstrap: true,
                     autoSize: false
                 }
             };
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_details_head.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head.html`

 * *Files 26% similar despite different names*

```diff
@@ -5,50 +5,52 @@
 <div class="row">
     <div class="col-md-6">
         {% include 'moonmining/partials/extraction_details_head_base.html' %}
     </div>
 
     <div class="col-md-6">
         <dl class="dl-horizontal">
-            <dt>Status:</dt>
+            <dt>{% translate 'Status:' %}</dt>
             <dd>{{ extraction.status_enum.bootstrap_tag_html }}</dd>
 
-            <dt>Started:</dt>
+            <dt>{% translate 'Started:' %}</dt>
             <dd>
                 <span title="{{ extraction.started_at|naturaltime }}">
                     {{ extraction.started_at|datetime }}
                 </span>
                     by {{ extraction.started_by|default:"?" }}
             </dd>
 
             {% if extraction.status == extraction.Status.CANCELED %}
-                <dt>Canceled:</dt>
+                <dt>{% translate 'Canceled:' %}</dt>
                 <dd>
                     <span title="{{ extraction.canceled_at|naturaltime|default:'?' }}">
                         {{ extraction.canceled_at|datetime|default:"?" }}
                     </span> by {{ extraction.canceled_by|default:"?" }}
                 </dd>
             {% endif %}
 
-            <dt>Chunk arrival:</dt>
+            <dt>{% translate 'Chunk arrival:' %}</dt>
             <dd>
                 {% if extraction.status == extraction.Status.CANCELED %}<s>{% endif %}
                 <span title="{{ extraction.chunk_arrival_at|naturaltime }}">
                     {{ extraction.chunk_arrival_at|datetime }}
                 </span>
                 {% if extraction.status == extraction.Status.CANCELED %}</s>{% endif %}
             </dd>
 
-            <dt>Auto Fracture:</dt>
+            <dt>{% translate 'Auto Fracture:' %}</dt>
             <dd>
                 {% if extraction.status == extraction.Status.CANCELED %}<s>{% endif %}
                 <span title="{{ extraction.auto_fracture_at|naturaltime }}">
                     {{ extraction.auto_fracture_at|datetime }}
                 </span>
                 {% if extraction.status == extraction.Status.CANCELED %}</s>{% endif %}
             </dd>
 
-            <dt>Duration:</dt>
-            <dd>{{ extraction.duration_in_days|floatformat }} days</dd>
+            <dt>{% translate 'Duration:' %}</dt>
+            <dd>
+                {% blocktranslate with duration_days=extraction.duration_in_days|floatformat %}{{ duration_days }} days{% endblocktranslate %}
+            </dd>
         </dl>
     </div>
 </div>
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_details_head_base.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head_base.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% load i18n %}
 {% load humanize %}
 {% load moonmining %}
 
 <dl class="dl-horizontal">
-    <dt>Refinery:</dt>
+    <dt>{% translate 'Refinery:' %}</dt>
     <dd>{{ extraction.refinery.name }}</dd>
 
-    <dt>Company:</dt>
+    <dt>{% translate 'Company:' %}</dt>
     <dd>{{ extraction.refinery.owner.name }}</dd>
 
-    <dt>Moon:</dt>
+    <dt>{% translate 'Moon:' %}</dt>
     <dd>{{ extraction.refinery.moon }}</dd>
 
-    <dt>Location:</dt>
+    <dt>{% translate 'Location:' %}</dt>
     <dd>
         {% include "moonmining/partials/location.html" with eve_solar_system=extraction.refinery.moon.eve_moon.eve_planet.eve_solar_system %}
     </dd>
 
-    <dt>Labels:</dt>
+    <dt>{% translate 'Labels:' %}</dt>
     <dd>{{ extraction.refinery.moon.labels_html }}</dd>
 </dl>
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_details_products.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_products.html`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 <div class="table-responsive">
     {% if extraction.products_sorted|length > 0 %}
         <table class="table table-striped" id="table_extraction_details">
             <thead>
                 <tr>
                     <th></th>
-                    <th>Ore Type</th>
-                    <th>Rarity</th>
-                    <th>Est. Unit Price</th>
-                    <th>Volume</th>
-                    <th>Est. Total Price. *</th>
+                    <th>{% translate 'Ore Type' %}</th>
+                    <th>{% translate 'Rarity' %}</th>
+                    <th>{% translate 'Est. Unit Price' %}</th>
+                    <th>{% translate 'Volume' %}</th>
+                    <th>{% translate 'Est. Total Price' %}</th>
                 </tr>
             </thead>
             <tbody>
                 {% for product in extraction.products_sorted %}
                     <tr>
                         <td><img src="{{ product.ore_type.icon_url_32 }}"/></td>
                         <td>
@@ -30,19 +30,19 @@
                         <td>{{ product.total_price|formatisk:"b"|default:""}}</td>
                     </tr>
                 {% endfor %}
             </tbody>
             <tfoot>
                 <tr>
                     <th></th>
-                    <th>TOTAL</th>
+                    <th>{% translate 'Total' %}</th>
                     <th></th>
                     <th></th>
                     <th>{{ extraction.volume|floatformat:"0"|intcomma }}</th>
                     <th>{{ extraction.value|formatisk:"b"|default:""}}</th>
                 </tr>
             </tfoot>
         </table>
     {% else %}
-        <p class="text-muted">No data.</p>
+        <p class="text-muted">{% translate 'No data.' %}</p>
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% load i18n %} {% load humanize %} {% load moonmining %}
 {% if extraction.products_sorted|length > 0 %}
-                             Ore Type              Rarity                                           Est. Unit Price                     Volume                         Est. Total Price. *
+                             {% translate 'Ore     {% translate 'Rarity' %}                         {% translate 'Est. Unit Price' %}   {% translate 'Volume' %}       {% translate 'Est. Total
+                             Type' %}                                                                                                                                  Price' %}
 [{                           {                     {                                                {                                                                  {
 {                            {                     {                                                {                                   {{ product.volume|floatformat: {
 product.ore_type.icon_url_32 product.ore_type.name product.ore_type.rarity_class.bootstrap_tag_html product.ore_type.price|floatformat: "0"|intcomma }}                product.total_price|formatisk:
 }}]                          }}                    }}                                               "0"|intcomma|default:"?" }}                                        "b"|default:""}}
                                                                                                                                         {
-                             TOTAL                                                                                                      {                              {{ extraction.value|formatisk:
-                                                                                                                                        extraction.volume|floatformat: "b"|default:""}}
+                             {% translate 'Total'                                                                                       {                              {{ extraction.value|formatisk:
+                             %}                                                                                                         extraction.volume|floatformat: "b"|default:""}}
                                                                                                                                         "0"|intcomma }}
 {% else %}
-No data.
+{% translate 'No data.' %}
 {% endif %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+{% load i18n %}
+
 {% include 'moonmining/partials/extraction_ledger_head.html' %}
 <!-- Nav tabs -->
 <ul class="nav nav-tabs" role="tablist">
-    <li role="presentation" class="active"><a href="#ledger" aria-controls="ledger" role="tab" data-toggle="tab">Ledger</a></li>
-    <li role="presentation"><a href="#characters" aria-controls="characters" role="tab" data-toggle="tab">Totals by character</a></li>
+    <li role="presentation" class="active"><a href="#ledger" aria-controls="ledger" role="tab" data-toggle="tab">
+        {% translate 'Ledger' %}
+    </a></li>
+    <li role="presentation"><a href="#characters" aria-controls="characters" role="tab" data-toggle="tab">
+        {% translate 'Totals by character' %}
+    </a></li>
 </ul>
 <!-- Tab panes -->
 <div class="panel panel-default panel-tabs">
     <div class="panel-body">
         <div class="tab-content">
             <div role="tabpanel" class="tab-pane active" id="ledger">
                 {% include 'moonmining/partials/extraction_ledger_ledger.html' %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger_characters.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_characters.html`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 {% load moonmining %}
 
 <div class="table-responsive">
     {% if character_totals|length > 0 %}
         <table class="table table-striped table-width-fix" id="table-ledger-character-totals">
             <thead>
                 <tr>
-                    <th>Character</th>
-                    <th>Main</th>
-                    <th>Corporation</th>
-                    <th class="text-right">Volume</th>
-                    <th class="text-right">Price</th>
-                    <th class="text-right">% Total Volume</th>
-                    <th class="text-right">% Total Price</th>
+                    <th>{% translate 'Character' %}</th>
+                    <th>{% translate 'Main' %}</th>
+                    <th>{% translate 'Corporation' %}</th>
+                    <th class="text-right">{% translate 'Volume' %}</th>
+                    <th class="text-right">{% translate 'Price' %}</th>
+                    <th class="text-right">{% translate '% Total Volume' %}</th>
+                    <th class="text-right">{% translate '% Total Price' %}</th>
                 </tr>
             </thead>
             <tbody>
                 {% for record in character_totals %}
                     <tr>
                         <td>{{ record.character_name }}</td>
                         <td>{{ record.main_name|default:"" }}</td>
@@ -32,21 +32,21 @@
                         <td class="text-right">{{ record.character_percent_volume }}</td>
                         <td class="text-right">{{ record.character_percent_value }}</td>
                     </tr>
                 {% endfor %}
             </tbody>
             <tfoot>
                 <tr class="info">
-                    <th>TOTALS</th>
+                    <th>{% translate 'Total' %}</th>
                     <th></th>
                     <th></th>
                     <th class="text-right">{{ total_volume|intcomma }}</th>
                     <th class="text-right">{{ total_value|formatisk:"m" }}</th>
                     <th></th>
                     <th></th>
                 </tr>
             </tfoot>
         </table>
     {% else %}
-        <p class="text-muted">No data.</p>
+        <p class="text-muted">{% translate 'No data.' %}</p>
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
 {% load i18n %} {% load static %} {% load humanize %} {% load moonmining %}
 {% if character_totals|length > 0 %}
-Character             Main                      Corporation                      Volume                                 Price                                   % Total Volume                  % Total Price
+{% translate          {% translate 'Main' %}    {% translate 'Corporation' %}    {% translate 'Volume' %}               {% translate 'Price' %}                 {% translate '% Total Volume'   {% translate '% Total Price'
+'Character' %}                                                                                                                                                  %}                              %}
 {                     {                         {                                {                                      {                                       {                               {
 {                     {                         {                                {                                      {                                       {                               {
 record.character_name record.main_name|default: record.corporation_name|default: record.character_total_volume|intcomma record.character_total_price|formatisk: record.character_percent_volume record.character_percent_value
 }}                    "" }}                     "" }}                            }}                                     "m" }}                                  }}                              }}
-TOTALS                                                                           {{ total_volume|intcomma }}            {{ total_value|formatisk:"m" }}
+{% translate 'Total'                                                             {{ total_volume|intcomma }}            {{ total_value|formatisk:"m" }}
+%}
 {% else %}
-No data.
+{% translate 'No data.' %}
 {% endif %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger_head.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_head.html`

 * *Files 12% similar despite different names*

```diff
@@ -15,16 +15,20 @@
                 {% if extraction.status == extraction.Status.CANCELED %}<s>{% endif %}
                 <span title="{{ extraction.chunk_arrival_at|naturaltime }}">
                     {{ extraction.chunk_arrival_at|datetime }}
                 </span>
                 {% if extraction.status == extraction.Status.CANCELED %}</s>{% endif %}
             </dd>
 
-            <dt>Total mined volume:</dt>
-            <dd>{{ total_volume|intword }} m3</dd>
+            <dt>{% translate 'Total mined volume:' %}</dt>
+            <dd>
+                {% blocktranslate with volume=total_volume|intword %}{{ volume }} m3{% endblocktranslate %}
+            </dd>
 
-            <dt>Total mined value:</dt>
-            <dd>{{ total_value|intword }} ISK</dd>
+            <dt>{% translate 'Total mined value:' %}</dt>
+            <dd>
+                {% blocktranslate with value=total_value|intword %}{{ value }} ISK{% endblocktranslate %}
+            </dd>
         </dl>
     </div>
 
 </div>
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html`

 * *Files 24% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 {% load moonmining %}
 
 <div class="table-responsive">
     {% if ledger|length > 0 %}
         <table class="table table-striped table-width-fix" id="table-ledger-ledger">
             <thead>
                 <tr>
-                    <th>Day</th>
-                    <th>Main</th>
-                    <th>Character</th>
-                    <th>Corporation</th>
-                    <th>Ore</th>
-                    <th class="text-right">Total Volume</th>
-                    <th class="text-right">Unit Price</th>
-                    <th class="text-right">Quantity</th>
-                    <th class="text-right">Total Price</th>
+                    <th>{% translate 'Day' %}</th>
+                    <th>{% translate 'Main' %}</th>
+                    <th>{% translate 'Character' %}</th>
+                    <th>{% translate 'Corporation' %}</th>
+                    <th>{% translate 'Ore' %}</th>
+                    <th class="text-right">{% translate 'Total Volume' %}</th>
+                    <th class="text-right">{% translate 'Unit Price' %}</th>
+                    <th class="text-right">{% translate 'Quantity' %}</th>
+                    <th class="text-right">{% translate 'Total Price' %}</th>
                 </tr>
             </thead>
             <tbody>
                 {% for record in ledger %}
                     <tr>
                         <td>{{ record.day }}</td>
                         <td>{{ record.user.profile.main_character.character_name }}</td>
@@ -40,23 +40,23 @@
                             {{ record.total_price|formatisk:"m" }}
                         </td>
                     </tr>
                 {% endfor %}
             </tbody>
             <tfoot>
                 <tr class="info">
-                    <th>TOTALS</th>
+                    <th>{% translate 'Total' %}</th>
                     <th></th>
                     <th></th>
                     <th></th>
                     <th></th>
                     <th class="text-right">{{ total_volume|intcomma }}</th>
                     <th class="text-right"></th>
                     <th class="text-right"></th>
                     <th class="text-right">{{ total_value|formatisk:"m" }}</th>
                 </tr>
             </tfoot>
         </table>
     {% else %}
-        <p class="text-muted">No data.</p>
+        <p class="text-muted">{% translate 'No data.' %}</p>
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,15 @@
 {% load i18n %} {% load static %} {% load humanize %} {% load moonmining %}
 {% if ledger|length > 0 %}
-Day        Main                                              Character             Corporation             Ore                  Total Volume                 Unit Price                                        Quantity                 Total Price
+{%                                                           {% translate          {% translate            {% translate 'Ore'   {% translate 'Total Volume'                                                    {% translate 'Quantity'
+translate  {% translate 'Main' %}                            'Character' %}        'Corporation' %}        %}                   %}                           {% translate 'Unit Price' %}                      %}                       {% translate 'Total Price' %}
+'Day' %}
 {          {                                                 {                     {                       {                    {                            {                                                 {                        {
 {          {                                                 {                     {                       {                    {                            {                                                 {                        {
 record.day record.user.profile.main_character.character_name record.character.name record.corporation.name record.ore_type.name record.total_volume|intcomma record.ore_type.extras.current_price|floatformat: record.quantity|intcomma record.total_price|formatisk:
 }}         }}                                                }}                    }}                      }}                   }}                           "0"|intcomma }}                                   }}                       "m" }}
-TOTALS                                                                                                                          {{ total_volume|intcomma }}                                                                             {{ total_value|formatisk:"m"
-                                                                                                                                                                                                                                        }}
+{%                                                                                                                                                                                                                                      {{ total_value|formatisk:"m"
+translate                                                                                                                       {{ total_volume|intcomma }}                                                                             }}
+'Total' %}
 {% else %}
-No data.
+{% translate 'No data.' %}
 {% endif %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/global_js.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/global_js.html`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/location.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/location.html`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/menu.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/menu.html`

 * *Files 12% similar despite different names*

```diff
@@ -15,39 +15,43 @@
             <a class="navbar-brand" href="{% url 'moonmining:index' %}">{% translate "Moon Mining" %}</a>
         </div>
 
         <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
             <ul class="nav navbar-nav">
                 {% if perms.moonmining.extractions_access %}
                     <li class="{% navactive request 'moonmining:extractions' %}">
-                        <a href="{% url 'moonmining:extractions' %}">Extractions</a>
+                        <a href="{% url 'moonmining:extractions' %}">
+                            {% translate 'Extractions' %}
+                        </a>
                     </li>
                 {% endif %}
                 {% if "/moonmining/extraction/" in request.path %}
                     <li class="{% renavactive request '/moonmining/extraction/' %}">
-                        <a href="#">Extraction Details</a>
+                        <a href="#">{% translate 'Extraction Details' %}</a>
                     </li>
                 {% endif %}
                 <li class="{% navactive request 'moonmining:moons' %}">
-                    <a href="{% url 'moonmining:moons' %}">Moons</a>
+                    <a href="{% url 'moonmining:moons' %}">{% translate 'Moons' %}</a>
                 </li>
                 {% if "/moonmining/moon/" in request.path %}
                     <li class="{% renavactive request '/moonmining/moon/' %}">
-                        <a href="#">Moon Details</a>
+                        <a href="#">{% translate 'Moon Details' %}</a>
                     </li>
                 {% endif %}
                  {% if perms.moonmining.reports_access %}
                     <li class="{% navactive request 'moonmining:reports' %}">
-                        <a href="{% url 'moonmining:reports' %}">Reports</a>
+                        <a href="{% url 'moonmining:reports' %}">{% translate 'Reports' %}</a>
                     </li>
                 {% endif %}
             </ul>
 
             {% if perms.moonmining.add_refinery_owner %}
-                <a class="btn btn-default navbar-btn" style="float: right" href="{% url 'moonmining:add_owner' %}">
-                    Add Corporation
+                <a  class="btn btn-default navbar-btn"
+                    style="float: right"
+                    href="{% url 'moonmining:add_owner' %}">
+                    {% translate 'Add Corporation' %}
                 </a>
             {% endif %}
         </div>
 
     </div>
 </nav>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 {% load static %} {% load i18n %} {% load navactive %}
  {% translate "Toggle navigation" %}     {%_translate_"Moon_Mining"_%}
     * {% if perms.moonmining.extractions_access %}
-    * Extractions
+    * {%_translate_'Extractions'_%}
     * {% endif %} {% if "/moonmining/extraction/" in request.path %}
-    * Extraction_Details
+    * {%_translate_'Extraction_Details'_%}
     * {% endif %}
-    * Moons
+    * {%_translate_'Moons'_%}
     * {% if "/moonmining/moon/" in request.path %}
-    * Moon_Details
+    * {%_translate_'Moon_Details'_%}
     * {% endif %} {% if perms.moonmining.reports_access %}
-    * Reports
+    * {%_translate_'Reports'_%}
     * {% endif %}
-{% if perms.moonmining.add_refinery_owner %} Add_Corporation {% endif %}
+{% if perms.moonmining.add_refinery_owner %} {%_translate_'Add_Corporation'_%}
+{% endif %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/moon_details_moon.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_moon.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 {% load i18n %}
 {% load moonmining %}
 
 <div class="row">
     <div class="col-md-2">
-        <p><strong>Name:</strong></p>
+        <p><strong>{% translate 'Name:' %}</strong></p>
     </div>
     <div class="col-md-10">
     <p>{{ moon.name }}&nbsp;</p>
     </div>
 </div>
 
 <div class="row">
     <div class="col-md-2">
-        <p><strong>Location:</strong></p>
+        <p><strong>{% translate 'Location:' %}</strong></p>
     </div>
     <div class="col-md-10">
         {% include "moonmining/partials/location.html" with eve_solar_system=moon.eve_moon.eve_planet.eve_solar_system %}
     </div>
 </div>
 
 <div class="row">
     <div class="col-md-2">
-        <p><strong>Labels:</strong></p>
+        <p><strong>{% translate 'Labels:' %}</strong></p>
     </div>
     <div class="col-md-10">
     <p>{{ moon.labels_html }}</p>
     </div>
 </div>
 
 <div class="row">
     <div class="col-md-2">
-        <p><strong>Refinery:</strong></p>
+        <p><strong>{% translate 'Refinery:' %}</strong></p>
     </div>
     <div class="col-md-10">
     {% if moon.refinery %}
         <p>{{ moon.refinery|default:"-" }}  / {{ moon.refinery.eve_type|default:"-" }}</p>
     {% else %}
         -
     {% endif %}
     </div>
 </div>
 
 <div class="row">
     <div class="col-md-2">
-        <p><strong>Corporation:</strong></p>
+        <p><strong>{% translate 'Corporation:' %}</strong></p>
     </div>
     <div class="col-md-10">
     <p>{{ moon.refinery.owner|default:"-" }}</p>
     </div>
 </div>
 
 <div class="row">
     <div class="col-md-2">
-        <p><strong>Est.&nbsp;Value:</strong></p>
+        <p><strong>{% translate 'Est. Value:' %}</strong></p>
     </div>
     <div class="col-md-10">
     <p>{{ moon.value | formatisk }}</p>
     </div>
 </div>
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/moon_details_products.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_products.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 {% load i18n %}
 {% load humanize %}
 {% load moonmining %}
 
 {% if product_rows|length_is:"0" %}
     <p class="text-warning"><strong>
-        We could not find a survey for this moon in our database.
+        {% translate 'There is no survey for this moon in the database.' %}
     </strong></p>
 {% else %}
 
     {% for product in moon.products_sorted %}
         <div class="row">
             <div class="col-md-2">
                 <img class="media-object" src="{{ product.ore_type.icon_url }}">
             </div>
 
             <div class="col-md-8">
                 <p>
                     <a href="{{ product.ore_type.profile_url }}" target="_blank">{{ product.ore_type.name }}</a>
                     &nbsp;{{ product.ore_type.rarity_class.bootstrap_tag_html }}
                     &nbsp;{{ product.ore_type.extras.current_price|floatformat:"0"|intcomma|default:"?" }}
-                    <small class="text-muted">ISK per unit</small>
+                    <small class="text-muted">{% translate 'ISK per unit' %}</small>
                 </p>
                 <div class="progress" style="height: 20px; width: 100%">
                     <div
                         class="progress-bar progress-bar-default progress-bar-striped"
                         role="progressbar"
                         aria-valuenow="{{ product.amount_percent }}"
                         aria-valuemin="0"
@@ -46,14 +46,15 @@
                     {{ product.total_price|formatisk:"b" }}
                 </span>
             </div>
         </div>
     {% endfor %}
 {% endif %}
 <p class="text-muted">
-    Last updated on
     {% if moon.products_updated_at %}
-        {{moon.products_updated_at|datetime|default:"?"}} by {{moon.products_updated_by.profile.main_character|default:"ESTIMATED"}}
+        {% translate 'Last updated at' %}
+        {% translate "App" as estimated_by %}
+        {% blocktranslate with updated_at=moon.products_updated_at|datetime|default:"?" updated_by=moon.products_updated_by.profile.main_character|default:estimated_by %}{{ updated_at }} by {{ updated_by }}{% endblocktranslate %}
     {% else %}
-        ?
+        {% translate 'Not yet updated' %}
     {% endif %}
 <p>
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
 {% load i18n %} {% load humanize %} {% load moonmining %} {% if
 product_rows|length_is:"0" %}
-We could not find a survey for this moon in our database.
+{% translate 'There is no survey for this moon in the database.' %}
 {% else %} {% for product in moon.products_sorted %}
 [{{ product.ore_type.icon_url }}]
 {{_product.ore_type.name_}}  {
 { product.ore_type.rarity_class.bootstrap_tag_html }}  {
 { product.ore_type.extras.current_price|floatformat:"0"|intcomma|default:"?" }}
-ISK per unit
+{% translate 'ISK per unit' %}
  {{ product.amount_percent|floatformat:"0" }}% {{ product.ore_type.name }}
 ** {{ product.amount_percent|floatformat:"0" }}% **
 
 {{ product.total_price|formatisk:"b" }}
 {% endfor %} {% endif %}
-Last updated on {% if moon.products_updated_at %} {
-{moon.products_updated_at|datetime|default:"?"}} by {
-{moon.products_updated_by.profile.main_character|default:"ESTIMATED"}} {% else
-%} ? {% endif %}
+{% if moon.products_updated_at %} {% translate 'Last updated at' %} {%
+translate "App" as estimated_by %} {% blocktranslate with
+updated_at=moon.products_updated_at|datetime|default:"?"
+updated_by=moon.products_updated_by.profile.main_character|default:estimated_by
+%}{{ updated_at }} by {{ updated_by }}{% endblocktranslate %} {% else %} {%
+translate 'Not yet updated' %} {% endif %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/moons_tab.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moons_tab.html`

 * *Files 25% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         {% endif %}
     </div>
 
     <div id="wrapper_{{ category }}" style="display: none !important;">
         <div class="table-responsive">
             <table class="table table-striped table-moons table-width-fix" id="table_{{ category }}">
                 <thead>
-                    <th>Moon</th>
-                    <th>System</th>
-                    <th>Const./Region</th>
-                    <th>Refinery</th>
-                    <th>Labels</th>
-                    <th>Est.&nbsp;Value</th>
+                    <th>{% translate 'Moon' %}</th>
+                    <th>{% translate 'System' %}</th>
+                    <th>{% translate 'Constellation' %}<br>{% translate 'Region' %}</th>
+                    <th>{% translate 'Refinery' %}<br>{% translate 'Corporation' %}</th>
+                    <th>{% translate 'Labels' %}</th>
+                    <th class="text-nowrap text-right">{% translate 'Est. Value' %}</th>
                     <th></th>
                 </thead>
             </table>
         </div>
     </div>
 </div>
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+{% load i18n %}
 {% load humanize %}
 
 <div role="tabpanel" class="tab-pane" id="tab_ore_prices">
-    <p class="report-title">Current ore prices</p>
+    <p class="report-title">{% translate 'Current ore prices' %}</p>
     <div class="table-responsive">
         <table class="table table-striped table-width-fix" id="table_ore_prices">
             <thead>
                 <tr>
-                    <th>Name</th>
-                    <th>Price&nbsp;(ISK)</th>
-                    <th>Group</th>
-                    <th>Rarity</th>
-                    <th>Description</th>
+                    <th>{% translate 'Name' %}</th>
+                    <th class="text-right">{% translate 'Price (ISK)' %}</th>
+                    <th>{% translate 'Group' %}</th>
+                    <th>{% translate 'Rarity' %}</th>
+                    <th>{% translate 'Description' %}</th>
                 </tr>
             </thead>
         </table>
     </div>
-    <p class="text-muted">Ore prices shown on this report are used for all calculations in this app.</p>
+    <p class="text-muted">
+        {% translate 'Ore prices shown on this report are used for all calculations in this app.' %}
+    </p>
     {% if use_reprocess_pricing %}
-        <p class="text-muted">Ore prices are calculated as sum of it's reprocessed materials with a yield of {{ reprocessing_yield }}%.</p>
+        <p class="text-muted">
+            {% blocktranslate %}Ore prices are calculated as sum of it's reprocessed materials with a yield of {{ reprocessing_yield }}%.{% endblocktranslate %}
+        </p>
     {% else %}
-        <p class="text-muted">The Eve client prices (average prices) are used for ore prices.</p>
+        <p class="text-muted">
+            {% translate 'The Eve client prices (average prices) are used for ore prices.' %}
+        </p>
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,13 @@
-{% load humanize %}
-Current ore prices
-Name Price (ISK)Group Rarity Description
-Ore prices shown on this report are used for all calculations in this app.
+{% load i18n %} {% load humanize %}
+{% translate 'Current ore prices' %}
+{% translate {% translate 'Price {% translate {% translate {% translate
+'Name' %}    (ISK)' %}           'Group' %}   'Rarity' %}  'Description' %}
+{% translate 'Ore prices shown on this report are used for all calculations in
+this app.' %}
 {% if use_reprocess_pricing %}
-Ore prices are calculated as sum of it's reprocessed materials with a yield of
-{{ reprocessing_yield }}%.
+{% blocktranslate %}Ore prices are calculated as sum of it's reprocessed
+materials with a yield of {{ reprocessing_yield }}%.{% endblocktranslate %}
 {% else %}
-The Eve client prices (average prices) are used for ore prices.
+{% translate 'The Eve client prices (average prices) are used for ore prices.'
+%}
 {% endif %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+{% load i18n %}
 {% load humanize %}
 
 <div role="tabpanel" class="tab-pane" id="tab_user_uploaded">
-    <p class="report-title">Uploaded moons per main</p>
+    <p class="report-title">{% translate 'Uploaded moons per main' %}</p>
     <div class="table-responsive">
         <table class="table table-striped table-width-fix" id="table_user_uploaded">
             <thead>
                 <tr>
-                    <th>Name</th>
-                    <th>Corporation</th>
-                    <th>State</th>
-                    <th>Count</th>
+                    <th>{% translate 'Name' %}</th>
+                    <th>{% translate 'Corporation' %}</th>
+                    <th>{% translate 'State' %}</th>
+                    <th class="text-nowrap text-right">{% translate 'Count' %}</th>
                 </tr>
             </thead>
             <tfoot>
-                <th class="info">GRAND&nbsp;TOTAL</th>
-                <th class="info"></th>
+                <th class="info">{% translate 'Grand Total' %}</th>
                 <th class="info"></th>
                 <th class="info"></th>
+                <th class="info text-right"></th>
             </tfoot>
         </table>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
-{% load humanize %}
-Uploaded moons per main
-Name Corporation State Count
+{% load i18n %} {% load humanize %}
+{% translate 'Uploaded moons per main' %}
+{% translate 'Name' {% translate     {% translate 'State' {% translate 'Count'
+%}                  'Corporation' %} %}                   %}
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/reports.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/reports.html`

 * *Files 5% similar despite different names*

```diff
@@ -143,19 +143,19 @@
                 lengthMenu: DEFAULT_LENGTH_MENU,
                 pageLength: DEFAULT_PAGE_LENGTH,
                 order: [ [0, "asc"] ],
                 filterDropDown: {
                     columns: [
                         {
                             idx: 1,
-                            title: "Corporation"
+                            title: "{% translate 'Corporation' %}"
                         },
                         {
                             idx: 2,
-                            title: "State"
+                            title: "{% translate 'State' %}"
                         }
                     ],
                     bootstrap: true,
                     autoSize: false
                 },
                 footerCallback: function (row, data, start, end, display) {
                     const api = this.api();
@@ -190,19 +190,19 @@
                 lengthMenu: DEFAULT_LENGTH_MENU,
                 pageLength: DEFAULT_PAGE_LENGTH,
                 order: [ [0, "asc"] ],
                 filterDropDown: {
                     columns: [
                         {
                             idx: 1,
-                            title: "Corporation"
+                            title: "{% translate 'Corporation' %}"
                         },
                         {
                             idx: 2,
-                            title: "State"
+                            title: "{% translate 'State' %}"
                         }
                     ],
                     bootstrap: true,
                     autoSize: false
                 },
                 footerCallback: function (row, data, start, end, display) {
                     dataTableFooterSumColumn(this.api(), 3);
@@ -243,15 +243,15 @@
                 filterDropDown: {
                     columns: [
                         {
                             idx: 2
                         },
                         {
                             idx: 5,
-                            title: "Rarity"
+                            title: "{% translate 'Rarity' %}"
                         }
                     ],
                     bootstrap: true,
                     autoSize: false
                 }
             });
```

### Comparing `aa-moonmining-1.8.2/moonmining/templates/moonmining/tests.html` & `aa_moonmining-1.9.0/moonmining/templates/moonmining/tests.html`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/templatetags/moonmining.py` & `aa_moonmining-1.9.0/moonmining/templatetags/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/helpers.py` & `aa_moonmining-1.9.0/moonmining/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_admin.py` & `aa_moonmining-1.9.0/moonmining/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_commands.py` & `aa_moonmining-1.9.0/moonmining/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_core.py` & `aa_moonmining-1.9.0/moonmining/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_helpers.py` & `aa_moonmining-1.9.0/moonmining/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_integration.py` & `aa_moonmining-1.9.0/moonmining/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_managers.py` & `aa_moonmining-1.9.0/moonmining/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_models.py` & `aa_moonmining-1.9.0/moonmining/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from django.utils.timezone import now
 from esi.models import Token
 from eveuniverse.models import EveMarketPrice, EveMoon, EveType
 
 from app_utils.testdata_factories import UserFactory
 from app_utils.testing import NoSocketsTestCase
 
-from ..constants import EveTypeId
-from ..core import CalculatedExtraction, CalculatedExtractionProduct
-from ..models import (
+from moonmining.constants import EveTypeId
+from moonmining.core import CalculatedExtraction, CalculatedExtractionProduct
+from moonmining.models import (
     EveOreType,
     Extraction,
     NotificationType,
     OreQualityClass,
     OreRarityClass,
     Refinery,
 )
+
 from . import helpers
 from .testdata.esi_client_stub import esi_client_stub
 from .testdata.factories import (
     CalculatedExtractionFactory,
     ExtractionFactory,
     ExtractionProductFactory,
     MiningLedgerRecordFactory,
@@ -468,14 +469,22 @@
         moon.products.all().delete()
         # when
         moon.update_products_from_latest_extraction()
         # then
         self.assertGreater(moon.products.count(), 0)
 
 
+class TestNotificationType(NoSocketsTestCase):
+    def test_str(self):
+        # given
+        obj = NotificationType.MOONMINING_EXTRACTION_CANCELLED
+        # when/then
+        self.assertIsInstance(str(obj), str)
+
+
 class TestNotification(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
         load_allianceauth()
```

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_templatetags.py` & `aa_moonmining-1.9.0/moonmining/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/test_views.py` & `aa_moonmining-1.9.0/moonmining/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/allianceauth.json` & `aa_moonmining-1.9.0/moonmining/tests/testdata/allianceauth.json`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/create_eveuniverse.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/esi.json` & `aa_moonmining-1.9.0/moonmining/tests/testdata/esi.json`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/esi_client_stub.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/eveuniverse.json` & `aa_moonmining-1.9.0/moonmining/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/factories.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/generate_many_moons.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/generate_many_moons.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/generate_moons.json` & `aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.json`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/generate_moons.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/load_allianceauth.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/load_allianceauth.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/load_eveuniverse.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/load_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/moon_ids.csv` & `aa_moonmining-1.9.0/moonmining/tests/testdata/moon_ids.csv`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/moon_survey_input_2.txt` & `aa_moonmining-1.9.0/moonmining/tests/testdata/moon_survey_input_2.txt`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/notification_details.py` & `aa_moonmining-1.9.0/moonmining/tests/testdata/notification_details.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/tests/testdata/notifications_full.json` & `aa_moonmining-1.9.0/moonmining/tests/testdata/notifications_full.json`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/urls.py` & `aa_moonmining-1.9.0/moonmining/urls.py`

 * *Files identical despite different names*

### Comparing `aa-moonmining-1.8.2/moonmining/views.py` & `aa_moonmining-1.9.0/moonmining/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime as dt
-from collections import defaultdict
 from enum import Enum
+from typing import Union
 
 from django_datatables_view.base_datatable_view import BaseDatatableView
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.contrib.auth.mixins import LoginRequiredMixin, PermissionRequiredMixin
 from django.contrib.auth.models import User
 from django.db import models
@@ -25,14 +25,15 @@
 )
 from django.db.models.functions import Coalesce, Concat
 from django.http import HttpResponseNotFound, JsonResponse
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.utils.html import format_html, strip_tags
 from django.utils.timezone import now
+from django.utils.translation import gettext_lazy as _
 from django.views.decorators.cache import cache_page
 from esi.decorators import token_required
 
 from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.eveonline.evelinks import dotlan
 from allianceauth.eveonline.models import EveCorporationInfo
 from allianceauth.services.hooks import get_extension_logger
@@ -68,17 +69,18 @@
     OURS = "our_moons"
 
 
 def moon_link_html(moon: Moon) -> str:
     return format_html(
         '<a href="#" data-toggle="modal" '
         'data-target="#modalMoonDetails" '
-        'title="Show details for this moon." '
+        'title="{}" '
         "data-ajax_url={}>"
         "{}</a>",
+        _("Show details for this moon."),
         reverse("moonmining:moon_details", args=[moon.pk]),
         moon.name,
     )
 
 
 def extraction_ledger_button_html(extraction: Extraction) -> str:
     return fontawesome_modal_button_html(
@@ -90,24 +92,24 @@
 
 
 def moon_details_button_html(moon: Moon) -> str:
     return fontawesome_modal_button_html(
         modal_id="modalMoonDetails",
         fa_code="fas fa-moon",
         ajax_url=reverse("moonmining:moon_details", args=[moon.pk]),
-        tooltip="Moon details",
+        tooltip=_("Moon details"),
     )
 
 
 def extraction_details_button_html(extraction_pk: int) -> str:
     return fontawesome_modal_button_html(
         modal_id="modalExtractionDetails",
         fa_code="fas fa-hammer",
         ajax_url=reverse("moonmining:extraction_details", args=[extraction_pk]),
-        tooltip="Extraction details",
+        tooltip=_("Extraction details"),
     )
 
 
 def default_if_none(value, default):
     """Return given default if value is None"""
     if value is None:
         return default
@@ -129,53 +131,53 @@
     return redirect("moonmining:moons")
 
 
 @login_required
 @permission_required(["moonmining.extractions_access", "moonmining.basic_access"])
 def extractions(request):
     context = {
-        "page_title": "Extractions",
+        "page_title": _("Extractions"),
         "ExtractionsCategory": ExtractionsCategory.to_dict(),
         "ExtractionsStatus": Extraction.Status,
         "use_reprocess_pricing": MOONMINING_USE_REPROCESS_PRICING,
         "reprocessing_yield": MOONMINING_REPROCESSING_YIELD * 100,
         "total_volume_per_month": MOONMINING_VOLUME_PER_MONTH / 1000000,
         "stale_hours": MOONMINING_COMPLETED_EXTRACTIONS_HOURS_UNTIL_STALE,
     }
     return render(request, "moonmining/extractions.html", context)
 
 
 @login_required
 @permission_required(["moonmining.extractions_access", "moonmining.basic_access"])
 def extractions_data(request, category):
     data = list()
-    cutover_dt = now() - dt.timedelta(
+    stale_cutoff = now() - dt.timedelta(
         hours=MOONMINING_COMPLETED_EXTRACTIONS_HOURS_UNTIL_STALE
     )
-    extractions = (
+    extractions_qs = (
         Extraction.objects.annotate_volume()
         .selected_related_defaults()
         .select_related(
             "refinery__moon__eve_moon__eve_planet__eve_solar_system",
             "refinery__moon__eve_moon__eve_planet__eve_solar_system__eve_constellation",
             "refinery__moon__eve_moon__eve_planet__eve_solar_system__eve_constellation__eve_region",
         )
     )
     if category == ExtractionsCategory.UPCOMING:
-        extractions = extractions.filter(auto_fracture_at__gte=cutover_dt).exclude(
-            status=Extraction.Status.CANCELED
-        )
+        extractions_qs = extractions_qs.filter(
+            auto_fracture_at__gte=stale_cutoff
+        ).exclude(status=Extraction.Status.CANCELED)
     elif category == ExtractionsCategory.PAST:
-        extractions = extractions.filter(
-            auto_fracture_at__lt=cutover_dt
-        ) | extractions.filter(status=Extraction.Status.CANCELED)
+        extractions_qs = extractions_qs.filter(
+            auto_fracture_at__lt=stale_cutoff
+        ) | extractions_qs.filter(status=Extraction.Status.CANCELED)
     else:
-        extractions = Extraction.objects.none()
+        extractions_qs = Extraction.objects.none()
     can_see_ledger = request.user.has_perm("moonmining.view_moon_ledgers")
-    for extraction in extractions:
+    for extraction in extractions_qs:
         corporation_name = extraction.refinery.owner.name
         alliance_name = extraction.refinery.owner.alliance_name
         moon = extraction.refinery.moon
         moon_name = str(moon)
         refinery_name = str(extraction.refinery.name)
         solar_system = moon.eve_moon.eve_planet.eve_solar_system
         constellation = region = solar_system.eve_constellation
@@ -266,15 +268,15 @@
         "page_title": (
             f"{extraction.refinery.moon} "
             f"| {extraction.chunk_arrival_at.strftime(DATE_FORMAT)}"
         ),
         "extraction": extraction,
     }
     if request.GET.get("new_page"):
-        context["title"] = "Extraction"
+        context["title"] = _("Extraction")
         context["content_file"] = "moonmining/partials/extraction_details.html"
         return render(request, "moonmining/_generic_modal_page.html", context)
     else:
         return render(request, "moonmining/modals/extraction_details.html", context)
 
 
 @login_required
@@ -338,25 +340,25 @@
         "extraction": extraction,
         "total_value": total_value,
         "total_volume": total_volume,
         "ledger": ledger,
         "character_totals": character_totals,
     }
     if request.GET.get("new_page"):
-        context["title"] = "Extraction Ledger"
+        context["title"] = _("Extraction Ledger")
         context["content_file"] = "moonmining/partials/extraction_ledger.html"
         return render(request, "moonmining/_generic_modal_page.html", context)
     return render(request, "moonmining/modals/extraction_ledger.html", context)
 
 
 @login_required()
 @permission_required("moonmining.basic_access")
 def moons(request):
     context = {
-        "page_title": "Moons",
+        "page_title": _("Moons"),
         "MoonsCategory": MoonsCategory.to_dict(),
         "use_reprocess_pricing": MOONMINING_USE_REPROCESS_PRICING,
         "reprocessing_yield": MOONMINING_REPROCESSING_YIELD * 100,
         "total_volume_per_month": MOONMINING_VOLUME_PER_MONTH / 1000000,
     }
     return render(request, "moonmining/moons.html", context)
 
@@ -499,41 +501,41 @@
         if search:
             qs = qs.filter(
                 Q(eve_moon__name__istartswith=search)
                 | Q(refinery__name__istartswith=search)
             )
         return qs
 
-        qs = self._apply_search_filter(qs, 4, "user__profile__state__name")
-        qs = self._apply_search_filter(qs, 6, "character__alliance_name")
-        qs = self._apply_search_filter(qs, 7, "character__corporation_name")
-        qs = self._apply_search_filter(
-            qs, 8, "user__profile__main_character__alliance_name"
-        )
-        qs = self._apply_search_filter(
-            qs, 9, "user__profile__main_character__corporation_name"
-        )
-        qs = self._apply_search_filter(
-            qs, 10, "user__profile__main_character__character_name"
-        )
-        qs = self._apply_search_filter(qs, 11, "unregistered")
+        # qs = self._apply_search_filter(qs, 4, "user__profile__state__name")
+        # qs = self._apply_search_filter(qs, 6, "character__alliance_name")
+        # qs = self._apply_search_filter(qs, 7, "character__corporation_name")
+        # qs = self._apply_search_filter(
+        #     qs, 8, "user__profile__main_character__alliance_name"
+        # )
+        # qs = self._apply_search_filter(
+        #     qs, 9, "user__profile__main_character__corporation_name"
+        # )
+        # qs = self._apply_search_filter(
+        #     qs, 10, "user__profile__main_character__character_name"
+        # )
+        # qs = self._apply_search_filter(qs, 11, "unregistered")
 
-        return qs
+        # return qs
 
     def _apply_search_filter(self, qs, column_num, field) -> models.QuerySet:
         my_filter = self.request.GET.get(f"columns[{column_num}][search][value]", None)
         if my_filter:
             if self.request.GET.get(f"columns[{column_num}][search][regex]", False):
                 kwargs = {f"{field}__iregex": my_filter}
             else:
                 kwargs = {f"{field}__istartswith": my_filter}
             return qs.filter(**kwargs)
         return qs
 
-    def render_column(self, row, column) -> str:
+    def render_column(self, row, column) -> Union[str, dict]:
         if column == "id":
             return row.pk
         if column == "moon_name":
             return row.name
         result = self._render_location(row, column)
         if result:
             return result
@@ -589,15 +591,15 @@
                 if row.extraction_pk
                 else ""
             )
             details_html += moon_details_button_html(row)
             return details_html
         return ""
 
-    def _render_refinery(self, row, column):
+    def _render_refinery(self, row, column) -> Union[str, dict]:
         if row.has_refinery:
             refinery = row.refinery
             refinery_html = refinery.name_html()
             refinery_name = refinery.name
             corporation_name = refinery.owner.name
             alliance_name = refinery.owner.alliance_name
         else:
@@ -606,15 +608,15 @@
             corporation_name = alliance_name = ""
         if column == "corporation_name":
             return corporation_name
         if column == "alliance_name":
             return alliance_name
         if column == "refinery":
             return {"display": refinery_html, "sort": refinery_name}
-        return None
+        return ""
 
 
 @login_required
 @permission_required("moonmining.basic_access")
 def moons_fdd_data(request, category) -> JsonResponse:
     """Provide lists for drop down fields."""
     qs = MoonListJson.initial_queryset(category=category, user=request.user)
@@ -676,22 +678,22 @@
         "page_title": moon.name,
         "moon": moon,
         "use_reprocess_pricing": MOONMINING_USE_REPROCESS_PRICING,
         "reprocessing_yield": MOONMINING_REPROCESSING_YIELD * 100,
         "total_volume_per_month": MOONMINING_VOLUME_PER_MONTH / 1000000,
     }
     if request.GET.get("new_page"):
-        context["title"] = "Moon"
+        context["title"] = _("Moon")
         context["content_file"] = "moonmining/partials/moon_details.html"
         return render(request, "moonmining/_generic_modal_page.html", context)
     return render(request, "moonmining/modals/moon_details.html", context)
 
 
 @permission_required(["moonmining.add_refinery_owner", "moonmining.basic_access"])
-@token_required(scopes=Owner.esi_scopes())
+@token_required(scopes=Owner.esi_scopes())  # type: ignore
 @login_required
 def add_owner(request, token):
     try:
         character_ownership = request.user.character_ownerships.select_related(
             "character"
         ).get(character__character_id=token.character_id)
     except CharacterOwnership.DoesNotExist:
@@ -702,49 +704,51 @@
         )
     except EveCorporationInfo.DoesNotExist:
         corporation = EveCorporationInfo.objects.create_corporation(
             corp_id=character_ownership.character.corporation_id
         )
         corporation.save()
 
-    owner, _ = Owner.objects.update_or_create(
+    owner = Owner.objects.update_or_create(
         corporation=corporation,
         defaults={"character_ownership": character_ownership},
-    )
+    )[0]
     tasks.update_owner.delay(owner.pk)
-    messages_plus.success(request, f"Update of refineres started for {owner}.")
+    messages_plus.success(request, f"Update of refineries started for {owner}.")
     if MOONMINING_ADMIN_NOTIFICATIONS_ENABLED:
         notify_admins(
-            message=("%(corporation)s was added as new owner by %(user)s.")
-            % {"corporation": owner, "user": request.user},
+            message=_(
+                "%(corporation)s was added as new owner by %(user)s."
+                % {"corporation": owner, "user": request.user}
+            ),
             title=f"{__title__}: Owner added: {owner}",
         )
     return redirect("moonmining:index")
 
 
 @permission_required(["moonmining.basic_access", "moonmining.upload_moon_scan"])
 @login_required()
 def upload_survey(request):
-    context = {"page_title": "Upload Moon Surveys"}
+    context = {"page_title": _("Upload Moon Surveys")}
     if request.method == "POST":
         form = MoonScanForm(request.POST)
         if form.is_valid():
             scans = request.POST["scan"]
             tasks.process_survey_input.delay(scans, request.user.pk)
             messages_plus.success(
                 request,
-                (
-                    "Your scan has been submitted for processing. You will"
-                    "receive a notification once processing is complete."
+                _(
+                    "Your scan has been submitted for processing. "
+                    "You will receive a notification once processing is complete."
                 ),
             )
         else:
             messages_plus.error(
                 request,
-                (
+                _(
                     "Oh No! Something went wrong with your moon scan submission. "
                     "Please try again."
                 ),
             )
         return redirect("moonmining:moons")
     return render(request, "moonmining/modals/upload_survey.html", context=context)
 
@@ -773,15 +777,15 @@
         try:
             ledger_last_updated = Refinery.objects.filter(
                 owner__is_enabled=True
             ).aggregate(Min("ledger_last_update_at"))["ledger_last_update_at__min"]
         except KeyError:
             ledger_last_updated = None
     context = {
-        "page_title": "Reports",
+        "page_title": _("Reports"),
         "use_reprocess_pricing": MOONMINING_USE_REPROCESS_PRICING,
         "reprocessing_yield": MOONMINING_REPROCESSING_YIELD * 100,
         "total_volume_per_month": MOONMINING_VOLUME_PER_MONTH / 1000000,
         "month_minus_3": month_minus_3.strftime(month_format),
         "month_minus_2": month_minus_2.strftime(month_format),
         "month_minus_1": month_minus_1.strftime(month_format),
         "month_current": now().strftime(month_format),
@@ -798,17 +802,19 @@
         "eve_moon__eve_planet__eve_solar_system",
         "eve_moon__eve_planet__eve_solar_system__eve_constellation__eve_region",
         "refinery",
         "refinery__owner",
         "refinery__owner__corporation",
         "refinery__owner__corporation__alliance",
     ).filter(refinery__isnull=False)
-    corporation_moons = defaultdict(lambda: {"moons": list(), "total": 0})
+    corporation_moons = {}
     for moon in moon_query.order_by("eve_moon__name"):
         corporation_name = moon.refinery.owner.name
+        if corporation_name not in corporation_moons:
+            corporation_moons[corporation_name] = {"moons": list(), "total": 0}
         corporation_moons[corporation_name]["moons"].append(moon)
         corporation_moons[corporation_name]["total"] += default_if_none(moon.value, 0)
 
     moon_ranks = {
         moon_pk: rank
         for rank, moon_pk in enumerate(
             moon_query.filter(value__isnull=False)
@@ -843,15 +849,15 @@
                     "grand_total_percent": grand_total_percent,
                 }
             )
             counter += 1
         data.append(
             {
                 "corporation": corporation,
-                "moon": {"display": "TOTAL", "sort": counter},
+                "moon": {"display": _("Total"), "sort": counter},
                 "region": None,
                 "rarity_class": None,
                 "value": None,
                 "rank": None,
                 "total": details["total"],
                 "is_total": True,
                 "grand_total_percent": None,
```

