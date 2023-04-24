# Comparing `tmp/flask-ligand-0.7.2.tar.gz` & `tmp/flask-ligand-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-ligand-0.7.2.tar", last modified: Fri Feb 10 20:53:12 2023, max compression
+gzip compressed data, was "flask-ligand-0.7.3.tar", last modified: Mon Apr 24 19:20:29 2023, max compression
```

## Comparing `flask-ligand-0.7.2.tar` & `flask-ligand-0.7.3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/
--rw-r--r--   0 root         (0) root         (0)       14 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.flaskenv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.368273 flask-ligand-0.7.2/.github/
--rw-r--r--   0 root         (0) root         (0)      528 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.372273 flask-ligand-0.7.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      625 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.github/workflows/bump_and_publish_release.yml
--rw-r--r--   0 root         (0) root         (0)      797 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.github/workflows/coverage.yml
--rw-r--r--   0 root         (0) root         (0)      622 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.github/workflows/pull_request.yml
--rw-r--r--   0 root         (0) root         (0)     1096 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      371 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.readthedocs.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.372273 flask-ligand-0.7.2/.run/
--rw-r--r--   0 root         (0) root         (0)     1296 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Flask - Debug.run.xml
--rw-r--r--   0 root         (0) root         (0)     1265 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Flask.run.xml
--rw-r--r--   0 root         (0) root         (0)      459 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Integration Test Environment.run.xml
--rw-r--r--   0 root         (0) root         (0)     1473 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Integration.run.xml
--rw-r--r--   0 root         (0) root         (0)      808 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Unit (tox).run.xml
--rw-r--r--   0 root         (0) root         (0)      856 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Unit (tox-fast).run.xml
--rw-r--r--   0 root         (0) root         (0)     1055 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Unit - Database.run.xml
--rw-r--r--   0 root         (0) root         (0)     1045 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Unit - JWT.run.xml
--rw-r--r--   0 root         (0) root         (0)     1047 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Unit - OpenAPI.run.xml
--rw-r--r--   0 root         (0) root         (0)     1506 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Unit - Settings.run.xml
--rw-r--r--   0 root         (0) root         (0)     1459 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/Unit.run.xml
--rw-r--r--   0 root         (0) root         (0)      369 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/develop-venv.run.xml
--rw-r--r--   0 root         (0) root         (0)      389 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/gen-admin-access-token.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/gen-docs.run.xml
--rw-r--r--   0 root         (0) root         (0)      353 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/lint.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/setup-db.run.xml
--rw-r--r--   0 root         (0) root         (0)      361 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/.run/test-all.run.xml
--rw-r--r--   0 root         (0) root         (0)       36 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    12394 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     3615 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    34523 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8962 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     5001 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3683 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      939 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.364273 flask-ligand-0.7.2/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.372273 flask-ligand-0.7.2/docker/env_files/
--rw-r--r--   0 root         (0) root         (0)      806 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docker/env_files/integration.env
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.372273 flask-ligand-0.7.2/docker/kc-data/
--rw-r--r--   0 root         (0) root         (0)    78994 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docker/kc-data/flask-ligand-realm.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.372273 flask-ligand-0.7.2/docker/postgres-data/
--rw-r--r--   0 root         (0) root         (0)      589 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docker/postgres-data/create-multiple-postgresql-databases.sh
--rw-r--r--   0 root         (0) root         (0)      799 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.376273 flask-ligand-0.7.2/docs/
--rw-r--r--   0 root         (0) root         (0)      632 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.376273 flask-ligand-0.7.2/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     7352 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/_static/small_logo.jpg
--rw-r--r--   0 root         (0) root         (0)     2704 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/api_reference.rst
--rw-r--r--   0 root         (0) root         (0)     6093 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/auth0.rst
--rw-r--r--   0 root         (0) root         (0)       41 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)       79 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6080 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)     2571 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/database_configuration.rst
--rw-r--r--   0 root         (0) root         (0)     3885 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/developer_guide.rst
--rw-r--r--   0 root         (0) root         (0)      207 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/development.rst
--rw-r--r--   0 root         (0) root         (0)    12374 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/flask_environments.rst
--rw-r--r--   0 root         (0) root         (0)     2411 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1139 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/integration_testing.rst
--rw-r--r--   0 root         (0) root         (0)       48 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/license.rst
--rw-r--r--   0 root         (0) root         (0)      765 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1304 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/oidc_configuration.rst
--rw-r--r--   0 root         (0) root         (0)     2546 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/openapi.rst
--rw-r--r--   0 root         (0) root         (0)    25967 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/quickstart.rst
--rw-r--r--   0 root         (0) root         (0)     1637 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/release_process.rst
--rw-r--r--   0 root         (0) root         (0)      131 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.376273 flask-ligand-0.7.2/flask_ligand/
--rw-r--r--   0 root         (0) root         (0)     3715 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/cli.py
--rw-r--r--   0 root         (0) root         (0)     5441 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/controllers.py
--rw-r--r--   0 root         (0) root         (0)    12650 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/default_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/flask_ligand/extensions/
--rw-r--r--   0 root         (0) root         (0)     1514 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6979 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/extensions/api.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/extensions/database.py
--rw-r--r--   0 root         (0) root         (0)     5210 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/extensions/jwt.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/py.typed
--rw-r--r--   0 root         (0) root         (0)     1116 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/flask_ligand/views/
--rw-r--r--   0 root         (0) root         (0)     1552 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/flask_ligand/views/common/
--rw-r--r--   0 root         (0) root         (0)       44 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/views/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/views/common/openapi_doc.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/flask_ligand/views/openapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.376273 flask-ligand-0.7.2/flask_ligand.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5001 2023-02-10 20:53:12.000000 flask-ligand-0.7.2/flask_ligand.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2670 2023-02-10 20:53:12.000000 flask-ligand-0.7.2/flask_ligand.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 20:53:12.000000 flask-ligand-0.7.2/flask_ligand.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-10 20:53:12.000000 flask-ligand-0.7.2/flask_ligand.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-10 20:53:12.000000 flask-ligand-0.7.2/flask_ligand.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      277 2023-02-10 20:53:12.000000 flask-ligand-0.7.2/flask_ligand.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-02-10 20:53:12.000000 flask-ligand-0.7.2/flask_ligand.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1112 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      516 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      330 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1437 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      737 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8190 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/tests/integration/migrations/
--rw-r--r--   0 root         (0) root         (0)       41 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/migrations/README
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/migrations/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     2736 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/migrations/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/migrations/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/tests/integration/migrations/versions/
--rw-r--r--   0 root         (0) root         (0)      691 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/migrations/versions/47f10265b5d7_.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/migrations/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/integration/test_basic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-10 20:53:12.380273 flask-ligand-0.7.2/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/unit/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/unit/test_api_extension.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/unit/test_database_extension.py
--rw-r--r--   0 root         (0) root         (0)     6791 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/unit/test_jwt_extension.py
--rw-r--r--   0 root         (0) root         (0)    10519 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/unit/test_openapi_api.py
--rw-r--r--   0 root         (0) root         (0)    21947 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tests/unit/test_settings.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-02-10 20:53:08.000000 flask-ligand-0.7.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.741305 flask-ligand-0.7.3/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.flaskenv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.725305 flask-ligand-0.7.3/.github/
+-rw-r--r--   0 root         (0) root         (0)      528 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.725305 flask-ligand-0.7.3/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      625 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.github/workflows/bump_and_publish_release.yml
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.github/workflows/coverage.yml
+-rw-r--r--   0 root         (0) root         (0)      622 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.github/workflows/pull_request.yml
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      371 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.readthedocs.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.729305 flask-ligand-0.7.3/.run/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Flask - Debug.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Flask.run.xml
+-rw-r--r--   0 root         (0) root         (0)      459 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Integration Test Environment.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Integration.run.xml
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Unit (tox).run.xml
+-rw-r--r--   0 root         (0) root         (0)      856 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Unit (tox-fast).run.xml
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Unit - Database.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Unit - JWT.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Unit - OpenAPI.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Unit - Settings.run.xml
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/Unit.run.xml
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/develop-venv.run.xml
+-rw-r--r--   0 root         (0) root         (0)      389 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/gen-admin-access-token.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/gen-docs.run.xml
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/lint.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/setup-db.run.xml
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/.run/test-all.run.xml
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    15394 2023-04-24 19:20:25.000000 flask-ligand-0.7.3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     3615 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-04-24 19:20:29.741305 flask-ligand-0.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3683 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.721305 flask-ligand-0.7.3/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.729305 flask-ligand-0.7.3/docker/env_files/
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docker/env_files/integration.env
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.729305 flask-ligand-0.7.3/docker/kc-data/
+-rw-r--r--   0 root         (0) root         (0)    78994 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docker/kc-data/flask-ligand-realm.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.729305 flask-ligand-0.7.3/docker/postgres-data/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docker/postgres-data/create-multiple-postgresql-databases.sh
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.733305 flask-ligand-0.7.3/docs/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.733305 flask-ligand-0.7.3/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     7352 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/_static/small_logo.jpg
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/api_reference.rst
+-rw-r--r--   0 root         (0) root         (0)     6093 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/auth0.rst
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/database_configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/developer_guide.rst
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/development.rst
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/flask_environments.rst
+-rw-r--r--   0 root         (0) root         (0)     2411 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/integration_testing.rst
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)      765 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/oidc_configuration.rst
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/openapi.rst
+-rw-r--r--   0 root         (0) root         (0)    25967 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/quickstart.rst
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/release_process.rst
+-rw-r--r--   0 root         (0) root         (0)      131 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.737305 flask-ligand-0.7.3/flask_ligand/
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-04-24 19:20:25.000000 flask-ligand-0.7.3/flask_ligand/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5441 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/controllers.py
+-rw-r--r--   0 root         (0) root         (0)    12650 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.737305 flask-ligand-0.7.3/flask_ligand/extensions/
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/extensions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6979 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/extensions/api.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/extensions/database.py
+-rw-r--r--   0 root         (0) root         (0)     5210 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/extensions/jwt.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.737305 flask-ligand-0.7.3/flask_ligand/views/
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.737305 flask-ligand-0.7.3/flask_ligand/views/common/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/views/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/views/common/openapi_doc.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/flask_ligand/views/openapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.737305 flask-ligand-0.7.3/flask_ligand.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5001 2023-04-24 19:20:29.000000 flask-ligand-0.7.3/flask_ligand.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-04-24 19:20:29.000000 flask-ligand-0.7.3/flask_ligand.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 19:20:29.000000 flask-ligand-0.7.3/flask_ligand.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 19:20:29.000000 flask-ligand-0.7.3/flask_ligand.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-24 19:20:29.000000 flask-ligand-0.7.3/flask_ligand.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      276 2023-04-24 19:20:29.000000 flask-ligand-0.7.3/flask_ligand.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 19:20:29.000000 flask-ligand-0.7.3/flask_ligand.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      329 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-24 19:20:29.741305 flask-ligand-0.7.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      737 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.737305 flask-ligand-0.7.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.741305 flask-ligand-0.7.3/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.741305 flask-ligand-0.7.3/tests/integration/migrations/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/migrations/README
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/migrations/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/migrations/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/migrations/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.741305 flask-ligand-0.7.3/tests/integration/migrations/versions/
+-rw-r--r--   0 root         (0) root         (0)      691 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/migrations/versions/47f10265b5d7_.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/migrations/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/integration/test_basic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 19:20:29.741305 flask-ligand-0.7.3/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/unit/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/unit/test_api_extension.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/unit/test_database_extension.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/unit/test_jwt_extension.py
+-rw-r--r--   0 root         (0) root         (0)    10519 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/unit/test_openapi_api.py
+-rw-r--r--   0 root         (0) root         (0)    21947 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tests/unit/test_settings.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-24 19:20:24.000000 flask-ligand-0.7.3/tox.ini
```

### Comparing `flask-ligand-0.7.2/.github/dependabot.yml` & `flask-ligand-0.7.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.github/workflows/bump_and_publish_release.yml` & `flask-ligand-0.7.3/.github/workflows/bump_and_publish_release.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.github/workflows/coverage.yml` & `flask-ligand-0.7.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.github/workflows/pull_request.yml` & `flask-ligand-0.7.3/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.pre-commit-config.yaml` & `flask-ligand-0.7.3/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -4,35 +4,35 @@
     hooks:
     -   id: check-yaml
     -   id: check-toml
     -   id: detect-private-key
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.2.0
     hooks:
     -   id: mypy
         additional_dependencies:
         -   "types-Flask-Cors~=3.0"
         -   "types-Flask-SQLAlchemy~=2.5"
         -   "types-mock~=4.0"
         -   "types-PyYAML~=6.0"
         -   "types-requests~=2.28"
         -   "types-setuptools~=63.4"
         -   "types-smorest~=1.1"
         -   "types-SQLAlchemy~=1.4"
         -   "types-sqlalchemy-utils~=1.0"
         -   "types-urllib3<1.27"
 -   repo: https://github.com/rstcheck/rstcheck
