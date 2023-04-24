# Comparing `tmp/lnhub_rest-0.8.2.tar.gz` & `tmp/lnhub_rest-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.8.2.tar", last modified: Sat Apr 22 05:00:47 2023, max compression
+gzip compressed data, was "lnhub_rest-0.9.0.tar", last modified: Mon Apr 24 12:43:14 2023, max compression
```

## Comparing `lnhub_rest-0.8.2.tar` & `lnhub_rest-0.9.0.tar`

### file list

```diff
@@ -1,198 +1,199 @@
--rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.8.2/.dockerignore
--rw-r--r--   0        0        0     3315 2023-04-22 04:03:15.788282 lnhub_rest-0.8.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     5113 2023-04-19 15:57:22.483317 lnhub_rest-0.8.2/.github/workflows/google-cloudrun-docker.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.8.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.8.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.8.2/.gitignore
--rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.8.2/.gitmodules
--rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.8.2/Dockerfile
--rw-r--r--   0        0        0     1140 2023-04-19 18:12:02.220748 lnhub_rest-0.8.2/README.md
--rw-r--r--   0        0        0     1754 2023-04-19 18:12:02.221232 lnhub_rest-0.8.2/docs/00-migrate.ipynb
--rw-r--r--   0        0        0     1189 2023-04-19 15:57:22.509145 lnhub_rest-0.8.2/docs/01-checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0     5218 2023-04-19 15:57:22.508991 lnhub_rest-0.8.2/docs/02-account/01-signup-signin.ipynb
--rw-r--r--   0        0        0     4487 2023-04-19 15:57:22.508836 lnhub_rest-0.8.2/docs/02-account/02-create-account.ipynb
--rw-r--r--   0        0        0     5566 2023-04-19 15:57:22.508666 lnhub_rest-0.8.2/docs/02-account/03-update-account.ipynb
--rw-r--r--   0        0        0     6146 2023-04-19 15:57:22.508504 lnhub_rest-0.8.2/docs/02-account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9088 2023-04-19 15:57:22.508334 lnhub_rest-0.8.2/docs/02-account/05-rls.ipynb
--rw-r--r--   0        0        0    11211 2023-04-21 10:12:34.724112 lnhub_rest-0.8.2/docs/03-instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5290 2023-04-19 15:57:22.507982 lnhub_rest-0.8.2/docs/03-instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6195 2023-04-19 15:57:22.507801 lnhub_rest-0.8.2/docs/03-instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     8667 2023-04-19 15:57:22.507620 lnhub_rest-0.8.2/docs/03-instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     7001 2023-04-19 15:57:22.507431 lnhub_rest-0.8.2/docs/03-instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19423 2023-04-19 15:57:22.507215 lnhub_rest-0.8.2/docs/03-instance/06-rls.ipynb
--rw-r--r--   0        0        0     3870 2023-04-21 10:12:34.724397 lnhub_rest-0.8.2/docs/04-storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9837 2023-04-19 15:57:22.506877 lnhub_rest-0.8.2/docs/04-storage/02-rls.ipynb
--rw-r--r--   0        0        0     3894 2023-04-19 15:57:22.506712 lnhub_rest-0.8.2/docs/05-organization/01-create-organization.ipynb
--rw-r--r--   0        0        0     4003 2023-04-19 15:57:22.506559 lnhub_rest-0.8.2/docs/05-organization/02-manage-members.ipynb
--rw-r--r--   0        0        0     5892 2023-04-19 15:57:22.506399 lnhub_rest-0.8.2/docs/05-organization/03-rls.ipynb
--rw-r--r--   0        0        0      125 2023-04-18 16:52:57.348114 lnhub_rest-0.8.2/docs/README.md
--rw-r--r--   0        0        0    22591 2023-04-22 05:00:27.269158 lnhub_rest-0.8.2/docs/changelog.md
--rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.8.2/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.8.2/docs/notes/index.md
--rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.8.2/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.8.2/lamin-project.yaml
--rw-r--r--   0        0        0     3832 2023-04-18 16:53:14.549682 lnhub_rest-0.8.2/lndb/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.8.2/lndb/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.8.2/lndb/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.8.2/lndb/.gitignore
--rw-r--r--   0        0        0     1772 2023-03-14 19:46:06.422493 lnhub_rest-0.8.2/lndb/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.8.2/lndb/LICENSE
--rw-r--r--   0        0        0      173 2023-04-18 16:53:14.549987 lnhub_rest-0.8.2/lndb/README.md
--rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.8.2/lndb/docs/api.md
--rw-r--r--   0        0        0    46285 2023-04-18 21:59:42.219504 lnhub_rest-0.8.2/lndb/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.8.2/lndb/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.8.2/lndb/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-04-18 16:53:14.550717 lnhub_rest-0.8.2/lndb/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-04-18 16:53:14.551192 lnhub_rest-0.8.2/lndb/docs/faq/index.md
--rw-r--r--   0        0        0     1180 2023-04-18 16:53:14.551280 lnhub_rest-0.8.2/lndb/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.8.2/lndb/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-18 16:53:14.551375 lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-18 16:53:14.551472 lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-18 16:53:14.551612 lnhub_rest-0.8.2/lndb/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10679 2023-04-18 16:53:14.551748 lnhub_rest-0.8.2/lndb/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5573 2023-04-18 16:53:14.551912 lnhub_rest-0.8.2/lndb/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     5290 2023-03-14 19:46:06.424075 lnhub_rest-0.8.2/lndb/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-04-18 16:53:14.552033 lnhub_rest-0.8.2/lndb/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-04-18 16:53:14.552137 lnhub_rest-0.8.2/lndb/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     3282 2023-04-18 16:53:14.552254 lnhub_rest-0.8.2/lndb/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.8.2/lndb/docs/guide/index.md
--rw-r--r--   0        0        0     3152 2023-04-18 16:53:14.552393 lnhub_rest-0.8.2/lndb/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.8.2/lndb/docs/index.md
--rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.8.2/lndb/lamin-project.yaml
--rw-r--r--   0        0        0     1932 2023-04-18 16:53:14.552609 lnhub_rest-0.8.2/lndb/lndb/__init__.py
--rw-r--r--   0        0        0     4242 2023-03-14 19:46:06.424708 lnhub_rest-0.8.2/lndb/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.8.2/lndb/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-18 16:53:14.553281 lnhub_rest-0.8.2/lndb/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      216 2023-04-18 16:53:14.553485 lnhub_rest-0.8.2/lndb/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-18 16:53:14.553610 lnhub_rest-0.8.2/lndb/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-18 16:53:14.553765 lnhub_rest-0.8.2/lndb/lndb/_delete.py
--rw-r--r--   0        0        0      222 2023-03-14 19:46:06.425064 lnhub_rest-0.8.2/lndb/lndb/_info.py
--rw-r--r--   0        0        0     5751 2023-04-18 21:59:42.219684 lnhub_rest-0.8.2/lndb/lndb/_init_instance.py
--rw-r--r--   0        0        0     4003 2023-04-18 21:59:42.219815 lnhub_rest-0.8.2/lndb/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-18 16:53:14.554421 lnhub_rest-0.8.2/lndb/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-18 16:53:14.554545 lnhub_rest-0.8.2/lndb/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3469 2023-04-18 16:53:14.554644 lnhub_rest-0.8.2/lndb/lndb/_migrate/core.py
--rw-r--r--   0        0        0     6303 2023-04-18 16:53:14.554756 lnhub_rest-0.8.2/lndb/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.8.2/lndb/lndb/_migrate/env.py
--rw-r--r--   0        0        0      341 2023-03-14 19:46:06.425679 lnhub_rest-0.8.2/lndb/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-18 16:53:14.554944 lnhub_rest-0.8.2/lndb/lndb/_migrate/utils.py
--rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.8.2/lndb/lndb/_schema.py
--rw-r--r--   0        0        0     1506 2023-04-18 21:59:42.219950 lnhub_rest-0.8.2/lndb/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 21:34:53.593994 lnhub_rest-0.8.2/lndb/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.8.2/lndb/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.8.2/lndb/lndb/_settings_store.py
--rw-r--r--   0        0        0     4940 2023-04-18 21:59:42.220094 lnhub_rest-0.8.2/lndb/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-18 16:53:14.555545 lnhub_rest-0.8.2/lndb/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-04-18 16:53:14.555802 lnhub_rest-0.8.2/lndb/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-18 16:53:14.555956 lnhub_rest-0.8.2/lndb/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.8.2/lndb/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.8.2/lndb/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-18 16:53:14.556103 lnhub_rest-0.8.2/lndb/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8429 2023-04-18 16:53:14.556252 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-04-18 16:53:14.556382 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-18 16:53:14.556505 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.8.2/lndb/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-04-18 16:53:14.556633 lnhub_rest-0.8.2/lndb/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     6997 2023-04-18 16:53:14.556779 lnhub_rest-0.8.2/lndb/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     4917 2023-04-18 16:53:14.556926 lnhub_rest-0.8.2/lndb/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.8.2/lndb/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-18 16:53:14.557004 lnhub_rest-0.8.2/lndb/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-18 16:53:14.557144 lnhub_rest-0.8.2/lndb/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.8.2/lndb/lndb/test/_env.py
--rw-r--r--   0        0        0     3870 2023-04-18 21:59:42.220234 lnhub_rest-0.8.2/lndb/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-18 16:53:14.557417 lnhub_rest-0.8.2/lndb/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.8.2/lndb/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.8.2/lndb/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-18 16:53:14.557535 lnhub_rest-0.8.2/lndb/noxfile.py
--rw-r--r--   0        0        0     1395 2023-04-18 16:53:14.557716 lnhub_rest-0.8.2/lndb/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-18 16:53:14.557862 lnhub_rest-0.8.2/lndb/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.8.2/lndb/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:53:14.558657 lnhub_rest-0.8.2/lndb/tests/test_notebooks.py
--rw-r--r--   0        0        0      158 2023-04-22 05:00:02.722421 lnhub_rest-0.8.2/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     8011 2023-04-19 18:12:02.222219 lnhub_rest-0.8.2/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.8.2/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0     1026 2023-01-15 12:17:52.330665 lnhub_rest-0.8.2/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1094 2023-04-22 04:59:42.149916 lnhub_rest-0.8.2/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.8.2/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0      998 2023-04-19 18:12:02.222640 lnhub_rest-0.8.2/lnhub_rest/_ci.py
--rw-r--r--   0        0        0     5726 2023-04-19 15:57:22.490723 lnhub_rest-0.8.2/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.8.2/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.8.2/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     2542 2023-04-21 10:12:34.724799 lnhub_rest-0.8.2/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.8.2/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      739 2023-04-19 15:57:22.491329 lnhub_rest-0.8.2/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3325 2023-04-19 15:57:22.491711 lnhub_rest-0.8.2/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1423 2023-04-19 15:57:22.491949 lnhub_rest-0.8.2/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.8.2/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     2735 2023-04-18 16:02:04.948532 lnhub_rest-0.8.2/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.8.2/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.8.2/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1284 2023-04-19 15:57:22.492340 lnhub_rest-0.8.2/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6751 2023-04-22 04:02:09.361507 lnhub_rest-0.8.2/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1532 2023-04-19 15:57:22.492860 lnhub_rest-0.8.2/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1067 2023-04-19 15:57:22.493104 lnhub_rest-0.8.2/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.8.2/lnhub_rest/core/member/__init__.py
--rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.8.2/lnhub_rest/core/member/_crud.py
--rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.8.2/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     2861 2023-04-19 15:57:22.493317 lnhub_rest-0.8.2/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.8.2/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      796 2023-04-19 18:12:02.223356 lnhub_rest-0.8.2/lnhub_rest/main.py
--rw-r--r--   0        0        0       39 2023-04-19 15:57:22.493742 lnhub_rest-0.8.2/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      224 2023-04-19 18:12:02.224109 lnhub_rest-0.8.2/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     2543 2023-04-19 18:12:02.224813 lnhub_rest-0.8.2/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      198 2023-04-18 16:02:04.950703 lnhub_rest-0.8.2/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     4121 2023-04-18 16:02:04.950818 lnhub_rest-0.8.2/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.8.2/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.8.2/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     4317 2023-04-19 15:57:22.493965 lnhub_rest-0.8.2/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.8.2/lnhub_rest/routers/organization.py
--rw-r--r--   0        0        0     1074 2023-04-19 15:57:22.494317 lnhub_rest-0.8.2/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.8.2/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.8.2/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.8.2/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.8.2/lnhub_rest/schema/_type.py
--rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.8.2/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.8.2/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.8.2/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       50 2023-04-18 16:02:04.953110 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/clone.py
--rw-r--r--   0        0        0     2979 2023-04-19 18:12:02.225453 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
--rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
--rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0      757 2023-04-19 18:12:02.225538 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/settings.py
--rw-r--r--   0        0        0     5549 2023-04-19 18:12:02.226092 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/testing.py
--rw-r--r--   0        0        0     9882 2023-04-18 16:52:57.349405 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-04-18 16:52:57.349781 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
--rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
--rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
--rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
--rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.8.2/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.8.2/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.8.2/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.8.2/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.8.2/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3820 2023-04-19 15:57:22.494545 lnhub_rest-0.8.2/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1782 2023-04-19 15:57:22.494980 lnhub_rest-0.8.2/noxfile.py
--rw-r--r--   0        0        0     1253 2023-04-18 16:02:04.957709 lnhub_rest-0.8.2/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.8.2/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.8.2/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.8.2/supabase/config.toml
--rw-r--r--   0        0        0      864 2023-04-19 15:57:22.495574 lnhub_rest-0.8.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 lnhub_rest-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-02-13 09:20:16.808732 lnhub_rest-0.9.0/.dockerignore
+-rw-r--r--   0        0        0     3315 2023-04-24 09:52:58.499162 lnhub_rest-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5113 2023-04-20 08:36:06.553682 lnhub_rest-0.9.0/.github/workflows/google-cloudrun-docker.yml
+-rw-r--r--   0        0        0      133 2022-12-05 16:31:02.016205 lnhub_rest-0.9.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-04-12 05:33:51.441718 lnhub_rest-0.9.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1212 2023-04-12 05:33:51.441856 lnhub_rest-0.9.0/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-17 19:46:07.717815 lnhub_rest-0.9.0/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-04-12 05:33:51.441994 lnhub_rest-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-04-17 19:46:07.718176 lnhub_rest-0.9.0/Dockerfile
+-rw-r--r--   0        0        0     1140 2023-04-20 08:36:06.554211 lnhub_rest-0.9.0/README.md
+-rw-r--r--   0        0        0     1754 2023-04-24 11:32:37.183458 lnhub_rest-0.9.0/docs/00-migrate.ipynb
+-rw-r--r--   0        0        0     1189 2023-04-20 08:36:06.554952 lnhub_rest-0.9.0/docs/01-checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0     5218 2023-04-20 08:36:06.555449 lnhub_rest-0.9.0/docs/02-account/01-signup-signin.ipynb
+-rw-r--r--   0        0        0     4487 2023-04-20 08:36:06.555802 lnhub_rest-0.9.0/docs/02-account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5566 2023-04-20 08:36:06.556172 lnhub_rest-0.9.0/docs/02-account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6111 2023-04-24 12:41:04.296948 lnhub_rest-0.9.0/docs/02-account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9088 2023-04-20 08:36:06.556607 lnhub_rest-0.9.0/docs/02-account/05-rls.ipynb
+-rw-r--r--   0        0        0    11211 2023-04-20 10:02:25.484019 lnhub_rest-0.9.0/docs/03-instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5293 2023-04-23 14:15:16.129559 lnhub_rest-0.9.0/docs/03-instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6498 2023-04-24 12:41:04.297311 lnhub_rest-0.9.0/docs/03-instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8667 2023-04-23 14:15:16.130114 lnhub_rest-0.9.0/docs/03-instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     7001 2023-04-20 08:36:06.558037 lnhub_rest-0.9.0/docs/03-instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19423 2023-04-23 19:34:36.515575 lnhub_rest-0.9.0/docs/03-instance/06-rls.ipynb
+-rw-r--r--   0        0        0     3870 2023-04-20 10:02:25.484312 lnhub_rest-0.9.0/docs/04-storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9837 2023-04-20 08:36:06.559024 lnhub_rest-0.9.0/docs/04-storage/02-rls.ipynb
+-rw-r--r--   0        0        0     3894 2023-04-20 08:36:06.559307 lnhub_rest-0.9.0/docs/05-organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     4749 2023-04-24 12:41:04.297609 lnhub_rest-0.9.0/docs/05-organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5892 2023-04-20 08:36:06.559674 lnhub_rest-0.9.0/docs/05-organization/03-rls.ipynb
+-rw-r--r--   0        0        0      125 2023-04-20 08:36:06.559940 lnhub_rest-0.9.0/docs/README.md
+-rw-r--r--   0        0        0    23211 2023-04-24 12:41:39.014596 lnhub_rest-0.9.0/docs/changelog.md
+-rw-r--r--   0        0        0      520 2023-04-12 05:33:51.446631 lnhub_rest-0.9.0/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-04-12 05:33:51.446714 lnhub_rest-0.9.0/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-04-12 05:33:51.447158 lnhub_rest-0.9.0/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0      137 2022-12-05 16:31:02.018378 lnhub_rest-0.9.0/lamin-project.yaml
+-rw-r--r--   0        0        0     3832 2023-04-12 15:45:55.670360 lnhub_rest-0.9.0/lndb/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-03 19:31:19.500521 lnhub_rest-0.9.0/lndb/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-03 19:31:19.500584 lnhub_rest-0.9.0/lndb/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-04-03 19:31:19.500654 lnhub_rest-0.9.0/lndb/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-24 10:07:43.479664 lnhub_rest-0.9.0/lndb/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-04-03 19:31:19.500812 lnhub_rest-0.9.0/lndb/LICENSE
+-rw-r--r--   0        0        0      173 2023-04-03 19:31:19.500865 lnhub_rest-0.9.0/lndb/README.md
+-rw-r--r--   0        0        0       52 2023-04-03 19:31:19.500947 lnhub_rest-0.9.0/lndb/docs/api.md
+-rw-r--r--   0        0        0    47603 2023-04-24 10:07:43.479910 lnhub_rest-0.9.0/lndb/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-04-03 19:31:19.501245 lnhub_rest-0.9.0/lndb/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-04-03 19:31:19.501331 lnhub_rest-0.9.0/lndb/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-04-03 19:31:19.501425 lnhub_rest-0.9.0/lndb/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-04-03 19:31:19.501475 lnhub_rest-0.9.0/lndb/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-24 10:07:43.480335 lnhub_rest-0.9.0/lndb/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-04-03 19:31:19.501612 lnhub_rest-0.9.0/lndb/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-12 15:45:55.670784 lnhub_rest-0.9.0/lndb/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-12 15:45:55.670929 lnhub_rest-0.9.0/lndb/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-03 19:31:19.501804 lnhub_rest-0.9.0/lndb/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-24 10:07:43.480526 lnhub_rest-0.9.0/lndb/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-24 10:07:43.480683 lnhub_rest-0.9.0/lndb/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-24 10:07:43.480795 lnhub_rest-0.9.0/lndb/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-24 11:38:30.442472 lnhub_rest-0.9.0/lndb/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-04-03 19:31:19.502118 lnhub_rest-0.9.0/lndb/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-20 09:03:40.403720 lnhub_rest-0.9.0/lndb/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-04-03 19:31:19.502231 lnhub_rest-0.9.0/lndb/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-24 10:07:43.480911 lnhub_rest-0.9.0/lndb/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-04-03 19:31:19.502354 lnhub_rest-0.9.0/lndb/docs/index.md
+-rw-r--r--   0        0        0      118 2023-04-03 19:31:19.502412 lnhub_rest-0.9.0/lndb/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-24 10:07:43.481042 lnhub_rest-0.9.0/lndb/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-24 10:07:43.481151 lnhub_rest-0.9.0/lndb/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-04-03 19:31:19.502658 lnhub_rest-0.9.0/lndb/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-12 15:45:55.671219 lnhub_rest-0.9.0/lndb/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-24 10:07:43.481253 lnhub_rest-0.9.0/lndb/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-12 15:45:55.671337 lnhub_rest-0.9.0/lndb/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-12 15:45:55.671440 lnhub_rest-0.9.0/lndb/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-04-03 19:31:19.502935 lnhub_rest-0.9.0/lndb/lndb/_info.py
+-rw-r--r--   0        0        0     6051 2023-04-24 10:07:43.481370 lnhub_rest-0.9.0/lndb/lndb/_init_instance.py
+-rw-r--r--   0        0        0     4003 2023-04-20 09:03:40.405278 lnhub_rest-0.9.0/lndb/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-12 15:45:55.671792 lnhub_rest-0.9.0/lndb/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-12 15:45:55.671882 lnhub_rest-0.9.0/lndb/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-24 10:07:43.481495 lnhub_rest-0.9.0/lndb/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-24 10:07:43.481621 lnhub_rest-0.9.0/lndb/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-04-03 19:31:19.503530 lnhub_rest-0.9.0/lndb/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-04-03 19:31:19.503593 lnhub_rest-0.9.0/lndb/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-12 15:45:55.672114 lnhub_rest-0.9.0/lndb/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      700 2023-04-24 10:07:43.481685 lnhub_rest-0.9.0/lndb/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-04-03 19:31:19.503661 lnhub_rest-0.9.0/lndb/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-24 10:07:43.481783 lnhub_rest-0.9.0/lndb/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-20 09:03:40.405705 lnhub_rest-0.9.0/lndb/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-04-03 19:31:19.503836 lnhub_rest-0.9.0/lndb/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-04-03 19:31:19.503900 lnhub_rest-0.9.0/lndb/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-24 10:07:43.481896 lnhub_rest-0.9.0/lndb/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-12 15:45:55.673128 lnhub_rest-0.9.0/lndb/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-04-03 19:31:19.504115 lnhub_rest-0.9.0/lndb/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-12 15:45:55.673226 lnhub_rest-0.9.0/lndb/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-04-03 19:31:19.504235 lnhub_rest-0.9.0/lndb/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-04-03 19:31:19.504287 lnhub_rest-0.9.0/lndb/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-12 15:45:55.673326 lnhub_rest-0.9.0/lndb/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8764 2023-04-24 10:07:43.482063 lnhub_rest-0.9.0/lndb/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-04-03 19:31:19.504528 lnhub_rest-0.9.0/lndb/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-04-03 19:31:19.504583 lnhub_rest-0.9.0/lndb/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-12 15:45:55.673539 lnhub_rest-0.9.0/lndb/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-04-03 19:31:19.504686 lnhub_rest-0.9.0/lndb/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-04-03 19:31:19.504753 lnhub_rest-0.9.0/lndb/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-24 10:07:43.482241 lnhub_rest-0.9.0/lndb/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-24 10:07:43.482348 lnhub_rest-0.9.0/lndb/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-04-03 19:31:19.504960 lnhub_rest-0.9.0/lndb/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-12 15:45:55.673699 lnhub_rest-0.9.0/lndb/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-12 15:45:55.673790 lnhub_rest-0.9.0/lndb/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-03 19:31:19.505138 lnhub_rest-0.9.0/lndb/lndb/test/_env.py
+-rw-r--r--   0        0        0     3870 2023-04-20 09:03:40.406913 lnhub_rest-0.9.0/lndb/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-12 15:45:55.673887 lnhub_rest-0.9.0/lndb/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-04-03 19:31:19.505348 lnhub_rest-0.9.0/lndb/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-04-03 19:31:19.505408 lnhub_rest-0.9.0/lndb/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-12 15:45:55.673980 lnhub_rest-0.9.0/lndb/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-24 10:07:43.482453 lnhub_rest-0.9.0/lndb/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-12 15:45:55.674169 lnhub_rest-0.9.0/lndb/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-04-03 19:31:19.505727 lnhub_rest-0.9.0/lndb/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-20 09:03:40.407355 lnhub_rest-0.9.0/lndb/tests/test_notebooks.py
+-rw-r--r--   0        0        0      157 2023-04-24 12:41:11.914101 lnhub_rest-0.9.0/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     8011 2023-04-20 08:36:06.561011 lnhub_rest-0.9.0/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       64 2023-02-13 09:20:16.812158 lnhub_rest-0.9.0/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0     1026 2023-02-13 09:20:16.812240 lnhub_rest-0.9.0/lnhub_rest/_assets/_instances.py
+-rw-r--r--   0        0        0     1094 2023-04-23 14:15:16.131245 lnhub_rest-0.9.0/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-04-19 06:39:29.557169 lnhub_rest-0.9.0/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0      998 2023-04-20 08:36:06.561252 lnhub_rest-0.9.0/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5726 2023-04-20 08:36:06.561589 lnhub_rest-0.9.0/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0       42 2023-04-12 05:33:51.449892 lnhub_rest-0.9.0/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-17 19:46:07.724724 lnhub_rest-0.9.0/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2542 2023-04-23 14:15:16.131687 lnhub_rest-0.9.0/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-04-12 05:33:51.450294 lnhub_rest-0.9.0/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      739 2023-04-20 08:36:06.562096 lnhub_rest-0.9.0/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3325 2023-04-20 08:36:06.562360 lnhub_rest-0.9.0/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1423 2023-04-20 08:36:06.562595 lnhub_rest-0.9.0/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-04-12 05:33:51.451054 lnhub_rest-0.9.0/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     3056 2023-04-24 12:41:04.298412 lnhub_rest-0.9.0/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-04-12 05:33:51.451365 lnhub_rest-0.9.0/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-12 05:33:51.451441 lnhub_rest-0.9.0/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1284 2023-04-20 08:36:06.563067 lnhub_rest-0.9.0/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6751 2023-04-23 14:15:16.132067 lnhub_rest-0.9.0/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1532 2023-04-20 08:36:06.563609 lnhub_rest-0.9.0/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1067 2023-04-20 08:36:06.563842 lnhub_rest-0.9.0/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-04-17 19:46:07.726669 lnhub_rest-0.9.0/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-04-17 19:46:07.726929 lnhub_rest-0.9.0/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-04-12 05:33:51.452504 lnhub_rest-0.9.0/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     2861 2023-04-20 08:36:06.564078 lnhub_rest-0.9.0/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-04-12 05:33:51.452880 lnhub_rest-0.9.0/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      796 2023-04-17 19:46:07.727862 lnhub_rest-0.9.0/lnhub_rest/main.py
+-rw-r--r--   0        0        0       39 2023-04-20 08:36:06.564287 lnhub_rest-0.9.0/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-12 05:33:51.453184 lnhub_rest-0.9.0/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     2543 2023-04-20 08:36:06.564910 lnhub_rest-0.9.0/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      198 2023-04-17 19:46:07.728270 lnhub_rest-0.9.0/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4661 2023-04-24 12:41:04.298691 lnhub_rest-0.9.0/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-04-12 05:33:51.454358 lnhub_rest-0.9.0/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0      408 2023-04-12 05:33:51.454427 lnhub_rest-0.9.0/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     5233 2023-04-24 12:41:04.298930 lnhub_rest-0.9.0/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-04-17 19:46:07.729123 lnhub_rest-0.9.0/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1074 2023-04-20 08:36:06.565374 lnhub_rest-0.9.0/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-04-19 06:39:29.557427 lnhub_rest-0.9.0/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-04-17 19:46:07.730209 lnhub_rest-0.9.0/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-03-02 11:17:31.752043 lnhub_rest-0.9.0/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-04-17 19:46:07.730671 lnhub_rest-0.9.0/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-03-02 11:17:31.752112 lnhub_rest-0.9.0/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-04-12 05:33:51.456009 lnhub_rest-0.9.0/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-02-13 09:20:16.814087 lnhub_rest-0.9.0/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       50 2023-04-17 19:46:07.731071 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-17 19:46:07.731439 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     2979 2023-04-17 19:46:07.731705 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-04-12 05:33:51.456564 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-04-17 19:46:07.731951 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-04-17 19:46:07.732205 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-04-12 05:33:51.457356 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-04-12 05:33:51.457588 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-04-12 05:33:51.457841 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-04-17 19:46:07.732575 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-04-17 19:46:07.732918 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-04-17 19:46:07.733294 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-04-17 19:46:07.733539 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-04-19 06:39:29.557590 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-04-12 05:33:51.459308 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-02-13 09:20:16.814349 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0      757 2023-04-12 05:33:51.459425 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/settings.py
+-rw-r--r--   0        0        0     5549 2023-04-20 08:36:06.565790 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     9882 2023-04-20 08:36:06.566134 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-04-20 08:36:06.566367 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-04-12 05:33:51.460064 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-04-12 05:33:51.460238 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-04-17 19:46:07.734101 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-04-17 19:46:07.734436 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-04-17 19:46:07.734632 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-04-17 19:46:07.734875 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-04-19 06:39:29.557744 lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-03-02 11:17:31.752459 lnhub_rest-0.9.0/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-04-17 19:46:07.735238 lnhub_rest-0.9.0/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-12 05:33:51.461642 lnhub_rest-0.9.0/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-04-17 19:46:07.735507 lnhub_rest-0.9.0/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-04-12 05:33:51.461902 lnhub_rest-0.9.0/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3820 2023-04-20 08:36:06.566596 lnhub_rest-0.9.0/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1842 2023-04-24 12:41:04.299217 lnhub_rest-0.9.0/noxfile.py
+-rw-r--r--   0        0        0     1253 2023-04-17 19:46:07.736606 lnhub_rest-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-04-12 05:33:51.462685 lnhub_rest-0.9.0/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-04-12 05:33:51.462759 lnhub_rest-0.9.0/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-04-12 05:33:51.462840 lnhub_rest-0.9.0/supabase/config.toml
+-rw-r--r--   0        0        0      864 2023-04-20 08:36:06.567005 lnhub_rest-0.9.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 lnhub_rest-0.9.0/PKG-INFO
```

### Comparing `lnhub_rest-0.8.2/.dockerignore` & `lnhub_rest-0.9.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/.github/workflows/build.yml` & `lnhub_rest-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/.github/workflows/google-cloudrun-docker.yml` & `lnhub_rest-0.9.0/.github/workflows/google-cloudrun-docker.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/.gitignore` & `lnhub_rest-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/.pre-commit-config.yaml` & `lnhub_rest-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/README.md` & `lnhub_rest-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/00-migrate.ipynb` & `lnhub_rest-0.9.0/docs/00-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/01-checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.9.0/docs/01-checks/01-check-break-lndb.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/02-account/01-signup-signin.ipynb` & `lnhub_rest-0.9.0/docs/02-account/01-signup-signin.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/02-account/02-create-account.ipynb` & `lnhub_rest-0.9.0/docs/02-account/02-create-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/02-account/03-update-account.ipynb` & `lnhub_rest-0.9.0/docs/02-account/03-update-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/02-account/04-fetch-account.ipynb` & `lnhub_rest-0.9.0/docs/02-account/04-fetch-account.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977872670807453%*

 * *Differences: {"'cells'": '{15: {\'source\': {insert: [(2, \'        **instance,\\n\'), (3, \'        "storage": '*

 * *            '{"root": storage["root"]},\\n\'), (4, \'        "account": {"handle": account_handle, '*

 * *            '"id": account_id},\\n\')], delete: [6, 5, 4, 3, 2]}}, 17: {\'source\': {insert: [(0, '*

 * *            '\'instances = get_account_instances(account_handle, False, f"Bearer '*

 * *            '{access_token}")\\n\')], delete: [0]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.12'}}"}*

