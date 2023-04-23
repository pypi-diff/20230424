# Comparing `tmp/pyLDAvis-3.4.0.tar.gz` & `tmp/pyLDAvis-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLDAvis-3.4.0.tar", last modified: Wed Feb 15 17:41:21 2023, max compression
+gzip compressed data, was "pyLDAvis-3.4.1.tar", last modified: Sun Apr 23 23:42:15 2023, max compression
```

## Comparing `pyLDAvis-3.4.0.tar` & `pyLDAvis-3.4.1.tar`

### file list

```diff
@@ -1,859 +1,859 @@
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.660251 pyLDAvis-3.4.0/
--rw-r--r--   0 root         (0) primarygroup (89939)      255 2021-02-25 22:36:39.000000 pyLDAvis-3.4.0/AUTHORS.rst
--rw-r--r--   0 root         (0) primarygroup (89939)     3896 2023-02-15 16:25:08.000000 pyLDAvis-3.4.0/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) primarygroup (89939)     5271 2023-02-15 17:19:46.000000 pyLDAvis-3.4.0/HISTORY.rst
--rw-r--r--   0 root         (0) primarygroup (89939)     1464 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/LICENSE
--rw-r--r--   0 root         (0) primarygroup (89939)      506 2021-03-16 04:45:30.000000 pyLDAvis-3.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) primarygroup (89939)     3946 2023-02-15 17:41:21.659981 pyLDAvis-3.4.0/PKG-INFO
--rw-r--r--   0 root         (0) primarygroup (89939)     3043 2023-02-11 17:46:33.000000 pyLDAvis-3.4.0/README.rst
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.258652 pyLDAvis-3.4.0/docs/
--rw-r--r--   0 root         (0) primarygroup (89939)     6770 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/Makefile
--rw-r--r--   0 root         (0) primarygroup (89939)       28 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/authors.rst
--rwxr-xr-x   0 root         (0) primarygroup (89939)     8806 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/conf.py
--rw-r--r--   0 root         (0) primarygroup (89939)       33 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/contributing.rst
--rw-r--r--   0 root         (0) primarygroup (89939)       28 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/history.rst
--rw-r--r--   0 root         (0) primarygroup (89939)      518 2023-02-11 17:29:34.000000 pyLDAvis-3.4.0/docs/index.rst
--rw-r--r--   0 root         (0) primarygroup (89939)     6463 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/make.bat
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.258989 pyLDAvis-3.4.0/docs/modules/
--rw-r--r--   0 root         (0) primarygroup (89939)      258 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/modules/API.rst
--rw-r--r--   0 root         (0) primarygroup (89939)       27 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/docs/readme.rst
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.265346 pyLDAvis-3.4.0/notebooks/
--rw-r--r--   0 root         (0) primarygroup (89939)     8178 2023-02-11 15:32:03.000000 pyLDAvis-3.4.0/notebooks/Gensim Newsgroup.ipynb
--rw-r--r--   0 root         (0) primarygroup (89939)   320314 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/notebooks/GraphLab.ipynb
--rw-r--r--   0 root         (0) primarygroup (89939)  1179825 2023-02-15 06:50:08.000000 pyLDAvis-3.4.0/notebooks/LDA model.ipynb
--rw-r--r--   0 root         (0) primarygroup (89939)  1836599 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/notebooks/Movie Reviews, AP News, and Jeopardy.ipynb
--rw-r--r--   0 root         (0) primarygroup (89939)     2203 2023-02-15 06:08:37.000000 pyLDAvis-3.4.0/notebooks/Untitled.ipynb
--rw-r--r--   0 root         (0) primarygroup (89939)  1416825 2023-02-11 23:47:20.000000 pyLDAvis-3.4.0/notebooks/pyLDAvis_overview.ipynb
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.273797 pyLDAvis-3.4.0/pyLDAvis/
--rwxr-xr-x   0 root         (0) primarygroup (89939)     1194 2023-02-11 19:40:32.000000 pyLDAvis-3.4.0/pyLDAvis/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14318 2023-02-11 17:29:34.000000 pyLDAvis-3.4.0/pyLDAvis/_display.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19288 2023-02-15 17:21:56.000000 pyLDAvis-3.4.0/pyLDAvis/_prepare.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3894 2021-03-16 18:20:19.000000 pyLDAvis-3.4.0/pyLDAvis/_server.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4824 2022-04-21 03:22:38.000000 pyLDAvis-3.4.0/pyLDAvis/gensim_models.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2406 2021-03-14 18:11:29.000000 pyLDAvis-3.4.0/pyLDAvis/graphlab.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.281218 pyLDAvis-3.4.0/pyLDAvis/js/
--rw-r--r--   0 root         (0) primarygroup (89939)   248314 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/pyLDAvis/js/d3.v5.min.js
--rw-r--r--   0 root         (0) primarygroup (89939)      684 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/pyLDAvis/js/ldavis.css
--rw-r--r--   0 root         (0) primarygroup (89939)    53291 2021-02-22 16:29:34.000000 pyLDAvis-3.4.0/pyLDAvis/js/ldavis.js
--rw-r--r--   0 root         (0) primarygroup (89939)      684 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/pyLDAvis/js/ldavis.v1.0.0.css
--rw-r--r--   0 root         (0) primarygroup (89939)    56137 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/pyLDAvis/js/ldavis.v1.0.0.js
--rw-r--r--   0 root         (0) primarygroup (89939)    53336 2021-03-23 20:07:41.000000 pyLDAvis-3.4.0/pyLDAvis/js/ldavis.v3.0.0.js
--rw-r--r--   0 root         (0) primarygroup (89939)     2957 2023-02-15 05:59:53.000000 pyLDAvis-3.4.0/pyLDAvis/lda_model.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.237220 pyLDAvis-3.4.0/pyLDAvis/lib/
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.237332 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.249440 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.282279 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/
--rw-r--r--   0 root         (0) primarygroup (89939)     6128 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)       44 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/override.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.284361 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/
--rw-r--r--   0 root         (0) primarygroup (89939)      357 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/__main__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1444 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/__pip-runner__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.288771 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/
--rw-r--r--   0 root         (0) primarygroup (89939)      573 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10234 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10734 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cache.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.294455 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/
--rw-r--r--   0 root         (0) primarygroup (89939)      132 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6676 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7842 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0 root         (0) primarygroup (89939)    29381 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)      774 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2472 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4338 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10817 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1968 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18172 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5118 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0 root         (0) primarygroup (89939)      116 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.301509 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/
--rw-r--r--   0 root         (0) primarygroup (89939)     3882 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7582 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1685 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9815 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6573 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5289 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2951 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1703 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1132 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4762 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3374 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0 root         (0) primarygroup (89939)    31726 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12343 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3680 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13529 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/configuration.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.303372 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/
--rw-r--r--   0 root         (0) primarygroup (89939)      858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1221 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0 root         (0) primarygroup (89939)      729 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6494 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1164 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    20942 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/exceptions.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.304938 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/
--rw-r--r--   0 root         (0) primarygroup (89939)       30 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    16503 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0 root         (0) primarygroup (89939)    37596 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6557 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/sources.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.306419 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/
--rw-r--r--   0 root         (0) primarygroup (89939)    17552 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6302 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7867 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2573 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0 root         (0) primarygroup (89939)      340 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/main.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.308024 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/
--rw-r--r--   0 root         (0) primarygroup (89939)     4280 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2595 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0 root         (0) primarygroup (89939)    25277 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/base.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.309749 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
--rw-r--r--   0 root         (0) primarygroup (89939)      107 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1882 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8181 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7457 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9773 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.315397 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/
--rw-r--r--   0 root         (0) primarygroup (89939)       63 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      990 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5877 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2520 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1030 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2617 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18083 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-r--r--   0 root         (0) primarygroup (89939)      738 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4644 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1907 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3600 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/wheel.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.321120 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/
--rw-r--r--   0 root         (0) primarygroup (89939)       50 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12190 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2145 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6096 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7638 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18443 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4073 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1791 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.323710 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.329388 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4133 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1404 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1456 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1063 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1405 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3064 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5109 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9784 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.332372 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/
--rw-r--r--   0 root         (0) primarygroup (89939)       51 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1354 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4105 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0 root         (0) primarygroup (89939)    27407 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    25091 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7074 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/pyproject.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.337475 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/
--rw-r--r--   0 root         (0) primarygroup (89939)     2807 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    16611 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17646 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0 root         (0) primarygroup (89939)    35600 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0 root         (0) primarygroup (89939)    24045 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.338541 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      583 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/base.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.339402 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    24129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.343274 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5220 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18963 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0 root         (0) primarygroup (89939)    27878 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5705 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9914 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2526 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5455 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11533 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8020 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.353376 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1015 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1884 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5377 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0 root         (0) primarygroup (89939)      242 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5764 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3206 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1115 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2203 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1169 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3064 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5122 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0 root         (0) primarygroup (89939)      716 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4831 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0 root         (0) primarygroup (89939)      795 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11632 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0 root         (0) primarygroup (89939)    21617 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1193 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2108 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5662 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9197 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7702 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8821 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1759 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3459 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4549 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.355482 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/
--rw-r--r--   0 root         (0) primarygroup (89939)      596 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3518 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18116 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5238 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11728 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0 root         (0) primarygroup (89939)    22811 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13079 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.356624 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/
--rw-r--r--   0 root         (0) primarygroup (89939)     4966 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.360281 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
--rw-r--r--   0 root         (0) primarygroup (89939)      465 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1379 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5033 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1535 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.361393 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
--rw-r--r--   0 root         (0) primarygroup (89939)      242 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5271 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1033 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0 root         (0) primarygroup (89939)      778 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)    16416 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3946 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4154 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7105 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0 root         (0) primarygroup (89939)      774 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.363068 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/
--rw-r--r--   0 root         (0) primarygroup (89939)       94 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      255 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4279 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.394944 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/
--rw-r--r--   0 root         (0) primarygroup (89939)     3705 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    31274 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1741 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9608 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3817 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4801 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.395827 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2406 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3559 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1838 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1619 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3864 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12021 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3676 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13566 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1731 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    36913 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1731 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    20735 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1737 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13919 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    25796 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0 root         (0) primarygroup (89939)    42498 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1730 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    26797 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0 root         (0) primarygroup (89939)   104562 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    98484 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    98196 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0 root         (0) primarygroup (89939)   101363 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0 root         (0) primarygroup (89939)   128035 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0 root         (0) primarygroup (89939)   102774 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    95372 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5260 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3367 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2056 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30068 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.396607 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13280 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6199 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3749 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13288 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8289 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2709 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0 root         (0) primarygroup (89939)      242 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.399063 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/
--rw-r--r--   0 root         (0) primarygroup (89939)      239 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2522 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10830 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1915 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5404 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6438 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.404864 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/
--rw-r--r--   0 root         (0) primarygroup (89939)      581 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    41259 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)    51697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0 root         (0) primarygroup (89939)    20834 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0 root         (0) primarygroup (89939)    51991 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14811 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5058 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0 root         (0) primarygroup (89939)    39801 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10820 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18102 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0 root         (0) primarygroup (89939)    66262 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0 root         (0) primarygroup (89939)    23513 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0 root         (0) primarygroup (89939)    43898 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.406426 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/
--rw-r--r--   0 root         (0) primarygroup (89939)      981 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)       64 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    48841 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.410555 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/
--rw-r--r--   0 root         (0) primarygroup (89939)      849 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3374 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0 root         (0) primarygroup (89939)      321 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12950 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0 root         (0) primarygroup (89939)    44375 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1881 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0 root         (0) primarygroup (89939)       21 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0 root         (0) primarygroup (89939)   206539 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.412385 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/
--rw-r--r--   0 root         (0) primarygroup (89939)     1132 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1081 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6080 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0 root         (0) primarygroup (89939)    34557 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.418332 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/
--rw-r--r--   0 root         (0) primarygroup (89939)      661 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      497 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11488 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4378 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1431 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8487 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4676 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0 root         (0) primarygroup (89939)    15699 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4200 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.424502 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/
--rw-r--r--   0 root         (0) primarygroup (89939)      130 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      138 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/_compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3443 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6083 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3994 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0 root         (0) primarygroup (89939)      607 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6081 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/envbuild.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.426191 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/
--rw-r--r--   0 root         (0) primarygroup (89939)      872 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10801 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2520 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12721 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/wrappers.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.427902 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
--rw-r--r--   0 root         (0) primarygroup (89939)   108287 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      562 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.435570 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/
--rw-r--r--   0 root         (0) primarygroup (89939)    12831 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1176 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4068 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4910 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2655 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6910 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0 root         (0) primarygroup (89939)       78 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6439 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.446509 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/
--rw-r--r--   0 root         (0) primarygroup (89939)     2999 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      353 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    23685 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1938 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.447126 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
--rw-r--r--   0 root         (0) primarygroup (89939)    40386 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2917 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.457225 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
--rw-r--r--   0 root         (0) primarygroup (89939)     4810 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4104 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3314 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5086 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0 root         (0) primarygroup (89939)    35441 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0 root         (0) primarygroup (89939)    21938 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5871 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19351 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5073 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2212 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5014 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7335 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4674 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11753 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0 root         (0) primarygroup (89939)    32005 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.459300 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
--rw-r--r--   0 root         (0) primarygroup (89939)    11174 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    70232 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0 root         (0) primarygroup (89939)    53376 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0 root         (0) primarygroup (89939)      986 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2591 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3072 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3092 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4630 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6257 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.460007 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
--rw-r--r--   0 root         (0) primarygroup (89939)     3419 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6184 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0 root         (0) primarygroup (89939)    63187 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.467435 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/
--rw-r--r--   0 root         (0) primarygroup (89939)     9171 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6426 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12936 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0 root         (0) primarygroup (89939)   213344 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.468095 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
--rw-r--r--   0 root         (0) primarygroup (89939)    23685 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9023 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)    39129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0 root         (0) primarygroup (89939)    25341 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13402 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10787 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6805 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.480025 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/
--rw-r--r--   0 root         (0) primarygroup (89939)     5178 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      440 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1397 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0 root         (0) primarygroup (89939)    21443 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6377 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10187 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0 root         (0) primarygroup (89939)      575 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1286 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18560 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3823 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3879 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0 root         (0) primarygroup (89939)      733 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0 root         (0) primarygroup (89939)    35287 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0 root         (0) primarygroup (89939)      695 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30180 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4235 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2912 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0 root         (0) primarygroup (89939)    33240 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.483163 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/
--rw-r--r--   0 root         (0) primarygroup (89939)      537 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.483847 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      156 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5872 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1583 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17592 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4794 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.518428 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/
--rw-r--r--   0 root         (0) primarygroup (89939)     5944 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8808 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10096 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0 root         (0) primarygroup (89939)   140235 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1064 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2114 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0 root         (0) primarygroup (89939)      265 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9695 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3225 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1236 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7063 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0 root         (0) primarygroup (89939)      423 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5472 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19919 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0 root         (0) primarygroup (89939)      351 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0 root         (0) primarygroup (89939)      417 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0 root         (0) primarygroup (89939)    22820 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1926 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2783 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1840 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0 root         (0) primarygroup (89939)      890 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10368 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6820 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3264 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9864 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4503 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17957 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1054 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7131 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0 root         (0) primarygroup (89939)    95885 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1288 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5497 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6630 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7954 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0 root         (0) primarygroup (89939)      972 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2501 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0 root         (0) primarygroup (89939)      642 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1616 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2507 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9585 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5051 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3252 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14074 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14172 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3667 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11471 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5305 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4970 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0 root         (0) primarygroup (89939)      828 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8744 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    36576 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0 root         (0) primarygroup (89939)    59746 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8161 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11303 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1391 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0 root         (0) primarygroup (89939)      166 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4449 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4773 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2842 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1591 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0 root         (0) primarygroup (89939)    24224 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4374 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4425 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0 root         (0) primarygroup (89939)    26240 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1258 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0 root         (0) primarygroup (89939)    34697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0 root         (0) primarygroup (89939)    39515 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3370 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0 root         (0) primarygroup (89939)    44666 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3627 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0 root         (0) primarygroup (89939)      102 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0 root         (0) primarygroup (89939)    26060 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9169 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0 root         (0) primarygroup (89939)    34549 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/six.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.527132 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/
--rw-r--r--   0 root         (0) primarygroup (89939)    18364 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3314 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1944 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1496 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1376 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1908 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1383 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7550 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2790 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2145 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8011 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.529952 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/
--rw-r--r--   0 root         (0) primarygroup (89939)      396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    22633 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2943 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0 root         (0) primarygroup (89939)      254 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0 root         (0) primarygroup (89939)    80114 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.534971 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/
--rw-r--r--   0 root         (0) primarygroup (89939)     3333 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10811 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0 root         (0) primarygroup (89939)       64 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0 root         (0) primarygroup (89939)    20070 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0 root         (0) primarygroup (89939)    39093 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.537620 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      957 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.538683 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17632 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13922 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11034 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4538 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17182 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 root         (0) primarygroup (89939)    34448 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7097 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8217 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8579 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2440 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.539333 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.540043 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1417 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0 root         (0) primarygroup (89939)    34665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19786 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5985 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30109 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.545711 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
--rw-r--r--   0 root         (0) primarygroup (89939)     1155 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4901 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1605 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0 root         (0) primarygroup (89939)      498 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3997 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3510 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0 root         (0) primarygroup (89939)    22001 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17177 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5758 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6895 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10003 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14287 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5403 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.547623 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/
--rw-r--r--   0 root         (0) primarygroup (89939)    10579 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8979 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1305 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6563 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4307 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.547973 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/
--rw-r--r--   0 root         (0) primarygroup (89939)   108568 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.549157 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    24701 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.552873 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-r--r--   0 root         (0) primarygroup (89939)      506 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4504 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2741 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2706 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)      884 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3494 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3886 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3566 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2836 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.553847 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5420 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13515 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.554185 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-r--r--   0 root         (0) primarygroup (89939)    15526 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.555388 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
--rw-r--r--   0 root         (0) primarygroup (89939)       83 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)   132569 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18410 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.559324 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
--rw-r--r--   0 root         (0) primarygroup (89939)      661 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      497 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11488 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4378 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1431 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8496 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4706 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30110 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0 root         (0) primarygroup (89939)    15699 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4200 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14665 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.563269 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/
--rw-r--r--   0 root         (0) primarygroup (89939)     9159 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6426 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12936 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0 root         (0) primarygroup (89939)   213310 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.563625 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-r--r--   0 root         (0) primarygroup (89939)    23668 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9023 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)    39129 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0 root         (0) primarygroup (89939)    25341 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13402 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10787 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6805 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8425 2023-02-15 07:12:34.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.564035 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/extern/
--rw-r--r--   0 root         (0) primarygroup (89939)     2426 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.582645 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/
--rw-r--r--   0 root         (0) primarygroup (89939)     8429 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      218 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.597047 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/
--rw-r--r--   0 root         (0) primarygroup (89939)      537 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1330 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0 root         (0) primarygroup (89939)      411 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0 root         (0) primarygroup (89939)      239 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19672 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8603 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14789 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0 root         (0) primarygroup (89939)    47369 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17973 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.605677 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/
--rw-r--r--   0 root         (0) primarygroup (89939)      430 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1614 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5441 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4701 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0 root         (0) primarygroup (89939)    22051 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5617 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7728 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0 root         (0) primarygroup (89939)    31558 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0 root         (0) primarygroup (89939)    16568 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5624 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4888 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2603 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13137 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30221 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2779 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2785 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1189 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8434 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1936 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0 root         (0) primarygroup (89939)      672 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11765 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19241 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7477 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4920 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9451 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12537 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0 root         (0) primarygroup (89939)      139 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3423 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8082 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0 root         (0) primarygroup (89939)    50186 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3589 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10270 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0 root         (0) primarygroup (89939)    17910 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8226 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13713 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1972 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30235 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0 root         (0) primarygroup (89939)    23602 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0 root         (0) primarygroup (89939)      217 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)      639 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3517 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12096 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0 root         (0) primarygroup (89939)    15641 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0 root         (0) primarygroup (89939)    18128 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12952 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5248 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1972 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2392 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_imp.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1311 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-r--r--   0 root         (0) primarygroup (89939)      675 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-r--r--   0 root         (0) primarygroup (89939)      749 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_path.py
--rw-r--r--   0 root         (0) primarygroup (89939)      501 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_reqs.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.607570 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.610776 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
--rw-r--r--   0 root         (0) primarygroup (89939)    30130 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1862 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 root         (0) primarygroup (89939)      743 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1828 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2895 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2068 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1154 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2166 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.613905 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
--rw-r--r--   0 root         (0) primarygroup (89939)      506 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4504 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2741 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2706 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)      884 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3494 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3886 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3566 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2836 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.614880 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
--rw-r--r--   0 root         (0) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5420 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13512 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.615353 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
--rw-r--r--   0 root         (0) primarygroup (89939)    15517 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.617375 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
--rw-r--r--   0 root         (0) primarygroup (89939)       82 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)   117959 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0 root         (0) primarygroup (89939)    16256 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0 root         (0) primarygroup (89939)    15130 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.624523 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/
--rw-r--r--   0 root         (0) primarygroup (89939)      661 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0 root         (0) primarygroup (89939)      497 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11488 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4378 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1431 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8493 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4700 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0 root         (0) primarygroup (89939)    30110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0 root         (0) primarygroup (89939)    15699 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4200 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.632959 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/
--rw-r--r--   0 root         (0) primarygroup (89939)     9159 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6426 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0 root         (0) primarygroup (89939)    12936 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0 root         (0) primarygroup (89939)   213310 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.633433 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-r--r--   0 root         (0) primarygroup (89939)    23668 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     9023 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)    39129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0 root         (0) primarygroup (89939)    25341 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13402 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0 root         (0) primarygroup (89939)    10787 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6805 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.634991 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/
--rw-r--r--   0 root         (0) primarygroup (89939)      396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    22633 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2943 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0 root         (0) primarygroup (89939)      254 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0 root         (0) primarygroup (89939)    87149 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8425 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7346 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19539 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/build_meta.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.644559 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/
--rw-r--r--   0 root         (0) primarygroup (89939)      396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2381 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-r--r--   0 root         (0) primarygroup (89939)    16623 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1182 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0 root         (0) primarygroup (89939)     6595 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4415 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0 root         (0) primarygroup (89939)    15821 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14115 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7012 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4800 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0 root         (0) primarygroup (89939)    85662 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0 root         (0) primarygroup (89939)    31188 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0 root         (0) primarygroup (89939)    26795 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5163 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2226 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3875 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2612 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4946 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)      468 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/register.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2128 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-r--r--   0 root         (0) primarygroup (89939)      658 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7071 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5086 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8102 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/test.py
--rw-r--r--   0 root         (0) primarygroup (89939)      462 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-r--r--   0 root         (0) primarygroup (89939)     7494 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/upload_docs.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.646361 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/
--rw-r--r--   0 root         (0) primarygroup (89939)     1121 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    13398 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.648845 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
--rw-r--r--   0 root         (0) primarygroup (89939)     1038 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)    11266 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1153 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1612 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0 root         (0) primarygroup (89939)   269900 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8736 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0 root         (0) primarygroup (89939)    16319 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-r--r--   0 root         (0) primarygroup (89939)    19304 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0 root         (0) primarygroup (89939)    25198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0 root         (0) primarygroup (89939)      949 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5499 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/depends.py
--rw-r--r--   0 root         (0) primarygroup (89939)    20799 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/discovery.py
--rw-r--r--   0 root         (0) primarygroup (89939)    45578 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/dist.py
--rw-r--r--   0 root         (0) primarygroup (89939)     2464 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/errors.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5591 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/extension.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.649221 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/extern/
--rw-r--r--   0 root         (0) primarygroup (89939)     2512 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4873 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/glob.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3824 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/installer.py
--rw-r--r--   0 root         (0) primarygroup (89939)      812 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/launch.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1210 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/logging.py
--rw-r--r--   0 root         (0) primarygroup (89939)     4857 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/monkey.py
--rw-r--r--   0 root         (0) primarygroup (89939)    47724 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/msvc.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3093 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-r--r--   0 root         (0) primarygroup (89939)    40020 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/package_index.py
--rw-r--r--   0 root         (0) primarygroup (89939)      245 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/py34compat.py
--rw-r--r--   0 root         (0) primarygroup (89939)    14348 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-r--r--   0 root         (0) primarygroup (89939)      941 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0 root         (0) primarygroup (89939)      144 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/version.py
--rw-r--r--   0 root         (0) primarygroup (89939)     8376 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/wheel.py
--rw-r--r--   0 root         (0) primarygroup (89939)      718 2023-02-15 07:12:35.000000 pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/windows_support.py
--rw-r--r--   0 root         (0) primarygroup (89939)     1188 2021-02-22 16:29:34.000000 pyLDAvis-3.4.0/pyLDAvis/urls.py
--rw-r--r--   0 root         (0) primarygroup (89939)     5074 2021-03-16 04:54:55.000000 pyLDAvis-3.4.0/pyLDAvis/utils.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.277852 pyLDAvis-3.4.0/pyLDAvis.egg-info/
--rw-r--r--   0 root         (0) primarygroup (89939)     3946 2023-02-15 17:41:20.000000 pyLDAvis-3.4.0/pyLDAvis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) primarygroup (89939)    53182 2023-02-15 17:41:21.000000 pyLDAvis-3.4.0/pyLDAvis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) primarygroup (89939)        1 2023-02-15 17:41:20.000000 pyLDAvis-3.4.0/pyLDAvis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) primarygroup (89939)        1 2021-02-28 17:40:06.000000 pyLDAvis-3.4.0/pyLDAvis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) primarygroup (89939)      107 2023-02-15 17:41:20.000000 pyLDAvis-3.4.0/pyLDAvis.egg-info/requires.txt
--rw-r--r--   0 root         (0) primarygroup (89939)        9 2023-02-15 17:41:20.000000 pyLDAvis-3.4.0/pyLDAvis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) primarygroup (89939)       81 2021-03-22 15:46:38.000000 pyLDAvis-3.4.0/pyproject.toml
--rw-r--r--   0 root         (0) primarygroup (89939)      107 2023-02-15 05:36:53.000000 pyLDAvis-3.4.0/requirements.txt
--rw-r--r--   0 root         (0) primarygroup (89939)       38 2023-02-15 17:41:21.660345 pyLDAvis-3.4.0/setup.cfg
--rwxr-xr-x   0 root         (0) primarygroup (89939)     1639 2023-02-15 06:52:59.000000 pyLDAvis-3.4.0/setup.py
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.252885 pyLDAvis-3.4.0/tests/
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.658630 pyLDAvis-3.4.0/tests/data/
--rwxr-xr-x   0 root         (0) primarygroup (89939)     1261 2021-02-17 22:18:20.000000 pyLDAvis-3.4.0/tests/data/export_data.R
--rw-r--r--   0 root         (0) primarygroup (89939)  7087084 2021-02-17 22:18:27.000000 pyLDAvis-3.4.0/tests/data/movie_reviews_input.json
--rw-r--r--   0 root         (0) primarygroup (89939)   159501 2021-02-17 22:18:21.000000 pyLDAvis-3.4.0/tests/data/movie_reviews_output.json
-drwxr-xr-x   0 root         (0) primarygroup (89939)        0 2023-02-15 17:41:21.659534 pyLDAvis-3.4.0/tests/pyLDAvis/
--rwxr-xr-x   0 root         (0) primarygroup (89939)     2528 2021-03-16 18:19:40.000000 pyLDAvis-3.4.0/tests/pyLDAvis/test_gensim_models.py
--rw-r--r--   0 root         (0) primarygroup (89939)     3277 2023-02-11 22:23:43.000000 pyLDAvis-3.4.0/tests/pyLDAvis/test_prepare.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.734932 pyLDAvis-3.4.1/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      255 2021-02-25 22:36:39.000000 pyLDAvis-3.4.1/AUTHORS.rst
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3891 2023-04-23 22:49:14.000000 pyLDAvis-3.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5380 2023-04-23 22:20:57.000000 pyLDAvis-3.4.1/HISTORY.rst
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1464 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/LICENSE
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      506 2021-03-16 04:45:30.000000 pyLDAvis-3.4.1/MANIFEST.in
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3933 2023-04-23 23:42:15.734775 pyLDAvis-3.4.1/PKG-INFO
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3043 2023-02-11 17:46:33.000000 pyLDAvis-3.4.1/README.rst
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.389380 pyLDAvis-3.4.1/docs/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6770 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/Makefile
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       28 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/authors.rst
+-rwxr-xr-x   0 msusol   (217018) primarygroup (89939)     8806 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/conf.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       33 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/contributing.rst
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       28 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/history.rst
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      518 2023-02-11 17:29:34.000000 pyLDAvis-3.4.1/docs/index.rst
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6463 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/make.bat
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.389578 pyLDAvis-3.4.1/docs/modules/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      258 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/modules/API.rst
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       27 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/docs/readme.rst
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.397070 pyLDAvis-3.4.1/notebooks/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    23693 2023-04-23 22:18:08.000000 pyLDAvis-3.4.1/notebooks/Gensim Newsgroup.ipynb
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   320314 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/notebooks/GraphLab.ipynb
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)  1179825 2023-02-15 06:50:08.000000 pyLDAvis-3.4.1/notebooks/LDA model.ipynb
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)  1836599 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/notebooks/Movie Reviews, AP News, and Jeopardy.ipynb
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2203 2023-02-15 06:08:37.000000 pyLDAvis-3.4.1/notebooks/Untitled.ipynb
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)  1416825 2023-02-11 23:47:20.000000 pyLDAvis-3.4.1/notebooks/pyLDAvis_overview.ipynb
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.401903 pyLDAvis-3.4.1/pyLDAvis/
+-rwxr-xr-x   0 msusol   (217018) primarygroup (89939)     1194 2023-02-11 19:40:32.000000 pyLDAvis-3.4.1/pyLDAvis/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14318 2023-04-21 03:21:01.000000 pyLDAvis-3.4.1/pyLDAvis/_display.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19293 2023-04-23 22:03:49.000000 pyLDAvis-3.4.1/pyLDAvis/_prepare.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3894 2021-03-16 18:20:19.000000 pyLDAvis-3.4.1/pyLDAvis/_server.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4824 2022-04-21 03:22:38.000000 pyLDAvis-3.4.1/pyLDAvis/gensim_models.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2406 2021-03-14 18:11:29.000000 pyLDAvis-3.4.1/pyLDAvis/graphlab.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.404750 pyLDAvis-3.4.1/pyLDAvis/js/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   248314 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/pyLDAvis/js/d3.v5.min.js
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      684 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/pyLDAvis/js/ldavis.css
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    53291 2021-02-22 16:29:34.000000 pyLDAvis-3.4.1/pyLDAvis/js/ldavis.js
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      684 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/pyLDAvis/js/ldavis.v1.0.0.css
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    56137 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/pyLDAvis/js/ldavis.v1.0.0.js
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    53336 2021-03-23 20:07:41.000000 pyLDAvis-3.4.1/pyLDAvis/js/ldavis.v3.0.0.js
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2957 2023-02-15 05:59:53.000000 pyLDAvis-3.4.1/pyLDAvis/lda_model.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.332397 pyLDAvis-3.4.1/pyLDAvis/lib/
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.332472 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.342952 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.406605 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6128 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       44 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/override.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.407534 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      357 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/__main__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1444 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/__pip-runner__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.409710 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      573 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10234 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10734 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cache.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.415859 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      132 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6676 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7842 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    29381 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      774 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2472 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4338 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10817 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1968 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18172 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5118 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      116 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.424831 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3882 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7582 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1685 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9815 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6573 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5289 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2951 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1703 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1132 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4762 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3374 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    31726 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12343 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3680 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13529 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/configuration.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.427765 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1221 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      729 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6494 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1164 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    20942 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/exceptions.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.428743 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       30 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    16503 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    37596 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6557 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/sources.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.429795 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17552 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6302 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7867 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2573 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      340 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/main.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.432393 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4280 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2595 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    25277 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.433465 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      107 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1882 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8181 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7457 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9773 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.436438 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       63 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      990 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5877 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2520 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1030 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2617 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18083 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      738 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4644 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1907 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3600 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.438046 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       50 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12190 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2145 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6096 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7638 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18443 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4073 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1791 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.438956 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.440843 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4133 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1404 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1456 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1063 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1405 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3064 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5109 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9784 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.441816 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       51 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1354 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4105 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    27407 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    25091 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7074 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/pyproject.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.455759 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2807 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    16611 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17646 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    35600 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    24045 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.456206 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      583 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.456562 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    24129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.458500 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5220 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18963 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    27878 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5705 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9914 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2526 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5455 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11533 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8020 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.464005 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1015 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1884 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5377 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      242 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5764 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3206 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1115 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2203 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1169 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3064 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5122 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      716 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4831 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      795 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11632 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    21617 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1193 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2108 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5662 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9197 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7702 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8821 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1759 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3459 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4549 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.465403 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      596 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3518 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18116 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5238 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11728 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    22811 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13079 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.466984 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4966 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.469742 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      465 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1379 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5033 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1535 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.471381 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      242 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5271 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1033 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      778 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    16416 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3946 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4154 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7105 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      774 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.472597 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       94 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      255 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4279 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.487416 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3705 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    31274 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1741 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9608 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3817 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4801 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.488107 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2406 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3559 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1838 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1619 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3864 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12021 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3676 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13566 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1731 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    36913 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1731 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    20735 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1737 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13919 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    25796 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    42498 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1730 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    26797 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   104562 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    98484 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    98196 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   101363 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   128035 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   102774 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    95372 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5260 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3367 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2056 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30068 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.488605 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13280 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6199 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3749 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13288 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8289 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2709 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      242 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.491713 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      239 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2522 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10830 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1915 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5404 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6438 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.498969 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      581 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    41259 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    51697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    20834 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    51991 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14811 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5058 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    39801 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10820 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18102 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    66262 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    23513 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    43898 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.499883 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      981 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       64 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    48841 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.502344 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      849 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3374 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      321 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12950 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    44375 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1881 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       21 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   206539 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.506892 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1132 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1081 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6080 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    34557 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.511498 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      661 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      497 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11488 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4378 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1431 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8487 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4676 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15699 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4200 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.514604 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      130 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      138 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/_compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3443 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/build.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6083 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/check.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3994 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      607 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6081 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/envbuild.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.516044 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      872 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10801 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2520 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/meta.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12721 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/wrappers.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.517414 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   108287 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      562 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.519135 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12831 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1176 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4068 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4910 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2655 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6910 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       78 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6439 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.524567 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2999 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      353 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    23685 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1938 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.524755 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    40386 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2917 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.535560 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4810 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4104 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3314 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5086 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    35441 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    21938 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5871 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19351 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5073 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2212 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5014 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7335 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4674 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11753 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    32005 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.547002 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11174 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    70232 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    53376 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      986 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2591 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3072 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3092 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4630 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6257 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.547319 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3419 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6184 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    63187 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.551622 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9171 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6426 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12936 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   213344 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.551974 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    23685 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9023 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    39129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    25341 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13402 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10787 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6805 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.557755 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5178 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      440 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1397 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    21443 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6377 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10187 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      575 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1286 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18560 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3823 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3879 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      733 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    35287 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      695 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30180 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4235 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2912 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    33240 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.560515 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      537 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.560851 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      156 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5872 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1583 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17592 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4794 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.604293 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5944 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8808 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10096 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   140235 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1064 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2114 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      265 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9695 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3225 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1236 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7063 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      423 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5472 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19919 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      351 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      417 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    22820 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1926 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2783 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1840 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      890 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10368 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6820 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3264 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9864 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4503 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17957 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1054 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7131 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    95885 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1288 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5497 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6630 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7954 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      972 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2501 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      642 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1616 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2507 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9585 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5051 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3252 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14074 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14172 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3667 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11471 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5305 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4970 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      828 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8744 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    36576 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    59746 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8161 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11303 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1391 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      166 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4449 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4773 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2842 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1591 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    24224 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4374 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4425 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    26240 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1258 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    34697 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    39515 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3370 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    44666 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3627 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      102 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    26060 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9169 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    34549 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/six.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.606683 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18364 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3314 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1944 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1496 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1376 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1908 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1383 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7550 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2790 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2145 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8011 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.607713 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    22633 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2943 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      254 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    80114 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.611263 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3333 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10811 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       64 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    20070 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    39093 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.613288 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      957 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.614085 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17632 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13922 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11034 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4538 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17182 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    34448 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7097 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8217 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8579 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2440 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.614419 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.616523 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1417 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    34665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19786 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5985 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30109 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.620158 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1155 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4901 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1605 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      498 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3997 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3510 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    22001 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17177 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5758 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6895 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10003 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14287 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5403 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.621306 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10579 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8979 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1305 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6563 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4307 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.621483 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   108568 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.622698 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    24701 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.626118 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      506 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4504 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2741 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2706 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      884 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3494 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3886 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3566 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2836 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.626807 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5420 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13515 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.627095 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15526 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.629996 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       83 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   132569 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18410 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.634395 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      661 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      497 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11488 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4378 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1431 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8496 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4706 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30110 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15699 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4200 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14665 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.642521 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9159 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6426 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12936 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   213310 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.642853 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    23668 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9023 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    39129 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    25341 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13402 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10787 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6805 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8425 2023-02-15 07:12:34.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.643309 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/extern/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2426 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.661910 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8429 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      218 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.674050 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      537 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1330 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      411 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      239 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19672 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8603 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14789 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    47369 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17973 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.685885 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      430 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1614 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5441 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4701 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    22051 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5617 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7728 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    31558 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    16568 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5624 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4888 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2603 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13137 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30221 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2779 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2785 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1189 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8434 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1936 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      672 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11765 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19241 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7477 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4920 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9451 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12537 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      139 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3423 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8082 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    50186 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3589 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10270 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    17910 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8226 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13713 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1972 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30235 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    23602 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      217 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      639 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3517 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18858 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12096 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15641 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    18128 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12952 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5248 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1972 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2392 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1311 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      675 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      749 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_path.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      501 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_reqs.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.687970 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.689877 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30130 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1862 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      743 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1828 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2895 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2068 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1154 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2166 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.694764 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      506 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4504 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2741 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2706 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      884 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3494 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3886 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3566 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2836 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.695391 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        0 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5420 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13512 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.695583 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15517 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.696411 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       82 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   117959 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    16256 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15130 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.700759 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      661 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      497 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11488 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4378 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1431 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8493 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4700 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    30110 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15699 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4200 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14665 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.707265 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9159 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6426 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    12936 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   213310 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.707539 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    23668 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     9023 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    39129 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    25341 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13402 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    10787 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6805 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.708986 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    22633 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2943 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      254 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    87149 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8425 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7346 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19539 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/build_meta.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.717708 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      396 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2381 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    16623 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1182 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     6595 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4415 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    15821 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14115 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7012 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4800 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    85662 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    31188 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    26795 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5163 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2226 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3875 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2612 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4946 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      468 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2128 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      658 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7071 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5086 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8102 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      462 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     7494 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.719201 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1121 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    13398 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.722513 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1038 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    11266 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1153 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1612 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   269900 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8736 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    16319 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    19304 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    25198 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      949 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5499 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/depends.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    20799 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    45578 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/dist.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2464 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/errors.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5591 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/extension.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.724025 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/extern/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     2512 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4873 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/glob.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3824 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/installer.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      812 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/launch.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1210 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/logging.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     4857 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    47724 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3093 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    40020 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      245 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/py34compat.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    14348 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      941 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      144 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/version.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     8376 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      718 2023-02-15 07:12:35.000000 pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/windows_support.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     1188 2021-02-22 16:29:34.000000 pyLDAvis-3.4.1/pyLDAvis/urls.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     5074 2021-03-16 04:54:55.000000 pyLDAvis-3.4.1/pyLDAvis/utils.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.402962 pyLDAvis-3.4.1/pyLDAvis.egg-info/
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3933 2023-04-23 23:42:14.000000 pyLDAvis-3.4.1/pyLDAvis.egg-info/PKG-INFO
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)    53182 2023-04-23 23:42:15.000000 pyLDAvis-3.4.1/pyLDAvis.egg-info/SOURCES.txt
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        1 2023-04-23 23:42:14.000000 pyLDAvis-3.4.1/pyLDAvis.egg-info/dependency_links.txt
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        1 2021-02-28 17:40:06.000000 pyLDAvis-3.4.1/pyLDAvis.egg-info/not-zip-safe
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      107 2023-04-23 23:42:14.000000 pyLDAvis-3.4.1/pyLDAvis.egg-info/requires.txt
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)        9 2023-04-23 23:42:14.000000 pyLDAvis-3.4.1/pyLDAvis.egg-info/top_level.txt
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       81 2021-03-22 15:46:38.000000 pyLDAvis-3.4.1/pyproject.toml
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)      107 2023-04-23 23:06:43.000000 pyLDAvis-3.4.1/requirements.txt
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)       38 2023-04-23 23:42:15.734977 pyLDAvis-3.4.1/setup.cfg
+-rwxr-xr-x   0 msusol   (217018) primarygroup (89939)     1638 2023-04-23 23:39:05.000000 pyLDAvis-3.4.1/setup.py
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.382878 pyLDAvis-3.4.1/tests/
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.731182 pyLDAvis-3.4.1/tests/data/
+-rwxr-xr-x   0 msusol   (217018) primarygroup (89939)     1261 2021-02-17 22:18:20.000000 pyLDAvis-3.4.1/tests/data/export_data.R
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)  7087084 2021-02-17 22:18:27.000000 pyLDAvis-3.4.1/tests/data/movie_reviews_input.json
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)   159501 2021-02-17 22:18:21.000000 pyLDAvis-3.4.1/tests/data/movie_reviews_output.json
+drwxr-xr-x   0 msusol   (217018) primarygroup (89939)        0 2023-04-23 23:42:15.733759 pyLDAvis-3.4.1/tests/pyLDAvis/
+-rwxr-xr-x   0 msusol   (217018) primarygroup (89939)     2528 2021-03-16 18:19:40.000000 pyLDAvis-3.4.1/tests/pyLDAvis/test_gensim_models.py
+-rw-r--r--   0 msusol   (217018) primarygroup (89939)     3285 2023-04-23 22:42:59.000000 pyLDAvis-3.4.1/tests/pyLDAvis/test_prepare.py
```

### Comparing `pyLDAvis-3.4.0/CONTRIBUTING.rst` & `pyLDAvis-3.4.1/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
-3. The pull request should work for Python 3.8, 3.9, 3.10, 3.11, and for PyPI. Check
+3. The pull request should work for Python 3.9, 3.10, 3.11, and for PyPI. Check
    https://travis-ci.org/bmabey/pyLDAvis/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Maintainers
 ------------
 
 Ready to publish a new version to PyPi? Here's how the workflow to follow.
