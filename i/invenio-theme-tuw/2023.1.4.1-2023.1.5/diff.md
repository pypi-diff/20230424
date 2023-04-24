# Comparing `tmp/invenio-theme-tuw-2023.1.4.1.tar.gz` & `tmp/invenio-theme-tuw-2023.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-theme-tuw-2023.1.4.1.tar", last modified: Mon Mar  6 14:22:58 2023, max compression
+gzip compressed data, was "invenio-theme-tuw-2023.1.5.tar", last modified: Mon Apr 24 12:02:26 2023, max compression
```

## Comparing `invenio-theme-tuw-2023.1.4.1.tar` & `invenio-theme-tuw-2023.1.5.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.682585 invenio-theme-tuw-2023.1.4.1/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      617 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.4.1/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.4.1/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.658585 invenio-theme-tuw-2023.1.4.1/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1042 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      287 2021-07-15 12:29:34.000000 invenio-theme-tuw-2023.1.4.1/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5835 2023-03-06 14:19:50.000000 invenio-theme-tuw-2023.1.4.1/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3370 2021-07-15 12:29:34.000000 invenio-theme-tuw-2023.1.4.1/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      202 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1688 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.4.1/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7796 2023-03-06 14:22:58.682585 invenio-theme-tuw-2023.1.4.1/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      535 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.658585 invenio-theme-tuw-2023.1.4.1/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7453 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10122 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.4.1/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      238 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      441 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7003 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/docs/requirements.txt
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.658585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      374 2023-03-06 14:19:50.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       78 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/.babelrc
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       11 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/.eslintignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      751 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/.eslintrc.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/build/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7024 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/build/webpack.config.js
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2681 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/package.json
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/patches/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      560 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/patches/watchpack+1.7.4.patch
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3296 2023-01-12 16:50:01.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2187 2022-11-24 12:58:26.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      763 2022-10-17 09:59:49.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/search.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      576 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/pdf-preview/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      383 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/pdf-preview/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      966 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      213 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       70 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      984 2022-09-07 12:08:20.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7027 2023-03-06 14:19:50.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       69 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      210 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      479 2022-09-08 10:53:10.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/contact.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      665 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1312 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3045 2022-11-25 16:08:24.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.666585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      503 2022-09-02 11:49:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-09-02 11:49:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      599 2022-09-02 13:37:47.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       68 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      331 2022-10-27 14:52:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.670585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   287936 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   209784 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   270524 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   278168 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168060 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   174108 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167336 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   171508 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   170504 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167000 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173172 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168644 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173416 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168260 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168488 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   172860 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.670585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      291 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4221 2022-10-11 15:00:42.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1150 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.670585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36366 2022-10-10 09:44:16.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22946 2022-10-10 09:44:16.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    43552 2022-10-10 09:44:16.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.674585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2569 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      154 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      161 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      369 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      338 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2326 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.674585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       60 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.overrides
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.variables
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2022-09-05 14:21:18.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/favicon-16x16.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1101 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/favicon-32x32.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12850 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/faq.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    27714 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13548 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/online-chat.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    21722 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/upload-file.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13376 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/fair-data-austria.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4636 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2512 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    17390 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/rdmlogo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     9811 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3926 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13674 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/pdf.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19926 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36394 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/connection.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8098 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/git.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37302 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/group.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    34924 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22964 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/team.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29404 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/user.webp
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    31176 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/version.webp
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/tuwstones/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    70038 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.654585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.658585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.658585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16215 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      944 2022-09-22 13:15:45.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_previewer/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16000 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_previewer/pdfjs.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1719 2022-10-03 16:21:50.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7653 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2836 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      842 2023-01-13 10:52:22.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1710 2023-02-20 18:21:08.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1816 2023-03-05 16:42:00.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.678585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      974 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.682585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2355 2023-03-06 14:19:50.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7864 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5012 2023-02-20 18:21:08.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      567 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1501 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8551 2022-10-27 14:52:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      759 2022-09-02 11:49:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2101 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2676 2023-02-20 18:21:08.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      668 2022-10-03 16:21:50.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1463 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.682585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1278 2022-09-05 14:21:18.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7982 2023-01-19 10:40:45.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/views.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3209 2022-10-17 09:59:49.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/webpack.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.662585 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7796 2023-03-06 14:22:58.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16065 2023-03-06 14:22:58.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-03-06 14:22:58.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      228 2023-03-06 14:22:58.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-03-06 14:22:58.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      140 2023-03-06 14:22:58.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       18 2023-03-06 14:22:58.000000 invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.4.1/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.4.1/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.4.1/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2364 2023-03-06 14:22:58.682585 invenio-theme-tuw-2023.1.4.1/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      294 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.4.1/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-03-06 14:22:58.682585 invenio-theme-tuw-2023.1.4.1/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      853 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      386 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.4.1/tests/test_invenio_theme_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      617 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.5/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.5/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.567720 invenio-theme-tuw-2023.1.5/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1042 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      287 2021-07-15 12:29:34.000000 invenio-theme-tuw-2023.1.5/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5958 2023-04-24 11:32:11.000000 invenio-theme-tuw-2023.1.5/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3370 2021-07-15 12:29:34.000000 invenio-theme-tuw-2023.1.5/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      202 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1688 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.5/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7917 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      535 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7453 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      233 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10122 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.5/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      238 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      441 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7003 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/docs/requirements.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      372 2023-04-24 11:32:11.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       78 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/.babelrc
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       11 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/.eslintignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      751 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/.eslintrc.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/build/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7024 2023-04-24 11:32:11.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/build/webpack.config.js
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2681 2023-04-24 11:32:11.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/package.json
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/patches/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      560 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/patches/watchpack+1.7.4.patch
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3508 2023-04-24 11:32:11.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2187 2022-11-24 12:58:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      763 2022-10-17 09:59:49.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/search.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.567720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.563719 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.563719 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.563719 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.563719 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      576 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/pdf-preview/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      383 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/pdf-preview/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      966 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.563719 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      213 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       70 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/breadcrumb.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      984 2022-09-07 12:08:20.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/grid.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7027 2023-03-06 14:19:50.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1040 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       69 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      210 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/message.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/table.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      479 2022-09-08 10:53:10.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/contact.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      665 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1312 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3045 2022-11-25 16:08:24.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.575720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      503 2022-09-02 11:49:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-09-02 11:49:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      599 2022-09-02 13:37:47.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       68 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/divider.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/flag.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/header.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      331 2022-10-27 14:52:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/icon.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/image.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/input.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/label.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/list.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/loader.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/rail.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/reveal.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/segment.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/step.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.579720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   287936 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   209784 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   270524 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   278168 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168060 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   174108 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167336 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   171508 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   170504 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   167000 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173172 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168644 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   173416 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168260 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   168488 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)   172860 2022-09-19 15:50:46.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.579720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      291 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/reset.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4302 2023-04-24 11:32:11.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1150 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.583720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36366 2022-10-10 09:44:16.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22946 2022-10-10 09:44:16.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    43552 2022-10-10 09:44:16.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.583720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       65 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/accordion.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/chatroom.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2569 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dimmer.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      154 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      161 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/dropdown.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/embed.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/modal.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       59 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/nag.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/popup.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       64 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/progress.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/rating.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/search.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/shape.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      369 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      338 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sidebar.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       62 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/sticky.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/tab.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       66 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/transition.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2326 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.587720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       56 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/ad.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/card.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       61 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/comment.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/feed.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       60 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       58 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/item.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.overrides
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       63 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/views/statistic.variables
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2022-09-05 14:21:18.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.567720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.587720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      794 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/favicon-16x16.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1101 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/favicon-32x32.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.587720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    12850 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/faq.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    27714 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13548 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/online-chat.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    21722 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/upload-file.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.587720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13376 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/fair-data-austria.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4636 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2512 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    17390 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/rdmlogo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     9811 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3926 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    13674 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/pdf.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.587720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    19926 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    36394 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/connection.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8098 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/git.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    37302 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/group.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    34924 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    22964 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/team.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    29404 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/user.webp
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    31176 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/version.webp
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.587720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/tuwstones/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    70038 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.567720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.567720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.567720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.587720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16215 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      944 2022-09-22 13:15:45.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_previewer/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16000 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_previewer/pdfjs.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1719 2022-10-03 16:21:50.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7653 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2836 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      842 2023-01-13 10:52:22.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1710 2023-02-20 18:21:08.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1649 2023-04-05 13:35:38.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/deposit.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      974 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2355 2023-03-06 14:19:50.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8208 2023-04-24 11:32:11.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5012 2023-02-20 18:21:08.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      567 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1501 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8551 2022-10-27 14:52:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      759 2022-09-02 11:49:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2101 2022-07-19 15:54:31.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2676 2023-02-20 18:21:08.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      668 2022-10-03 16:21:50.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1463 2022-11-30 11:55:52.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1278 2022-09-05 14:21:18.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7982 2023-01-19 10:40:45.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/views.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3209 2022-10-17 09:59:49.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw/webpack.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.571720 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7917 2023-04-24 12:02:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    16065 2023-04-24 12:02:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-24 12:02:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      228 2023-04-24 12:02:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-24 12:02:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      140 2023-04-24 12:02:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       18 2023-04-24 12:02:26.000000 invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.5/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      491 2021-07-05 13:11:26.000000 invenio-theme-tuw-2023.1.5/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      725 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.5/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2364 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      294 2022-11-23 16:27:37.000000 invenio-theme-tuw-2023.1.5/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 12:02:26.591720 invenio-theme-tuw-2023.1.5/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      853 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      386 2022-07-14 09:43:44.000000 invenio-theme-tuw-2023.1.5/tests/test_invenio_theme_tuw.py
```

### Comparing `invenio-theme-tuw-2023.1.4.1/.editorconfig` & `invenio-theme-tuw-2023.1.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/.tx/config` & `invenio-theme-tuw-2023.1.5/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/CHANGES.rst` & `invenio-theme-tuw-2023.1.5/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,26 @@
     Invenio Theme TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.1 (released 2023-01-13, updated 2023-03-06)