```diff
@@ -167,19 +167,17 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "account_instances_expected = [\n",
                 "    {\n",
-                "        **instance_collaborator,\n",
-                "        \"instance\": {\n",
-                "            **instance,\n",
-                "            \"account\": {\"handle\": account_handle, \"id\": account_id},\n",
-                "        },\n",
+                "        **instance,\n",
+                "        \"storage\": {\"root\": storage[\"root\"]},\n",
+                "        \"account\": {\"handle\": account_handle, \"id\": account_id},\n",
                 "    }\n",
                 "]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -189,15 +187,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "instances = get_account_instances(account_handle, f\"Bearer {access_token}\")\n",
+                "instances = get_account_instances(account_handle, False, f\"Bearer {access_token}\")\n",
                 "assert DeepDiff(instances, account_instances_expected, ignore_order=True) == {}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -256,15 +254,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.2/docs/02-account/05-rls.ipynb` & `lnhub_rest-0.9.0/docs/02-account/05-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/03-instance/01-init-instance.ipynb` & `lnhub_rest-0.9.0/docs/03-instance/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/03-instance/02-load-instance.ipynb` & `lnhub_rest-0.9.0/docs/03-instance/02-load-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999580472921434%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(7, \'existing_storage_root = "s3://lnhub-rest-ci"\\n\')], '*

 * *            "delete: [7]}}, 15: {'source': {insert: [(1, 'assert storage.region == "*

 * *            '"eu-central-1"\')], delete: [1]}}}'}*

```diff
@@ -52,15 +52,15 @@
                 "hub = connect_hub()\n",
                 "\n",
                 "auth = create_test_auth()\n",
                 "access_token = auth[\"access_token\"]\n",
                 "account = create_test_account(handle=auth[\"handle\"], access_token=access_token)\n",
                 "handle = account[\"handle\"]\n",
                 "\n",
