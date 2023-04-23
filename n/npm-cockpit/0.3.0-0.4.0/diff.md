# Comparing `tmp/npm-cockpit-0.3.0.tar.gz` & `tmp/npm-cockpit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npm-cockpit-0.3.0.tar", max compression
+gzip compressed data, was "npm-cockpit-0.4.0.tar", max compression
```

## Comparing `npm-cockpit-0.3.0.tar` & `npm-cockpit-0.4.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1857 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/README.md
--rw-r--r--   0        0        0      604 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/__init__.py
--rw-r--r--   0        0        0     2348 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/Router.py
--rw-r--r--   0        0        0      885 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/Server.py
--rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/__init__.py
--rw-r--r--   0        0        0      916 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/app.py
--rw-r--r--   0        0        0      259 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Error.py
--rw-r--r--   0        0        0     1686 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Lib.py
--rw-r--r--   0        0        0      175 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Response.py
--rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/Semver.py
--rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/classes/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/__init__.py
--rw-r--r--   0        0        0     4185 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/dependencies.py
--rw-r--r--   0        0        0     1120 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/deprecated.py
--rw-r--r--   0        0        0      202 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/package.py
--rw-r--r--   0        0        0      797 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/updates.py
--rw-r--r--   0        0        0      890 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/data/vulnerabilities.py
--rw-r--r--   0        0        0     1068 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/src/app/path.py
--rw-r--r--   0        0        0      831 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/app/utils.py
--rw-r--r--   0        0        0      739 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/colors.css
--rw-r--r--   0        0        0     3919 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/styles.classes.css
--rw-r--r--   0        0        0     6144 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/styles.components.css
--rw-r--r--   0        0        0      738 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/src/client/css/styles.ids.css
--rw-r--r--   0        0        0     1579 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/css/styles.main.css
--rw-r--r--   0        0        0    15406 2023-03-13 15:18:57.374789 npm-cockpit-0.3.0/src/client/favicon.ico
--rw-r--r--   0        0        0   126616 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/font/Arimo-Bold.woff2
--rw-r--r--   0        0        0   126592 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/font/Arimo-Regular.woff2
--rw-r--r--   0        0        0   135036 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/font/Arimo-SemiBold.woff2
--rw-r--r--   0        0        0     1910 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/index.html
--rw-r--r--   0        0        0     2966 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/dashboard.js
--rw-r--r--   0        0        0     2673 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-filter.js
--rw-r--r--   0        0        0      756 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-info.js
--rw-r--r--   0        0        0     3679 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-item.js
--rw-r--r--   0        0        0      155 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/dependency-version.js
--rw-r--r--   0        0        0      342 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/icon.js
--rw-r--r--   0        0        0      233 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/index.js
--rw-r--r--   0        0        0     2071 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/select.js
--rw-r--r--   0        0        0     1985 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/elements/table.js
--rw-r--r--   0        0        0     2278 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/index.js
--rw-r--r--   0        0        0     2416 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/Item.js
--rw-r--r--   0        0        0     3973 2023-04-09 16:22:23.818755 npm-cockpit-0.3.0/src/client/js/components/items/basic-info.js
--rw-r--r--   0        0        0     3100 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/dependencies-list.js
--rw-r--r--   0        0        0     1545 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/dependencies-network.js
--rw-r--r--   0        0        0     2446 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/dependencies-tree.js
--rw-r--r--   0        0        0     1319 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/deprecated-table.js
--rw-r--r--   0        0        0      861 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/frequency.js
--rw-r--r--   0        0        0      665 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/index.js
--rw-r--r--   0        0        0      877 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/issues-table.js
--rw-r--r--   0        0        0     1362 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/package-data.js
--rw-r--r--   0        0        0     2871 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/updates-table.js
--rw-r--r--   0        0        0     1199 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/updates.js
--rw-r--r--   0        0        0     2962 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities-table.js
--rw-r--r--   0        0        0     1031 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities.js
--rw-r--r--   0        0        0      849 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/items/weight.js
--rw-r--r--   0        0        0      420 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/Popup.js
--rw-r--r--   0        0        0      791 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/group-data.js
--rw-r--r--   0        0        0      152 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/index.js
--rw-r--r--   0        0        0     2686 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/module-data.js
--rw-r--r--   0        0        0     3898 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups/section-info.js
--rw-r--r--   0        0        0     1682 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/popups.js
--rw-r--r--   0        0        0      369 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/components/widget.js
--rw-r--r--   0        0        0      336 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/index.js
--rw-r--r--   0        0        0   273912 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/lib/d3.min.js
--rw-r--r--   0        0        0     2846 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/plots/bar.js
--rw-r--r--   0        0        0     6813 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/js/plots/dependencies-network.js
--rw-r--r--   0        0        0     4261 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/js/plots/dependencies-tree.js
--rw-r--r--   0        0        0     2145 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/plots/donut.js
--rw-r--r--   0        0        0      171 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/plots/utils.js
--rw-r--r--   0        0        0      388 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/utils.js
--rw-r--r--   0        0        0      689 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/workers/dependenciesList.js
--rw-r--r--   0        0        0     2216 2023-03-13 15:18:57.378789 npm-cockpit-0.3.0/src/client/js/workers/dependenciesNetwork.js
--rw-r--r--   0        0        0     2479 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/dependenciesTree.js
--rw-r--r--   0        0        0      906 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/frequency.js
--rw-r--r--   0        0        0      268 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/issuesTable.js
--rw-r--r--   0        0        0      700 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/updates.js
--rw-r--r--   0        0        0      829 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/updatesTable.js
--rw-r--r--   0        0        0      341 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/js/workers/vulnerabilitiesTable.js
--rw-r--r--   0        0        0     1089 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/js/workers/weight.js
--rw-r--r--   0        0        0     2593 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/layout.json
--rw-r--r--   0        0        0     1207 2023-04-09 16:22:23.822756 npm-cockpit-0.3.0/src/client/static/center-icon.svg
--rw-r--r--   0        0        0     1025 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/clear-icon.svg
--rw-r--r--   0        0        0      668 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/dep-icon.svg
--rw-r--r--   0        0        0      325 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/info-icon.svg
--rw-r--r--   0        0        0     3649 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/loading.svg
--rw-r--r--   0        0        0     2103 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/net-icon.svg
--rw-r--r--   0        0        0        0 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/theme-icon.svg
--rw-r--r--   0        0        0     1643 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/tree-icon.svg
--rw-r--r--   0        0        0      402 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/update-icon.svg
--rw-r--r--   0        0        0      733 2023-03-13 15:18:57.382789 npm-cockpit-0.3.0/src/client/static/vuln-icon.svg
--rw-r--r--   0        0        0     3137 2023-04-09 16:27:16.643936 npm-cockpit-0.3.0/setup.py
--rw-r--r--   0        0        0     2575 2023-04-09 16:27:16.644183 npm-cockpit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1857 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/README.md
+-rw-r--r--   0        0        0      604 2023-04-23 21:45:26.729481 npm-cockpit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/__init__.py
+-rw-r--r--   0        0        0     2348 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/Router.py
+-rw-r--r--   0        0        0      885 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/Server.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/__init__.py
+-rw-r--r--   0        0        0      916 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/app.py
+-rw-r--r--   0        0        0      259 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/classes/Error.py
+-rw-r--r--   0        0        0     1686 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/classes/Lib.py
+-rw-r--r--   0        0        0      175 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/classes/Response.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/classes/Semver.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/classes/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/data/__init__.py
+-rw-r--r--   0        0        0     4185 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/data/dependencies.py
+-rw-r--r--   0        0        0     1120 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/data/deprecated.py
+-rw-r--r--   0        0        0      202 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/data/package.py
+-rw-r--r--   0        0        0      797 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/data/updates.py
+-rw-r--r--   0        0        0      890 2023-04-23 20:57:43.311521 npm-cockpit-0.4.0/src/app/data/vulnerabilities.py
+-rw-r--r--   0        0        0     1068 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/app/path.py
+-rw-r--r--   0        0        0      831 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/app/utils.py
+-rw-r--r--   0        0        0      739 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/css/colors.css
+-rw-r--r--   0        0        0     3917 2023-04-23 21:43:57.059126 npm-cockpit-0.4.0/src/client/css/styles.classes.css
+-rw-r--r--   0        0        0     6142 2023-04-23 21:44:05.991367 npm-cockpit-0.4.0/src/client/css/styles.components.css
+-rw-r--r--   0        0        0      738 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/css/styles.ids.css
+-rw-r--r--   0        0        0     1579 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/css/styles.main.css
+-rw-r--r--   0        0        0    15406 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/favicon.ico
+-rw-r--r--   0        0        0   126616 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/font/Arimo-Bold.woff2
+-rw-r--r--   0        0        0   126592 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/font/Arimo-Regular.woff2
+-rw-r--r--   0        0        0   135036 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/font/Arimo-SemiBold.woff2
+-rw-r--r--   0        0        0     1910 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/index.html
+-rw-r--r--   0        0        0     2966 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/dashboard.js
+-rw-r--r--   0        0        0     2673 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/dependency-filter.js
+-rw-r--r--   0        0        0      756 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/dependency-info.js
+-rw-r--r--   0        0        0     3679 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/dependency-item.js
+-rw-r--r--   0        0        0      155 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/dependency-version.js
+-rw-r--r--   0        0        0      342 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/icon.js
+-rw-r--r--   0        0        0      233 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/index.js
+-rw-r--r--   0        0        0     2071 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/select.js
+-rw-r--r--   0        0        0     1985 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/elements/table.js
+-rw-r--r--   0        0        0     2278 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/index.js
+-rw-r--r--   0        0        0     2416 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/Item.js
+-rw-r--r--   0        0        0     3973 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/basic-info.js
+-rw-r--r--   0        0        0     3967 2023-04-23 22:01:18.937065 npm-cockpit-0.4.0/src/client/js/components/items/dependencies-list.js
+-rw-r--r--   0        0        0     1545 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/dependencies-network.js
+-rw-r--r--   0        0        0     2446 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/dependencies-tree.js
+-rw-r--r--   0        0        0     1319 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/deprecated-table.js
+-rw-r--r--   0        0        0      861 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/frequency.js
+-rw-r--r--   0        0        0      665 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/index.js
+-rw-r--r--   0        0        0      877 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/issues-table.js
+-rw-r--r--   0        0        0     1362 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/package-data.js
+-rw-r--r--   0        0        0     2871 2023-04-23 21:36:57.041383 npm-cockpit-0.4.0/src/client/js/components/items/updates-table.js
+-rw-r--r--   0        0        0     1199 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/updates.js
+-rw-r--r--   0        0        0     2962 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/vulnerabilities-table.js
+-rw-r--r--   0        0        0     1031 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/vulnerabilities.js
+-rw-r--r--   0        0        0      849 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/items/weight.js
+-rw-r--r--   0        0        0      420 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/popups/Popup.js
+-rw-r--r--   0        0        0      791 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/popups/group-data.js
+-rw-r--r--   0        0        0      152 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/popups/index.js
+-rw-r--r--   0        0        0     2686 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/popups/module-data.js
+-rw-r--r--   0        0        0     3997 2023-04-23 21:43:13.553924 npm-cockpit-0.4.0/src/client/js/components/popups/section-info.js
+-rw-r--r--   0        0        0     1682 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/popups.js
+-rw-r--r--   0        0        0      369 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/components/widget.js
+-rw-r--r--   0        0        0      336 2023-04-23 20:57:43.315521 npm-cockpit-0.4.0/src/client/js/index.js
+-rw-r--r--   0        0        0   273912 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/lib/d3.min.js
+-rw-r--r--   0        0        0     2846 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/plots/bar.js
+-rw-r--r--   0        0        0     6813 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/plots/dependencies-network.js
+-rw-r--r--   0        0        0     4261 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/plots/dependencies-tree.js
+-rw-r--r--   0        0        0     2145 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/plots/donut.js
+-rw-r--r--   0        0        0      171 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/plots/utils.js
+-rw-r--r--   0        0        0      388 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/utils.js
+-rw-r--r--   0        0        0      689 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/dependenciesList.js
+-rw-r--r--   0        0        0     2216 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/dependenciesNetwork.js
+-rw-r--r--   0        0        0     2479 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/dependenciesTree.js
+-rw-r--r--   0        0        0      906 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/frequency.js
+-rw-r--r--   0        0        0      268 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/issuesTable.js
+-rw-r--r--   0        0        0      700 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/updates.js
+-rw-r--r--   0        0        0      829 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/updatesTable.js
+-rw-r--r--   0        0        0      341 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/vulnerabilitiesTable.js
+-rw-r--r--   0        0        0     1089 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/js/workers/weight.js
+-rw-r--r--   0        0        0     2593 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/layout.json
+-rw-r--r--   0        0        0     1207 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/center-icon.svg
+-rw-r--r--   0        0        0     1025 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/clear-icon.svg
+-rw-r--r--   0        0        0      668 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/dep-icon.svg
+-rw-r--r--   0        0        0      325 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/info-icon.svg
+-rw-r--r--   0        0        0     3649 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/loading.svg
+-rw-r--r--   0        0        0     2103 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/net-icon.svg
+-rw-r--r--   0        0        0        0 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/theme-icon.svg
+-rw-r--r--   0        0        0     1643 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/tree-icon.svg
+-rw-r--r--   0        0        0      402 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/update-icon.svg
+-rw-r--r--   0        0        0      733 2023-04-23 20:57:43.319521 npm-cockpit-0.4.0/src/client/static/vuln-icon.svg
+-rw-r--r--   0        0        0     3137 2023-04-23 22:05:47.238184 npm-cockpit-0.4.0/setup.py
+-rw-r--r--   0        0        0     2575 2023-04-23 22:05:47.238473 npm-cockpit-0.4.0/PKG-INFO
```

### Comparing `npm-cockpit-0.3.0/README.md` & `npm-cockpit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/pyproject.toml` & `npm-cockpit-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "npm-cockpit"
-version = "0.3.0"
+version = "0.4.0"
 description = "Installable command-line tool with web interface which helps to track nodejs project dependencies state"
 authors = ["Alex Chirkin <hello@alexchirkin.me>"]
 readme = "README.md"
 packages = [{include = "src"}]
 keywords=[
   "command",
   "dashboard",
```

### Comparing `npm-cockpit-0.3.0/src/app/Router.py` & `npm-cockpit-0.4.0/src/app/Router.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/Server.py` & `npm-cockpit-0.4.0/src/app/Server.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/app.py` & `npm-cockpit-0.4.0/src/app/app.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/classes/Lib.py` & `npm-cockpit-0.4.0/src/app/classes/Lib.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/data/dependencies.py` & `npm-cockpit-0.4.0/src/app/data/dependencies.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/data/deprecated.py` & `npm-cockpit-0.4.0/src/app/data/deprecated.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/data/updates.py` & `npm-cockpit-0.4.0/src/app/data/updates.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/data/vulnerabilities.py` & `npm-cockpit-0.4.0/src/app/data/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/path.py` & `npm-cockpit-0.4.0/src/app/path.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/app/utils.py` & `npm-cockpit-0.4.0/src/app/utils.py`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/css/colors.css` & `npm-cockpit-0.4.0/src/client/css/colors.css`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/css/styles.classes.css` & `npm-cockpit-0.4.0/src/client/css/styles.classes.css`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
   align-items: center;
   border-bottom: 1px solid var(--border);
   font-family: 'ArimoSemiBold';
 }
 
 .popup-body {
   max-height: 300px;
-  overflow-y: scroll;
+  overflow-y: auto;
   width: 100%;
 }
 
 .popup-section {
   padding: 16px 8px;
   border-bottom: 1px solid var(--border);
   color: var(--text);
```

### Comparing `npm-cockpit-0.3.0/src/client/css/styles.components.css` & `npm-cockpit-0.4.0/src/client/css/styles.components.css`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 popups-root {
   position: absolute;
   top: 0;
   left: 0;
 }
 
 updates-table, vulnerabilities-table, issues-table, deprecated-table {
-  overflow-y: scroll;
+  overflow-y: auto;
   border-radius: 6px;
 }
 
 .total {
   fill: #5F7278;
 }