```

### Comparing `pyLDAvis-3.4.0/HISTORY.rst` & `pyLDAvis-3.4.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 History
 -------
 
+3.4.1 (2023-04-23)
+~~~~~~~~~~~~~~~~~~
+* Pandas 2.x release, the drop shall use .drop(saliency, axis=1) #247
+
 3.4.0 (2023-02-12)
 ~~~~~~~~~~~~~~~~~~
 
 * Adding testing for Python 3.10, 3.11, move default version to Python 3.10.
 * Tox testing: No module named 'sklearn.manifold'; 'sklearn' is not a package.
   * Rename sklearn.py to lda_model.py.
 * ValueError: The parameter init="pca" cannot be used with metric="precomputed".
```

### Comparing `pyLDAvis-3.4.0/LICENSE` & `pyLDAvis-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/PKG-INFO` & `pyLDAvis-3.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pyLDAvis
-Version: 3.4.0
+Version: 3.4.1
 Summary: Interactive topic model visualization. Port of the R package.
 Home-page: https://github.com/bmabey/pyLDAvis
-Download-URL: https://github.com/bmabey/pyLDAvis/tarball/3.4.0
+Download-URL: https://github.com/bmabey/pyLDAvis/tarball/3.4.1
 Author: Ben Mabey
 Author-email: ben@benmabey.com
 License: BSD-3-Clause
 Keywords: data science,visualization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 pyLDAvis
 ========
 
 Python library for interactive topic model visualization.