-    rev: v6.1.1
+    rev: v6.1.2
     hooks:
     -   id: rstcheck
         additional_dependencies: [sphinx]
         exclude: "docs/authors.rst|docs/changelog.rst|docs/license.rst"
```

### Comparing `flask-ligand-0.7.2/.run/Flask - Debug.run.xml` & `flask-ligand-0.7.3/.run/Flask - Debug.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Flask.run.xml` & `flask-ligand-0.7.3/.run/Flask.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Integration.run.xml` & `flask-ligand-0.7.3/.run/Integration.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Unit (tox).run.xml` & `flask-ligand-0.7.3/.run/Unit (tox).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Unit (tox-fast).run.xml` & `flask-ligand-0.7.3/.run/Unit (tox-fast).run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Unit - Database.run.xml` & `flask-ligand-0.7.3/.run/Unit - Database.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Unit - JWT.run.xml` & `flask-ligand-0.7.3/.run/Unit - JWT.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Unit - OpenAPI.run.xml` & `flask-ligand-0.7.3/.run/Unit - OpenAPI.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Unit - Settings.run.xml` & `flask-ligand-0.7.3/.run/Unit - Settings.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/.run/Unit.run.xml` & `flask-ligand-0.7.3/.run/Unit.run.xml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/CHANGELOG.md` & `flask-ligand-0.7.3/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,35 @@
 Changelog
 =========
 
 <!--next-version-placeholder-->
 