```

### Comparing `npm-cockpit-0.3.0/src/client/css/styles.ids.css` & `npm-cockpit-0.4.0/src/client/css/styles.ids.css`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/css/styles.main.css` & `npm-cockpit-0.4.0/src/client/css/styles.main.css`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/favicon.ico` & `npm-cockpit-0.4.0/src/client/favicon.ico`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/font/Arimo-Bold.woff2` & `npm-cockpit-0.4.0/src/client/font/Arimo-Bold.woff2`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/font/Arimo-Regular.woff2` & `npm-cockpit-0.4.0/src/client/font/Arimo-Regular.woff2`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/font/Arimo-SemiBold.woff2` & `npm-cockpit-0.4.0/src/client/font/Arimo-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/index.html` & `npm-cockpit-0.4.0/src/client/index.html`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/dashboard.js` & `npm-cockpit-0.4.0/src/client/js/components/dashboard.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/elements/dependency-filter.js` & `npm-cockpit-0.4.0/src/client/js/components/elements/dependency-filter.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/elements/dependency-info.js` & `npm-cockpit-0.4.0/src/client/js/components/elements/dependency-info.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/elements/dependency-item.js` & `npm-cockpit-0.4.0/src/client/js/components/elements/dependency-item.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/elements/select.js` & `npm-cockpit-0.4.0/src/client/js/components/elements/select.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/elements/table.js` & `npm-cockpit-0.4.0/src/client/js/components/elements/table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/index.js` & `npm-cockpit-0.4.0/src/client/js/components/index.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/Item.js` & `npm-cockpit-0.4.0/src/client/js/components/items/Item.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/basic-info.js` & `npm-cockpit-0.4.0/src/client/js/components/items/basic-info.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/dependencies-list.js` & `npm-cockpit-0.4.0/src/client/js/components/items/dependencies-list.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -13,14 +13,19 @@
         super('/api/dependencies')
 
         window.addEventListener('dependency-filter-applied-dependencies-list', (e) => {
             this.applyFilter('dependency', e.detail)
             this.renderDependencies()
         })
 
