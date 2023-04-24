# Comparing `tmp/lndb-0.44.2.tar.gz` & `tmp/lndb-0.44.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.44.2.tar", last modified: Sat Apr 22 19:12:42 2023, max compression
+gzip compressed data, was "lndb-0.44.3.tar", last modified: Mon Apr 24 00:39:20 2023, max compression
```

## Comparing `lndb-0.44.2.tar` & `lndb-0.44.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.44.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.44.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.44.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.44.2/.gitignore
--rw-r--r--   0        0        0     1772 2023-01-16 03:13:03.815140 lndb-0.44.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.44.2/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.44.2/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.44.2/docs/api.md
--rw-r--r--   0        0        0    47427 2023-04-22 19:12:27.272250 lndb-0.44.2/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.44.2/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.44.2/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.44.2/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.44.2/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.44.2/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.44.2/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.44.2/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.44.2/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.44.2/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.44.2/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.44.2/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5418 2023-04-20 08:37:12.609361 lndb-0.44.2/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.44.2/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.44.2/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.44.2/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.44.2/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-21 17:24:54.958979 lndb-0.44.2/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.44.2/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.44.2/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-22 19:12:22.465207 lndb-0.44.2/lndb/__init__.py
--rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.44.2/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.44.2/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.44.2/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-22 05:22:50.971625 lndb-0.44.2/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.44.2/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.44.2/lndb/_delete.py
--rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.44.2/lndb/_info.py
--rw-r--r--   0        0        0     6051 2023-04-21 12:45:57.904490 lndb-0.44.2/lndb/_init_instance.py
--rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.44.2/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.44.2/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.44.2/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-21 17:30:25.327407 lndb-0.44.2/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-22 12:00:39.395914 lndb-0.44.2/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.44.2/lndb/_migrate/env.py
--rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.44.2/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.44.2/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.44.2/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.44.2/lndb/_schema.py
--rw-r--r--   0        0        0     1313 2023-04-20 08:37:12.610024 lndb-0.44.2/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.44.2/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.44.2/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.44.2/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.44.2/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.44.2/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.44.2/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.44.2/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.44.2/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.44.2/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.44.2/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8764 2023-04-21 12:45:57.904794 lndb-0.44.2/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.44.2/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.44.2/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.44.2/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.44.2/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.44.2/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-22 19:12:00.877065 lndb-0.44.2/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     4917 2023-04-08 10:27:51.835175 lndb-0.44.2/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.44.2/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.44.2/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.44.2/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.44.2/lndb/test/_env.py
--rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.44.2/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.44.2/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.44.2/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.44.2/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.44.2/noxfile.py
--rw-r--r--   0        0        0     1395 2023-04-22 05:22:50.971891 lndb-0.44.2/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.44.2/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.44.2/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.44.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lndb-0.44.2/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.44.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.44.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.44.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.44.3/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-23 22:02:46.131957 lndb-0.44.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.44.3/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.44.3/README.md
+-rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.44.3/docs/api.md
+-rw-r--r--   0        0        0    47603 2023-04-24 00:38:47.209653 lndb-0.44.3/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.44.3/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.44.3/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.44.3/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.44.3/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.44.3/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.44.3/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.44.3/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.44.3/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.44.3/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.44.3/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.44.3/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-23 22:02:46.132862 lndb-0.44.3/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-03-22 05:59:33.864269 lndb-0.44.3/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.44.3/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.44.3/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.44.3/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-21 17:24:54.958979 lndb-0.44.3/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.44.3/docs/index.md
+-rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.44.3/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-24 00:38:36.617657 lndb-0.44.3/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.44.3/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.44.3/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.44.3/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-22 05:22:50.971625 lndb-0.44.3/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.44.3/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.44.3/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-02-16 21:53:37.660919 lndb-0.44.3/lndb/_info.py
+-rw-r--r--   0        0        0     6051 2023-04-21 12:45:57.904490 lndb-0.44.3/lndb/_init_instance.py
+-rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.44.3/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.44.3/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.44.3/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-21 17:30:25.327407 lndb-0.44.3/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-22 12:00:39.395914 lndb-0.44.3/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.44.3/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-02-16 21:53:37.661843 lndb-0.44.3/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.44.3/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.44.3/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.44.3/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-23 22:02:46.133073 lndb-0.44.3/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.44.3/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.44.3/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.44.3/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.44.3/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.44.3/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.44.3/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.44.3/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.44.3/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.44.3/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.44.3/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8764 2023-04-21 12:45:57.904794 lndb-0.44.3/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.44.3/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.44.3/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.44.3/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.44.3/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.44.3/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-22 19:12:00.877065 lndb-0.44.3/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-23 22:02:46.133274 lndb-0.44.3/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.44.3/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.44.3/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.44.3/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.44.3/lndb/test/_env.py
+-rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.44.3/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.44.3/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.44.3/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.44.3/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.44.3/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-23 22:02:46.133475 lndb-0.44.3/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.44.3/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.44.3/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.44.3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.3/PKG-INFO
```

### Comparing `lndb-0.44.2/.github/workflows/build.yml` & `lndb-0.44.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/.github/workflows/latest-changes.yml` & `lndb-0.44.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/.gitignore` & `lndb-0.44.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/.pre-commit-config.yaml` & `lndb-0.44.3/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     hooks:
       - id: mypy
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.1.1
     hooks:
       - id: pydocstyle
         args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