+## v0.7.3 (2023-04-24)
+### Fix
+* :arrow_up: Update python-semantic-release requirement ([`65190bc`](https://github.com/cowofevil/flask-ligand/commit/65190bc8295f4442e7ecd7ab4291d9fffcfede4f))
+* :arrow_up: Update coverage[toml] requirement from ~=7.1 to ~=7.2 ([`ebcc2df`](https://github.com/cowofevil/flask-ligand/commit/ebcc2dffbb7597bce59ec1943fdbed92f8f0b334))
+* :arrow_up: Update marshmallow-sqlalchemy requirement ([`6035d9e`](https://github.com/cowofevil/flask-ligand/commit/6035d9e5b7a5e399c177014131ec41d8419d55f3))
+* :arrow_up: Update python-dotenv requirement from ~=0.21 to ~=1.0 ([`93e5967`](https://github.com/cowofevil/flask-ligand/commit/93e5967257f5e2b97cb70b6672542bc2ddae9f9d))
+* :arrow_up: Update pre-commit requirement from ~=3.0 to ~=3.1 ([`f9b423a`](https://github.com/cowofevil/flask-ligand/commit/f9b423aa0c90f5e5a4b5cb0d25efe1eea780ceaa))
+* :arrow_up: Update tox requirement from ~=4.1 to ~=4.4 ([`f4f748b`](https://github.com/cowofevil/flask-ligand/commit/f4f748beb29b5749d8f603643772d6cf110e7048))
+* :arrow_up: Update pygments requirement from ~=2.13 to ~=2.14 ([`299411f`](https://github.com/cowofevil/flask-ligand/commit/299411fb85b2f70a5c093fa4d8de4600ee04265e))
+* :arrow_up: Update pipdeptree requirement from ~=2.3 to ~=2.5 ([`2e5e48c`](https://github.com/cowofevil/flask-ligand/commit/2e5e48c601b046a1ce3c33cd2f54877ccb92fadc))
+* :arrow_up: Update sphinx-toolbox requirement from ~=3.2 to ~=3.4 ([`3d51f77`](https://github.com/cowofevil/flask-ligand/commit/3d51f77c078d7c9099aa47287e52c6cb48d320d3))
+* :arrow_up: Update ipython requirement from ~=8.7 to ~=8.11 ([`5c64f0a`](https://github.com/cowofevil/flask-ligand/commit/5c64f0a4d63c77cd459a2026e6f6a6f5ef26b518))
+* :arrow_up: Update sqlalchemy-utils requirement from ~=0.39 to ~=0.40 ([`e78cef9`](https://github.com/cowofevil/flask-ligand/commit/e78cef914fa93b59632af4cc59d3c50058f857d5))
+* :arrow_up: Update black requirement from ~=22.12 to ~=23.1 ([`c269598`](https://github.com/cowofevil/flask-ligand/commit/c269598af164b71a7119e8c404e0da22bf3d6518))
+* :arrow_up: Update coverage[toml] requirement from ~=6.5 to ~=7.1 ([`1592a7e`](https://github.com/cowofevil/flask-ligand/commit/1592a7eb94abe61995c703439275a14fa08feedf))
+* :arrow_up: Update mypy requirement from ~=0.991 to ~=1.0 ([`dae22d7`](https://github.com/cowofevil/flask-ligand/commit/dae22d78f8d52c3f4175e8dfb025c16d32e23619))
+* :arrow_up: Update types-setuptools requirement from ~=65.6 to ~=67.3 ([`af1d7eb`](https://github.com/cowofevil/flask-ligand/commit/af1d7ebc72a532ae0951b3f355cf7b642246eee1))
+
+### Other
+* [pre-commit.ci] pre-commit autoupdate ([`dc4659d`](https://github.com/cowofevil/flask-ligand/commit/dc4659d9cca99992478f54a6a1cfcee3985c2863))
+* [pre-commit.ci] pre-commit autoupdate ([`09d0008`](https://github.com/cowofevil/flask-ligand/commit/09d000802e874855f534c1d901556e35bbefad8b))
+* [pre-commit.ci] pre-commit autoupdate ([`88561b9`](https://github.com/cowofevil/flask-ligand/commit/88561b9e2abaf5d0704189749628e6a8aa46f654))
+
 ## v0.7.2 (2023-02-10)
 ### Fix
 * [560:robot:] Fix Packaging Issues ([`afd0075`](https://github.com/cowofevil/flask-ligand/commit/afd0075e67dd37b7d34048743d9a3d3bb6099641))
 
 ### Other
 * [pre-commit.ci] auto fixes from pre-commit.com hooks ([`380e1bc`](https://github.com/cowofevil/flask-ligand/commit/380e1bc138200f18029f19fd5865c0e2e263f4ac))
 * [pre-commit.ci] pre-commit autoupdate ([`c3204a1`](https://github.com/cowofevil/flask-ligand/commit/c3204a11945e9aa212b4bd84d5493a3c8355d7ad))
```

### Comparing `flask-ligand-0.7.2/CONTRIBUTING.rst` & `flask-ligand-0.7.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/LICENSE` & `flask-ligand-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/Makefile` & `flask-ligand-0.7.3/Makefile`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/PKG-INFO` & `flask-ligand-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand
-Version: 0.7.2
+Version: 0.7.3
 Summary: A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand/issues
```

### Comparing `flask-ligand-0.7.2/README.rst` & `flask-ligand-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/app.py` & `flask-ligand-0.7.3/app.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docker/env_files/integration.env` & `flask-ligand-0.7.3/docker/env_files/integration.env`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docker/kc-data/flask-ligand-realm.json` & `flask-ligand-0.7.3/docker/kc-data/flask-ligand-realm.json`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docker/postgres-data/create-multiple-postgresql-databases.sh` & `flask-ligand-0.7.3/docker/postgres-data/create-multiple-postgresql-databases.sh`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docker-compose.yml` & `flask-ligand-0.7.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/Makefile` & `flask-ligand-0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/_static/small_logo.jpg` & `flask-ligand-0.7.3/docs/_static/small_logo.jpg`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/api_reference.rst` & `flask-ligand-0.7.3/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/auth0.rst` & `flask-ligand-0.7.3/docs/auth0.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/conf.py` & `flask-ligand-0.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/database_configuration.rst` & `flask-ligand-0.7.3/docs/database_configuration.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/developer_guide.rst` & `flask-ligand-0.7.3/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/flask_environments.rst` & `flask-ligand-0.7.3/docs/flask_environments.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/index.rst` & `flask-ligand-0.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/integration_testing.rst` & `flask-ligand-0.7.3/docs/integration_testing.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/make.bat` & `flask-ligand-0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/oidc_configuration.rst` & `flask-ligand-0.7.3/docs/oidc_configuration.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/openapi.rst` & `flask-ligand-0.7.3/docs/openapi.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/quickstart.rst` & `flask-ligand-0.7.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/docs/release_process.rst` & `flask-ligand-0.7.3/docs/release_process.rst`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/__init__.py` & `flask-ligand-0.7.3/flask_ligand/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from typing import Any, Tuple
     from flask_ligand.extensions.api import Api
 
 
 # ======================================================================================================================
 # Globals
 # ======================================================================================================================
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 
 # ======================================================================================================================
 # Functions: Public
 # ======================================================================================================================
 def create_app(
     flask_app_name: str,
```

### Comparing `flask-ligand-0.7.2/flask_ligand/cli.py` & `flask-ligand-0.7.3/flask_ligand/cli.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/controllers.py` & `flask-ligand-0.7.3/flask_ligand/controllers.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/default_settings.py` & `flask-ligand-0.7.3/flask_ligand/default_settings.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/extensions/__init__.py` & `flask-ligand-0.7.3/flask_ligand/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/extensions/api.py` & `flask-ligand-0.7.3/flask_ligand/extensions/api.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/extensions/database.py` & `flask-ligand-0.7.3/flask_ligand/extensions/database.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/extensions/jwt.py` & `flask-ligand-0.7.3/flask_ligand/extensions/jwt.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/schemas.py` & `flask-ligand-0.7.3/flask_ligand/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/views/__init__.py` & `flask-ligand-0.7.3/flask_ligand/views/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/views/common/openapi_doc.py` & `flask-ligand-0.7.3/flask_ligand/views/common/openapi_doc.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand/views/openapi.py` & `flask-ligand-0.7.3/flask_ligand/views/openapi.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/flask_ligand.egg-info/PKG-INFO` & `flask-ligand-0.7.3/flask_ligand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-ligand
-Version: 0.7.2
+Version: 0.7.3
 Summary: A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 Author: Ryan Gard
 Author-email: ryan@gardiancapitol.com
 License: GNU Affero General Public License v3
 Project-URL: Changelog, https://github.com/cowofevil/flask-ligand/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/cowofevil/flask-ligand
 Project-URL: Tracker, https://github.com/cowofevil/flask-ligand/issues
```

### Comparing `flask-ligand-0.7.2/flask_ligand.egg-info/SOURCES.txt` & `flask-ligand-0.7.3/flask_ligand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/pyproject.toml` & `flask-ligand-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/requirements-dev.txt` & `flask-ligand-0.7.3/requirements-dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Dependency constraints
 flake8~=6.0
-mypy~=0.991
-pygments~=2.13
+mypy~=1.0
+pygments~=2.14
 pytest~=7.2
 twine~=3.8
 # Installation requirements
-black~=22.12
-coverage[toml]~=6.5
+black~=23.1
+coverage[toml]~=7.2
 flake8-bugbear>=22.9.11
-ipython~=8.7
+ipython~=8.11
 pg8000~=1.29
-pipdeptree~=2.3
+pipdeptree~=2.5
 pytest-cov~=4.0
-pre-commit~=3.0
+pre-commit~=3.1
 pytest-flask-ligand~=0.1
 pytest-mock~=3.10
-python-semantic-release~=7.32
-tox~=4.1
+python-semantic-release~=7.33
+tox~=4.4
 types-Flask-Cors~=3.0
 types-mock~=5.0
 types-PyYAML~=6.0
 types-requests~=2.28
-types-setuptools~=65.6
+types-setuptools~=67.3
 types-smorest~=1.1
 types-SQLAlchemy~=1.4
 types-sqlalchemy-utils~=1.0
 types-urllib3<1.27
```

### Comparing `flask-ligand-0.7.2/setup.cfg` & `flask-ligand-0.7.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flask-ligand
-version = 0.7.2
+version = 0.7.3
 summary = A simple flask library for building microservices with RBAC JWT security, OpenAPI client and SQLAlchemy database support.
 description_file = README.rst
 description_content_type = text/x-rst; charset=UTF-8
 author = Ryan Gard
 author_email = ryan@gardiancapitol.com
 keywords = flask
 license = GNU Affero General Public License v3
```

### Comparing `flask-ligand-0.7.2/setup.py` & `flask-ligand-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/integration/conftest.py` & `flask-ligand-0.7.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/integration/migrations/alembic.ini` & `flask-ligand-0.7.3/tests/integration/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/integration/migrations/env.py` & `flask-ligand-0.7.3/tests/integration/migrations/env.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/integration/migrations/versions/47f10265b5d7_.py` & `flask-ligand-0.7.3/tests/integration/migrations/versions/47f10265b5d7_.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/integration/test_basic.py` & `flask-ligand-0.7.3/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/unit/conftest.py` & `flask-ligand-0.7.3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/unit/test_api_extension.py` & `flask-ligand-0.7.3/tests/unit/test_api_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/unit/test_database_extension.py` & `flask-ligand-0.7.3/tests/unit/test_database_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/unit/test_jwt_extension.py` & `flask-ligand-0.7.3/tests/unit/test_jwt_extension.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/unit/test_openapi_api.py` & `flask-ligand-0.7.3/tests/unit/test_openapi_api.py`

 * *Files identical despite different names*

### Comparing `flask-ligand-0.7.2/tests/unit/test_settings.py` & `flask-ligand-0.7.3/tests/unit/test_settings.py`

 * *Files identical despite different names*