+        window.addEventListener('custom-select-applied-dependencies-direct', (e) => {
+            this.applyFilter('direct', e.detail)
+            this.renderDependencies()
+        })
+
         this.listWorker = new Worker('/js/workers/dependenciesList.js', {
             type: "module"
         })
         this.listWorker.onmessage = (e) => {
             this.processedData = e.data
             super.loading = false
             this.render()
@@ -51,15 +56,20 @@
         this.render()
     }
 
     addFilters(container) {
         const dependencyFilter = document.createElement('dependency-filter')
         dependencyFilter.id = 'dependencies-list'
 
-        container.append(dependencyFilter)
+        const direct = document.createElement('custom-select')
+        direct.id = 'dependencies-direct'
+        direct.__options__ = ['true', 'false']
+        direct.__placeholder__ = 'Direct'
+
+        container.append(direct, dependencyFilter)
     }
 
     renderDependencies() {
         let dependenciesList = this.querySelector('.dependencies-list_list')
 
         if (!dependenciesList) {
             dependenciesList = document.createElement('div')
@@ -67,20 +77,35 @@
         }
 
         // clear before re-render
         dependenciesList.textContent = ''
 
         const dependencies = this.processedData
         const filter = this.filters['dependency']
+        const directFilter = this.filters['direct']
 
         let items = Object.entries(dependencies)
 
+        if (filter || directFilter) {
+            items = items.filter(item => {
+                if (filter && !(item[0] === filter)) {
+                    return false
+                }
+
+                if (directFilter === 'true' && !this.data.dependencies[this.data.root][0].connections.find(connection => connection.name === item[0])) {
+                    return false
+                }
+
+                if (directFilter === 'false' && this.data.dependencies[this.data.root][0].connections.find(connection => connection.name === item[0])) {
+                    return false
+                }
+
 
-        if (filter) {
-            items = items.filter(item => item[0] === filter)
+                return true
+            })
         }
 
         items = items.map(dependency => {
             const [name, versions] = dependency
             const dependencyItem = document.createElement('dependency-item')
             dependencyItem.addEventListener('click', (e) => {
                 e.stopPropagation()
```

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/dependencies-network.js` & `npm-cockpit-0.4.0/src/client/js/components/items/dependencies-network.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/dependencies-tree.js` & `npm-cockpit-0.4.0/src/client/js/components/items/dependencies-tree.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/deprecated-table.js` & `npm-cockpit-0.4.0/src/client/js/components/items/deprecated-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/frequency.js` & `npm-cockpit-0.4.0/src/client/js/components/items/frequency.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/index.js` & `npm-cockpit-0.4.0/src/client/js/components/items/index.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/issues-table.js` & `npm-cockpit-0.4.0/src/client/js/components/items/issues-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/package-data.js` & `npm-cockpit-0.4.0/src/client/js/components/items/package-data.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/updates-table.js` & `npm-cockpit-0.4.0/src/client/js/components/items/updates-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/updates.js` & `npm-cockpit-0.4.0/src/client/js/components/items/updates.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities-table.js` & `npm-cockpit-0.4.0/src/client/js/components/items/vulnerabilities-table.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/vulnerabilities.js` & `npm-cockpit-0.4.0/src/client/js/components/items/vulnerabilities.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/items/weight.js` & `npm-cockpit-0.4.0/src/client/js/components/items/weight.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/popups/group-data.js` & `npm-cockpit-0.4.0/src/client/js/components/popups/group-data.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/popups/module-data.js` & `npm-cockpit-0.4.0/src/client/js/components/popups/module-data.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/components/popups/section-info.js` & `npm-cockpit-0.4.0/src/client/js/components/popups/section-info.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -12,14 +12,15 @@
         'Updates diagram - shows how many updates of different types are found.'
     ],
     'dependencies-list': [
         'Dependencies list shows all dependencies in a row.',
         'Every dependency row contains list of versions found in dependencies tree.',
         'Row also contains indicators of found states - updates / vulnerabilities found, package is deprecated (click on an indicator to see dependency in a proper section).',
         'To see dependency in the tree or network chart click on a proper icon.',
+        'To show only direct dependencies or exclude them from the list "Direct" filter can be used.',
         'Specific dependency can be found by using dependencies filter.'
     ],
     'updates-list': [
         'Updates list represents all available updates for dependencies in a table.',
         'Updatable column shows is dependency can be updated by running "npm update" command',
         'Table can be filtered by specific dependency name, update type or updatable state by using proper filter.'
     ],
```

### Comparing `npm-cockpit-0.3.0/src/client/js/components/popups.js` & `npm-cockpit-0.4.0/src/client/js/components/popups.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/lib/d3.min.js` & `npm-cockpit-0.4.0/src/client/js/lib/d3.min.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/plots/bar.js` & `npm-cockpit-0.4.0/src/client/js/plots/bar.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/plots/dependencies-network.js` & `npm-cockpit-0.4.0/src/client/js/plots/dependencies-network.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/plots/dependencies-tree.js` & `npm-cockpit-0.4.0/src/client/js/plots/dependencies-tree.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/plots/donut.js` & `npm-cockpit-0.4.0/src/client/js/plots/donut.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/workers/dependenciesList.js` & `npm-cockpit-0.4.0/src/client/js/workers/dependenciesList.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/workers/dependenciesNetwork.js` & `npm-cockpit-0.4.0/src/client/js/workers/dependenciesNetwork.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/workers/dependenciesTree.js` & `npm-cockpit-0.4.0/src/client/js/workers/dependenciesTree.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/workers/frequency.js` & `npm-cockpit-0.4.0/src/client/js/workers/frequency.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/workers/updates.js` & `npm-cockpit-0.4.0/src/client/js/workers/updates.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/workers/updatesTable.js` & `npm-cockpit-0.4.0/src/client/js/workers/updatesTable.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/js/workers/weight.js` & `npm-cockpit-0.4.0/src/client/js/workers/weight.js`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/layout.json` & `npm-cockpit-0.4.0/src/client/layout.json`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/static/center-icon.svg` & `npm-cockpit-0.4.0/src/client/static/center-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/static/clear-icon.svg` & `npm-cockpit-0.4.0/src/client/static/clear-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/static/dep-icon.svg` & `npm-cockpit-0.4.0/src/client/static/dep-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/static/loading.svg` & `npm-cockpit-0.4.0/src/client/static/loading.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/static/net-icon.svg` & `npm-cockpit-0.4.0/src/client/static/net-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/static/tree-icon.svg` & `npm-cockpit-0.4.0/src/client/static/tree-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/src/client/static/vuln-icon.svg` & `npm-cockpit-0.4.0/src/client/static/vuln-icon.svg`

 * *Files identical despite different names*

### Comparing `npm-cockpit-0.3.0/setup.py` & `npm-cockpit-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ['requests>=2.28.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['npm-cockpit = src.app.app:init']}
 
 setup_kwargs = {
     'name': 'npm-cockpit',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Installable command-line tool with web interface which helps to track nodejs project dependencies state',
     'long_description': '# NPM-COCKPIT\n\nA user-friendly application for JavaScript developers to visualize the dependency tree of NPM packages and NodeJS applications. \n\nAllows to get statistical info about application dependencies tree state. Provides an interface for filtering and viewing information through convenient tables and diagrams.\n\n## Features\n\nVisual representation of the entire dependency tree of a project. With ability to look all the paths for a specific package. Dependency tree can be visualized as a tree or directed network chart\n\n![tree chart](https://chartexample.com/images/npm-cockpit/network.jpg)\n\nDetailed information about each package, including version, description, and related links.\n\n![packages list](https://chartexample.com/images/npm-cockpit/list.jpg)\n\nIdentify potential issues such as outdated, deprecated or vulnerable packages.\n\n![packages list](https://chartexample.com/images/npm-cockpit/deprecated.jpg)\n\n**AND MUCH MORE!**\n\n\n## Requirements\n\n### General\n- Terminal or command prompt access\n- Target application folder should contain node_modules folder with installed dependencies and package.json\n- Node.js and NPM installed\n\n### As NPM package\n- `python` command should be available\n\n## Usage\n\n### Command params\n\n`path` - a path to project folder with package.json and node_modules inside\n\n`port` - available local port to serve the app (default `8080`)\n\n### PIP\n`pip install npm-cockpit`\n\n`npm-cockpit [path] [port]`\n\n### NPM globally installed\n`npm install --global npm-cockpit`\n\n`npm-cockpit [path] [port]`\n\n### NPX\n`npx npm-cockpit [path] [port]`\n\n### NPM dependency in package\n`npm install npm-cockpit` and add the run script in the package json with proper params\n\n## Development\n- `git clone https://github.com/b0000ring/npm-cockpit.git`\n- `cd npm-cockpit`\n- `node index.js [path] [port]` or `python __main__.py [path] [port]`\n',
     'author': 'Alex Chirkin',
     'author_email': 'hello@alexchirkin.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `npm-cockpit-0.3.0/PKG-INFO` & `npm-cockpit-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npm-cockpit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Installable command-line tool with web interface which helps to track nodejs project dependencies state
 License: MIT
 Keywords: command,dashboard,npm,statistic,dependencies,packages,info
 Author: Alex Chirkin
 Author-email: hello@alexchirkin.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