+Version 2023.1 (released 2023-01-13, updated 2023-04-24)
 
 - Display the record's first uploaders on the landing pages
 - Fix the draft preview page failing with a 404 code
 - Update links to policies
 - UI: fix header warning styling and improve permission guard pages
 - UI: rework deposit permission guard page text
 - UI: further improve deposit permission guard page text and modify its header icon
 - Footer: Improve layout and responsiveness on smaller screens
 - Fix naming of grid classes in css to avoid overlaps with `semantic-ui-less`
+- UI: remove reference to test instance from deposit guard page
+- Add possibility to a render an info box in the frontpage
 
 
 Version 2022.6 (released 2022-10-17, updated 2022-11-30)
 
 - v10 compat: Replace direct 'elasticsearch' import
 - v10 compat: Load and pass ``custom_fields`` in ``communities_new`` view function
 - Override ``app.config`` to specially handle our ``SITE_{API,UI}_URL`` config items
```

### Comparing `invenio-theme-tuw-2023.1.4.1/CONTRIBUTING.rst` & `invenio-theme-tuw-2023.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/LICENSE` & `invenio-theme-tuw-2023.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/MANIFEST.in` & `invenio-theme-tuw-2023.1.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/PKG-INFO` & `invenio-theme-tuw-2023.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tuw
-Version: 2023.1.4.1
+Version: 2023.1.5
 Summary: "TU Wien theme for Invenio (RDM)."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-theme-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio theme tuw
 Platform: any
