# Comparing `tmp/blueapi-0.2.2.tar.gz` & `tmp/blueapi-0.2.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.2.2.tar", last modified: Fri Apr 21 15:29:18 2023, max compression
+gzip compressed data, was "blueapi-0.2.3b1.tar", last modified: Mon Apr 24 15:19:11 2023, max compression
```

## Comparing `blueapi-0.2.2.tar` & `blueapi-0.2.3b1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.364698 blueapi-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 15:29:08.000000 blueapi-0.2.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-21 15:29:08.000000 blueapi-0.2.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.348698 blueapi-0.2.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-21 15:29:08.000000 blueapi-0.2.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-21 15:29:08.000000 blueapi-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 15:29:08.000000 blueapi-0.2.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 15:29:08.000000 blueapi-0.2.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-21 15:29:08.000000 blueapi-0.2.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-21 15:29:08.000000 blueapi-0.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-21 15:29:08.000000 blueapi-0.2.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 15:29:08.000000 blueapi-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-21 15:29:18.364698 blueapi-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-21 15:29:08.000000 blueapi-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 15:29:08.000000 blueapi-0.2.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/config/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 15:29:08.000000 blueapi-0.2.2/config/adsim.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 15:29:08.000000 blueapi-0.2.2/config/bl45p.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/docs/developer/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/explanations/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/explanations/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/explanations/type_validators.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.352698 blueapi-0.2.2/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   236122 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/images/blueapi-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-21 15:29:08.000000 blueapi-0.2.2/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.348698 blueapi-0.2.2/helm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 15:29:08.000000 blueapi-0.2.2/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-21 15:29:08.000000 blueapi-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:29:18.364698 blueapi-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.348698 blueapi-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 15:29:18.000000 blueapi-0.2.2/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/cli/amq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/src/blueapi/plans/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/plans/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/plans/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/service/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/service/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/startup/adsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/startup/bl45p.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/startup/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/utils/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/utils/thread_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/utils/type_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-21 15:29:08.000000 blueapi-0.2.2/src/blueapi/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.356698 blueapi-0.2.2/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-21 15:29:18.000000 blueapi-0.2.2/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-21 15:29:18.000000 blueapi-0.2.2/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:29:18.000000 blueapi-0.2.2/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 15:29:18.000000 blueapi-0.2.2/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 15:29:18.000000 blueapi-0.2.2/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 15:29:18.000000 blueapi-0.2.2/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/core/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.360698 blueapi-0.2.2/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/messaging/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.364698 blueapi-0.2.2/tests/plans/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/plans/test_scanspec_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:18.364698 blueapi-0.2.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/test_thread_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-21 15:29:08.000000 blueapi-0.2.2/tests/utils/test_type_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.756741 blueapi-0.2.3b1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/config/adsim.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/config/bl45p.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/developer/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.760741 blueapi-0.2.3b1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/explanations/type_validators.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   236122 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.756741 blueapi-0.2.3b1/helm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.756741 blueapi-0.2.3b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/amq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/plans/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/plans/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/service/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/service/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/adsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/bl45p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/utils/type_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.768741 blueapi-0.2.3b1/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/src/blueapi/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.764741 blueapi-0.2.3b1/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 15:19:11.000000 blueapi-0.2.3b1/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/plans/test_scanspec_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:11.772741 blueapi-0.2.3b1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-04-24 15:19:02.000000 blueapi-0.2.3b1/tests/utils/test_type_validator.py
```

### Comparing `blueapi-0.2.2/.devcontainer/Dockerfile` & `blueapi-0.2.3b1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.devcontainer/devcontainer.json` & `blueapi-0.2.3b1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/CONTRIBUTING.rst` & `blueapi-0.2.3b1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/actions/install_requirements/action.yml` & `blueapi-0.2.3b1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/dependabot.yml` & `blueapi-0.2.3b1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/pages/make_switcher.py` & `blueapi-0.2.3b1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/workflows/code.yml` & `blueapi-0.2.3b1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/workflows/docs.yml` & `blueapi-0.2.3b1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/workflows/docs_clean.yml` & `blueapi-0.2.3b1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/workflows/helm.yml` & `blueapi-0.2.3b1/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.github/workflows/linkcheck.yml` & `blueapi-0.2.3b1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.gitignore` & `blueapi-0.2.3b1/.gitignore`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.pre-commit-config.yaml` & `blueapi-0.2.3b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.vscode/launch.json` & `blueapi-0.2.3b1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/.vscode/settings.json` & `blueapi-0.2.3b1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/LICENSE` & `blueapi-0.2.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/PKG-INFO` & `blueapi-0.2.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.2.2
+Version: 0.2.3b1
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.2.2/README.rst` & `blueapi-0.2.3b1/README.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/conf.py` & `blueapi-0.2.3b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/explanations/architecture.rst` & `blueapi-0.2.3b1/docs/developer/explanations/architecture.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/explanations/decisions.rst` & `blueapi-0.2.3b1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/explanations/lifecycle.rst` & `blueapi-0.2.3b1/docs/developer/explanations/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/explanations/type_validators.rst` & `blueapi-0.2.3b1/docs/developer/explanations/type_validators.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/how-to/build-docs.rst` & `blueapi-0.2.3b1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/how-to/lint.rst` & `blueapi-0.2.3b1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/how-to/make-release.rst` & `blueapi-0.2.3b1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/how-to/run-tests.rst` & `blueapi-0.2.3b1/docs/developer/how-to/run-tests.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/how-to/update-tools.rst` & `blueapi-0.2.3b1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/index.rst` & `blueapi-0.2.3b1/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/reference/standards.rst` & `blueapi-0.2.3b1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/developer/tutorials/dev-install.rst` & `blueapi-0.2.3b1/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/images/blueapi-architecture.png` & `blueapi-0.2.3b1/docs/images/blueapi-architecture.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/images/dls-favicon.ico` & `blueapi-0.2.3b1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/images/dls-logo.svg` & `blueapi-0.2.3b1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/index.rst` & `blueapi-0.2.3b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/user/explanations/docs-structure.rst` & `blueapi-0.2.3b1/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/user/index.rst` & `blueapi-0.2.3b1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/docs/user/tutorials/installation.rst` & `blueapi-0.2.3b1/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/helm/blueapi/Chart.yaml` & `blueapi-0.2.3b1/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.2.3b1/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/helm/blueapi/templates/deployment.yaml` & `blueapi-0.2.3b1/helm/blueapi/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.2.3b1/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/helm/blueapi/values.yaml` & `blueapi-0.2.3b1/helm/blueapi/values.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/pyproject.toml` & `blueapi-0.2.3b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/cli/amq.py` & `blueapi-0.2.3b1/src/blueapi/cli/amq.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/cli/cli.py` & `blueapi-0.2.3b1/src/blueapi/cli/cli.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/cli/updates.py` & `blueapi-0.2.3b1/src/blueapi/cli/updates.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/config.py` & `blueapi-0.2.3b1/src/blueapi/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/core/__init__.py` & `blueapi-0.2.3b1/src/blueapi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/core/bluesky_types.py` & `blueapi-0.2.3b1/src/blueapi/core/bluesky_types.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/core/context.py` & `blueapi-0.2.3b1/src/blueapi/core/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from dataclasses import dataclass, field
 from importlib import import_module
 from pathlib import Path
 from types import ModuleType
 from typing import Dict, Iterable, List, Optional, Union
 
 from bluesky import RunEngine
-from bluesky.protocols import Flyable, Readable
 
 from blueapi.utils import (
     BlueapiPlanModelConfig,
     TypeValidatorDefinition,
     create_model_with_type_validators,
     load_module_all,
 )
 
 from .bluesky_types import (
     BLUESKY_PROTOCOLS,
     Device,
+    HasName,
     Plan,
     PlanGenerator,
     is_bluesky_compatible_device,
     is_bluesky_plan_generator,
 )
 from .device_lookup import find_component
 
@@ -140,15 +140,15 @@
             KeyError: If no name is found/supplied
         """
 
         if not is_bluesky_compatible_device(device):
             raise TypeError(f"{device} is not a Bluesky compatible device")
 
         if name is None:
-            if isinstance(device, Readable) or isinstance(device, Flyable):
+            if isinstance(device, HasName):
                 name = device.name
             else:
                 raise KeyError(f"Must supply a name for this device: {device}")
 
         self.devices[name] = device
```