```

### Comparing `pyLDAvis-3.4.0/README.rst` & `pyLDAvis-3.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/docs/Makefile` & `pyLDAvis-3.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/docs/conf.py` & `pyLDAvis-3.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/docs/index.rst` & `pyLDAvis-3.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/docs/make.bat` & `pyLDAvis-3.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/notebooks/GraphLab.ipynb` & `pyLDAvis-3.4.1/notebooks/GraphLab.ipynb`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/notebooks/LDA model.ipynb` & `pyLDAvis-3.4.1/notebooks/LDA model.ipynb`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/notebooks/Movie Reviews, AP News, and Jeopardy.ipynb` & `pyLDAvis-3.4.1/notebooks/Movie Reviews, AP News, and Jeopardy.ipynb`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/notebooks/Untitled.ipynb` & `pyLDAvis-3.4.1/notebooks/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/notebooks/pyLDAvis_overview.ipynb` & `pyLDAvis-3.4.1/notebooks/pyLDAvis_overview.ipynb`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/_display.py` & `pyLDAvis-3.4.1/pyLDAvis/_display.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/_prepare.py` & `pyLDAvis-3.4.1/pyLDAvis/_prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     default_term_info = pd.DataFrame({
         'saliency': saliency,
         'Term': vocab,
         'Freq': term_frequency,
         'Total': term_frequency,
         'Category': 'Default'})
     default_term_info = default_term_info.sort_values(
-        by='saliency', ascending=False).head(R).drop('saliency', 1)
+        by='saliency', ascending=False).head(R).drop('saliency', axis=1)
     # Rounding Freq and Total to integer values to match LDAvis code:
     default_term_info['Freq'] = np.floor(default_term_info['Freq'])
     default_term_info['Total'] = np.floor(default_term_info['Total'])
     ranks = np.arange(R, 0, -1)
     default_term_info['logprob'] = default_term_info['loglift'] = ranks
     default_term_info = default_term_info.reindex(columns=[
         "Term", "Freq", "Total", "Category", "logprob", "loglift"
```

### Comparing `pyLDAvis-3.4.0/pyLDAvis/_server.py` & `pyLDAvis-3.4.1/pyLDAvis/_server.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/gensim_models.py` & `pyLDAvis-3.4.1/pyLDAvis/gensim_models.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/graphlab.py` & `pyLDAvis-3.4.1/pyLDAvis/graphlab.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/js/d3.v5.min.js` & `pyLDAvis-3.4.1/pyLDAvis/js/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/js/ldavis.css` & `pyLDAvis-3.4.1/pyLDAvis/js/ldavis.css`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/js/ldavis.js` & `pyLDAvis-3.4.1/pyLDAvis/js/ldavis.js`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/js/ldavis.v1.0.0.css` & `pyLDAvis-3.4.1/pyLDAvis/js/ldavis.v1.0.0.css`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/js/ldavis.v1.0.0.js` & `pyLDAvis-3.4.1/pyLDAvis/js/ldavis.v1.0.0.js`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/js/ldavis.v3.0.0.js` & `pyLDAvis-3.4.1/pyLDAvis/js/ldavis.v3.0.0.js`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lda_model.py` & `pyLDAvis-3.4.1/pyLDAvis/lda_model.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/__main__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/__pip-runner__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/build_env.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cache.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/base_command.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/command_context.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/parser.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/req_command.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/spinners.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/cache.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/check.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/completion.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/configuration.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/debug.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/download.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/freeze.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/hash.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/help.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/index.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/inspect.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/install.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/list.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/search.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/show.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/configuration.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/base.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/installed.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/collector.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/package_finder.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/sources.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/base.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/_json.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/base.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/candidate.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/direct_url.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/format_control.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/index.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/installation_report.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/link.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/scheme.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/search_scope.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/target_python.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/auth.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/cache.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/download.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/session.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/check.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/freeze.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/prepare.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/pyproject.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/constructors.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_file.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_install.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_set.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/base.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/_log.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/encoding.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/glibc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/hashes.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/logging.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/misc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/models.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/packaging.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/urls.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/git.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_internal/wheel_builder.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/core.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/database.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/index.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/version.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/distro.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/codec.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/core.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/version.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/build.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/check.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/colorlog.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/dirtools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/envbuild.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/_in_process.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/meta.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/wrappers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/console.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/style.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/token.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/api.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/auth.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/certs.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/help.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/models.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/packages.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/structures.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/abc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/align.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/bar.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/box.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/cells.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/columns.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/console.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/containers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/control.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/errors.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/json.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/layout.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/logging.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/markup.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/measure.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/padding.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pager.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/palette.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/panel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/repr.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/rule.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/scope.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/screen.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/segment.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/status.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/style.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/styled.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/table.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/text.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/theme.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/tree.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/six.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/pkg_resources/extern/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_collections.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cmd.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/check.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/config.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/register.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/config.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/core.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dist.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/errors.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/extension.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/file_util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/filelist.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/log.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/spawn.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/text_file.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/version.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_entry_points.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_imp.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_importlib.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_itertools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_path.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/zipp.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/archive_util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/build_meta.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/alias.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_egg.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_clib.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_ext.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_py.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/develop.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/dist_info.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/easy_install.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/editable_wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/egg_info.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_egg_info.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_lib.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_scripts.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/py36compat.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/rotate.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/saveopts.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/sdist.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/setopt.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/test.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/command/upload_docs.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/expand.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/config/setupcfg.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/dep_util.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/depends.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/discovery.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/dist.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/errors.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/extension.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/extern/__init__.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/glob.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/installer.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/launch.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/logging.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/monkey.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/msvc.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/namespaces.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/package_index.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/sandbox.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/unicode_utils.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/wheel.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/lib/python3.11/site-packages/setuptools/windows_support.py` & `pyLDAvis-3.4.1/pyLDAvis/lib/python3.11/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/urls.py` & `pyLDAvis-3.4.1/pyLDAvis/urls.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis/utils.py` & `pyLDAvis-3.4.1/pyLDAvis/utils.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/pyLDAvis.egg-info/PKG-INFO` & `pyLDAvis-3.4.1/pyLDAvis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pyLDAvis
-Version: 3.4.0
+Version: 3.4.1
 Summary: Interactive topic model visualization. Port of the R package.
 Home-page: https://github.com/bmabey/pyLDAvis
-Download-URL: https://github.com/bmabey/pyLDAvis/tarball/3.4.0
+Download-URL: https://github.com/bmabey/pyLDAvis/tarball/3.4.1
 Author: Ben Mabey
 Author-email: ben@benmabey.com
 License: BSD-3-Clause
 Keywords: data science,visualization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 pyLDAvis
 ========
 
 Python library for interactive topic model visualization.
```

### Comparing `pyLDAvis-3.4.0/pyLDAvis.egg-info/SOURCES.txt` & `pyLDAvis-3.4.1/pyLDAvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/setup.py` & `pyLDAvis-3.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,36 +14,36 @@
     requirements = []
 else:
     with open('requirements.txt') as f:
         requirements = f.read().splitlines()
 
 setup(
     name='pyLDAvis',
-    version='3.4.0',
+    version='3.4.1',
     description='Interactive topic model visualization. Port of the R package.',
+    long_description_content_type="text/x-rst",
     long_description=readme,
     author='Ben Mabey',
     author_email='ben@benmabey.com',
     url='https://github.com/bmabey/pyLDAvis',
-    download_url='https://github.com/bmabey/pyLDAvis/tarball/3.4.0',
+    download_url='https://github.com/bmabey/pyLDAvis/tarball/3.4.1',
     packages=['pyLDAvis'],
     package_dir={'pyLDAvis': 'pyLDAvis'},
     tests_require=['pytest'],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     include_package_data=True,
     install_requires=requirements,
     license='BSD-3-Clause',
     zip_safe=False,
     keywords=['data science', 'visualization'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ]
 )
```

### Comparing `pyLDAvis-3.4.0/tests/data/export_data.R` & `pyLDAvis-3.4.1/tests/data/export_data.R`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/tests/data/movie_reviews_input.json` & `pyLDAvis-3.4.1/tests/data/movie_reviews_input.json`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/tests/data/movie_reviews_output.json` & `pyLDAvis-3.4.1/tests/data/movie_reviews_output.json`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/tests/pyLDAvis/test_gensim_models.py` & `pyLDAvis-3.4.1/tests/pyLDAvis/test_gensim_models.py`

 * *Files identical despite different names*

### Comparing `pyLDAvis-3.4.0/tests/pyLDAvis/test_prepare.py` & `pyLDAvis-3.4.1/tests/pyLDAvis/test_prepare.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,25 +57,25 @@
     ejoined = remove_col_suffixes(joined[['Term', 'Category', 'Freq_e',
                                           'Total_e', 'loglift_e', 'logprob_e']])
     ojoined = remove_col_suffixes(joined[['Term', 'Category', 'Freq_o', 'Total_o',
                                           'loglift_o', 'logprob_o']])
 
     join_percent = float(len(joined)) / len(etinfo)
     print('Topic Info join was %.0f%%' % (100 * join_percent))
-    assert_frame_equal(ejoined, ojoined, check_less_precise=True)
+    assert_frame_equal(ejoined, ojoined, check_exact=False, rtol=0.1)
     assert join_percent > 0.95
 
     def abs_basis(df):
         df.x = df.x.abs()
         df.y = df.y.abs()
         return df
 
     emds, omds = both(lambda r: abs_basis(pd.DataFrame(r['mdsDat'])))
     assert_frame_equal(emds.reindex(sorted(oddf.columns), axis=1),
-                       omds.reindex(sorted(oddf.columns), axis=1), check_less_precise=True)
+                       omds.reindex(sorted(oddf.columns), axis=1), check_exact=False, rtol=0.1)
 
     def rounded_token_table(r):
         tt = pd.DataFrame(r['token.table'])
         tt.Freq = tt.Freq.round(5)
         return tt
     ett, ott = both(rounded_token_table)
     joined = pd.DataFrame(pd.merge(ott, ett, on=['Freq', 'Term'],
```