-                "existing_storage_root = \"s3://lndb-setup-ci\"\n",
+                "existing_storage_root = \"s3://lnhub-rest-ci\"\n",
                 "instance_name = f\"lamin.ci.instance.{base26(6)}\"\n",
                 "db = f\"postgresql://postgres:pwd@0.0.0.0:5432/{instance_name}\"\n",
                 "\n",
                 "init_instance(\n",
                 "    owner=handle,\n",
                 "    name=instance_name,\n",
                 "    storage=existing_storage_root,\n",
@@ -154,15 +154,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert storage.root == existing_storage_root\n",
-                "assert storage.region == \"us-east-1\""
+                "assert storage.region == \"eu-central-1\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
```

### Comparing `lnhub_rest-0.8.2/docs/03-instance/03-update-instance.ipynb` & `lnhub_rest-0.9.0/docs/03-instance/03-update-instance.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886080586080586%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(6, \'instance_id = instance["id"]\')], delete: [13, 12, '*

 * *            "11, 10, 9, 8, 6, 5]}}, insert: [(4, OrderedDict([('cell_type', 'markdown'), "*

 * *            "('metadata', OrderedDict()), ('source', ['## Add a collaborator'])])), (5, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            "OrderedDict()), ('outputs', []), ('source', ['response = client.post(\\n', '    "*

 * *            'f"/instance/resources/accounts/?h […]*

```diff
@@ -43,22 +43,36 @@
             "source": [
                 "auth = create_test_auth()\n",
                 "access_token = auth[\"access_token\"]\n",
                 "account = create_test_account(handle=auth[\"handle\"], access_token=access_token)\n",
                 "storage = create_test_storage(access_token=access_token)\n",
                 "instance = create_test_instance(storage_id=storage[\"id\"], access_token=access_token)\n",
                 "\n",
-                "instance_id = instance[\"id\"]\n",
+                "instance_id = instance[\"id\"]"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Add a collaborator"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "response = client.post(\n",
+                "    f\"/instance/resources/accounts/?handle={account['handle']}&instance_id={instance_id}&role=admin\",\n",
+                "    headers={\"authentication\": f\"Bearer {access_token}\"},\n",
+                ").json()\n",
                 "\n",
-                "add_test_collaborator(\n",
-                "    instance_id=instance_id,\n",
-                "    account_id=account[\"id\"],\n",
-                "    role=\"admin\",\n",
-                "    access_token=access_token,\n",
-                ")"
+                "assert response == \"success\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Update an instance"
@@ -262,15 +276,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.8.2/docs/03-instance/04-delete-instance.ipynb` & `lnhub_rest-0.9.0/docs/03-instance/04-delete-instance.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999803921568627%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(16, 'existing_storage_root = "*

 * *            '"s3://lnhub-rest-ci"\\n\')], delete: [16]}}}'}*

```diff
@@ -73,15 +73,15 @@
                 "# Create account 2\n",
                 "auth_2 = create_test_auth()\n",
                 "access_token_2 = auth_2[\"access_token\"]\n",
                 "account_2 = create_test_account(handle=auth_2[\"handle\"], access_token=access_token_2)\n",
                 "handle_2 = account_2[\"handle\"]\n",
                 "account_hub_2 = connect_hub_with_auth(access_token=access_token_2)\n",
                 "\n",
-                "existing_storage_root = \"s3://lndb-setup-ci\"\n",
+                "existing_storage_root = \"s3://lnhub-rest-ci\"\n",
                 "\n",
                 "instance_name_1 = f\"lamin.ci.instance.{base26(6)}\"\n",
                 "db_1 = f\"postgresql://postgres:pwd@0.0.0.0:5432/{instance_name_1}\"\n",
                 "\n",
                 "instance_name_2 = f\"lamin.ci.instance.{base26(6)}\"\n",
                 "db_2 = f\"postgresql://postgres:pwd@0.0.0.0:5432/{instance_name_2}\"\n",
                 "\n",
```

### Comparing `lnhub_rest-0.8.2/docs/03-instance/05-fetch-instance.ipynb` & `lnhub_rest-0.9.0/docs/03-instance/05-fetch-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/03-instance/06-rls.ipynb` & `lnhub_rest-0.9.0/docs/03-instance/06-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/04-storage/01-add-storage.ipynb` & `lnhub_rest-0.9.0/docs/04-storage/01-add-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/04-storage/02-rls.ipynb` & `lnhub_rest-0.9.0/docs/04-storage/02-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/05-organization/01-create-organization.ipynb` & `lnhub_rest-0.9.0/docs/05-organization/01-create-organization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/05-organization/02-manage-members.ipynb` & `lnhub_rest-0.9.0/docs/05-organization/02-manage-members.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9726984126984127%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, 'from lnhub_rest.routers.account import "*

 * *            "get_account_organizations\\n')]}}, insert: [(4, OrderedDict([('cell_type', "*

 * *            '\'markdown\'), (\'metadata\', OrderedDict()), (\'source\', ["## Test fetching of '*

 * *            'account\'s organizations"])])), (5, OrderedDict([(\'cell_type\', \'code\'), '*

 * *            "('execution_count', None), ('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            "['organizations = client.get(\\n', '    […]*

```diff
@@ -13,14 +13,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import sqlmodel as sqm\n",
                 "\n",
                 "# Test assets\n",
                 "from lnhub_rest.core.account import create_organization_account\n",
+                "from lnhub_rest.routers.account import get_account_organizations\n",
                 "\n",
                 "# Test utils\n",
                 "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
                 "from lnhub_rest.orm._sbclient import connect_hub_with_auth\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci\n",
                 "from lnhub_rest.utils._id import base62"
@@ -58,14 +59,43 @@
                 "organization_id = (\n",
                 "    hub.table(\"account\").select(\"id\").eq(\"handle\", org_handle_1).execute().data[0][\"id\"]\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Test fetching of account's organizations"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "organizations = client.get(\n",
+                "    f\"/account/resources/organizations/{account_1['handle']}\",\n",
+                "    headers={\"authentication\": f\"Bearer {access_token_1}\"},\n",
+                ").json()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "assert len(organizations) == 1\n",
+                "assert organizations[0][\"account\"][\"handle\"] == org_handle_1"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "## Test addition of a member "
             ]
         },
@@ -154,13 +184,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lnhub_rest-0.8.2/docs/05-organization/03-rls.ipynb` & `lnhub_rest-0.9.0/docs/05-organization/03-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/changelog.md` & `lnhub_rest-0.9.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🔖  Staging version 0.9.0 | [170](https://github.com/laminlabs/lnhub-rest/pull/170) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.9.0
+🎨 Redesign acct-instances endpoint | [190](https://github.com/laminlabs/lnhub-rest/pull/190) | [bpenteado](https://github.com/bpenteado) | 2023-04-23 |
+✨ Create add-collaborator endpoint | [189](https://github.com/laminlabs/lnhub-rest/pull/189) | [bpenteado](https://github.com/bpenteado) | 2023-04-23 |
+🎨 Enrich account organizations endpoint | [188](https://github.com/laminlabs/lnhub-rest/pull/188) | [bpenteado](https://github.com/bpenteado) | 2023-04-23 |
 🍱  Add schema module `lamin1` | [187](https://github.com/laminlabs/lnhub-rest/pull/187) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.8.2
 :children_crossing: Ask for postgresql instead of postgres | [186](https://github.com/laminlabs/lnhub-rest/pull/186) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 |
 👷 Run tests on staging | [179](https://github.com/laminlabs/lnhub-rest/pull/179) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 ✅ Decouple tests from lndb-related objects | [184](https://github.com/laminlabs/lnhub-rest/pull/184) | [bpenteado](https://github.com/bpenteado) | 2023-04-20 |
 💚 Fix tests | [178](https://github.com/laminlabs/lnhub-rest/pull/178) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 🚚 Rename folders in docs | [177](https://github.com/laminlabs/lnhub-rest/pull/177) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 🏗️ Clean up historical migrations & remove cloning from production for migrations testing | [175](https://github.com/laminlabs/lnhub-rest/pull/175) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
```

### Comparing `lnhub_rest-0.8.2/docs/migrations.md` & `lnhub_rest-0.9.0/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.9.0/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/.github/workflows/build.yml` & `lnhub_rest-0.9.0/lndb/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.0/lndb/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/.gitignore` & `lnhub_rest-0.9.0/lndb/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/.pre-commit-config.yaml` & `lnhub_rest-0.9.0/lndb/.pre-commit-config.yaml`

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

### Comparing `lnhub_rest-0.8.2/lndb/LICENSE` & `lnhub_rest-0.9.0/lndb/LICENSE`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/changelog.md` & `lnhub_rest-0.9.0/lndb/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Allow to set additional fsspec kwargs for cloud instances | [366](https://github.com/laminlabs/lndb/pull/366) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 | 0.44.3
+⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
+🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
+🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
+🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
+🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
+👷 Remove lnhub-rest CI calls | [360](https://github.com/laminlabs/lndb/pull/360) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
+🚸 Enable non-owner to set storage | [358](https://github.com/laminlabs/lndb/pull/358) | [falexwolf](https://github.com/falexwolf) | 2023-04-19 |
 ♻️ Restructure hub imports | [357](https://github.com/laminlabs/lndb/pull/357) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 |
 ⬆️ Upgrade to lnhub_rest 0.8.1 | [356](https://github.com/laminlabs/lndb/pull/356) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 | 0.42.0
 ✅ Use nbproject-test directly | [355](https://github.com/laminlabs/lndb/pull/355) | [Koncopd](https://github.com/Koncopd) | 2023-04-18 |
 🔊 Clarify access based on locally cached instance metadata | [354](https://github.com/laminlabs/lndb/pull/354) | [falexwolf](https://github.com/falexwolf) | 2023-04-11 | 0.41.0
 🎨 Move setup checks from lamindb here | [352](https://github.com/laminlabs/lndb/pull/352) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 | 0.41rc1
 🔧 Increase configure-aws-credentials version from v1 to v2 | [344](https://github.com/laminlabs/lndb/pull/344) | [Zethson](https://github.com/Zethson) | 2023-04-07 |
 🚸 Expose `id` in `StorageSettings` | [351](https://github.com/laminlabs/lndb/pull/351) | [falexwolf](https://github.com/falexwolf) | 2023-04-07 | 0.40.2
```

### Comparing `lnhub_rest-0.8.2/lndb/docs/faq/check-synchronization.ipynb` & `lnhub_rest-0.9.0/lndb/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/faq/clone.ipynb` & `lnhub_rest-0.9.0/lndb/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/faq/edge-cases-login-init.ipynb` & `lnhub_rest-0.9.0/lndb/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/faq/manage-migrations.ipynb` & `lnhub_rest-0.9.0/lndb/docs/faq/manage-migrations.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'cells'": '{3: {\'source\': [\'# lndb.migrate.generate(package_name="lnschema_core")\']}}'}*

```diff
@@ -29,15 +29,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lndb.migrate.generate(package_name=\"lnschema_core\")"
+                "# lndb.migrate.generate(package_name=\"lnschema_core\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lnhub_rest-0.8.2/lndb/docs/faq/switch-environment.ipynb` & `lnhub_rest-0.9.0/lndb/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-e2e.ipynb` & `lnhub_rest-0.9.0/lndb/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/faq/test-migrations-unit.ipynb` & `lnhub_rest-0.9.0/lndb/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/01-setup-user.ipynb` & `lnhub_rest-0.9.0/lndb/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/02-init-instance.ipynb` & `lnhub_rest-0.9.0/lndb/docs/guide/02-init-instance.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9863140792031098%*

 * *Differences: {"'cells'": '{3: {\'source\': [\'ln.setup.login("testuser1")  # CLI: lamin login testuser1\']}, 6: '*

 * *            "{'source': {insert: [(1, '!lamin init --storage ./mydata\\n')], delete: [1]}, "*

 * *            "'attachments': OrderedDict()}, 8: {'source': ['This automatically assigns an instance "*

 * *            "name that equals the name of the storage root along with a few other settings:'], "*

 * *            "'attachments': OrderedDict()}, 9: {'source': ['ln.setup.settings.instance']}, 18: "*

 * *            "{'source': […]*

```diff
@@ -29,15 +29,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.login(\"testuser1\")  # shell: lamin login testuser1"
+                "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Init a local instance"
@@ -47,45 +47,47 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### SQLite"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```\n",
-                "!lamin init --storage mydata\n",
+                "!lamin init --storage ./mydata\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(storage=\"./mydata\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This automatically assigns an instance name that equals the name of the storage root:"
+                "This automatically assigns an instance name that equals the name of the storage root along with a few other settings:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.settings.instance.name"
+                "ln.setup.settings.instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -184,31 +186,28 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "# clean up settings\n",
-                "ln.setup.delete(\"pgtest\")"
+                "!lamin delete pgtest\n",
+                "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
-            "source": [
-                "# clean up docker\n",
-                "!docker stop pgtest && docker rm pgtest"
-            ]
+            "source": []
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Provide a custom instance name"
             ]
@@ -256,15 +255,18 @@
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.dialect == \"postgresql\"\n",
                 "assert ln.setup.settings.instance.db == pgurl\n",
                 "assert (\n",
                 "    ln.setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"mystorage\").absolute().as_posix()\n",
                 ")\n",
-                "assert ln.setup.settings.instance.storage.cache_dir is None"
+                "assert ln.setup.settings.instance.storage.cache_dir is None\n",
+                "\n",
+                "!lamin delete mydata2\n",
+                "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Configure with cloud storage"
@@ -305,42 +307,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.settings.instance.name"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.storage.root"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.storage.cache_dir"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.settings.instance.db"
+                "ln.setup.settings.instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -432,14 +407,58 @@
                 "ln.setup.delete(\"lndb-setup-ci-us\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Register a local instance on the hub"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pgurl = setup_local_test_postgres(name=\"pgtest-registered\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "```\n",
+                "!lamin init --storage ./mydatapg --name pgtest-registered --hub\n",
+                "```"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.init(storage=\"s3://lndb-setup-ci\", db=pgurl)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.register()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Re-initializing an existing instance"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/03-load-instance.ipynb` & `lnhub_rest-0.9.0/lndb/docs/guide/03-load-instance.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928039965986395%*

 * *Differences: {"'cells'": '{7: {\'source\': {insert: [(1, \'ln.setup.load("pgtest-registered")\\n\'), (2, '*

 * *            "'assert settings.instance.storage.is_cloud == True\\n'), (3, 'assert "*

 * *            'settings.instance.name == "pgtest-registered"\\n\'), (4, \'assert '*

 * *            'settings.instance.storage.root_as_str == "s3://lndb-setup-ci"\')], delete: [5, 4, 3, '*

 * *            "2, 1]}}, 11: {'source': {insert: [(1, 'assert settings.instance.storage.root_as_str "*

 * *            '== "s3://lndb-setup-ci"\\n\'), (2, \'asse […]*

```diff
@@ -85,19 +85,18 @@
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# another test case, this time with a manually configured instance name\n",
-                "ln.setup.load(\"mydata2\")\n",
-                "assert settings.instance.storage.is_cloud == False\n",
-                "assert settings.instance.name == \"mydata2\"\n",
-                "assert settings.instance.storage.root.as_posix() == f\"{os.getcwd()}/mystorage\"\n",
-                "assert settings.instance.storage.cache_dir is None"
+                "ln.setup.load(\"pgtest-registered\")\n",
+                "assert settings.instance.storage.is_cloud == True\n",
+                "assert settings.instance.name == \"pgtest-registered\"\n",
+                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3f47a1d4",
             "metadata": {},
             "source": [
@@ -137,16 +136,18 @@
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "assert settings.instance.storage.is_cloud == True\n",
-                "assert str(settings.instance.storage.root) == \"s3://lndb-setup-ci/\"\n",
-                "assert str(settings.instance._sqlite_file) == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\""
+                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
+                "assert (\n",
+                "    settings.instance._sqlite_file.as_posix() == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "914af9a6",
             "metadata": {},
             "source": [
@@ -215,30 +216,16 @@
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "# clean up\n",
-                "ln.setup.delete(\"mydata2\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "35c91d7f-8fbf-455f-ae61-6690eaf29154",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "# clean up\n",
-                "!docker stop pgtest && docker rm pgtest"
+                "!lamin delete pgtest-registered\n",
+                "!docker stop pgtest-registered && docker rm pgtest-registered"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/04-set-storage.ipynb` & `lnhub_rest-0.9.0/lndb/docs/guide/04-set-storage.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672351953601954%*

 * *Differences: {"'cells'": "{1: {'source': ['import lamindb as ln\\n', 'from pathlib import Path\\n', 'import "*

 * *            "laminci']}, 3: {'source': ['pgurl = laminci.db.setup_local_test_postgres()']}, 5: "*

 * *            "{'source': {insert: [(2, '!lamin set --storage ./storage_2\\n')], delete: [2]}}, 7: "*

 * *            "{'metadata': {'tags': []}, 'source': ['assert ln.setup.settings.storage.root_as_str "*

 * *            '== f"{Path.cwd()}/storage_2"\']}, 10: {\'source\': [\'assert '*

 * *            "ln.setup.settings.storage.is_cl […]*

```diff
@@ -13,15 +13,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb as ln"
+                "import lamindb as ln\n",
+                "from pathlib import Path\n",
+                "import laminci"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a7cf42fb",
             "metadata": {},
             "source": [
@@ -35,17 +37,15 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "import lndb\n",
-                "\n",
-                "pgurl = lndb.dev.setup_local_test_postgres()"
+                "pgurl = laminci.db.setup_local_test_postgres()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d6b0bd5e",
             "metadata": {},
@@ -57,15 +57,15 @@
         {
             "cell_type": "markdown",
             "id": "ceb57cc9",
             "metadata": {},
             "source": [
                 "Running \n",
                 "```\n",
-                "!lamin set --storage storage_2\n",
+                "!lamin set --storage ./storage_2\n",
                 "```\n",
                 "on the command line runs the following Python function:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -77,23 +77,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8e481aa0",
             "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
+                "tags": []
             },
             "outputs": [],
             "source": [
-                "from pathlib import Path\n",
-                "\n",
-                "assert ln.setup.settings.instance.storage.root.as_posix() == f\"{Path.cwd()}/storage_2\""
+                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "25a13298",
             "metadata": {},
             "source": [
@@ -122,16 +118,57 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.settings.instance.storage.is_cloud == True\n",
-                "assert str(ln.setup.settings.instance.storage.root) == \"s3://lndb-setup-ci/\""
+                "assert ln.setup.settings.storage.is_cloud\n",
+                "assert ln.setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\""
+            ]
+        },
+        {
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
             ]
         },
         {
             "cell_type": "markdown",
             "id": "529e68e5-9b10-4fdb-9d4c-ac8206bbbb68",
             "metadata": {},
             "source": [
@@ -151,21 +188,33 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2ed8716f-852f-4ce9-8eef-5b824d6e92b3",
             "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "ln.setup.set.storage(\"./storage_3\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "cad87623",
+            "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.set.storage(\"storage_3\") == \"only-owner-can-set-storage\""
+                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "78a819fa-48d6-4c6f-95d4-7dc7e94283bb",
             "metadata": {
@@ -175,15 +224,14 @@
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
@@ -218,17 +266,15 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e4f2545f",
             "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
+                "tags": []
             },
             "outputs": [],
             "source": [
                 "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\""
             ]
         },
         {
@@ -244,29 +290,29 @@
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

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/05-schema-modules.ipynb` & `lnhub_rest-0.9.0/lndb/docs/guide/05-schema-modules.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969494047619047%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(1, '!lamin init --storage mydata2 --schema "*

 * *            "bionty,lamin1\\n')], delete: [1]}, 'attachments': OrderedDict()}, 8: {'source': "*

 * *            '[\'ln.setup.init(storage="mydata2", schema="bionty,lamin1")\']}, 18: {\'source\': '*

 * *            '[\'ln.setup.init(storage="mydata2", schema="bionty,lamin1", db=pgurl)\']}}'}*

```diff
@@ -52,29 +52,30 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Mount schema modules bionty and wetlab"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```\n",
-                "!lamin init --storage mydata2 --schema bionty,wetlab\n",
+                "!lamin init --storage mydata2 --schema bionty,lamin1\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,wetlab\")"
+                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -150,15 +151,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,wetlab\", db=pgurl)"
+                "ln.setup.init(storage=\"mydata2\", schema=\"bionty,lamin1\", db=pgurl)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/06-info.ipynb` & `lnhub_rest-0.9.0/lndb/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/07-delete.ipynb` & `lnhub_rest-0.9.0/lndb/docs/guide/07-delete.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9674479166666666%*

 * *Differences: {"'cells'": "{1: {'source': ['import lamindb as ln']}, 2: {'source': "*

 * *            '[\'ln.setup.login("testuser1")\']}, 4: {\'source\': '*

 * *            '[\'ln.setup.init(storage="mydata-delete")\']}, 6: {\'source\': '*

 * *            '[\'ln.setup.delete("mydata-delete")\']}, 7: {\'metadata\': {replace: '*

 * *            "OrderedDict([('tags', ['hide-cell'])])}, 'source': {insert: [(0, 'from "*

 * *            "lndb.dev._settings_store import instance_settings_file\\n'), (1, '\\n'), (2, "*

 * *            '\'settings_file = ins […]*

```diff
@@ -13,28 +13,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lndb import delete, load, login, init, settings\n",
-                "from lndb.dev._settings_store import instance_settings_file\n",
-                "from pathlib import Path\n",
-                "from datetime import datetime"
+                "import lamindb as ln"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "485f5ee1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "login(\"testuser1\")"
+                "ln.setup.login(\"testuser1\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "cceb6b43",
             "metadata": {},
             "source": [
@@ -44,16 +41,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2609e58d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "init(storage=\"mydata-delete\")\n",
-                "settings_file = instance_settings_file(\"mydata-delete\", \"testuser1\")"
+                "ln.setup.init(storage=\"mydata-delete\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "25a13298",
             "metadata": {},
             "source": [
@@ -66,83 +62,60 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8436575d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "delete(\"mydata-delete\")"
+                "ln.setup.delete(\"mydata-delete\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d2e607c9",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
+                "from lndb.dev._settings_store import instance_settings_file\n",
+                "\n",
+                "settings_file = instance_settings_file(\"mydata-delete\", \"testuser1\")\n",
                 "assert settings_file.exists() == False"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3286fbcc",
             "metadata": {},
             "source": [
                 "## With remote default storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fa1efbce",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "instance_name = f\"lamin.ci.instance.{datetime.now().timestamp()}\""
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "037f38a3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "init(storage=\"s3://lndb-setup-delete-ci\", name=instance_name)"
+                "ln.setup.init(storage=\"s3://lndb-setup-delete-ci\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b2593ef8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "delete(instance_name)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "06a22900",
-            "metadata": {},
-            "source": [
-                "Clean up instances."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9117428e",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from lnhub_rest._clean_ci import delete_ci_instances\n",
-                "\n",
-                "delete_ci_instances()"
+                "ln.setup.delete(\"lndb-setup-delete-ci\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `lnhub_rest-0.8.2/lndb/docs/guide/migrate.md` & `lnhub_rest-0.9.0/lndb/docs/guide/migrate.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 ```
 
 This page documents how to create a tested migration using the CI-guided workflow for postgres-based instances.
 
 1. Create a new branch (e.g. `migr`) in your repository: Update an ORM, e.g., by renaming a column.
 
    :::{dropdown} Example: Rename a column.
-   Let's try to rename the `v` column to `version` in `Notebook` table of `lnschema_core`.
+   Let's try to rename the `version` column to `v` in the `Transform` ORM of `lnschema_core`.
 
-   In the `lnschema_core/_core.py` `Notebook` class, modify line:
+   In the `lnschema_core/_core.py` `Transform` ORM, modify line:
 
    ```{code-block} python
    ---
    emphasize-lines: 1, 3
    ---
-   v: str = Field(default="1", primary_key=True)
-   to:
    version: str = Field(default="1", primary_key=True)
+   to:
+   v: str = Field(default="1", primary_key=True)
    ```
 
    :::
 
-2. On the command line (at the root of the repository), run `lamin migrate generate` to generate an empty script file under `{package_name}/migrations/versions/`.
+2. On the command line (at the root of the repository), run `lamin migrate generate` to generate a migration script under `{package_name}/migrations/versions/`.
 
    :::{dropdown} Example
 
    Migration script location: The script will be named `{date}-{revision}-vx_x_x.py`.
 
    ```{code-block} yaml
    ---
@@ -42,15 +42,15 @@
    |-- migrations
    |   |-- versions
    |       |-- 2023-02-16-dd2b4a9499f2-vx_x_x.py
    |-- __init__.py
    |-- _core.py
    ```
 
-   Content of migration script.
+   Example of an empty migration script.
 
    ```{code-block} python
    ---
    emphasize-lines: 10
    ---
    """vX.X.X."""
    from alembic import op
@@ -73,25 +73,25 @@
 
    ```{code-block} python
    _migration = "dd2b4a9499f2"
    ```
 
    :::
 
-3. Commit all changes, create a pull request from the `migr` branch, and inspect the output of the failing CI step `Build`.
+3. Commit all changes, create a pull request from the `migr` branch, and inspect the CI step `Build`.
 
    :::{dropdown} Example: Bottom of failed CI output.
 
    ```{code-block} python
    op.alter_column("notebook", column_name="v", new_column_name="version", schema="core")
    ```
 
    :::
 
-4. Copy the suggested changes into the `update()` function in the `{date}-{revision}-vx_x_x.py` file.
+4. In case CI failed, copy the suggested changes into the `update()` function in the `{date}-{revision}-vx_x_x.py` file.
    Commit & push changes: Now CI should pass! 🎉
 
    :::{dropdown} Example: Modified migration script.
 
    ```{code-block} python
    def upgrade() -> None:
        op.alter_column("notebook", column_name="v", new_column_name="version", schema="core")
```

### Comparing `lnhub_rest-0.8.2/lndb/lndb/__init__.py` & `lnhub_rest-0.9.0/lndb/lndb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 .. autosummary::
    :toctree:
 
    close
    delete
    info
    set
+   register
 
 Manage creating and testing migrations (deployment is automatic):
 
 .. autosummary::
    :toctree:
 
    migrate
@@ -46,27 +47,28 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.42.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.3"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
 from ._delete import delete  # noqa
 from ._info import info  # noqa
 from ._init_instance import init  # noqa
 from ._load_instance import load  # noqa
 from ._migrate import migrate
+from ._register_instance import register  # noqa
 from ._schema import schema  # noqa
 from ._set import set, set_storage  # noqa
 from ._settings import settings  # noqa
 from ._setup_user import login, signup  # noqa
 
 
 # unlock and clear even if an uncaught exception happens
```

### Comparing `lnhub_rest-0.8.2/lndb/lndb/__main__.py` & `lnhub_rest-0.9.0/lndb/lndb/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import argparse
 import os
 import sys
 
 from lamin_logger import logger
 
-from . import _init_instance, _setup_user, delete, info, set_storage
+from . import _init_instance, _setup_user, delete, info, register, set
 from ._close import close as close_instance
 from ._init_instance import description as instance
 from .dev._settings_user import user_description as user
 
 signup_help = "First time sign up."
 login_help = "Log in an already-signed-up user."
 init_help = "Init & config instance with db & storage."
 load_help = "Load instance by name."
 set_storage_help = "Set storage used by an instance."
 info_help = "Show current instance information."
 close_help = "Close instance."
 migr_help = "Manage migrations."
 delete_help = "Delete an instance."
+register_help = (
+    "Register instance on hub (local instances are not automatically registered)."
+)
+
 
 description_cli = "Configure LaminDB and perform simple actions."
 parser = argparse.ArgumentParser(
     description=description_cli, formatter_class=argparse.RawTextHelpFormatter
 )
 subparsers = parser.add_subparsers(dest="command")
 
@@ -67,15 +71,18 @@
 
 # set storage
 set_storage_parser = subparsers.add_parser("set", help=set_storage_help)
 aa = set_storage_parser.add_argument
 aa("--storage", type=str, metavar="s", help=instance.storage_root)
 
 # close instance
-close = subparsers.add_parser("close", help=close_help)
+subparsers.add_parser("close", help=close_help)
+
+# register instance
+subparsers.add_parser("register", help=register_help)
 
 # migrate
 migr = subparsers.add_parser("migrate", help=migr_help)
 aa = migr.add_argument
 aa("action", choices=["generate"], help="Generate migration.")
 
 # parse args
@@ -97,32 +104,37 @@
     if args.command == "login":
         return _setup_user.login(
             args.user,
             password=args.password,
         )
     elif args.command == "init":
         result = _init_instance.init(
-            storage=args.storage, db=args.db, schema=args.schema, name=args.name
+            storage=args.storage,
+            db=args.db,
+            schema=args.schema,
+            name=args.name,
         )
         return process_result(result)
     elif args.command == "load":
         result = _init_instance.load(
             identifier=args.instance,
         )
         return process_result(result)
     elif args.command == "close":
         return close_instance()
+    elif args.command == "register":
+        return register()
     elif args.command == "delete":
         return delete(
             instance_name=args.instance,
         )
     elif args.command == "info":
         return info()
     elif args.command == "set":
-        return set_storage(storage=args.storage)
+        return set.storage(args.storage)
     elif args.command == "migrate":
         from . import migrate
 
         if args.action == "generate":
             return migrate.generate()
     else:
         logger.error("Invalid command. Try `lamin -h`.")
```

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_check_instance_setup.py` & `lnhub_rest-0.9.0/lndb/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_close.py` & `lnhub_rest-0.9.0/lndb/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_delete.py` & `lnhub_rest-0.9.0/lndb/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_init_instance.py` & `lnhub_rest-0.9.0/lndb/lndb/_init_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,36 +117,44 @@
         ):
             raise RuntimeError(
                 ERROR_SQLITE_CACHE.format(
                     isettings._sqlite_file, isettings._sqlite_file_local
                 )
             )
 
-    # for remote instance, a lot of validation happens in the next function
-    # if this errors, the whole function errors
     if isettings.is_remote:
         result = init_instance_hub(
             owner=owner,
             name=name_str,
             storage=str(storage),
             db=db,
             schema=schema,
         )
         if result == "instance-exists-already":
             pass  # everything is alright!
         elif isinstance(result, str):
             raise RuntimeError(f"Creating instance on hub failed:\n{result}")
+        logger.success(f"Registered instance on hub: https://lamin.ai/{owner}/{name}")
+    else:
+        logger.info(
+            "Not registering instance on hub, if you want, call `lamin register`"
+        )
 
+    # this does not yet setup a setup for a new database
     persist_settings_load_schema(isettings)
 
     message = None
-    if not isettings._is_db_setup()[0]:
+    if not isettings._is_db_setup(mute=True)[0]:
         setup_schema(isettings, settings.user)
         register(isettings, settings.user)
         write_bionty_versions(isettings)
+        # now ensure that everything worked
+        check, msg = isettings._is_db_setup()
+        if not check:
+            raise RuntimeError(msg)
     else:
         # we're currently using this for testing migrations
         # passing connection strings of databases that need to be tested
         # for migrations
         logger.warning("Your instance seems already set up, attempt load:")
         message = load_from_isettings(isettings, migrate=_migrate)
```

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_load_instance.py` & `lnhub_rest-0.9.0/lndb/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_migrate/alembic.ini` & `lnhub_rest-0.9.0/lndb/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_migrate/core.py` & `lnhub_rest-0.9.0/lndb/lndb/_migrate/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,31 +48,39 @@
         """
         if package_name is None:
             package_name = get_package_name()
         package_dir, migrations_dir, schema_id = get_schema_package_info(package_name)
         generate_module_files(package_name)
         testdb_path = package_dir.parent / "testdb/testdb.lndb"  # type: ignore # noqa
         if testdb_path.exists():
-            # runs dev mode to write migration scripts
             rm = False
             set_alembic_logging_level(migrations_dir, level="INFO")
             logger.info(f"Generating based on {testdb_path}")
         else:
-            # runs CI-guided mode to generate empty migration scripts
             rm = True
             from lndb._settings import settings
 
+            if settings._instance_exists:
+                response = input(
+                    "Will generate migration for instance"
+                    " f{settings.instance.identifier}. Continue? (y/n)"
+                )
+                if response != "y":
+                    return None
+            else:
+                logger.error("Please load the instance you'd like to migrate!")
+                return None
+
             modify_alembic_ini(
                 filepath=package_dir / "alembic.ini",
                 isettings=settings.instance,
                 package_name=package_name,
                 move_sl=False,
             )
             set_alembic_logging_level(migrations_dir, level="WARN")
-            logger.info("Generate empty migration script.")
         command = (
             f"alembic --config {str(package_dir)}/alembic.ini --name"
             f" {schema_id} revision --autogenerate -m '{version}'"
         )
         process = run(command, shell=True)
 
         modify_migration_id_in__init__(package_name)
```

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_migrate/deploy.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_setup_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,176 +1,169 @@
-"""Check and auto-deploy migrations."""
-
 import importlib
-import os
-from pathlib import Path
-from subprocess import run
-from typing import Any, Optional
+from types import ModuleType
 
+import sqlalchemy as sa
 import sqlmodel as sqm
+from importlib_metadata import requires as importlib_requires
+from importlib_metadata import version as get_pip_version
 from lamin_logger import logger
-from natsort import natsorted
-from packaging.version import parse as vparse
+from lnhub_rest._assets._schemas import get_schema_lookup_name, get_schema_module_name
+from packaging.requirements import Requirement
 
-from lndb._migrate.utils import generate_module_files, modify_alembic_ini
-from lndb.dev._db import insert
-from lndb.dev._settings_instance import InstanceSettings
-from lndb.dev._settings_user import UserSettings
-from lndb.dev._setup_schema import create_schema_if_not_exists, get_schema_module_name
-
-
-def check_deploy_migration(
-    *,
-    usettings: UserSettings,
-    isettings: InstanceSettings,
-    attempt_deploy: Optional[bool] = None,
-):
-    if "LAMIN_SKIP_MIGRATION" in os.environ:
-        if os.environ["LAMIN_SKIP_MIGRATION"] == "true":
-            return "migrate-skipped"
-
-    # lock the whole migration
-    locker = isettings._cloud_sqlite_locker
-    locker.lock()
-    # synchronize the sqlite file before proceeding
-    isettings._update_local_sqlite_file()
+from ._db import insert
+from ._settings_instance import InstanceSettings
+from ._settings_user import UserSettings
+
+
+def create_schema_if_not_exists(schema_name: str, isettings: InstanceSettings):
+    # create the SQL-level schema module in case it doesn't exist
+    schema_lookup_name = get_schema_lookup_name(schema_name)
+    if isettings.dialect != "sqlite":
+        with isettings.engine.connect() as conn:
+            if not conn.dialect.has_schema(conn, schema_lookup_name):
+                conn.execute(sa.schema.CreateSchema(schema_lookup_name))
+            conn.commit()
+
+
+def reload_orms(schema_name, module, isettings):
+    # root-level ORMs
+    orms = [cls for cls in module.__dict__.values() if hasattr(cls, "__table__")]
+    # dev-level ORMs
+    if hasattr(module, "dev"):
+        orms += [
+            cls
+            for cls in module.dev.__dict__.values()
+            if hasattr(cls, "__table__")
+            # exclude the version_* and migration_* tables in the root namespace
+            and not cls.__name__.startswith("version_")
+            and not cls.__name__.startswith("migration_")
+        ]
+    # link tables
+    if hasattr(module, "link"):
+        orms += [
+            cls for cls in module.link.__dict__.values() if hasattr(cls, "__table__")
+        ]
+    if isettings.dialect == "sqlite":
+        # only those orms that are actually in a schema
+        orms = [
+            orm
+            for orm in orms
+            if hasattr(orm.__table__, "schema") and orm.__table__.schema is not None
+        ]
+        for orm in orms:
+            orm.__table__.schema = None
+            # I don't know why the following is needed... it shouldn't
+            if not orm.__table__.name.startswith(f"{schema_name}."):
+                orm.__table__.name = f"{schema_name}.{orm.__table__.name}"
+    else:  # postgres
+        orms = [
+            orm
+            for orm in orms
+            if (hasattr(orm.__table__, "schema") and orm.__table__.schema is None)
+        ]
+        for orm in orms:
+            orm.__table__.schema = schema_name
+            orm.__table__.name = orm.__table__.name.replace(f"{schema_name}.", "")
 
-    status = []
-    schema_names = ["core"] + list(isettings.schema)
-    # enforce order (if bionty is part of schema_names, it needs to come 2nd)
-    if "bionty" in schema_names:
-        schema_names.remove("bionty")
-        schema_names.insert(1, "bionty")
 
-    for schema_name in schema_names:
-        create_schema_if_not_exists(schema_name, isettings)
+def check_schema_version_and_import(schema_name) -> ModuleType:
+    def check_version(module_version):
         schema_module_name = get_schema_module_name(schema_name)
-        schema_module = importlib.import_module(schema_module_name)
-        # if _migration is None, there hasn't yet been any
-        if schema_module._migration is None:
-            status.append("migrate-unnecessary")
-            continue
+        lamindb_version = get_pip_version("lamindb")
+        for req in importlib_requires("lamindb"):
+            req = Requirement(req)
+            if schema_module_name == req.name:
+                if not req.specifier.contains(module_version):
+                    # it's currently important that we only import lamindb in
+                    # case of an error being raised
+                    # the following might mask the actual error because this is
+                    # raised during instance creation time where lamindb
+                    # cannot yet be imported
+                    # import lamindb
+                    # if lamindb.__version__ != lamindb_version:
+                    #     warning = (
+                    #         "\nWARNING: importlib_metadata.version('lamindb') gives"
+                    #         f" v{lamindb_version}, whereas `import lamindb` gives"
+                    #         f" v{lamindb.__version__}"
+                    #         f"\nConsider `pip install lamindb=={lamindb_version}`"
+                    #     )
+                    # else:
+                    #     warning = ""
+                    raise RuntimeError(
+                        f"lamindb v{lamindb_version} needs"
+                        f" lnschema_{schema_name}{req.specifier}, you have"
+                        f" {module_version}"
+                    )
 
-        schema_id = schema_module._schema_id
+    try:
+        # use live version if we can import
+        module = importlib.import_module(get_schema_module_name(schema_name))
+        module_version = module.__version__
+    except Exception as import_error:
+        # use pypi version instead
+        module_version = get_pip_version(get_schema_module_name(schema_name))
+        check_version(module_version)
+        raise import_error
 
-        with sqm.Session(isettings.engine) as session:
-            table_loc = (
-                schema_module.dev if hasattr(schema_module, "dev") else schema_module
-            )
-            version_table = getattr(table_loc, f"version_{schema_id}")
-            versions = session.exec(sqm.select(version_table.v)).all()
-            versions = natsorted(versions)  # latest version is last
-
-        current_version = schema_module.__version__
-
-        # attempt deploy as we want to test migrating the database
-        if attempt_deploy:
-            deploy_migration = True
-        # check whether we need to deploy based on version comparison
-        elif current_version not in versions and len(versions) > 0:
-            if vparse(current_version) < vparse(versions[-1]):  # type: ignore
-                raise RuntimeError(
-                    f"You are trying to connect to a DB ({isettings.identifier}) that"
-                    f" runs v{versions[-1]} of {schema_module_name} but you only have"
-                    f" v{current_version} installed.\nPlease run `pip install"
-                    f" {schema_module_name}=={versions[-1]}`, or install the latest"
-                    " schema module version from GitHub."
-                )
-            logger.warning(
-                f"Schema {schema_name} v{versions[-1]} is not up to date"
-                f" with {current_version}"
-            )
-            # if migration is confirmed, continue
-            if "PYTEST_CURRENT_TEST" not in os.environ:
-                logger.warning(
-                    "Run the command in the shell to respond to the following dialogue"
-                )
-
-                response = input(
-                    f"Do you want to migrate {schema_name} from {versions[-1]} to"
-                    f" {current_version} (y/n)?"
-                )
-
-                if response != "y":
-                    logger.warning(
-                        f"Instance {isettings.identifier} does not match the latest version of schema {schema_name}.\n"  # noqa
-                        "For production use, either install"
-                        f" {schema_module_name} {versions[-1]} "
-                        f"or migrate the database to {current_version}."
-                    )
-                    return None
-            else:
-                logger.warning(
-                    f"Migrate instance {isettings.name} outside a test (CI) run. "
-                    "Unexpected errors might happen."
-                )
-                return "migrate-failed"
-
-            deploy_migration = True
-
-        else:
-            deploy_migration = False
-            status.append("migrate-unnecessary")
-
-        if deploy_migration:
-            generate_module_files(
-                package_name=schema_module_name,
-                migrations_path=Path(schema_module.__file__).parent / "migrations",  # type: ignore  # noqa
-                schema_id=schema_id,
-            )
-            migrate_status = deploy(
-                version=current_version,
-                usettings=usettings,
-                isettings=isettings,
-                schema_name=schema_name,
-                schema_id=schema_id,
-                schema_module=schema_module,
-            )
-            status.append(migrate_status)
+    check_version(module_version)
+    return module
 
-    locker.unlock()
 
-    if "migrate-failed" in status:
-        return "migrate-failed"
-    elif "migrate-success" in status:
-        return "migrate-success"
-    else:
-        return "migrate-unnecessary"
-
-
-def deploy(
-    *,
-    version: str,
-    usettings: UserSettings,
-    isettings: InstanceSettings,
-    schema_name: str,
-    schema_id: str,
-    schema_module: Any,
-):
-    """Migrate database to latest version."""
-    schema_root = Path(schema_module.__file__).parent
-    filepath = schema_root / "alembic.ini"
-
-    modify_alembic_ini(filepath, isettings, schema_name)
-
-    process = run(
-        f"python -m alembic --name {schema_id} upgrade head",
-        cwd=f"{schema_root}",
-        shell=True,
+def load_schema(isettings: InstanceSettings):
+    reload = False  # see comments below
+    schema_names = ["core"] + list(isettings.schema)
+    msg = "Loading schema modules: "
+    for schema_name in schema_names:
+        create_schema_if_not_exists(schema_name, isettings)
+        module = check_schema_version_and_import(schema_name)
+        if schema_name == "core":
+            # here, we determine whether we have to reload the ORMs
+            # it's necessary if switching from or to sqlite
+            user_table = module.User.__table__
+            if isettings.dialect != "sqlite" and user_table.schema is None:
+                reload = True
+            if isettings.dialect == "sqlite" and user_table.schema is not None:
+                reload = True
+        if reload:  # importlib.reload doesn't do the job! hence, manual below
+            reload_orms(schema_name, module, isettings)
+        msg += f"{schema_name}=={module.__version__} "
+    return msg, schema_names
+
+
+def setup_schema(isettings: InstanceSettings, usettings: UserSettings):
+    msg, schema_names = load_schema(isettings)
+    logger.info(f"{msg}")
+
+    sqm.SQLModel.metadata.create_all(isettings.engine)
+
+    # we could try to also retrieve the user name here at some point
+    insert.user(
+        email=usettings.email,
+        user_id=usettings.id,
+        handle=usettings.handle,
+        name=usettings.name,
     )
 
-    if process.returncode == 0:
-        logger.success(f"Migrated schema {schema_name} to v{version}")
-        # The following call will also update the sqlite file in the cloud.
+    for schema_name in schema_names:
+        schema_module = importlib.import_module(get_schema_module_name(schema_name))
         insert.version(
             schema_module=schema_module,
             user_id=usettings.id,  # type: ignore
+            cloud_sqlite=False,
         )
-    else:
-        logger.error("Automatic migration failed.")
-
-    modify_alembic_ini(filepath, isettings, schema_name, revert=True)
-
-    if process.returncode == 0:
-        return "migrate-success"
-    else:
-        return "migrate-failed"
+        # this is the only time we need manipulate the migration table
+        # in all other cases alembic is going to to do this for us
+        schema_id, migration = schema_module._schema_id, schema_module._migration
+        if migration is not None:
+            table_loc = (
+                schema_module.dev if hasattr(schema_module, "dev") else schema_module
+            )
+            migration_table = getattr(table_loc, f"migration_{schema_id}")
+            # we purposefully do not use isettings.session(), here, as we do *not*
+            # want to update the local sqlite file from the cloud while looping over
+            # schema modules
+            # in fact, a synchronization issue led to loss of version information,
+            # because the old cloud sqlite file overwrote the newer local file
+            with sqm.Session(isettings.engine) as session:
+                session.add(migration_table(version_num=migration))
+                session.commit()
+    isettings._update_cloud_sqlite_file()
```

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_migrate/env.py` & `lnhub_rest-0.9.0/lndb/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_migrate/utils.py` & `lnhub_rest-0.9.0/lndb/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_schema.py` & `lnhub_rest-0.9.0/lndb/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/_settings.py` & `lnhub_rest-0.9.0/lndb/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/__init__.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_clone.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_db.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_deprecated.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_exclusion.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_instance.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_settings_instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Literal, Optional, Set, Tuple, Union
 
 import sqlalchemy as sa
 import sqlmodel as sqm
+from lamin_logger import logger
 from pydantic import PostgresDsn
 from sqlalchemy.future import Engine
 
 from ._exclusion import empty_locker, get_locker
 from ._settings_save import save_instance_settings
 from ._settings_store import current_instance_settings_file, instance_settings_file
 from ._storage import Storage
@@ -53,15 +54,15 @@
     def __repr__(self):
         """Rich string representation."""
         representation = f"Current instance: {self.identifier}"
         attrs = ["owner", "name", "storage", "db", "schema"]
         for attr in attrs:
             value = getattr(self, attr)
             if attr == "storage":
-                representation += f"\n- storage root: {value.root}"
+                representation += f"\n- storage root: {value.root_as_str}"
                 representation += f"\n- storage region: {value.region}"
             else:
                 representation += f"\n- {attr}: {value}"
         return representation
 
     @property
     def owner(self) -> str:
@@ -209,35 +210,40 @@
         shutil.copy2(filepath, current_instance_settings_file())
         # persist under settings class for same session reference
         # need to import here to avoid circular import
         from .._settings import settings
 
         settings._instance_settings = self
 
-    def _is_db_setup(self) -> Tuple[bool, str]:
+    def _is_db_setup(self, mute: bool = False) -> Tuple[bool, str]:
         """Is the database available and initialized as LaminDB?"""
+        if not self._is_db_reachable(mute=mute):
+            if self.dialect == "sqlite":
+                return False, f"SQLite file {self._sqlite_file} does not exist"
+            else:
+                return False, f"Connection {self.db} not reachable"
+        # cannot import lnschema_core here, yet!
+
+        with self.engine.connect() as conn:
+            try:
+                result = conn.execute(sa.text("select * from version_yvzi")).first()
+            except Exception as e:
+                return False, f"Your DB is not initialized: {e}"
+            if result is None:
+                return False, "Your DB is not initialized: version_yvzi has no row"
+        return True, ""
+
+    def _is_db_reachable(self, mute: bool = False) -> bool:
         if self.dialect == "sqlite":
             if not self._sqlite_file.exists():
-                return False, "SQLite file does not exist"
-            else:
-                return True, ""
-        else:  # postgres
-            assert self.dialect == "postgresql"
-            with self.engine.connect() as conn:
-                results = conn.execute(
-                    sa.text(
-                        """
-                    SELECT EXISTS (
-                        SELECT FROM
-                            information_schema.tables
-                        WHERE
-                            table_schema LIKE 'public' AND
-                            table_name = 'version_yvzi'
-                    );
-                """
-                    )
-                ).first()  # returns tuple of boolean
-                check = results[0]
-                if not check:
-                    return False, "Postgres does not seem initialized."
-                else:
-                    return True, ""
+                if not mute:
+                    logger.warning(f"SQLite file {self._sqlite_file} does not exist")
+                return False
+        else:
+            engine = sa.create_engine(self.db)
+            try:
+                engine.connect()
+            except Exception:
+                if not mute:
+                    logger.warning(f"Connection {self.db} not reachable")
+                return False
+        return True
```

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_load.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_save.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_store.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_settings_user.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_setup_knowledge.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/_storage.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/_storage.py`

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

### Comparing `lnhub_rest-0.8.2/lndb/lndb/dev/upath.py` & `lnhub_rest-0.9.0/lndb/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/test/_migrations_e2e.py` & `lnhub_rest-0.9.0/lndb/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/lndb/test/_migrations_unit.py` & `lnhub_rest-0.9.0/lndb/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/noxfile.py` & `lnhub_rest-0.9.0/lndb/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/pyproject.toml` & `lnhub_rest-0.9.0/lndb/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.8.1",
+    "lnhub_rest==0.8.2",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.28.0",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
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

### Comparing `lnhub_rest-0.8.2/lndb/tests/test_bionty.py` & `lnhub_rest-0.9.0/lndb/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lndb/tests/test_init_instance.py` & `lnhub_rest-0.9.0/lndb/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/__main__.py` & `lnhub_rest-0.9.0/lnhub_rest/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/_assets/_instances.py` & `lnhub_rest-0.9.0/lnhub_rest/_assets/_instances.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.9.0/lnhub_rest/_assets/_schemas.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.9.0/lnhub_rest/_check_breaks_lndb.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/_ci.py` & `lnhub_rest-0.9.0/lnhub_rest/_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.9.0/lnhub_rest/_clean_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.9.0/lnhub_rest/core/account/_create_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.9.0/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.9.0/lnhub_rest/core/account/_delete_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.9.0/lnhub_rest/core/account/_signup_signin.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.9.0/lnhub_rest/core/account/_update_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.9.0/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.9.0/lnhub_rest/core/instance/_delete_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.9.0/lnhub_rest/core/instance/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.9.0/lnhub_rest/core/instance/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.9.0/lnhub_rest/core/instance/_update_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/member/_crud.py` & `lnhub_rest-0.9.0/lnhub_rest/core/member/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.9.0/lnhub_rest/core/storage/_add_storage.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.9.0/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/main.py` & `lnhub_rest-0.9.0/lnhub_rest/main.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.9.0/lnhub_rest/orm/_sbclient.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/routers/account.py` & `lnhub_rest-0.9.0/lnhub_rest/routers/account.py`

 * *Files 23% similar despite different names*

```diff
@@ -97,34 +97,49 @@
         supabase_client.table("account").select("*").eq("handle", handle).execute().data
     )
     return data[0] if len(data) > 0 else None
 
 
 @router.get("/resources/instances/{handle}")
 def get_account_instances(
-    handle: str, authentication: Union[str, None] = Header(default=None)
+    handle: str,
+    owner: bool = False,
+    authentication: Union[str, None] = Header(default=None),
 ):
     access_token = extract_access_token(authentication)
     supabase_client = get_supabase_client(access_token)
 
     try:
-        account_instances = (
-            supabase_client.table("account")
-            .select(
-                """account_instance(*, instance(
-                *, account!fk_instance_account_id_account(handle, id)))""".replace(
-                    "\n", ""
+        if owner:
+            instances = (
+                supabase_client.table("account")
+                .select(
+                    "instance!fk_instance_account_id_account(*, storage(root),"
+                    " account!fk_instance_account_id_account(handle, id))"
                 )
+                .eq("handle", handle)
+                .execute()
+                .data[0]["instance"]
             )
-            .eq("handle", handle)
-            .execute()
-            .data[0]["account_instance"]
-        )
 
-        return account_instances
+            return instances
+        else:
+            account_instances = (
+                supabase_client.table("account")
+                .select(
+                    "account_instance(instance(*, storage(root),"
+                    " account!fk_instance_account_id_account(handle, id)))"
+                )
+                .eq("handle", handle)
+                .execute()
+                .data[0]["account_instance"]
+            )
+            account_instances = [entry["instance"] for entry in account_instances]
+
+            return account_instances
 
     finally:
         supabase_client.auth.sign_out()
 
 
 @router.get("/resources/organizations/{handle}")
 def get_account_organizations(
@@ -133,16 +148,16 @@
     access_token = extract_access_token(authentication)
     supabase_client = get_supabase_client(access_token)
 
     try:
         user_id = get_account_by_handle(handle)["id"]
         organizations_user = (
             supabase_client.table("organization_user")
-            .select()
+            .select("""*, account(*)""")
             .eq("user_id", user_id)
             .execute()
             .data
         )
-        return organizations_user if len(organizations_user) > 0 else None
+        return organizations_user
 
     finally:
         supabase_client.auth.sign_out()
```

### Comparing `lnhub_rest-0.8.2/lnhub_rest/routers/ci.py` & `lnhub_rest-0.9.0/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/routers/instance.py` & `lnhub_rest-0.9.0/lnhub_rest/routers/instance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 
 from fastapi import APIRouter, Header
 
+from lnhub_rest.core.collaborator._crud import sb_insert_collaborator
 from lnhub_rest.core.instance._delete_instance import (
     delete_instance as delete_instance_base,
 )
 from lnhub_rest.core.instance._init_instance import init_instance as init_instance_base
 from lnhub_rest.core.instance._update_instance import (
     update_instance as update_instance_base,
 )
@@ -89,14 +90,45 @@
 
         return {"accounts": account_instances, "role": role}
 
     finally:
         supabase_client.auth.sign_out()
 
 
+@router.post("/resources/accounts/")
+def add_collaborator(
+    handle: str,
+    instance_id: str,
+    role: str = "read",
+    authentication: Union[str, None] = Header(default=None),
+):
+    access_token = extract_access_token(authentication)
+    supabase_client = get_supabase_client(access_token)
+
+    try:
+        account = get_account_by_handle(handle)
+        if account is None:
+            return "account-not-exists"
+        account_instance_fields = {
+            "account_id": account["id"],
+            "instance_id": instance_id,
+            "role": role,
+        }
+        data = sb_insert_collaborator(account_instance_fields, supabase_client)
+
+        assert data is not None
+
+        if data == "collaborator-exists-already":
+            return data
+        return "success"
+
+    finally:
+        supabase_client.auth.sign_out()
+
+
 @router.post("/")
 def create_instance(
     account_handle: str,
     name: str,
     storage: str,
     db: Union[str, None] = None,
     schema: Union[str, None] = None,
```

### Comparing `lnhub_rest-0.8.2/lnhub_rest/routers/organization.py` & `lnhub_rest-0.9.0/lnhub_rest/routers/organization.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/routers/utils.py` & `lnhub_rest-0.9.0/lnhub_rest/routers/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/_core.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/alembic.ini` & `lnhub_rest-0.9.0/lnhub_rest/schema/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/clone.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/settings.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/settings.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/testing.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/testing.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py` & `lnhub_rest-0.9.0/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/lnhub_rest/utils/_test.py` & `lnhub_rest-0.9.0/lnhub_rest/utils/_test.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/noxfile.py` & `lnhub_rest-0.9.0/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         "-s",
         "--cov=lnhub_rest",
         "--cov-append",
         "--cov-report=term-missing",
         env={"LN_SERVER_DEPLOY": "1", "LAMIN_ENV": lamin_env},
     )
     if package == "lndb":
-        login_testuser1(session)
-        login_testuser2(session)
+        login_testuser1(session, env={"LAMIN_ENV": lamin_env})
+        login_testuser2(session, env={"LAMIN_ENV": lamin_env})
         os.chdir(f"./{package}")
         session.run(
             "pytest",
             "-s",
             "./tests",
             env={"LAMIN_ENV": lamin_env},
         )
```

### Comparing `lnhub_rest-0.8.2/pyproject.toml` & `lnhub_rest-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/supabase/config.toml` & `lnhub_rest-0.9.0/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/tests/test_notebooks.py` & `lnhub_rest-0.9.0/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.8.2/PKG-INFO` & `lnhub_rest-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.8.2
+Version: 0.9.0
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: supabase==1.0.2
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
```