### Comparing `blueapi-0.2.2/src/blueapi/core/device_lookup.py` & `blueapi-0.2.3b1/src/blueapi/core/device_lookup.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/core/event.py` & `blueapi-0.2.3b1/src/blueapi/core/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/messaging/base.py` & `blueapi-0.2.3b1/src/blueapi/messaging/base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.2.3b1/src/blueapi/messaging/stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/messaging/utils.py` & `blueapi-0.2.3b1/src/blueapi/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/plans/plans.py` & `blueapi-0.2.3b1/src/blueapi/plans/plans.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/plans/stubs.py` & `blueapi-0.2.3b1/src/blueapi/plans/stubs.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/service/app.py` & `blueapi-0.2.3b1/src/blueapi/service/app.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/service/model.py` & `blueapi-0.2.3b1/src/blueapi/service/model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/startup/adsim.py` & `blueapi-0.2.3b1/src/blueapi/startup/adsim.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/startup/bl45p.py` & `blueapi-0.2.3b1/src/blueapi/startup/bl45p.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/startup/example.py` & `blueapi-0.2.3b1/src/blueapi/startup/example.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/startup/simmotor.py` & `blueapi-0.2.3b1/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/utils/__init__.py` & `blueapi-0.2.3b1/src/blueapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/utils/base_model.py` & `blueapi-0.2.3b1/src/blueapi/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/utils/config.py` & `blueapi-0.2.3b1/src/blueapi/utils/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/utils/modules.py` & `blueapi-0.2.3b1/src/blueapi/utils/modules.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/utils/serialization.py` & `blueapi-0.2.3b1/src/blueapi/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/utils/thread_exception.py` & `blueapi-0.2.3b1/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/utils/type_validator.py` & `blueapi-0.2.3b1/src/blueapi/utils/type_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Optional,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     get_args,
+    get_type_hints,
     overload,
 )
 
 from pydantic import BaseConfig, BaseModel, create_model, validator
 from pydantic.fields import Undefined
 
 if TYPE_CHECKING:
@@ -171,17 +172,18 @@
     if func is not None:
         all_fields = {**all_fields, **_extract_fields_from_function(func)}
     for name, field in all_fields.items():
         annotation, val = field
         all_fields[name] = apply_type_validators(annotation, definitions), val
 
     validators = _type_validators(all_fields, definitions)
-    return create_model(  # type: ignore
+    model = create_model(  # type: ignore
         name, **all_fields, __base__=base, __validators__=validators, __config__=config
     )
+    return model
 
 
 def apply_type_validators(
     model_type: Type,
     definitions: List[TypeValidatorDefinition],
 ) -> Type:
     """
@@ -250,18 +252,22 @@
         name: (field.type_, field.field_info)
         for name, field in model.__fields__.items()
     }
 
 
 def _extract_fields_from_function(func: Callable[..., Any]) -> Fields:
     fields: Dict[str, FieldDefinition] = {}
+    # We must use get_type_hints to evaluate annotations due to
+    # PEP 563, see link:
+    # https://stackoverflow.com/questions/66734640/any-downsides-to-using-from-future-import-annotations-everywhere
+    type_hints = get_type_hints(func)
     for name, param in signature(func).parameters.items():
-        type_annotation = param.annotation
-        if type_annotation is Parameter.empty:
+        if name not in type_hints:
             raise TypeError(f"Missing type annotation for parameter {name}")
+        type_annotation = type_hints[name]
         default_value = param.default
         if default_value is Parameter.empty:
             default_value = Undefined
 
         anno = (type_annotation, default_value)
         fields[name] = anno
```

### Comparing `blueapi-0.2.2/src/blueapi/worker/event.py` & `blueapi-0.2.3b1/src/blueapi/worker/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/worker/multithread.py` & `blueapi-0.2.3b1/src/blueapi/worker/multithread.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/worker/reworker.py` & `blueapi-0.2.3b1/src/blueapi/worker/reworker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/worker/task.py` & `blueapi-0.2.3b1/src/blueapi/worker/task.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi/worker/worker.py` & `blueapi-0.2.3b1/src/blueapi/worker/worker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.2.3b1/src/blueapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.2.2
+Version: 0.2.3b1
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.2.2/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.2.3b1/src/blueapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/conftest.py` & `blueapi-0.2.3b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/core/test_context.py` & `blueapi-0.2.3b1/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/core/test_event.py` & `blueapi-0.2.3b1/tests/core/test_event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/messaging/test_stomptemplate.py` & `blueapi-0.2.3b1/tests/messaging/test_stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/messaging/test_utils.py` & `blueapi-0.2.3b1/tests/messaging/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/plans/test_scanspec_metadata.py` & `blueapi-0.2.3b1/tests/plans/test_scanspec_metadata.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/utils/test_config.py` & `blueapi-0.2.3b1/tests/utils/test_config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/utils/test_thread_exception.py` & `blueapi-0.2.3b1/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.2/tests/utils/test_type_validator.py` & `blueapi-0.2.3b1/tests/utils/test_type_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type, Union
 
 import pytest
 from pydantic import BaseConfig, BaseModel, Field, parse_obj_as
 from pydantic.dataclasses import dataclass
 from pydantic.fields import Undefined
 from scanspec.regions import Circle
@@ -95,14 +97,18 @@
     ...
 
 
 def baz(bar: Bar) -> None:
     ...
 
 
+def no_hints(a, b) -> None:
+    ...
+
+
 _DB: Mapping[str, ComplexObject] = {name: ComplexObject(name) for name in _REG.keys()}
 
 
 def lookup(letter: str) -> int:
     assert type(letter) is str, f"Expteced a string, got a {type(letter)}"
     return _REG[letter]
 
@@ -499,14 +505,23 @@
         "Foo", [TypeValidatorDefinition(int, lookup)], func=foo
     )
     parsed = parse_obj_as(model, {"a": "g", "b": "hello"})
     assert parsed.a == 6  # type: ignore
     assert parsed.b == "hello"  # type: ignore
 
 
+def test_does_not_allow_parameters_without_type_hints() -> None:
+    with pytest.raises(TypeError):
+        create_model_with_type_validators(
+            "Foo",
+            [TypeValidatorDefinition(int, lookup)],
+            func=no_hints,
+        )
+
+
 def test_model_from_complex_function_signature() -> None:
     model = create_model_with_type_validators(
         "Foo",
         [TypeValidatorDefinition(ComplexObject, lookup_complex)],
         func=bar,
         config=DefaultConfig,
     )
```