-          - --ignore=D100,D101,D102,D103,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D413
+          - --ignore=D100,D101,D102,D103,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413
```

### Comparing `lndb-0.44.2/LICENSE` & `lndb-0.44.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/changelog.md` & `lndb-0.44.3/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Allow to set additional fsspec kwargs for cloud instances | [366](https://github.com/laminlabs/lndb/pull/366) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 | 0.44.3
 ⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
 🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
 🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 👷 Remove lnhub-rest CI calls | [360](https://github.com/laminlabs/lndb/pull/360) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 🚸 Enable non-owner to set storage | [358](https://github.com/laminlabs/lndb/pull/358) | [falexwolf](https://github.com/falexwolf) | 2023-04-19 |
```

### Comparing `lndb-0.44.2/docs/faq/check-synchronization.ipynb` & `lndb-0.44.3/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/faq/clone.ipynb` & `lndb-0.44.3/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.44.3/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/faq/manage-migrations.ipynb` & `lndb-0.44.3/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/faq/switch-environment.ipynb` & `lndb-0.44.3/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.44.3/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/faq/test-migrations-unit.ipynb` & `lndb-0.44.3/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/guide/01-setup-user.ipynb` & `lndb-0.44.3/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/guide/02-init-instance.ipynb` & `lndb-0.44.3/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/guide/03-load-instance.ipynb` & `lndb-0.44.3/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/guide/04-set-storage.ipynb` & `lndb-0.44.3/docs/guide/04-set-storage.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9738858363858365%*

 * *Differences: {"'cells'": "{5: {delete: ['attachments']}, 20: {delete: ['attachments']}, insert: [(11, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('id', '7bd9997b'), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['# root.fs contains the "*

 * *            "underlying fsspec filesystem\\n', 'assert (\\n', '    "*

 * *            'ln.setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by '*

 * *            "default\\n', ')'])])), (12, OrderedDict([('ce […]*

```diff
@@ -51,15 +51,14 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(storage=\"./storage_1\", db=pgurl)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "ceb57cc9",
             "metadata": {},
             "source": [
                 "Running \n",
                 "```\n",
                 "!lamin set --storage ./storage_2\n",
@@ -124,14 +123,55 @@
             "outputs": [],
             "source": [
                 "assert ln.setup.settings.storage.is_cloud\n",
                 "assert ln.setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\""
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "7bd9997b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# root.fs contains the underlying fsspec filesystem\n",
+                "assert (\n",
+                "    ln.setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "ae953b6a",
+            "metadata": {},
+            "source": [
+                "It is possible to set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f9294082",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.set.storage(\"s3://lndb-setup-ci\", cache_regions=False)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "5f320819",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "assert not ln.setup.settings.storage.root.fs.cache_regions"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "id": "529e68e5-9b10-4fdb-9d4c-ac8206bbbb68",
             "metadata": {},
             "source": [
                 "### Set storage not by owner"
             ]
         },
@@ -184,15 +224,14 @@
             },
             "outputs": [],
             "source": [
                 "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "id": "3fb6a223",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "## Set storage for SQLite instance"
@@ -251,29 +290,29 @@
             "source": [
                 "ln.setup.set_storage(\"mydata_storage_2\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "py39",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
             }
         }
     },
```

### Comparing `lndb-0.44.2/docs/guide/05-schema-modules.ipynb` & `lndb-0.44.3/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/guide/06-info.ipynb` & `lndb-0.44.3/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/guide/07-delete.ipynb` & `lndb-0.44.3/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/docs/guide/migrate.md` & `lndb-0.44.3/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/__init__.py` & `lndb-0.44.3/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.44.2"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.3"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.44.2/lndb/__main__.py` & `lndb-0.44.3/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_check_instance_setup.py` & `lndb-0.44.3/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_close.py` & `lndb-0.44.3/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_delete.py` & `lndb-0.44.3/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_init_instance.py` & `lndb-0.44.3/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_load_instance.py` & `lndb-0.44.3/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_migrate/alembic.ini` & `lndb-0.44.3/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_migrate/core.py` & `lndb-0.44.3/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_migrate/deploy.py` & `lndb-0.44.3/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_migrate/env.py` & `lndb-0.44.3/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_migrate/utils.py` & `lndb-0.44.3/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_register_instance.py` & `lndb-0.44.3/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_schema.py` & `lndb-0.44.3/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_settings.py` & `lndb-0.44.3/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/_setup_user.py` & `lndb-0.44.3/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/__init__.py` & `lndb-0.44.3/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_clone.py` & `lndb-0.44.3/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_db.py` & `lndb-0.44.3/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_deprecated.py` & `lndb-0.44.3/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_exclusion.py` & `lndb-0.44.3/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_settings_instance.py` & `lndb-0.44.3/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_settings_load.py` & `lndb-0.44.3/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_settings_save.py` & `lndb-0.44.3/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_settings_store.py` & `lndb-0.44.3/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_settings_user.py` & `lndb-0.44.3/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_setup_knowledge.py` & `lndb-0.44.3/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_setup_schema.py` & `lndb-0.44.3/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/dev/_storage.py` & `lndb-0.44.3/lndb/dev/_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,14 +66,26 @@
         return self._id
 
     @property
     def root(self) -> Union[Path, UPath]:
         """Root storage location."""
         return self._root
 
+    def _set_fs_kwargs(self, **kwargs):
+        """Set additional fsspec arguments for cloud root.
+
+        Example:
+
+        >>> ln.setup.settings.storage._set_fs_kwargs(  # any fsspec args
+        >>>    profile="some_profile", cache_regions=True
+        >>> )
+        """
+        if isinstance(self._root, UPath):
+            self._root = UPath(self._root, **kwargs)
+
     @property
     def root_as_str(self) -> str:
         """Formatted root string."""
         return self.root.as_posix().rstrip("/")
 
     @property
     def cache_dir(
```

### Comparing `lndb-0.44.2/lndb/dev/upath.py` & `lndb-0.44.3/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/test/_migrations_e2e.py` & `lndb-0.44.3/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/lndb/test/_migrations_unit.py` & `lndb-0.44.3/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/noxfile.py` & `lndb-0.44.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/pyproject.toml` & `lndb-0.44.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
-    "lamindb[bionty,wetlab]>=0.35.6",
+    "lamindb[bionty,lamin1]>=0.39rc1",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test>=0.4.3",
     "nbproject",
 ]
 
 [project.scripts]
```

### Comparing `lndb-0.44.2/tests/test_bionty.py` & `lndb-0.44.3/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/tests/test_init_instance.py` & `lndb-0.44.3/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.2/PKG-INFO` & `lndb-0.44.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.44.2
+Version: 0.44.3
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.8.2
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
@@ -17,15 +17,15 @@
 Requires-Dist: erdiagram
 Requires-Dist: alembic
 Requires-Dist: natsort
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
-Requires-Dist: lamindb[bionty,wetlab]>=0.35.6 ; extra == "test"
+Requires-Dist: lamindb[bionty,lamin1]>=0.39rc1 ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb
 Provides-Extra: dev
 Provides-Extra: test
```