@@ -66,24 +66,26 @@
     Invenio Theme TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.1 (released 2023-01-13, updated 2023-03-06)
+Version 2023.1 (released 2023-01-13, updated 2023-04-24)
 
 - Display the record's first uploaders on the landing pages
 - Fix the draft preview page failing with a 404 code
 - Update links to policies
 - UI: fix header warning styling and improve permission guard pages
 - UI: rework deposit permission guard page text
 - UI: further improve deposit permission guard page text and modify its header icon
 - Footer: Improve layout and responsiveness on smaller screens
 - Fix naming of grid classes in css to avoid overlaps with `semantic-ui-less`
+- UI: remove reference to test instance from deposit guard page
+- Add possibility to a render an info box in the frontpage
 
 
 Version 2022.6 (released 2022-10-17, updated 2022-11-30)
 
 - v10 compat: Replace direct 'elasticsearch' import
 - v10 compat: Load and pass ``custom_fields`` in ``communities_new`` view function
 - Override ``app.config`` to specially handle our ``SITE_{API,UI}_URL`` config items
```

### Comparing `invenio-theme-tuw-2023.1.4.1/README.rst` & `invenio-theme-tuw-2023.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/babel.ini` & `invenio-theme-tuw-2023.1.5/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/docs/Makefile` & `invenio-theme-tuw-2023.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/docs/conf.py` & `invenio-theme-tuw-2023.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/docs/make.bat` & `invenio-theme-tuw-2023.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/.eslintrc.js` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/build/webpack.config.js` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/build/webpack.config.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/package.json` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/package.json`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/build_project/patches/watchpack+1.7.4.patch` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/build_project/patches/watchpack+1.7.4.patch`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/config.py` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2022 TU Wien.
+# Copyright (C) 2020-2023 TU Wien.
 #
 # Invenio-Theme-TUW is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """TU Wien theme for Invenio (RDM)."""
 
 THEME_TUW_MATOMO_ENABLED = False
@@ -18,18 +18,24 @@
 
 THEME_TUW_HEADER_WARNING = None
 """The (HTML-formatted) message to display in the header.
 
 A value of ``None`` (which is the default) causes the message box to not be displayed.
 """
 
+THEME_TUW_FRONTPAGE_INFO = None
+"""The (HTML-formatted) info message to display in the frontpage.
+
+A value of ``None`` (which is the default) causes the info message box to not be displayed.
+"""
+
 THEME_TUW_FRONTPAGE_WARNING = None
-"""The (HTML-formatted) message to display in the frontpage.
+"""The (HTML-formatted) warning message to display in the frontpage.
 
-A value of ``None`` (which is the default) causes the message box to not be displayed.
+A value of ``None`` (which is the default) causes the warning message box to not be displayed.
 """
 
 THEME_TUW_CONTACT_EMAIL = "tudata@tuwien.ac.at"
 """The e-mail address provided as contact."""
 
 APP_THEME = ["semantic-ui"]
 """The application theme to use."""
```

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/ext.py` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/search.py` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/search.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/mobilemenu/index.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/js/invenio_theme_tuw/tracking/index.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/form.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/collections/menu.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/file-list.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/flip-card.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/custom/fonts.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/button.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/elements/container.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/PTSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.overrides`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,19 @@
   background-color: #FEEFB3;
   display: flex;
   text-align: center;
   width: 100%;
   flex: 1 0 auto;
   align-items: center;
 
+  .close.icon {
+    top: 1em;
+    margin-right: 1em;
+  }
+
   .exclamation.triangle.icon {
     margin-right: 1em;
     flex: 0 0 auto;
     animation: tilt-shaking 4s infinite;
 
     @keyframes tilt-shaking {
       0% { transform: rotate(0deg); }
@@ -49,14 +54,15 @@
       15% { transform: rotate(-10deg); }
       20% { transform: rotate(0deg); }
     }
   }
 
   p {
     margin-top: 0;
+    margin-right: 1em;
     text-align: left;
   }
 }
 
 /* remove the large top margin for the footer from invenio-theme's site.overrides */
 footer {
   margin-top: 0;
```

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/globals/site.variables`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-background.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-contact.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/images/hero-policies.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/modules/checkbox.overrides`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/theme/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/assets/semantic-ui/less/invenio_theme_tuw/tuwstone.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/favicon-16x16.png` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/favicon-32x32.png` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/faq.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/faq.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/magnifying-glass.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/online-chat.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/online-chat.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/features/upload-file.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/features/upload-file.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/fair-data-austria.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/fair-data-austria.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/openaire-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/rdmlogo.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/rdmlogo.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/footer-logos/re3data-logo.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/pdf.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/pdf.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/analytics.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/connection.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/connection.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/git.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/git.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/group.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/group.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/online-community.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/team.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/team.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/user.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/user.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/planned-features/version.webp` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/planned-features/version.webp`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/static/images/tuwstones/fwoerister.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/detail.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_app_rdm/records/search.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_previewer/pdfjs.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_previewer/pdfjs.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/contact.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/details.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/side_bar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/details/uploaders.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/guards/community.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/macros/detail.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/frontpage.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {# -*- coding: utf-8 -*-
 
   Copyright (C) 2019-2020 CERN.
   Copyright (C) 2019-2020 Northwestern University.
   Copyright (C) 2021 New York University.
-  Copyright (C) 2020-2022 TU Wien.
+  Copyright (C) 2020-2023 TU Wien.
 
   Invenio Theme TUW is free software; you can redistribute it and/or modify it
   under the terms of the MIT License; see LICENSE file for more details.
 #}
 
 {#- base: invenio-app-rdm v9.1.2. #}
 {#- changes: everything, including view function #}
@@ -21,14 +21,26 @@
 {%- block page_hero %}
   <section class="frontpage no-shrink" id="hero">
     {% include "invenio_theme_tuw/search_bar.html" %}
   </section>
 {%- endblock page_hero %}
 
 {%- block page_body %}
+  {%- block frontpage_info %}
+    {%- if config.THEME_TUW_FRONTPAGE_INFO %}
+      <div class="ui frontpage info message">
+        <i class="large info circle icon"></i>
+        <i class="close icon"></i>
+        <p class="bold">
+          {{ config.THEME_TUW_FRONTPAGE_INFO|safe }}
+        </p>
+      </div>
+    {%- endif %}
+  {%- endblock %}
+
   {%- block frontpage_warning %}
     {%- if config.THEME_TUW_FRONTPAGE_WARNING %}
       <div class="ui frontpage message">
         <i class="large exclamation triangle icon"></i>
         <p class="bold">
           {{ config.THEME_TUW_FRONTPAGE_WARNING|safe }}
         </p>
```

#### html2text {}

```diff
@@ -1,17 +1,21 @@
 {# -*- coding: utf-8 -*- Copyright (C) 2019-2020 CERN. Copyright (C) 2019-2020
 Northwestern University. Copyright (C) 2021 New York University. Copyright (C)
-2020-2022 TU Wien. Invenio Theme TUW is free software; you can redistribute it
+2020-2023 TU Wien. Invenio Theme TUW is free software; you can redistribute it
 and/or modify it under the terms of the MIT License; see LICENSE file for more
 details. #} {#- base: invenio-app-rdm v9.1.2. #} {#- changes: everything,
 including view function #} {%- extends config.BASE_TEMPLATE %} {%- block
 page_header %} {% include config.THEME_HEADER_TEMPLATE %} {%- endblock %} {%-
 block page_hero %}  {% include "invenio_theme_tuw/search_bar.html" %}  {%-
-endblock page_hero %} {%- block page_body %} {%- block frontpage_warning %} {%-
-if config.THEME_TUW_FRONTPAGE_WARNING %}
+endblock page_hero %} {%- block page_body %} {%- block frontpage_info %} {%- if
+config.THEME_TUW_FRONTPAGE_INFO %}
+
+{{ config.THEME_TUW_FRONTPAGE_INFO|safe }}
+{%- endif %} {%- endblock %} {%- block frontpage_warning %} {%- if
+config.THEME_TUW_FRONTPAGE_WARNING %}
 {{ config.THEME_TUW_FRONTPAGE_WARNING|safe }}
 {%- endif %} {%- endblock %}
 ****** Welcome to {{ config.THEME_SITENAME }} ******
 {{ config.THEME_SITENAME }} is an institutional repository of TU Wien to enable
 storing, sharing and publishing of digital objects, in particular research
 data. It facilitates the funders' requirements for open access to research data
 and the FAIR principles by making research output findable, accessible,
```

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/javascript.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/page_error.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/overrides/signup.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/policies.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/search_bar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/terms_of_use.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/theme/templates/semantic-ui/invenio_theme_tuw/tuwstones/florian_woerister.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/views.py` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw/webpack.py` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/PKG-INFO` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tuw
-Version: 2023.1.4.1
+Version: 2023.1.5
 Summary: "TU Wien theme for Invenio (RDM)."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-theme-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio theme tuw
 Platform: any
@@ -66,24 +66,26 @@
     Invenio Theme TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.1 (released 2023-01-13, updated 2023-03-06)
+Version 2023.1 (released 2023-01-13, updated 2023-04-24)
 
 - Display the record's first uploaders on the landing pages
 - Fix the draft preview page failing with a 404 code
 - Update links to policies
 - UI: fix header warning styling and improve permission guard pages
 - UI: rework deposit permission guard page text
 - UI: further improve deposit permission guard page text and modify its header icon
 - Footer: Improve layout and responsiveness on smaller screens
 - Fix naming of grid classes in css to avoid overlaps with `semantic-ui-less`
+- UI: remove reference to test instance from deposit guard page
+- Add possibility to a render an info box in the frontpage
 
 
 Version 2022.6 (released 2022-10-17, updated 2022-11-30)
 
 - v10 compat: Replace direct 'elasticsearch' import
 - v10 compat: Load and pass ``custom_fields`` in ``communities_new`` view function
 - Override ``app.config`` to specially handle our ``SITE_{API,UI}_URL`` config items
```

### Comparing `invenio-theme-tuw-2023.1.4.1/invenio_theme_tuw.egg-info/SOURCES.txt` & `invenio-theme-tuw-2023.1.5/invenio_theme_tuw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/run-tests.sh` & `invenio-theme-tuw-2023.1.5/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/setup.cfg` & `invenio-theme-tuw-2023.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tuw-2023.1.4.1/tests/conftest.py` & `invenio-theme-tuw-2023.1.5/tests/conftest.py`

 * *Files identical despite different names*

