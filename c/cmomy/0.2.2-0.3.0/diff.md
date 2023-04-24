# Comparing `tmp/cmomy-0.2.2.tar.gz` & `tmp/cmomy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmomy-0.2.2.tar", last modified: Thu Apr  6 01:15:59 2023, max compression
+gzip compressed data, was "cmomy-0.3.0.tar", last modified: Mon Apr 24 20:51:25 2023, max compression
```

## Comparing `cmomy-0.2.2.tar` & `cmomy-0.3.0.tar`

### file list

```diff
@@ -1,140 +1,144 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.535226 cmomy-0.2.2/
--rw-r--r--   0 wpk      (42033)    36681     1469 2023-04-06 00:58:31.000000 cmomy-0.2.2/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681       31 2023-01-25 16:37:02.000000 cmomy-0.2.2/.gitattributes
--rw-r--r--   0 wpk      (42033)    36681     1337 2023-04-06 00:58:31.000000 cmomy-0.2.2/.gitignore
--rw-r--r--   0 wpk      (42033)    36681     2864 2023-04-06 00:58:31.000000 cmomy-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681      131 2023-03-22 20:26:04.000000 cmomy-0.2.2/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     6716 2023-04-06 00:58:31.000000 cmomy-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681       59 2023-03-22 20:26:04.000000 cmomy-0.2.2/HISTORY.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-03-15 19:07:26.000000 cmomy-0.2.2/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      313 2023-03-22 20:26:04.000000 cmomy-0.2.2/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681     8349 2023-04-06 00:58:31.000000 cmomy-0.2.2/Makefile
--rw-r--r--   0 wpk      (42033)    36681     8208 2023-04-06 01:15:59.535663 cmomy-0.2.2/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     5541 2023-03-22 20:26:04.000000 cmomy-0.2.2/README.md
--rw-r--r--   0 wpk      (42033)    36681      652 2023-01-25 16:37:02.000000 cmomy-0.2.2/commands.sh
--rw-r--r--   0 wpk      (42033)    36681      366 2023-01-25 16:37:02.000000 cmomy-0.2.2/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.417643 cmomy-0.2.2/docs/
--rw-r--r--   0 wpk      (42033)    36681     1201 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.387482 cmomy-0.2.2/docs/_build/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.388759 cmomy-0.2.2/docs/_build/html/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.388067 cmomy-0.2.2/docs/_build/html/_sources/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.420740 cmomy-0.2.2/docs/_build/html/_sources/reference/
--rw-r--r--   0 wpk      (42033)    36681      158 2023-03-28 20:18:42.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/api-baseclasses.rst
--rw-r--r--   0 wpk      (42033)    36681      122 2023-03-28 18:24:46.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/api-modules.rst
--rw-r--r--   0 wpk      (42033)    36681      398 2023-03-28 20:18:42.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/api-public.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.427956 cmomy-0.2.2/docs/_build/html/_sources/reference/generated/
--rw-r--r--   0 wpk      (42033)    36681     2209 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/generated/cmomy.CentralMoments.rst
--rw-r--r--   0 wpk      (42033)    36681      109 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/generated/cmomy.central_moments.rst
--rw-r--r--   0 wpk      (42033)    36681      201 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/generated/cmomy.convert.rst
--rw-r--r--   0 wpk      (42033)    36681      202 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/generated/cmomy.resample.rst
--rw-r--r--   0 wpk      (42033)    36681     2614 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/generated/cmomy.xCentralMoments.rst
--rw-r--r--   0 wpk      (42033)    36681      112 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/_build/html/_sources/reference/generated/cmomy.xcentral_moments.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.432182 cmomy-0.2.2/docs/_build/html/_static/
--rw-r--r--   0 wpk      (42033)    36681      286 2023-03-22 18:45:53.000000 cmomy-0.2.2/docs/_build/html/_static/file.png
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.434073 cmomy-0.2.2/docs/_build/html/_static/images/
--rw-r--r--   0 wpk      (42033)    36681     7601 2023-03-22 18:45:54.000000 cmomy-0.2.2/docs/_build/html/_static/images/logo_colab.png
--rw-r--r--   0 wpk      (42033)    36681       90 2023-03-22 18:45:53.000000 cmomy-0.2.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 wpk      (42033)    36681       90 2023-03-22 18:45:53.000000 cmomy-0.2.2/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.389812 cmomy-0.2.2/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.435812 cmomy-0.2.2/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2777 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.438176 cmomy-0.2.2/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      703 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      624 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.442488 cmomy-0.2.2/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.447902 cmomy-0.2.2/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.451103 cmomy-0.2.2/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       31 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681    14406 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       36 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/contributing.md
--rw-r--r--   0 wpk      (42033)    36681     1094 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/example.md
--rw-r--r--   0 wpk      (42033)    36681       31 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/history.md
--rw-r--r--   0 wpk      (42033)    36681      367 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681     1100 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       39 2023-03-22 20:26:04.000000 cmomy-0.2.2/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-03-15 18:41:43.000000 cmomy-0.2.2/docs/make.bat
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.454485 cmomy-0.2.2/docs/notebooks/
--rw-r--r--   0 wpk      (42033)    36681   156802 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/notebooks/motivation.ipynb
--rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/notebooks/usage_notebook.ipynb
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.463057 cmomy-0.2.2/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      158 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/reference/api-baseclasses.rst
--rw-r--r--   0 wpk      (42033)    36681      122 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/reference/api-modules.rst
--rw-r--r--   0 wpk      (42033)    36681      398 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/reference/api-public.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.475664 cmomy-0.2.2/docs/reference/generated/
--rw-r--r--   0 wpk      (42033)    36681     2209 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/reference/generated/cmomy.CentralMoments.rst
--rw-r--r--   0 wpk      (42033)    36681      109 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/reference/generated/cmomy.central_moments.rst
--rw-r--r--   0 wpk      (42033)    36681      201 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/reference/generated/cmomy.convert.rst
--rw-r--r--   0 wpk      (42033)    36681      202 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/reference/generated/cmomy.resample.rst
--rw-r--r--   0 wpk      (42033)    36681     2614 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/reference/generated/cmomy.xCentralMoments.rst
--rw-r--r--   0 wpk      (42033)    36681      112 2023-03-28 18:40:35.000000 cmomy-0.2.2/docs/reference/generated/cmomy.xcentral_moments.rst
--rw-r--r--   0 wpk      (42033)    36681      196 2023-04-06 00:58:31.000000 cmomy-0.2.2/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681      491 2023-01-25 16:37:02.000000 cmomy-0.2.2/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.487920 cmomy-0.2.2/environment/
--rw-r--r--   0 wpk      (42033)    36681     1075 2023-03-22 20:26:04.000000 cmomy-0.2.2/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      248 2023-03-22 20:26:04.000000 cmomy-0.2.2/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      120 2023-03-22 20:26:04.000000 cmomy-0.2.2/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       76 2023-04-06 00:58:31.000000 cmomy-0.2.2/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      694 2023-04-06 00:58:31.000000 cmomy-0.2.2/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      373 2023-04-06 00:58:31.000000 cmomy-0.2.2/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       27 2023-03-22 20:26:04.000000 cmomy-0.2.2/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      150 2023-03-22 20:26:04.000000 cmomy-0.2.2/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      173 2023-03-22 20:26:04.000000 cmomy-0.2.2/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.497592 cmomy-0.2.2/examples/
--rw-r--r--   0 wpk      (42033)    36681    71020 2023-04-06 00:58:31.000000 cmomy-0.2.2/examples/bootstrap.ipynb
--rw-r--r--   0 wpk      (42033)    36681   136964 2023-04-06 00:58:31.000000 cmomy-0.2.2/examples/central_moments.ipynb
--rw-r--r--   0 wpk      (42033)    36681    44856 2023-04-06 00:58:31.000000 cmomy-0.2.2/examples/example_usage.ipynb
--rw-r--r--   0 wpk      (42033)    36681    12361 2023-04-06 00:58:31.000000 cmomy-0.2.2/examples/parallel_test.ipynb
--rw-r--r--   0 wpk      (42033)    36681    58228 2023-04-06 00:58:31.000000 cmomy-0.2.2/examples/test_accumulator.ipynb
--rw-r--r--   0 wpk      (42033)    36681     4245 2023-04-06 01:14:49.000000 cmomy-0.2.2/pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681      383 2023-04-06 01:15:59.537233 cmomy-0.2.2/setup.cfg
--rw-r--r--   0 wpk      (42033)    36681       88 2023-04-06 00:58:31.000000 cmomy-0.2.2/setup.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.393724 cmomy-0.2.2/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.518772 cmomy-0.2.2/src/cmomy/
--rw-r--r--   0 wpk      (42033)    36681     1045 2023-03-29 00:12:57.000000 cmomy-0.2.2/src/cmomy/__init__.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.522414 cmomy-0.2.2/src/cmomy/_docfiller/
--rw-r--r--   0 wpk      (42033)    36681       23 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/_docfiller/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    19686 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/_docfiller/docfiller.py
--rw-r--r--   0 wpk      (42033)    36681    23537 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/_docfiller/docscrape.py
--rw-r--r--   0 wpk      (42033)    36681     3362 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/_docstrings.py
--rw-r--r--   0 wpk      (42033)    36681     2544 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/_formatting.py
--rw-r--r--   0 wpk      (42033)    36681     6463 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/_resample.py
--rw-r--r--   0 wpk      (42033)    36681     2311 2023-01-25 16:37:02.000000 cmomy-0.2.2/src/cmomy/_testing.py
--rw-r--r--   0 wpk      (42033)    36681      658 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/_typing.py
--rw-r--r--   0 wpk      (42033)    36681    39728 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/abstract_central.py
--rw-r--r--   0 wpk      (42033)    36681     5598 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/cached_decorators.py
--rw-r--r--   0 wpk      (42033)    36681    51556 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/central.py
--rw-r--r--   0 wpk      (42033)    36681      967 2023-01-25 16:37:02.000000 cmomy-0.2.2/src/cmomy/compile.py
--rw-r--r--   0 wpk      (42033)    36681    10869 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/convert.py
--rw-r--r--   0 wpk      (42033)    36681     1834 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/options.py
--rw-r--r--   0 wpk      (42033)    36681     3122 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/pusher_interface.py
--rw-r--r--   0 wpk      (42033)    36681    14250 2023-01-25 16:37:02.000000 cmomy-0.2.2/src/cmomy/pushers.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/py.typed
--rw-r--r--   0 wpk      (42033)    36681    13752 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/resample.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.533730 cmomy-0.2.2/src/cmomy/tests/
--rw-r--r--   0 wpk      (42033)    36681        0 2023-01-25 16:37:02.000000 cmomy-0.2.2/src/cmomy/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    11871 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/conftest.py
--rw-r--r--   0 wpk      (42033)    36681     5427 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/test_central.py
--rw-r--r--   0 wpk      (42033)    36681     9554 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/test_central_2.py
--rw-r--r--   0 wpk      (42033)    36681     1085 2023-01-25 16:37:02.000000 cmomy-0.2.2/src/cmomy/tests/test_convert.py
--rw-r--r--   0 wpk      (42033)    36681     4085 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/test_resample.py
--rw-r--r--   0 wpk      (42033)    36681     2354 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/test_stability.py
--rw-r--r--   0 wpk      (42033)    36681     2682 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/test_verify.py
--rw-r--r--   0 wpk      (42033)    36681     6183 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/test_xcentral.py
--rw-r--r--   0 wpk      (42033)    36681     4879 2023-03-22 20:26:04.000000 cmomy-0.2.2/src/cmomy/tests/test_xcentral_constructors.py
--rw-r--r--   0 wpk      (42033)    36681     3207 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/utils.py
--rw-r--r--   0 wpk      (42033)    36681    62223 2023-04-06 00:58:31.000000 cmomy-0.2.2/src/cmomy/xcentral.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-06 01:15:59.534731 cmomy-0.2.2/src/cmomy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     3397 2023-04-06 01:15:59.000000 cmomy-0.2.2/src/cmomy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681     3988 2023-04-06 00:58:31.000000 cmomy-0.2.2/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.185413 cmomy-0.3.0/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1475 2023-04-24 20:47:28.000000 cmomy-0.3.0/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      513 2023-04-24 20:47:28.000000 cmomy-0.3.0/.editorconfig
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       31 2023-01-25 16:37:02.000000 cmomy-0.3.0/.gitattributes
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1313 2023-04-24 20:47:28.000000 cmomy-0.3.0/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-24 20:47:28.000000 cmomy-0.3.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3421 2023-04-24 20:47:28.000000 cmomy-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-24 20:47:28.000000 cmomy-0.3.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-24 20:47:28.000000 cmomy-0.3.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2171 2023-04-24 20:47:28.000000 cmomy-0.3.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8861 2023-04-24 20:47:28.000000 cmomy-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-03-15 19:07:26.000000 cmomy-0.3.0/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-24 20:47:28.000000 cmomy-0.3.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10386 2023-04-24 20:47:28.000000 cmomy-0.3.0/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9353 2023-04-24 20:51:25.185770 cmomy-0.3.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4599 2023-04-24 20:47:28.000000 cmomy-0.3.0/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.133343 cmomy-0.3.0/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      584 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/20230424_125230_william.krekelberg_update_cruft.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.134000 cmomy-0.3.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.135152 cmomy-0.3.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      652 2023-01-25 16:37:02.000000 cmomy-0.3.0/commands.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      366 2023-01-25 16:37:02.000000 cmomy-0.3.0/conftest.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.140030 cmomy-0.3.0/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1201 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.117786 cmomy-0.3.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.140432 cmomy-0.3.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.141219 cmomy-0.3.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.142747 cmomy-0.3.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.144824 cmomy-0.3.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.146053 cmomy-0.3.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14554 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/contributing.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      891 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/example_for_readme.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.146870 cmomy-0.3.0/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      887 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/create-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       84 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.147996 cmomy-0.3.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   156774 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   295212 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      860 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-03-15 18:41:43.000000 cmomy-0.3.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.149995 cmomy-0.3.0/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      158 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/reference/api-baseclasses.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/reference/api-modules.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      398 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/reference/api-public.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      194 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      491 2023-04-21 20:37:24.000000 cmomy-0.3.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.154283 cmomy-0.3.0/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      967 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      282 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      640 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      435 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      175 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      166 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      159 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.154676 cmomy-0.3.0/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.157041 cmomy-0.3.0/examples/archived/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    70967 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/bootstrap.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   136974 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/central_moments.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    44856 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/example_usage.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12217 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/parallel_test.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    58117 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/test_accumulator.ipynb
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.158099 cmomy-0.3.0/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   156774 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   295212 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5218 2023-04-24 20:47:28.000000 cmomy-0.3.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.159245 cmomy-0.3.0/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-24 20:47:28.000000 cmomy-0.3.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-24 20:47:28.000000 cmomy-0.3.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      286 2023-04-24 20:51:25.186801 cmomy-0.3.0/setup.cfg
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      323 2023-04-24 20:47:28.000000 cmomy-0.3.0/setup.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.121475 cmomy-0.3.0/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.169553 cmomy-0.3.0/src/cmomy/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1045 2023-03-29 00:12:57.000000 cmomy-0.3.0/src/cmomy/__init__.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.177109 cmomy-0.3.0/src/cmomy/_docfiller/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       23 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/_docfiller/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    19686 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/_docfiller/docfiller.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23537 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/_docfiller/docscrape.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3354 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/_docstrings.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2736 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/_formatting.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6463 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/_resample.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2311 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/_testing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      658 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/_typing.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    39709 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/abstract_central.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5598 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/cached_decorators.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    51565 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/central.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      967 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/compile.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10911 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/convert.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1834 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/options.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3122 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/pusher_interface.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14250 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/pushers.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/py.typed
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13795 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/resample.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.184783 cmomy-0.3.0/src/cmomy/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11871 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/conftest.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5427 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_central.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9554 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_central_2.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1085 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/tests/test_convert.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4085 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_resample.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2354 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_stability.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2682 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_verify.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6183 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_xcentral.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4879 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_xcentral_constructors.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3249 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/utils.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    62270 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/xcentral.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.174623 cmomy-0.3.0/src/cmomy.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9353 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3235 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-06 00:42:47.000000 cmomy-0.3.0/src/cmomy.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        6 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4507 2023-04-24 20:47:28.000000 cmomy-0.3.0/tox.ini
```

### Comparing `cmomy-0.2.2/.gitignore` & `cmomy-0.3.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -103,11 +103,10 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
-/docs/generated/
+/docs/**/generated/
 /monkeytype.sqlite3
 /dist-conda/
-/docs/reference/generated/
```

### Comparing `cmomy-0.2.2/.pre-commit-config.yaml` & `cmomy-0.3.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,127 @@
 ---
 # pre-commit install
 # pre-commit run --all-files
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
+default_install_hook_types:
+  - pre-commit
+  - commit-msg
 repos:
+  #* Top level
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-added-large-files
       - id: check-yaml
-        #     args: [--unsafe]
-  # Ruff
+      - id: check-json
+      - id: check-merge-conflict
+      - id: check-symlinks
+      - id: check-toml
+  #* Formatting
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: "v3.0.0-alpha.6"
+    hooks:
+      - id: prettier
+        stages: [commit]
+        additional_dependencies:
+          - prettier-plugin-toml
+        exclude: ^docs/example_for_readme.md
+  #* Linting
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.254'
+    rev: "v0.0.261"
     hooks:
       - id: ruff
-        args: ["--fix"]
-  # isort should run before black as black sometimes tweaks the isort output
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        stages: [manual]
-  # https://github.com/python/black#version-control-integration
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
-      - id: black-jupyter
+      # - id: black-jupyter
+      # Move to just black.  use nbqa for notebook formatting
+      - id: black
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: "1.13.0"  # replace with latest tag on GitHub
+    rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
-          - black==23.1.0
+          - black==23.3.0
         exclude: ^README.md
-  - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.8
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: blackdoc
-        additional_dependencies: ["black==23.1.0"]
-      - id: blackdoc-autoupdate-black
-  - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+      - id: nbqa-ruff
+        additional_dependencies: [ruff]
+        exclude: examples/archived/
+      - id: nbqa-black
+        additional_dependencies: [black]
+
+  #* Commit message
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: v3.0.1
+    hooks:
+      - id: commitizen
+        stages: [commit-msg]
+
+  #* Manual Linting
+  - repo: local
     hooks:
-      - id: codespell
-        types_or: [python, rst, markdown, cython, c]
-        additional_dependencies: [tomli]
-        args: [-I, docs/spelling_wordlist.txt]
+      - id: mypy
+        name: mypy
+        entry: tox
+        args: ["-e", "lint-mypy"]
+        language: system
+        pass_filenames: false
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
+        stages: [manual]
+  # isort, pyupgrade, flake8 defer to ruff
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
         stages: [manual]
-  # this should be run before flake8 to
-  # this should be run externally
-  # messes up too many things
-  # - repo: https://github.com/PyCQA/docformatter
-  #   rev: v1.5.0
-  #   hooks:
-  #     - id: docformatter
-  #       args: [--in-place]
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.3.1
+    hooks:
+      - id: pyupgrade
+        stages: [manual]
+        args: [--py38-plus]
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         stages: [manual]
-        additional_dependencies: [flake8-docstrings]
+        additional_dependencies:
+          - flake8-docstrings
+          - Flake8-pyproject
+          # - pep8-naming
+          # - flake8-rst-docstrings
         exclude: ^tests/|^src/cmomy/tests/|^docs/conf.py|^setup.py
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: mypy
-        # `properies` & `asv_bench` are copied from setup.cfg.
-        # `_typed_ops.py` is added since otherwise mypy will complain (but notably only in pre-commit)
-        exclude: properties|asv_bench|_typed_ops.py|conf.py
-        # This is slow and so we take it out of the fast-path; requires passing
-        # `--hook-stage manual` to pre-commit
+      - id: nbqa-pyupgrade
+        additional_dependencies: [pyupgrade]
         stages: [manual]
-        additional_dependencies: [types-pkg_resources, typing-extensions==3.10.0.0, numpy]
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+        args: [--py38-plus]
+      - id: nbqa-isort
+        additional_dependencies: [isort]
+        stages: [manual]
+  #** spelling
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.4
     hooks:
-      - id: pyupgrade
+      - id: codespell
+        types_or: [python, rst, markdown, cython, c]
+        additional_dependencies: [tomli]
+        args: [-I, docs/spelling_wordlist.txt]
+        stages: [manual]
+  #** markdown
+  - repo: https://github.com/DavidAnson/markdownlint-cli2
+    rev: v0.6.0
+    hooks:
+      - id: markdownlint-cli2
         stages: [manual]
-        args:
-          - --py38-plus
-          # remove on f-strings in Py3.7
-          - --keep-percent-format
+        args: ["--style prettier"]
```

### Comparing `cmomy-0.2.2/CONTRIBUTING.md` & `cmomy-0.3.0/CONTRIBUTING.md`

 * *Files 23% similar despite different names*

```diff
@@ -25,119 +25,182 @@
 ### Implement Features
 
 Look through the GitHub issues for features. Anything tagged with "enhancement"
 and "help wanted" is open to whoever wants to implement it.
 
 ### Write Documentation
 
-`cmomy` could always use more documentation, whether as part of the
-official `cmomy` docs, in docstrings, or even on the web in blog posts,
-articles, and such.
+`cmomy` could always use more documentation, whether as part of the official
+`cmomy` docs, in docstrings, or even on the web in blog posts, articles, and
+such.
 
 ### Submit Feedback
 
-The best way to send feedback is to file an issue at <https://github.com/usnistgov/cmomy/issues>.
+The best way to send feedback is to file an issue at
+<https://github.com/usnistgov/cmomy/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
-- Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-## Get Started!
+- Remember that this is a volunteer-driven project, and that contributions are
+  welcome :)
 
+## Get Started
 
 ### Environment setup
 
 [pipx]: https://github.com/pypa/pipx
 [condax]: https://github.com/mariusvniekerk/condax
 [mamba]: https://github.com/mamba-org/mamba
-[conda-fast-setup]: https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
+[conda-fast-setup]:
+  https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community
 [pre-commit]: https://pre-commit.com/
 [tox]: https://tox.wiki/en/latest/
 [tox-conda]: https://github.com/tox-dev/tox-conda
 [cruft]: https://github.com/cruft/cruft
 [conda-merge]: https://github.com/amitbeka/conda-merge
 [git-flow]: https://github.com/nvie/gitflow
-
-This project uses a host of tools to (hopefully) make development easier.  We recommend installing some of these tools system wide.  For this, we recommend using
-either [pipx] or [condax].  We mostly use conda/condax, but the choice is yours.  For conda, we recommend actually using [mamba]. Alternatively, you can setup `conda` to use the faster `mamba` solver.
-See [here][conda-fast-setup] for details.
-
-Additional dependencies are:
-
-* [pre-commit]
-* [tox] and [tox-conda]
-* [cruft]
-* [conda-merge]
+[scriv]: https://github.com/nedbat/scriv
+[conventional-style]: https://www.conventionalcommits.org/en/v1.0.0/
+[commitizen]: https://github.com/commitizen-tools/commitizen
+[nb-conda-kernels]: https://github.com/Anaconda-Platform/nb_conda_kernels
+
+This project uses a host of tools to (hopefully) make development easier. We
+recommend installing some of these tools system wide. For this, we recommend
+using either [pipx] or [condax]. We mostly use conda/condax, but the choice is
+yours. For conda, we recommend actually using [mamba]. Alternatively, you can
+setup `conda` to use the faster `mamba` solver. See [here][conda-fast-setup] for
+details.
+
+Additional tools are:
+
+- [pre-commit]
+- [tox] and [tox-conda]
+- [cruft]
+- [conda-merge]
+- [scriv]
 
 These are setup using the following:
 
-```bash
+```console
 condax install pre-commit
 condax install tox
 condax inject tox tox-conda
 condax install cruft
 condax install conda-merge
+condax install commitizen
+pipx install scriv
 ```
 
+Alternatively, you can install these dependencies using:
+
+```console
+conda env update -n {env-name} environment/tools.yaml
+```
 
 ### Getting the repo
 
 Ready to contribute? Here's how to set up `cmomy` for local development.
 
-1. Fork the `cmomy` repo on GitHub.
+1.  Fork the `cmomy` repo on GitHub.
 
-2. Clone your fork locally:
+1.  Clone your fork locally:
 
     ```bash
     git clone git@github.com:your_name_here/cmomy.git
     ```
 
-3. Create development environment.  Using the `make` will install a development version using mamba.
+    If the repo includes submodules, you can add them either with the initial
+    close using:
 
     ```bash
-    make mamba-dev
+    git clone --recursive-submodules git@github.com:your_name_here/cmomy.git
     ```
 
-4. Initiate pre-commit with:
+    or after the clone using
 
     ```bash
-    pre-commit init
+    cd cmomy
+    git submodule update --init --recursive
     ```
 
-    To update the recipe, periodically run:
+1.  Create development environment. There are two options to create the
+    development environment.
+
+    a. The recommended method is to use tox by using either:
+
+        ```bash
+        tox -e dev
+        ```
+
+        or
+
+        ```bash
+        make dev-env
+        ```
+        These create a development environment located at `.tox/dev`.
+
+        ```bash
+        make tox-ipykernel-display-name
+        ```
+
+        This will add a meaningful display name for the kernel (assuming you're using
+        [nb-conda-kernels])
+
+    b. Alternativley, you can create centrally located conda environmentment
+    using the command:
+
+        ```bash
+        make mamba-dev
+        ```
+
+        This will create a conda environment 'cmomy-env' in the default location.
+
+        To install (an editable version) of the current package:
+
+        ```bash
+        pip install -e . --no-deps
+        ```
+
+        or
+
+        ```bash
+        make install-dev
+        ```
+
+1.  Initiate [pre-commit] with:
 
     ```bash
-    pre-commit autoupdate
+    pre-commit install
     ```
 
-5. Install editable package:
+    To update the recipe, periodically run:
 
     ```bash
-    pip install -e . --no-deps
+    pre-commit autoupdate
     ```
 
-    or
+    If recipes change over time, you can clean up old installs with:
 
     ```bash
-    make install-dev
+    pre-commit gc
     ```
 
-07. Create a branch for local development:
+1.  Create a branch for local development:
 
     ```bash
     git checkout -b name-of-your-bugfix-or-feature
     ```
 
-    Now you can make your changes locally.  Alternatively, we recommend using [git-flow].
+    Now you can make your changes locally. Alternatively, we recommend using
+    [git-flow].
 
-08. When you're done making changes, check that your changes pass the pre-commit checks:
-    tests.
+1.  When you're done making changes, check that your changes pass the pre-commit
+    checks: tests.
 
     ```bash
     pre-commit run [--all-files]
     ```
 
     To run tests, use:
 
@@ -153,115 +216,153 @@
 
     or using the `make`:
 
     ```bash
     make test-all
     ```
 
+    Additionally, you should run the following:
 
-09. Commit your changes and push your branch to GitHub:
+    ```bash
+    make pre-commit-lint-markdown
+    make pre-commit-codespell
+    ```
 
+1.  Create changelog fragment. See [scriv] for more info.
+
+    ```bash
+    scriv create --edit
     ```
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
+
+1.  Commit your changes and push your branch to GitHub:
+
+    ```bash
+    git add .
+    git commit -m "Your detailed description of your changes."
+    git push origin name-of-your-bugfix-or-feature
     ```
 
-10. Submit a pull request through the GitHub website.
+    Note that the pre-commit hooks will force the commit message to be in the
+    [conventional sytle][conventional-style]. To assist this, you may want to
+    commit using [commitizen].
 
+    ```bash
+    cz commit
+    ```
 
-### Dependency management
+1.  Submit a pull request through the GitHub website.
 
-Dependencies need to be placed in a few locations, which depend on the nature of the dependency.
+### Dependency management
 
-* Package dependency: `environment.yaml` and `dependencies` section of `pyproject.toml`
-* Documentation dependency: `environment/docs-extras.yaml` and `test` section of `pyproject.toml`
-* Development dependency: `environment/dev-extras.yaml` and `dev` section of `pyproject.toml`
+Dependencies need to be placed in a few locations, which depend on the nature of
+the dependency.
 
-Note that total yaml files are build using [conda-merge].  For example, `environment.yaml` is combined with `environment/docs-extras.yaml` to produce `environment/docs.yaml`.  This is automated in the `Makefile`.  You can also run, after doing any updates,
+- Package dependency: `environment.yaml` and `dependencies` section of
+  `pyproject.toml`
+- Documentation dependency: `environment/docs-extras.yaml` and `test` section of
+  `pyproject.toml`
+- Development dependency: `environment/dev-extras.yaml` and `dev` section of
+  `pyproject.toml`
+
+Note that total yaml files are build using [conda-merge]. For example,
+`environment.yaml` is combined with `environment/docs-extras.yaml` to produce
+`environment/docs.yaml`. This is automated in the `Makefile`. You can also run,
+after doing any updates,
 
 ```bash
-make environment-files
+make environment-files-build
 ```
 
 which will rebuild all the needed yaml files.
 
-
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
+2. If the pull request adds functionality, the docs should be updated. Put your
+   new functionality into a function with a docstring, and add the feature to
+   the list in README.rst.
 3. The pull request should work for Python 3.8, 3.9, 3.10.
 
 ## Building the docs
 
-We use [tox] to isolate the documentation build.  Useful commands are as follows.
+We use [tox] to isolate the documentation build. Useful commands are as follows.
 
-* Build the docs:
+- Build the docs:
 
-    ```bash
-    tox -e docs-build
-    ```
+  ```bash
+  tox -e docs-build
+  ```
 
-* Spellcheck the docs:
+- Spellcheck the docs:
 
-    ```bash
-    tox -e docs-spelling
-    ```
+  ```bash
+  tox -e docs-spelling
+  ```
 
-* Create a release of the docs:
+- Create a release of the docs:
 
-    ```bash
-    tox -e docs-release
-    ```
+  ```bash
+  tox -e docs-release
+  ```
+
+  If you make any changes to `docs/examples`, you should run:
 
-    After this, the docs can be pushed to the correct branch for distribution.
+  ```bash
+  make docs-examples-symlink
+  ```
 
-* Live documentation updates using
+  to update symlinks from `docs/examples` to `examples`.
+
+  After this, the docs can be pushed to the correct branch for distribution.
+
+- Live documentation updates using
 
 ## Using tox
 
-The package is setup to use tox to test, build and release pip and conda distributions, and release the docs.  Most of these tasks have a command in the `Makefile`.  To test against multiple versions, use:
+The package is setup to use tox to test, build and release pip and conda
+distributions, and release the docs. Most of these tasks have a command in the
+`Makefile`. To test against multiple versions, use:
 
-```
-$ make test-all
+```bash
+make test-all
 ```
 
 To build the documentation in an isolated environment, use:
 
-```
-$ make docs-build
+```bash
+make docs-build
 ```
 
 To release the documentation use:
 
-```
-$ make docs-release posargs='-m "commit message" -r origin -p'
+```bash
+make docs-release posargs='-m "commit message" -r origin -p'
 ```
 
-Where posargs is are passed to ghp-import.  Note that the branch created is called `nist-pages`.  This can be changed in `tox.ini`.
+Where posargs is are passed to ghp-import. Note that the branch created is
+called `nist-pages`. This can be changed in `tox.ini`.
 
 To build the distribution, use:
 
-```
-$ make dist-pypi-[build-testrelease-release]
+```bash
+make dist-pypi-[build-testrelease-release]
 ```
 
-where `build` build to distro, `testrelease` tests putting on `testpypi` and release puts the distro on pypi.
+where `build` build to distro, `testrelease` tests putting on `testpypi` and
+release puts the distro on pypi.
 
 To build the conda distribution, use:
 
-```
-$ make dist-conda-[recipe, build]
+```bash
+make dist-conda-[recipe, build]
 ```
 
-where `recipe` makes the conda recipe (using grayskull), and `build` makes the distro.  This can be manually added to a channel.
+where `recipe` makes the conda recipe (using grayskull), and `build` makes the
+distro. This can be manually added to a channel.
 
 To test the created distributions, you can use one of:
 
-```
-$ make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
+```bash
+make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
 ```
```

### Comparing `cmomy-0.2.2/LICENSE` & `cmomy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/Makefile` & `cmomy-0.3.0/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 endef
 export BROWSER_PYSCRIPT
 
 define PRINT_HELP_PYSCRIPT
 import re, sys
 
 for line in sys.stdin:
-	match = re.match(r'^([a-zA-Z_-]+):.*?## (.*)$$', line)
+	match = re.match(r'^([a-zA-Z_/.-]+):.*?## (.*)$$', line)
 	if match:
 		target, help = match.groups()
 		print("%-20s %s" % (target, help))
 endef
 export PRINT_HELP_PYSCRIPT
 
 BROWSER := python -c "$$BROWSER_PYSCRIPT"
@@ -50,54 +50,61 @@
 
 
 
 
 ################################################################################
 # utilities
 ################################################################################
-.PHONY: lint pre-commit-init pre-commit-run pre-commit-run-all pre-commit-lint-extra pre-commit-codespell init
-
-lint: ## check style with flake8
-	flake8 cmomy tests
-
+.PHONY: pre-commit-init pre-commit pre-commit-all
 pre-commit-init: ## install pre-commit
 	pre-commit install
 
-pre-commit-run: ## run pre-commit
+pre-commit: ## run pre-commit
 	pre-commit run
 
-pre-commit-run-all: ## run pre-commit on all files
+pre-commit-all: ## run pre-commit on all files
 	pre-commit run --all-files
 
-pre-commit-manual: ## run pre-commit manual flags
-	pre-commit run --hook-stage manual
+.PHONY: pre-commit-lint pre-commit-lint-notebooks pre-commit-prettier pre-commit-lint-markdown
+pre-commit-lint: ## run ruff and black on on all files
+	pre-commit run --all-files ruff
+	pre-commit run --all-files black
+	pre-commit run --all-files blacken-docs
+
+pre-commit-lint-notebooks: ## Run nbqa linting
+	pre-commit run --all-files nbqa-ruff
+	pre-commit run --all-files nbqa-black
+
+pre-commit-prettier: ## run prettier on all files.
+	pre-commit run --all-files prettier
 
-pre-commit-lint-extra: ## run all linting
+pre-commit-lint-markdown: ## run markdown linter.
+	pre-commit run --all-files --hook-stage manual markdownlint-cli2
+
+.PHONY: pre-commit-lint-extra pre-commit-mypy pre-commit-codespell
+pre-commit-lint-extra: ## run all extra linting (isort, flake8, pyupgrade, nbqa isort and pyupgrade)
 	pre-commit run --all-files --hook-stage manual isort
 	pre-commit run --all-files --hook-stage manual flake8
 	pre-commit run --all-files --hook-stage manual pyupgrade
+	pre-commit run --all-files --hook-stage manual nbqa-pyupgrade
+	pre-commit run --all-files --hook-stage manual nbqa-isort
 
 pre-commit-mypy: ## run mypy
 	pre-commit run --all-files --hook-stage manual mypy
 
 pre-commit-codespell: ## run codespell. Note that this imports allowed words from docs/spelling_wordlist.txt
 	pre-commit run --all-files --hook-stage manual codespell
 
-.git: ## init git
-	git init
-
-init: .git pre-commit-init ## run git-init pre-commit
-
 
 ################################################################################
 # my convenience functions
 ################################################################################
 .PHONY: user-venv user-autoenv-zsh user-all
 user-venv: ## create .venv file with name of conda env
-	echo cmomy-env > .venv
+	echo $${PWD}/.tox/dev > .venv
 
 user-autoenv-zsh: ## create .autoenv.zsh files
 	echo conda activate $$(cat .venv) > .autoenv.zsh
 	echo conda deactivate > .autoenv_leave.zsh
 
 user-all: user-venv user-autoenv-zsh ## runs user scripts
 
@@ -128,27 +135,40 @@
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
 
-environment/dev.yaml: environment.yaml environment/dev-extras.yaml ## build development yaml file
-	conda-merge $^ > $@
+ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
+PRETTIER = pre-commit run prettier --files
 
-environment/docs.yaml: environment.yaml environment/docs-extras.yaml ## build docs yaml file
+environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
 	conda-merge $^ > $@
+	-$(PRETTIER) $@ &> /dev/null || true
+
+environment/dev.yaml: ## development environment yaml file
+environment/test.yaml: ## testing environment yaml file
+enviornment/docs.yaml: ## docs environment yaml file
 
-environment/test.yaml: environment.yaml environment/test-extras.yaml ## build test yaml file
+
+# special for linters
+environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
+	echo $^
 	conda-merge $^ > $@
+	-$(PRETTIER) $@ &> /dev/null || true
 
-.PHONY: environment-files
+ENVIRONMENTS += environment/lint.yaml
 
-environment-files: environment/dev.yaml environment/docs.yaml environment/test.yaml ## rebuild all environment files
+.PHONY: environment-files-clean
+environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
+	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
+.PHONY: environment-files-build
+environment-files-build: $(ENVIRONMENTS) ## rebuild all environment files
 
 ################################################################################
 # virtual env
 ################################################################################
 .PHONY: mamba-env mamba-dev mamba-env-update mamba-dev-update
 
 mamba-env: environment.yaml ## create base environment
@@ -165,22 +185,36 @@
 
 ################################################################################
 # TOX
 ###############################################################################
 tox_posargs?=-v
 TOX=CONDA_EXE=mamba tox $(tox_posargs)
 
-## testing
 
+.PHONY: tox-ipykernel-display-name
+tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
+	bash ./scripts/tox-ipykernel-display-name.sh cmomy
+
+## dev env
+.PHONY: dev-env
+dev-env: environment/dev.yaml ## create development environment using tox
+	tox -e dev
+
+## testing
 .PHONY: test-all
 test-all: environment/test.yaml ## run tests on every Python version with tox
 	$(TOX) -- $(posargs)
 
 
 ## docs
+.PHONY: docs-examples-symlink
+docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
+	bash ./scripts/docs-examples-symlinks.sh
+
+
 .PHONY: docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-open docs-live docs-clean-build docs-linkcheck
 posargs=
 docs-build: ## build docs in isolation
 	$(TOX) -e $@ -- $(posargs)
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
@@ -253,7 +287,19 @@
 ################################################################################
 .PHONY: install install-dev
 install: ## install the package to the active Python's site-packages (run clean?)
 	pip install . --no-deps
 
 install-dev: ## install development version (run clean?)
 	pip install -e . --no-deps
+
+
+################################################################################
+# other tools
+################################################################################
+
+# Note that this requires `auto-changelog`, which can be installed with pip(x)
+auto-changelog: ## autogenerate changelog and print to stdout
+	auto-changelog -u -r usnistgov -v unreleased --tag-prefix v --stdout --template changelog.d/templates/auto-changelog/template.jinja2
+
+commitizen-changelog:
+	cz changelog --unreleased-version unreleased --dry-run --incremental
```

### Comparing `cmomy-0.2.2/PKG-INFO` & `cmomy-0.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.2.2
+Version: 0.3.0
 Summary: Central (co)moment calculation/manipulation
 Home-page: https://github.com/usnistgov/cmomy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/usnistgov/cmomy
 Project-URL: documentation, https://pages.nist.gov/cmomy/
 Keywords: cmomy
@@ -18,104 +18,93 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
-License-File: AUTHORS.md
 
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+# cmomy
+
+A Python package to calculate and manipulate Central (co)moments. The main
+features of `cmomy` are as follows:
+
+- [Numba][Numba] accelerated computation of central moments and co-moments
+- Routines to combine, and resample central moments.
+- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
+  Data.
+- Routines to convert between central and raw moments.
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
-
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/ambv/black
 [pypi-badge]: https://img.shields.io/pypi/v/cmomy
+
 <!-- [pypi-badge]: https://badge.fury.io/py/cmomy.svg -->
+
 [pypi-link]: https://pypi.org/project/cmomy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/cmomy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/cmomy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/cmomy
 [conda-link]: https://anaconda.org/wpk-nist/cmomy
 [numpy]: https://numpy.org
 [Numba]: https://numba.pydata.org/
 [xarray]: https://docs.xarray.dev/en/stable/
+
 <!-- Use total link so works from anywhere -->
+
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/cmomy/blob/master/LICENSE
 
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
-<!-- [github-ci]: https://github.com/executablebooks/MyST-Parser/workflows/continuous-integration/badge.svg?branch=master -->
-<!-- [github-link]: https://github.com/executablebooks/MyST-Parser -->
-<!-- [codecov-badge]: https://codecov.io/gh/executablebooks/MyST-Parser/branch/master/graph/badge.svg -->
-<!-- [codecov-link]: https://codecov.io/gh/executablebooks/MyST-Parser -->
-<!-- [rtd-badge]: https://readthedocs.org/projects/myst-parser/badge/?version=latest -->
-<!-- [rtd-link]: https://myst-parser.readthedocs.io/en/latest/?badge=latest -->
-<!-- [pypi-badge]: https://img.shields.io/pypi/v/cmomy -->
-<!-- [conda-badge]: https://anaconda.org/conda-forge/myst-parser/badges/version.svg -->
-<!-- [conda-link]: https://anaconda.org/conda-forge/myst-parser -->
-<!-- [install-badge]: https://img.shields.io/pypi/dw/myst-parser?label=pypi%20installs -->
-<!-- [Install-link]: https://pypistats.org/packages/myst-parser -->
-
-# cmomy
-
-A Python package to calculate and manipulate Central (co)moments. The main features of ``cmomy`` are as follows:
-
-* [Numba][Numba] accelerated computation of central moments and co-moments
-* Routines to combine, and resample central moments.
-* Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
-  Data.
-* Routines to convert between central and raw moments.
-
-
+<!-- For more badges see
+https://shields.io/category/other
+https://naereen.github.io/badges/
+-->
 
 ## Overview
 
-`cmomy` is an open source package to calculate central moments and
-co-moments in a numerical stable and direct way. Behind the scenes,
-`cmomy` makes use of [Numba][Numba] to rapidly
-calculate moments. A good introduction to the type of formulas used can
-be found
+`cmomy` is an open source package to calculate central moments and co-moments in
+a numerical stable and direct way. Behind the scenes, `cmomy` makes use of
+[Numba][Numba] to rapidly calculate moments. A good introduction to the type of
+formulas used can be found
 [here](https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance).
 
-
 ## Features
-* Fast calculation of central moments and central co-moments with weights
-* Support for scalar or vector inputs
-* numpy and xarray api's
-* bootstrap resampling
 
+- Fast calculation of central moments and central co-moments with weights
+- Support for scalar or vector inputs
+- numpy and xarray api's
+- bootstrap resampling
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
-
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 Use one of the following
 
-``` bash
+```bash
 pip install cmomy
 ```
 
 or
 
-``` bash
+```bash
 conda install -c wpk-nist cmomy
 ```
 
-
 ## Example usage
 
 ```python
 import numpy as np
 
 import cmomy
 
@@ -152,65 +141,148 @@
 
 c = cs[0] + cs[1] + cs[2]
 
 c.cmom()
 Out[15]: array([1.    , 0.    , 0.0731, 0.0075])
 ```
 
-
-
 ## Note on caching
 
-This code makes extensive use of the numba python package. This uses a
-jit compiler to speed up vital code sections. This means that the first
-time a function called, it has to compile the underlying code. However,
-caching has been implemented. Therefore, the very first time you run a
-function, it may be slow. But all subsequent uses (including other
-sessions) will be already compiled.
+This code makes extensive use of the numba python package. This uses a jit
+compiler to speed up vital code sections. This means that the first time a
+function called, it has to compile the underlying code. However, caching has
+been implemented. Therefore, the very first time you run a function, it may be
+slow. But all subsequent uses (including other sessions) will be already
+compiled.
 
-A quick way to cache (most all) the [Numba][Numba] functions is to run the tests.  This can be done with
+A quick way to cache (most all) the [Numba][Numba] functions is to run the
+tests. This can be done with
 
-``` bash
+```bash
 conda/mamba/pip install pytest
 
 pytest --pyargs cmomy
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `cmomy` in action.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Related work
 
-This package is used extensively in the newest version of ``thermoextrap``.  See [here](https://github.com/usnistgov/thermo-extrap).
-
+This package is used extensively in the newest version of `thermoextrap`. See
+[here](https://github.com/usnistgov/thermo-extrap).
 
 ## Contact
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
-# History
+# Changelog
+
+Changelog for `cmomy`
+
+## Unreleased
+
+See the fragment files in [changelog.d](https://github.com/usnistgov/cmomy)
+
+<!-- scriv-insert-here -->
+
+## v0.2.2 - 2023-04-05
+
+Full set of changes:
+[`v0.2.1...v0.2.2`](https://github.com/usnistgov/cmomy/compare/v0.2.1...v0.2.2)
+
+## v0.2.1 - 2023-04-05
+
+Full set of changes:
+[`v0.2.0...v0.2.1`](https://github.com/usnistgov/cmomy/compare/v0.2.0...v0.2.1)
+
+## v0.2.0 - 2023-03-22
+
+Full set of changes:
+[`v0.1.9...v0.2.0`](https://github.com/usnistgov/cmomy/compare/v0.1.9...v0.2.0)
+
+## v0.1.9 - 2023-02-15
+
+Full set of changes:
+[`v0.1.8...v0.1.9`](https://github.com/usnistgov/cmomy/compare/v0.1.8...v0.1.9)
+
+## v0.1.8 - 2022-12-02
+
+Full set of changes:
+[`v0.1.7...v0.1.8`](https://github.com/usnistgov/cmomy/compare/v0.1.7...v0.1.8)
+
+## v0.1.7 - 2022-09-28
+
+Full set of changes:
+[`v0.1.6...v0.1.7`](https://github.com/usnistgov/cmomy/compare/v0.1.6...v0.1.7)
+
+## v0.1.6 - 2022-09-27
+
+Full set of changes:
+[`v0.1.5...v0.1.6`](https://github.com/usnistgov/cmomy/compare/v0.1.5...v0.1.6)
+
+## v0.1.5 - 2022-09-26
+
+Full set of changes:
+[`v0.1.4...v0.1.5`](https://github.com/usnistgov/cmomy/compare/v0.1.4...v0.1.5)
+
+## v0.1.4 - 2022-09-15
+
+Full set of changes:
+[`v0.1.3...v0.1.4`](https://github.com/usnistgov/cmomy/compare/v0.1.3...v0.1.4)
+
+## v0.1.3 - 2022-09-15
+
+Full set of changes:
+[`v0.1.2...v0.1.3`](https://github.com/usnistgov/cmomy/compare/v0.1.2...v0.1.3)
+
+## v0.1.2 - 2022-09-13
+
+Full set of changes:
+[`v0.1.1...v0.1.2`](https://github.com/usnistgov/cmomy/compare/v0.1.1...v0.1.2)
+
+## v0.1.1 - 2022-09-13
+
+Full set of changes:
+[`v0.1.0...v0.1.1`](https://github.com/usnistgov/cmomy/compare/v0.1.0...v0.1.1)
+
+## v0.1.0 - 2022-09-13
+
+Full set of changes:
+[`v0.0.7...v0.1.0`](https://github.com/usnistgov/cmomy/compare/v0.0.7...v0.1.0)
+
+## v0.0.7 - 2021-05-18
+
+Full set of changes:
+[`v0.0.6...v0.0.7`](https://github.com/usnistgov/cmomy/compare/v0.0.6...v0.0.7)
+
+## v0.0.6 - 2021-02-03
+
+Full set of changes:
+[`v0.0.4...v0.0.6`](https://github.com/usnistgov/cmomy/compare/v0.0.4...v0.0.6)
 
-## 0.0.5 (2020-12-30)
+## v0.0.4 - 2020-12-21
 
-- First release on PyPI.
+Full set of changes:
+[`v0.0.3...v0.0.4`](https://github.com/usnistgov/cmomy/compare/v0.0.3...v0.0.4)
 
 This software was developed by employees of the National Institute of Standards
 and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
 United States Code Section 105, works of NIST employees are not subject to
 copyright protection in the United States and are considered to be in the public
 domain. Permission to freely use, copy, modify, and distribute this software and
 its documentation without fee is hereby granted, provided that this notice and
```

### Comparing `cmomy-0.2.2/README.md` & `cmomy-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,85 @@
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+# cmomy
+
+A Python package to calculate and manipulate Central (co)moments. The main
+features of `cmomy` are as follows:
+
+- [Numba][Numba] accelerated computation of central moments and co-moments
+- Routines to combine, and resample central moments.
+- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
+  Data.
+- Routines to convert between central and raw moments.
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
-
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/ambv/black
 [pypi-badge]: https://img.shields.io/pypi/v/cmomy
+
 <!-- [pypi-badge]: https://badge.fury.io/py/cmomy.svg -->
+
 [pypi-link]: https://pypi.org/project/cmomy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/cmomy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/cmomy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/cmomy
 [conda-link]: https://anaconda.org/wpk-nist/cmomy
 [numpy]: https://numpy.org
 [Numba]: https://numba.pydata.org/
 [xarray]: https://docs.xarray.dev/en/stable/
+
 <!-- Use total link so works from anywhere -->
+
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/cmomy/blob/master/LICENSE
 
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
-<!-- [github-ci]: https://github.com/executablebooks/MyST-Parser/workflows/continuous-integration/badge.svg?branch=master -->
-<!-- [github-link]: https://github.com/executablebooks/MyST-Parser -->
-<!-- [codecov-badge]: https://codecov.io/gh/executablebooks/MyST-Parser/branch/master/graph/badge.svg -->
-<!-- [codecov-link]: https://codecov.io/gh/executablebooks/MyST-Parser -->
-<!-- [rtd-badge]: https://readthedocs.org/projects/myst-parser/badge/?version=latest -->
-<!-- [rtd-link]: https://myst-parser.readthedocs.io/en/latest/?badge=latest -->
-<!-- [pypi-badge]: https://img.shields.io/pypi/v/cmomy -->
-<!-- [conda-badge]: https://anaconda.org/conda-forge/myst-parser/badges/version.svg -->
-<!-- [conda-link]: https://anaconda.org/conda-forge/myst-parser -->
-<!-- [install-badge]: https://img.shields.io/pypi/dw/myst-parser?label=pypi%20installs -->
-<!-- [Install-link]: https://pypistats.org/packages/myst-parser -->
-
-# cmomy
-
-A Python package to calculate and manipulate Central (co)moments. The main features of ``cmomy`` are as follows:
-
-* [Numba][Numba] accelerated computation of central moments and co-moments
-* Routines to combine, and resample central moments.
-* Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
-  Data.
-* Routines to convert between central and raw moments.
-
-
+<!-- For more badges see
+https://shields.io/category/other
+https://naereen.github.io/badges/
+-->
 
 ## Overview
 
-`cmomy` is an open source package to calculate central moments and
-co-moments in a numerical stable and direct way. Behind the scenes,
-`cmomy` makes use of [Numba][Numba] to rapidly
-calculate moments. A good introduction to the type of formulas used can
-be found
+`cmomy` is an open source package to calculate central moments and co-moments in
+a numerical stable and direct way. Behind the scenes, `cmomy` makes use of
+[Numba][Numba] to rapidly calculate moments. A good introduction to the type of
+formulas used can be found
 [here](https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance).
 
-
 ## Features
-* Fast calculation of central moments and central co-moments with weights
-* Support for scalar or vector inputs
-* numpy and xarray api's
-* bootstrap resampling
 
+- Fast calculation of central moments and central co-moments with weights
+- Support for scalar or vector inputs
+- numpy and xarray api's
+- bootstrap resampling
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
-
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 Use one of the following
 
-``` bash
+```bash
 pip install cmomy
 ```
 
 or
 
-``` bash
+```bash
 conda install -c wpk-nist cmomy
 ```
 
-
 ## Example usage
 
 ```python
 import numpy as np
 
 import cmomy
 
@@ -126,47 +116,46 @@
 
 c = cs[0] + cs[1] + cs[2]
 
 c.cmom()
 Out[15]: array([1.    , 0.    , 0.0731, 0.0075])
 ```
 
-
-
 ## Note on caching
 
-This code makes extensive use of the numba python package. This uses a
-jit compiler to speed up vital code sections. This means that the first
-time a function called, it has to compile the underlying code. However,
-caching has been implemented. Therefore, the very first time you run a
-function, it may be slow. But all subsequent uses (including other
-sessions) will be already compiled.
+This code makes extensive use of the numba python package. This uses a jit
+compiler to speed up vital code sections. This means that the first time a
+function called, it has to compile the underlying code. However, caching has
+been implemented. Therefore, the very first time you run a function, it may be
+slow. But all subsequent uses (including other sessions) will be already
+compiled.
 
-A quick way to cache (most all) the [Numba][Numba] functions is to run the tests.  This can be done with
+A quick way to cache (most all) the [Numba][Numba] functions is to run the
+tests. This can be done with
 
-``` bash
+```bash
 conda/mamba/pip install pytest
 
 pytest --pyargs cmomy
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `cmomy` in action.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Related work
 
-This package is used extensively in the newest version of ``thermoextrap``.  See [here](https://github.com/usnistgov/thermo-extrap).
-
+This package is used extensively in the newest version of `thermoextrap`. See
+[here](https://github.com/usnistgov/thermo-extrap).
 
 ## Contact
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
```

### Comparing `cmomy-0.2.2/commands.sh` & `cmomy-0.3.0/commands.sh`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/Makefile` & `cmomy-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/_static/css/nist-combined.css` & `cmomy-0.3.0/docs/_static/css/nist-combined.css`

 * *Files 13% similar despite different names*

```diff
@@ -2,168 +2,168 @@
  * @file
  * Header and Footer styles
  *
  */
 
 /* Header Styles */
 .nist-header {
-  background: #000;
-  font-family: Helvetica, Arial, sans-serif;
-  padding: 10px 16px 0;
-  font-size: 16px;
+    background: #000;
+    font-family: Helvetica, Arial, sans-serif;
+    padding: 10px 16px 0;
+    font-size: 16px;
 }
 
 .nist-header__logo-link {
-  display: inline-block;
-  height: 35px;
+    display: inline-block;
+    height: 35px;
 }
 
 /* For Bootstrap Users - Updated the vertical align property since it interfered with NIST SVG icon. */
 .nist-header__logo-link svg {
-  vertical-align: inherit;
+    vertical-align: inherit;
 }
 
 .nist-header__logo-icon {
-  fill: #fff;
-  display: inline-block;
-  height: 16px;
-  position: relative;
-  top: -2px;
-  margin-right: 2px;
+    fill: #fff;
+    display: inline-block;
+    height: 16px;
+    position: relative;
+    top: -2px;
+    margin-right: 2px;
 }
 
 .nist-header__logo-image {
-  fill: #fff;
-  display: inline-block;
-  height: 24px;
-  width: 90px;
+    fill: #fff;
+    display: inline-block;
+    height: 24px;
+    width: 90px;
 }
 
 /* Limit main content area width */
 .nist-main {
-  margin-left: auto;
-  margin-right: auto;
-  max-width: 1200px;
-  padding: 0 16px;
-  box-sizing: border-box;
+    margin-left: auto;
+    margin-right: auto;
+    max-width: 1200px;
+    padding: 0 16px;
+    box-sizing: border-box;
 }
 
 /* Make sure body has no margin or padding when using only this header component */
 body {
-  padding: 0;
-  margin: 0;
+    padding: 0;
+    margin: 0;
 }
 
 /* Footer styles */
 
 .nist-footer {
-  background: #333333;
-  position: relative;
-  z-index: 200;
-  font-family: Helvetica, Arial, sans-serif;
-  font-size: 16px;
-  box-sizing: border-box;
+    background: #333333;
+    position: relative;
+    z-index: 200;
+    font-family: Helvetica, Arial, sans-serif;
+    font-size: 16px;
+    box-sizing: border-box;
 }
 
 .nist-footer__inner {
-  margin-left: auto;
-  margin-right: auto;
-  max-width: 1200px;
-  padding: 0 16px;
+    margin-left: auto;
+    margin-right: auto;
+    max-width: 1200px;
+    padding: 0 16px;
 }
 
 .nist-footer__inner:after {
-  content: "";
-  display: table;
-  clear: both;
+    content: "";
+    display: table;
+    clear: both;
 }
 
 .nist-footer {
-  background: #333333;
-  color: white;
-  padding: 40px 0px;
-  position: relative;
+    background: #333333;
+    color: white;
+    padding: 40px 0px;
+    position: relative;
 }
 
 .nist-footer a {
-  color: white;
-  text-decoration: none;
+    color: white;
+    text-decoration: none;
 }
 
 .nist-footer .nist-footer__logo img {
-  width: 340px;
-  display: block;
-  margin-left: auto;
-  margin-right: auto;
-  margin-top: 30px;
+    width: 340px;
+    display: block;
+    margin-left: auto;
+    margin-right: auto;
+    margin-top: 30px;
 }
 
 .nist-footer__logo {
-  display: flex;
-  justify-content: center;
-  align-items: center;
+    display: flex;
+    justify-content: center;
+    align-items: center;
 }
 
 .nist-footer__menu {
-  clear: both;
-  margin-bottom: 10px;
+    clear: both;
+    margin-bottom: 10px;
 }
 
 .nist-footer__menu.first {
-  padding-top: 20px;
+    padding-top: 20px;
 }
 
 .nist-footer__menu ul {
-  margin: 0;
-  padding: 0;
-  list-style: none;
-  text-align: center;
+    margin: 0;
+    padding: 0;
+    list-style: none;
+    text-align: center;
 }
 
 .nist-footer__menu-item {
-  display: inline-block;
-  font-size: 14px;
-  padding: 0;
-  margin-left: 0;
+    display: inline-block;
+    font-size: 14px;
+    padding: 0;
+    margin-left: 0;
 }
 
 .nist-footer__menu-item:after {
-  content: '|';
-  margin-right: 1.6px;
-  display: inherit;
-  position: static;
-  font: inherit;
-  line-height: inherit;
-  color: inherit;
+    content: "|";
+    margin-right: 1.6px;
+    display: inherit;
+    position: static;
+    font: inherit;
+    line-height: inherit;
+    color: inherit;
 }
 
 .nist-footer__menu-item:last-child:after {
-  content: none;
+    content: none;
 }
 
 .nist-footer__menu-item a {
-  font-weight: normal;
-  margin-right: 6px;
-  white-space: nowrap;
-  padding: 0.5em 0;
-  display: inline-block;
+    font-weight: normal;
+    margin-right: 6px;
+    white-space: nowrap;
+    padding: 0.5em 0;
+    display: inline-block;
 }
 
 /**
  * Stick footer to bottom of page
  * Source: https://css-tricks.com/couple-takes-sticky-footer/
  */
 
 html.nist-footer-bottom,
 html.nist-footer-bottom body {
-  height: 100%;
+    height: 100%;
 }
 html.nist-footer-bottom body {
-  display: flex;
-  flex-direction: column;
+    display: flex;
+    flex-direction: column;
 }
 html.nist-footer-bottom #main {
-  flex: 1 0 auto;
+    flex: 1 0 auto;
 }
 html.nist-footer-bottom .nist-footer {
-  flex-shrink: 0;
+    flex-shrink: 0;
 }
```

### Comparing `cmomy-0.2.2/docs/_static/js/nist-header-footer.js` & `cmomy-0.3.0/docs/_static/js/nist-header-footer.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,27 @@
 /**
  * @file
  * Header and footer scripts
  *
  */
 
 $(document).ready(function() {
-
     $("body").prepend('<div id="nistheadergoeshere"></div>');
     $.ajax({
         url: "https://pages.nist.gov/nist-header-footer/boilerplate-header.html",
         cache: false,
         dataType: "html",
         success: function(data) {
-            $('#nistheadergoeshere').append(data);
+            $("#nistheadergoeshere").append(data);
         },
     });
 
     $("body").append('<div id="nistfootergoeshere"></div>');
     $.ajax({
         url: "https://pages.nist.gov/nist-header-footer/boilerplate-footer.html",
         cache: false,
         dataType: "html",
         success: function(data) {
-            $('#nistfootergoeshere').append(data);
+            $("#nistfootergoeshere").append(data);
         },
     });
-
 });
```

### Comparing `cmomy-0.2.2/docs/_templates/autosummary/class.rst` & `cmomy-0.3.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/_templates/autosummary/module.rst` & `cmomy-0.3.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/_templates/class-individual-pages.rst` & `cmomy-0.3.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/_templates/module-custom.rst` & `cmomy-0.3.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/_templates/module-single.rst` & `cmomy-0.3.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/_templates/module-template.rst` & `cmomy-0.3.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/conf.py` & `cmomy-0.3.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
+"""Build docs."""
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
 import cmomy
 
@@ -119,15 +120,15 @@
 # set github_username variable to be subbed later.
 # this makes it easy to switch from wpk -> usnistgov later
 github_username = "usnistgov"
 
 html_context = {
     "github_user": "usnistgov",
     "github_repo": "cmomy",
-    "github_version": "master",
+    "github_version": "main",
     "doc_path": "docs",
 }
 
 # -- python3 ---------------------------------------------------------------
 autosummary_generate = True
 # autosummary_generate = False
 autodoc_member_order = "bysource"
@@ -275,23 +276,23 @@
 #
 
 html_theme = "sphinx_book_theme"
 
 html_theme_options = dict(
     # analytics_id=''  this is configured in rtfd.io
     # canonical_url="",
-    repository_url="https://github.com/usnistgov/cmomy",
+    repository_url=f"https://github.com/{github_username}/cmomy",
     repository_branch=html_context["github_version"],
     path_to_docs=html_context["doc_path"],
     # use_edit_page_button=True,
     use_repository_button=True,
     use_issues_button=True,
     home_page_in_toc=True,
-    show_toc_level=6,
-    show_navbar_depth=2,
+    show_toc_level=2,
+    show_navbar_depth=0,
 )
 # handle nist css/js from here.
 html_css_files = [
     # "css/nist-combined.css",
     "https://pages.nist.gov/nist-header-footer/css/nist-combined.css",
     "https://pages.nist.gov/leaveNotice/css/jquery.leaveNotice.css",
 ]
@@ -416,35 +417,36 @@
     "sparse": ("https://sparse.pydata.org/en/latest/", None),
     "xarray": ("https://docs.xarray.dev/en/stable/", None),
 }
 
 
 # based on numpy doc/source/conf.py
 def linkcode_resolve(domain, info):
-    """
-    Determine the URL corresponding to Python object
-    """
+    """Determine the URL corresponding to Python object"""
     import inspect
+    from operator import attrgetter
 
     if domain != "py":
         return None
 
-    modname = info["module"]
-    fullname = info["fullname"]
+    parent_name, *sub_parts = info["module"].split(".")
+    parent_mod = sys.modules.get(parent_name)
 
-    submod = sys.modules.get(modname)
-    if submod is None:
-        return None
+    try:
+        if len(sub_parts) > 0:
+            sub_name = ".".join(sub_parts)
+            obj = attrgetter(sub_name)(parent_mod)
+        else:
+            obj = parent_mod
 
-    obj = submod
-    for part in fullname.split("."):
-        try:
-            obj = getattr(obj, part)
-        except AttributeError:
-            return None
+        # get fullname
+        obj = attrgetter(info["fullname"])(obj)
+
+    except AttributeError:
+        return None
 
     try:
         fn = inspect.getsourcefile(inspect.unwrap(obj))
     except TypeError:
         fn = None
     if not fn:
         return None
```

### Comparing `cmomy-0.2.2/docs/example.md` & `cmomy-0.3.0/docs/example_for_readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 <!-- jupytext: -->
 <!--   text_representation: -->
 <!--     format_name: myst -->
 <!-- kernelspec: -->
 <!--   display_name: Python 3 -->
 <!--   name: python3 -->
 <!-- --- -->
-
-
 # Example usage
 
-
 ```{eval-rst}
 .. ipython:: python
     :suppress:
 
     import numpy as np
 
     np.set_printoptions(precision=4)
@@ -46,19 +43,7 @@
     cs = [cmomy.CentralMoments.from_vals(_, mom=3) for _ in (x0, x1, x2)]
 
     c = cs[0] + cs[1] + cs[2]
 
     c.cmom()
 
 ```
-
-<!-- ```{code-cell} ipython3 -->
-<!-- b = 2 -->
-<!-- print('b value', b) -->
-<!-- ``` -->
-
-<!-- ```python -->
-<!-- import numpy as np -->
-
-<!-- for x in [1, 2, 3]: -->
-<!--     pass -->
-<!-- ``` -->
```

### Comparing `cmomy-0.2.2/docs/make.bat` & `cmomy-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/docs/notebooks/motivation.ipynb` & `cmomy-0.3.0/docs/examples/usage/motivation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999489728108149%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(1, \'    """Create central moments using stable '*

 * *            'method"""\\n\')], delete: [3, 2, 1]}}, 28: {\'source\': {insert: [(1, \'    """Create '*

 * *            'central moments using stable method"""\\n\')], delete: [1]}}}'}*

```diff
@@ -41,17 +41,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "id": "f3d00a97",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def cmom_1(x, axis=0, mom=3):\n",
-                "    \"\"\"\n",
-                "    create central moments using stable method\n",
-                "    \"\"\"\n",
+                "    \"\"\"Create central moments using stable method\"\"\"\n",
                 "    # output shape\n",
                 "    shape = x.shape[:axis] + x.shape[axis + 1 :] + (mom + 1,)\n",
                 "    output = np.zeros(shape, dtype=x.dtype)\n",
                 "\n",
                 "    output[..., 0] = x.shape[axis]\n",
                 "    output[..., 1] = x.mean(axis=axis)\n",
                 "\n",
@@ -2379,15 +2377,15 @@
             "cell_type": "code",
             "execution_count": 30,
             "id": "b2ed66e7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def get_cmom_with_weights(x, w, axis=0, mom=3):\n",
-                "    \"\"\"create central moments using stable method\"\"\"\n",
+                "    \"\"\"Create central moments using stable method\"\"\"\n",
                 "    # output shape\n",
                 "    shape = x.shape[:axis] + x.shape[axis + 1 :] + (mom + 1,)\n",
                 "    output = np.zeros(shape, dtype=x.dtype)\n",
                 "\n",
                 "    w_sum = w.sum(axis=axis)\n",
                 "    w_norm = 1.0 / w_sum\n",
                 "\n",
```

### Comparing `cmomy-0.2.2/docs/notebooks/usage_notebook.ipynb` & `cmomy-0.3.0/docs/examples/usage/usage_notebook.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999771062271062%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'import cmomy\\n')], delete: [2]}}}"}*

```diff
@@ -1545,17 +1545,17 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import numpy as np\n",
                 "import xarray as xr\n",
-                "import cmomy\n",
                 "from IPython.display import display\n",
                 "\n",
+                "import cmomy\n",
                 "\n",
                 "np.random.seed(0)\n",
                 "\n",
                 "nsamp = 100\n",
                 "energy = xr.DataArray(np.random.rand(nsamp), dims=[\"samp\"])\n",
                 "\n",
                 "position = xr.DataArray(np.random.rand(nsamp, 3), dims=[\"samp\", \"dim\"])\n",
```

### Comparing `cmomy-0.2.2/environment/dev-extras.yaml` & `cmomy-0.3.0/environment/dev-extras.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 dependencies:
-    # numerics/tests
-    # - matplotlib
-    # - pandas
-    # development
-    # - isort
-    # - black
-    # - blackdoc
-    # - flake8
-    # testing
-    - pytest
-    - pytest-cov
-    - pytest-xdist
-    # - tox-conda
-    # specials
-    # - pre-commit
-    # repl
-    - ipython
-    - ipykernel
-    # build
-    - setuptools-scm
-    # - setuptools
-    # - twine
-    # - setuptools_scm_git_archive
-    # - build
-    # conda specific
-    # - conda-build
-    # - anaconda-client
-    # - greyskull
-    # doc stuff
-    # - sphinx
-    # - sphinx_rtd_theme
-    # - recommonmark # if want markdown
-    # - nbsphinx # if want notebooks
-    # - sphinxcontrib-spelling
-    # - sphinx-toolbox
-    # lsp stuff
-    # - autoflake
-    # - pyls-mypy
-    # - pyls-black
-    # - pyls-isort
-    # mypy
-    # - mypy
-    # - pytest-mypy
-    # # Monkeytype: autocreate type hints
-    # - MonkeyType
-    - pip
-    - pip:
-        - pytest-accept
-        # - mypy-extensions
-        # - pytest-monkeytype
-        # - flake8-mypy
-        # - attr-utils
-        # spelling?
-        # - pyenchant
+  # numerics/tests
+  # - matplotlib
+  # - pandas
+  # development
+  # - isort
+  # - black
+  # - blackdoc
+  # - flake8
+  # testing
+  - pytest
+  - pytest-cov
+  - pytest-xdist
+  # - tox-conda
+  # specials
+  # - pre-commit
+  # repl
+  - ipython
+  - ipykernel
+  # build
+  - setuptools-scm
+  # - setuptools
+  # - twine
+  # - setuptools_scm_git_archive
+  # - build
+  # conda specific
+  # - conda-build
+  # - anaconda-client
+  # - greyskull
+  # doc stuff
+  # - sphinx
+  # - sphinx_rtd_theme
+  # - recommonmark # if want markdown
+  # - nbsphinx # if want notebooks
+  # - sphinxcontrib-spelling
+  # - sphinx-toolbox
+  # lsp stuff
+  # - autoflake
+  # - pyls-mypy
+  # - pyls-black
+  # - pyls-isort
+  # mypy
+  # - mypy
+  # - pytest-mypy
+  # # Monkeytype: autocreate type hints
+  # - MonkeyType
+  - pip
+  - pip:
+      - pytest-accept
+      # - mypy-extensions
+      # - pytest-monkeytype
+      # - flake8-mypy
+      # - attr-utils
+      # spelling?
+      # - pyenchant
```

### Comparing `cmomy-0.2.2/environment/docs-extras.yaml` & `cmomy-0.3.0/environment/docs-extras.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 channels:
   - conda-forge
 dependencies:
-    - setuptools-scm
-    - ipython
-    ## package deps
-    # - matplotlib
-    # - pandas
-    - pip
-    - pip:
-        - pyenchant
-        # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
-        - ghp-import
-        - sphinx
-        ## themes
-        - sphinx-book-theme
-        ## error with == 0.13.3
-        - pydata-sphinx-theme==0.13.1
-        ## optionals
-        # sphinx-design
-        - sphinx-copybutton
-        - sphinxcontrib-spelling
-        # sphinxext-rediraffe
-        ## autobuild
-        - sphinx-autobuild
-        ## myst
-        # myst-parser
-        - myst-nb
-        ## others
-        - autodocsumm
+  - setuptools-scm
+  - ipython
+  ## package deps
+  # - matplotlib
+  # - pandas
+  - pip
+  - pip:
+      - pyenchant
+      # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
+      - ghp-import
+      - sphinx
+      ## themes
+      - sphinx-book-theme
+      ## error with == 0.13.3
+      - pydata-sphinx-theme==0.13.1
+      ## optionals
+      # sphinx-design
+      - sphinx-copybutton
+      - sphinxcontrib-spelling
+      # sphinxext-rediraffe
+      ## autobuild
+      - sphinx-autobuild
+      ## myst
+      # myst-parser
+      - myst-nb
+      ## others
+      - autodocsumm
```

### Comparing `cmomy-0.2.2/examples/bootstrap.ipynb` & `cmomy-0.3.0/examples/archived/bootstrap.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998217093441151%*

 * *Differences: {"'cells'": "{0: {'source': {delete: [1]}}, 5: {'source': {insert: [(1, '\\n')]}}, 19: {'source': "*

 * *            "{insert: [(232, '                _w * f\\n'), (259, '                _w * f\\n')], "*

 * *            "delete: [259, 232]}}, 20: {'source': {insert: [(1, '\\n'), (2, '\\n')]}}, 21: "*

 * *            "{'source': {insert: [(1, '\\n')]}}, 26: {'source': {insert: [(3, '\\n'), (16, '# "*

 * *            "np.testing.assert_allclose(out, out2)')], delete: [17, 16, 3]}}, 68: {'source': "*

 * *            '{insert: [(1, \'  […]*

```diff
@@ -3,15 +3,14 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib inline\n",
-                "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "from numba import njit"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
@@ -153,14 +152,15 @@
                     "execution_count": 40,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from importlib import reload\n",
+                "\n",
                 "import accumulator as acc\n",
                 "\n",
                 "reload(acc)"
             ]
         },
         {
             "cell_type": "code",
@@ -574,15 +574,15 @@
                 "                continue\n",
                 "            for imeta in range(nmeta):\n",
                 "                _w = data[idat, imeta, 0]\n",
                 "                if _w == 0.0:\n",
                 "                    continue\n",
                 "                a = data[idat, imeta, 1]\n",
                 "                v = data[idat, imeta, 2]\n",
-                "                w = _w * f\n",
+                "                _w * f\n",
                 "                _push_stat(out[irep, imeta], _w * f, a, v)\n",
                 "\n",
                 "    return out\n",
                 "\n",
                 "\n",
                 "@njit(parallel=True)\n",
                 "def _resample_2d(data, freq):\n",
@@ -601,27 +601,29 @@
                 "                continue\n",
                 "            for imeta in range(nmeta):\n",
                 "                _w = data[idat, imeta, 0]\n",
                 "                if _w == 0.0:\n",
                 "                    continue\n",
                 "                a = data[idat, imeta, 1]\n",
                 "                v = data[idat, imeta, 2]\n",
-                "                w = _w * f\n",
+                "                _w * f\n",
                 "                acc._push_stat(out[irep, imeta], _w * f, a, v)\n",
                 "\n",
                 "    return out"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 165,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# this seems to be the best one by far.\n",
+                "\n",
+                "\n",
                 "@njit(parallel=True)\n",
                 "def _resample_2b(data, freq):\n",
                 "    ndata = data.shape[0]\n",
                 "    nmeta = data.shape[1]\n",
                 "\n",
                 "    ndat = freq.shape[0]\n",
                 "    nrep = freq.shape[1]\n",
@@ -661,14 +663,15 @@
             "cell_type": "code",
             "execution_count": 168,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# out2 = np.zeros_like(out)\n",
                 "\n",
+                "\n",
                 "out2 = _resample_2b(s.data, freq)\n",
                 "\n",
                 "np.testing.assert_allclose(out, out2)"
             ]
         },
         {
             "cell_type": "code",
@@ -742,29 +745,28 @@
                     ]
                 }
             ],
             "source": [
                 "for func in [_resample_2b, _resample_2b2, _resample_2c, _resample_2d]:\n",
                 "    out2 = func(s.data, freq)\n",
                 "    np.testing.assert_allclose(out, out2)\n",
-                "    \n",
+                "\n",
                 "    %timeit -n 5 -r 3 func(s.data, freq)\n",
                 "\n",
                 "# out2 = _resample_2b(s.data, freq)\n",
                 "# np.testing.assert_allclose(out, out2)\n",
                 "\n",
                 "# out2 = _resample_2b2(s.data, freq)\n",
                 "# np.testing.assert_allclose(out, out2)\n",
                 "\n",
                 "# out2 = _resample_2c(s.data, freq)\n",
                 "# np.testing.assert_allclose(out, out2)\n",
                 "\n",
                 "# out2 = _resample_2d(s.data, freq)\n",
-                "# np.testing.assert_allclose(out, out2)\n",
-                "\n"
+                "# np.testing.assert_allclose(out, out2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 405,
             "metadata": {},
             "outputs": [
@@ -1963,17 +1965,15 @@
         {
             "cell_type": "code",
             "execution_count": 21,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def resample_data(data, freq, out=None):\n",
-                "    \"\"\"\n",
-                "    reduce data along axis=0 from freq table\n",
-                "    \"\"\"\n",
+                "    \"\"\"Reduce data along axis=0 from freq table\"\"\"\n",
                 "    data_shape = data.shape\n",
                 "    assert data_shape[-1] == 3\n",
                 "\n",
                 "    ndim = data.ndim\n",
                 "    assert ndim > 1\n",
                 "\n",
                 "    assert data_shape[0] == freq.shape[0]\n",
```

### Comparing `cmomy-0.2.2/examples/central_moments.ipynb` & `cmomy-0.3.0/examples/archived/central_moments.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998641304347826%*

 * *Differences: {"'cells'": "{0: {'source': ['# import xarray as xr']}, 1: {'source': ['from importlib import "*

 * *            "reload\\n', '\\n', 'import numpy as np']}, 2: {'source': {insert: [(0, 'import "*

 * *            "cmomy.accumulator as accumulator\\n'), (1, 'import cmomy.accumulator_central as "*

 * *            "accumulator_central\\n')], delete: [0]}}}"}*

```diff
@@ -2,26 +2,26 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# import xarray as xr\n",
-                "import numpy as np"
+                "# import xarray as xr"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import cmomy.accumulator as accumulator\n",
-                "import cmomy.accumulator_central as accumulator_central"
+                "from importlib import reload\n",
+                "\n",
+                "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
@@ -33,15 +33,16 @@
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from importlib import reload\n",
+                "import cmomy.accumulator as accumulator\n",
+                "import cmomy.accumulator_central as accumulator_central\n",
                 "\n",
                 "reload(accumulator)\n",
                 "reload(accumulator_central)"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `cmomy-0.2.2/examples/example_usage.ipynb` & `cmomy-0.3.0/examples/archived/example_usage.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999826388888889%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import scipy.stats\\n'), (3, 'import cmomy')], delete: "*

 * *            '[3, 1]}}}'}*

```diff
@@ -10,17 +10,17 @@
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "import cmomy\n",
+                "import scipy.stats\n",
                 "\n",
-                "import scipy.stats"
+                "import cmomy"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
```

### Comparing `cmomy-0.2.2/examples/parallel_test.ipynb` & `cmomy-0.3.0/examples/archived/parallel_test.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955408653846154%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, 'from importlib import reload\\n'), (4, 'import numpy as "*

 * *            "np')], delete: [5, 4, 0]}}, 16: {'source': {insert: [(1, 'from numba import jit, "*

 * *            "njit, prange\\n')], delete: [1]}}, delete: [0]}"}*

```diff
@@ -1,30 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import numba"
-            ]
-        },
-        {
-            "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numpy as np\n",
+                "from importlib import reload\n",
                 "\n",
                 "import accumulator as Accum\n",
                 "import accumulator2 as Accum2\n",
-                "\n",
-                "from importlib import reload"
+                "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
@@ -278,15 +268,15 @@
         {
             "cell_type": "code",
             "execution_count": 41,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# numba\n",
-                "from numba import njit, prange, jit\n",
+                "from numba import jit, njit, prange\n",
                 "\n",
                 "_PARALLEL = True\n",
                 "\n",
                 "\n",
                 "@njit(parallel=True)\n",
                 "def _push_vals_vec(data, W, X):\n",
                 "    nmeta = data.shape[0]\n",
```

### Comparing `cmomy-0.2.2/examples/test_accumulator.ipynb` & `cmomy-0.3.0/examples/archived/test_accumulator.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987746766507828%*

 * *Differences: {"'cells'": "{0: {'source': ['from importlib import reload\\n', '\\n', 'import accumulator as "*

 * *            "Accum\\n', 'import numpy as np\\n', 'from numba import njit']}, 78: {'source': "*

 * *            "{insert: [(2, '    np.zeros((a.shape[0],) * 2)\\n')], delete: [2]}}, delete: [0]}"}*

```diff
@@ -1,30 +1,23 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numpy as np\n",
+                "from importlib import reload\n",
+                "\n",
                 "import accumulator as Accum\n",
+                "import numpy as np\n",
                 "from numba import njit"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 2,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from importlib import reload"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Scalar data"
             ]
         },
         {
@@ -1163,15 +1156,15 @@
             "cell_type": "code",
             "execution_count": 75,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def get_cov(a, ns):\n",
                 "    ave = np.nanmean(a, axis=1)\n",
-                "    ave_ij = np.zeros((a.shape[0],) * 2)\n",
+                "    np.zeros((a.shape[0],) * 2)\n",
                 "\n",
                 "    cov = np.zeros((a.shape[0],) * 2)\n",
                 "    cnt = np.zeros_like(cov)\n",
                 "    for var0 in range(a.shape[0]):\n",
                 "        for var1 in range(a.shape[0]):\n",
                 "            s = (a[var0, :] - ave[var0]) * (a[var1, :] - ave[var1])\n",
                 "            cnt[var0, var1] = np.isfinite(s).sum()\n",
```

### Comparing `cmomy-0.2.2/pyproject.toml` & `cmomy-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 [build-system]
-requires = [
-    "setuptools>=61.2",
-    "setuptools_scm[toml]>=7.0",
-]
+requires = ["setuptools>=61.2", "setuptools_scm[toml]>=7.0"]
 build-backend = "setuptools.build_meta"
 
-
 [project]
 name = "cmomy"
-authors = [{name = "William P. Krekelberg", email = "wpk@nist.gov"}]
-license = {text = "NIST license"}
+authors = [{ name = "William P. Krekelberg", email = "wpk@nist.gov" }]
+license = { text = "NIST license" }
 description = "Central (co)moment calculation/manipulation"
 # if using markdown
 # long_description_content_type = text/markdown
 keywords = ["cmomy"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
@@ -37,34 +33,37 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/usnistgov/cmomy"
 documentation = "https://pages.nist.gov/cmomy/"
 
 [project.optional-dependencies]
-test = [
-    "pytest",
-]
+test = ["pytest"]
+
 # dev = []
 # docs = []
-
 ## Defer this to setup.cfg
 ## Will transition when everything works (grayskull in particular)
 ## and will remove setup.py
 # [tool.setuptools]
 # zip-safe = true # if using mypy, must be False
 # include-package-data = true
 # license-files = ["LICENSE"]
-
 # [tool.setuptools.packages.find]
 # namespaces = true
 # where = ["src"]
-
+## include = []
+## exclude = []
+##
 [tool.setuptools.dynamic]
-readme = {file = ["README.md", "HISTORY.md", "LICENSE"], content-type = "text/markdown"}
+readme = { file = [
+    "README.md",
+    "CHANGELOG.md",
+    "LICENSE"
+], content-type = "text/markdown" }
 
 [tool.setuptools_scm]
 fallback_version = "999"
 
 [tool.aliases]
 test = "pytest"
 
@@ -73,53 +72,51 @@
 testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["cmomy"]
 
-
 [tool.ruff]
+fix = true
 line-length = 88
 update-check = false
 target-version = "py38"
-
 select = [
-  # pyflakes
-  "F",
-  # pycodestyle
-  "E",
-  "W",
-  # isort
-  "I",
-  # pyupgrade
-  "UP",
-  # # flake8-2020
-  # "YTT",
-  # # flake8-bugbear
-  # "B",
-  # # flake8-quotes
-  # "Q",
-  # # pylint
-  # "PLE", "PLR", "PLW",
-  # # misc lints
-  # "PIE",
-  # # tidy imports
-  # "TID",
-  # # implicit string concatenation
-  # "ISC",
-  # # type-checking imports
-  # "TCH",
+    # pyflakes
+    "F",
+    # pycodestyle
+    "E",
+    "W",
+    # isort
+    "I",
+    # pyupgrade
+    "UP",
+    # pydocstyle
+    "D",
+    # # flake8-2020
+    "YTT",
+    # # flake8-bugbear
+    # "B",
+    # flake8-quotes
+    "Q",
+    # # pylint
+    # "PLE", "PLR", "PLW",
+    # # misc lints
+    "PIE",
+    # # tidy imports
+    "TID",
+    # # implicit string concatenation
+    # "ISC",
+    # # type-checking imports
+    "TCH",
 ]
-
-
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 # fixable = ["A", "B", "C", "D", "E", "F", "..."]
 unfixable = []
-
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
@@ -134,18 +131,17 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "tests/",
     "src/cmomy/tests",
 ]
-
-
 ignore = [
     # # whitespace before ':' - doesn't work well with black
     # "E203",
     # module level import not at top of file
     "E402",
     # line too long - let black worry about that
     "E501",
@@ -166,50 +162,81 @@
     "D103",
     # these are useful, but too many errors
     # due to use of docfiller
     "D417",
     "D107",
     "D203",
     "D212",
+    # Allow relative imports
+    "TID252",
 ]
-
-per-file-ignores = {}
-
+per-file-ignores = {  }
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.isort]
 known-first-party = ["cmomy"]
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
-[tool.cruft]
+[tool.nbqa.addopts]
+ruff = ["--fix", "--extend-ignore=D100,B018"]
+
+[tool.flake8]
+docstring-convention = "numpy"
+ignore = [
+    # # whitespace before ':' - doesn't work well with black
+    "E203",
+    # module level import not at top of file
+    "E402",
+    # line too long - let black worry about that
+    "E501",
+    # do not assign a lambda expression, use a def
+    "E731",
+    # # line break before binary operator
+    "W503",
+    # allow black line after docstring
+    "D202",
+    "D105",
+    "D205",
+    # this leads to errors with placing titles in module
+    # docstrings
+    "D400",
+    "D401",
+    "D415",
+    "D102",
+    "D103",
+    # these are useful, but too many errors
+    # due to use of docfiller
+    "D417",
+    "D107",
+    "D203",
+    "D212",
+]
 
+[tool.scriv]
+format = "md"
+md_header_level = "2"
+new_fragment_template = "file: changelog.d/templates/new_fragment.md.j2"
+
+[tool.commitizen]
+use_shortcuts = true
+
+[tool.cruft]
 
 [tool.mypy]
 files = ["src/cmomy"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
-exclude = [
-    ".eggs",
-    ".tox",
-    "doc",
-    "docs",
-]
+exclude = [".eggs", ".tox", "doc", "docs"]
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
-module = [
-       "numpy.*",
-       "pandas.*",
-       "pytest.*",
-       "scipy.*",
-       "setuptools",
-]
+module = []
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 module = []
```

### Comparing `cmomy-0.2.2/src/cmomy/__init__.py` & `cmomy-0.3.0/src/cmomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/_docfiller/docfiller.py` & `cmomy-0.3.0/src/cmomy/_docfiller/docfiller.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/_docfiller/docscrape.py` & `cmomy-0.3.0/src/cmomy/_docfiller/docscrape.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/_docstrings.py` & `cmomy-0.3.0/src/cmomy/_docstrings.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     to resamples values.  See :func:`~cmomy.resample.randsamp_freq`
 indices : array of int, optional
     Array of shape ``(nrep, size)``.  If passed, create `freq` from indices.
     See :func:`~cmomy.resample.randsamp_freq`.
 nrep : int, optional
     Number of replicates.  Create `freq` with this many replicates.
     See :func:`~cmomy.resample.randsamp_freq`
-pushed : same as object
+pushed : object
     Same as object, with new data pushed onto `self.data`
 resample_kws : mapping
     Extra arguments to :func:`~cmomy.resample.resample_vals`
 full_output : bool, optional
     If True, also return `freq` array
 convert_kws : mapping
     Extra arguments to :func:`~cmomy.convert.to_central_moments` or :func:`~cmomy.convert.to_central_comoments`
```

### Comparing `cmomy-0.2.2/src/cmomy/_formatting.py` & `cmomy-0.3.0/src/cmomy/_formatting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """pretty formatting for notebook."""
 
 from functools import partial
 
 from xarray.core import formatting as ff
 from xarray.core import formatting_html as fm
 
+if hasattr(ff, "short_array_repr"):
+    short_numpy_repr = ff.short_array_repr
+elif hasattr(ff, "short_numpy_repr"):
+    short_numpy_repr = ff.short_numpy_repr
+else:
+    short_numpy_rerp = repr
+
 
 def tuple_to_str(x):
     """Convert tuple to a string."""
     if len(x) == 0:
         return "*empty*"
 
     out = ", ".join(map(str, x))
@@ -36,15 +43,15 @@
         "checked"
         if fm._get_boolean_with_default("display_expand_data", default=True)
         else ""
     )
     preview = fm.escape(ff.format_array_flat(x, max_width=70))
 
     # short data repr
-    text = fm.escape(ff.short_numpy_repr(x))
+    text = fm.escape(short_numpy_repr(x))
     data_repr = f"<pre>{text}</pre>"
     data_icon = fm._icon("icon-database")
 
     return (
         "<div class='xr-array-wrap'>"
         f"<input id='{data_id}' class='xr-array-in' type='checkbox' {collapsed}>"
         f"<label for='{data_id}' title='Show/hide data repr'>{data_icon}</label>"
```

### Comparing `cmomy-0.2.2/src/cmomy/_resample.py` & `cmomy-0.3.0/src/cmomy/_resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/_testing.py` & `cmomy-0.3.0/src/cmomy/_testing.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/_typing.py` & `cmomy-0.3.0/src/cmomy/_typing.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/abstract_central.py` & `cmomy-0.3.0/src/cmomy/abstract_central.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 """Base class for central moments calculations."""
 
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Literal,
     Mapping,
     Tuple,
     Union,
     cast,
     no_type_check,
 )
 
 import numpy as np
-import xarray as xr
 from custom_inherit import DocInheritMeta
 from numpy.core.numeric import normalize_axis_index  # type: ignore
-from numpy.typing import ArrayLike, DTypeLike
 
 from . import convert
 from ._docstrings import docfiller_shared
 from ._formatting import repr_html
 from ._typing import Moments, T_Array, T_CentralMoments
 from .cached_decorators import gcached
 from .options import DOC_SUB
 from .pushers import factory_pushers
 
+if TYPE_CHECKING:
+    import xarray as xr
+    from numpy.typing import ArrayLike, DTypeLike
+
 # * TODO Main
 # TODO: Total rework is called for to handle typing correctly.
 
 
 def _get_metaclass():
     if DOC_SUB:
         return DocInheritMeta(style="numpy_with_merge")
@@ -104,15 +107,14 @@
         """
         return cast(np.ndarray, self._data)
 
     @property
     @abstractmethod
     def values(self) -> T_Array:
         """Access underlying central moments array."""
-        pass
 
     @property
     def shape(self) -> tuple[int, ...]:
         """self.data.shape."""
         return self.data.shape
 
     @property
@@ -243,15 +245,14 @@
 
 
         See Also
         --------
         from_data
 
         """
-        pass
 
     def zeros_like(self: T_CentralMoments) -> T_CentralMoments:
         """
         Create new empty object like self.
 
         Returns
         -------
@@ -1027,15 +1028,14 @@
 
         See Also
         --------
         from_data : General constructor
         numpy.zeros
 
         """
-        pass
 
     @classmethod
     @abstractmethod
     @docfiller_shared
     def from_data(
         cls: type[T_CentralMoments],
         data: Any,
@@ -1250,15 +1250,14 @@
 
         Notes
         -----
         Weights are taken from ``raw[...,0, 0]``.
         Using raw moments can result in numerical issues, especially for higher moments.  Use with care.
 
         """
-        pass
 
     @classmethod
     @abstractmethod
     @docfiller_shared
     def from_raws(
         cls: type[T_CentralMoments],
         raws,
@@ -1296,15 +1295,14 @@
         ~cmomy.convert.to_central_comoments : convert raw to central comoments
 
         Notes
         -----
         Weights are taken from ``raw[...,0, 0]``.
         Using raw moments can result in numerical issues, especially for higher moments.  Use with care.
         """
-        pass
 
     # --------------------------------------------------
     # mom_ndim == 1 specific
     # --------------------------------------------------
 
     # @staticmethod
     # def _raise_if_not_1d(mom_ndim: int) -> None:
```

### Comparing `cmomy-0.2.2/src/cmomy/cached_decorators.py` & `cmomy-0.3.0/src/cmomy/cached_decorators.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/central.py` & `cmomy-0.3.0/src/cmomy/central.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Hashable, Literal, Mapping, Sequence, cast
 
 import numpy as np
 import xarray as xr
 from numpy.core.numeric import normalize_axis_index  # type: ignore
-from numpy.typing import ArrayLike, DTypeLike
 
 from . import convert
 from ._docstrings import docfiller_shared
-from ._typing import ArrayOrder, Moments, T_CentralMoments
 from .resample import randsamp_freq, resample_data, resample_vals
 from .utils import _axis_expand_broadcast, _shape_insert_axis, _shape_reduce
 
 if TYPE_CHECKING:
+    from numpy.typing import ArrayLike, DTypeLike
+
+    from ._typing import ArrayOrder, Moments, T_CentralMoments
     from .xcentral import xCentralMoments
 
 
 ###############################################################################
 # central mom/comoments routines
 ###############################################################################
 def _central_moments(
```

### Comparing `cmomy-0.2.2/src/cmomy/compile.py` & `cmomy-0.3.0/src/cmomy/compile.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/convert.py` & `cmomy-0.3.0/src/cmomy/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # type: ignore
 """
 Routines to convert central (co)moments to raw (co)moments. (:mod:`cmomy.convert`)
 ==================================================================================
 """
 from __future__ import annotations
 
-from typing import Any, Callable, Sequence, no_type_check
+from typing import TYPE_CHECKING, Any, Callable, Sequence, no_type_check
 
 import numpy as np
 from numpy import ndarray
-from numpy.typing import ArrayLike, DTypeLike
 
 from ._docstrings import DocFiller
-from ._typing import ArrayOrder
 from .options import OPTIONS
 from .utils import factory_binomial, myjit
 
 _bfac = factory_binomial(OPTIONS["nmax"])
 
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike, DTypeLike
+
+    from ._typing import ArrayOrder
 
 _shared_docs = r"""
 Parameters
 ----------
 x_cmom | x : ndarray
     Central moments array.  The expected structure is:
```

### Comparing `cmomy-0.2.2/src/cmomy/options.py` & `cmomy-0.3.0/src/cmomy/options.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/pusher_interface.py` & `cmomy-0.3.0/src/cmomy/pusher_interface.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/pushers.py` & `cmomy-0.3.0/src/cmomy/pushers.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/resample.py` & `cmomy-0.3.0/src/cmomy/resample.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 #     resample_data
 #     resample_vals
 #     bootstrap_confidence_interval
 #     xbootstrap_confidence_interval
 
 from __future__ import annotations
 
-from typing import Hashable, Literal, Sequence, Tuple, cast
+from typing import TYPE_CHECKING, Hashable, Literal, Sequence, Tuple, cast
 
 import numpy as np
 import xarray as xr
-from numpy.typing import ArrayLike, DTypeLike
 
 from ._resample import factory_resample_data, factory_resample_vals
-from ._typing import ArrayOrder, Moments, XvalStrict
 from .utils import _axis_expand_broadcast, myjit
 
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike, DTypeLike
+
+    from ._typing import ArrayOrder, Moments, XvalStrict
+
 ##############################################################################
 # resampling
 ###############################################################################
 
 
 @myjit
 def numba_random_seed(seed):
```

### Comparing `cmomy-0.2.2/src/cmomy/tests/conftest.py` & `cmomy-0.3.0/src/cmomy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_central.py` & `cmomy-0.3.0/src/cmomy/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_central_2.py` & `cmomy-0.3.0/src/cmomy/tests/test_central_2.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_convert.py` & `cmomy-0.3.0/src/cmomy/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_resample.py` & `cmomy-0.3.0/src/cmomy/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_stability.py` & `cmomy-0.3.0/src/cmomy/tests/test_stability.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_verify.py` & `cmomy-0.3.0/src/cmomy/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_xcentral.py` & `cmomy-0.3.0/src/cmomy/tests/test_xcentral.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/tests/test_xcentral_constructors.py` & `cmomy-0.3.0/src/cmomy/tests/test_xcentral_constructors.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.2.2/src/cmomy/utils.py` & `cmomy-0.3.0/src/cmomy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Utilities."""
 from __future__ import annotations
 
 from functools import lru_cache
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
 import numpy as np
 from numba import njit
-from numpy.typing import ArrayLike, DTypeLike
-
-from ._typing import ArrayOrder
 
 # from .cached_decorators import gcached  # , cached_clear
 from .options import OPTIONS
 
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike, DTypeLike
+
+    from ._typing import ArrayOrder
+
 
 def myjit(func):
     """Jitter with option inline='always', fastmath=True."""
     return njit(inline="always", fastmath=OPTIONS["fastmath"], cache=OPTIONS["cache"])(
         func
     )
```

### Comparing `cmomy-0.2.2/src/cmomy/xcentral.py` & `cmomy-0.3.0/src/cmomy/xcentral.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 
 """Thin wrapper around central routines with xarray support."""
 
 
 from __future__ import annotations
 
 from typing import (  # TYPE_CHECKING,
+    TYPE_CHECKING,
     Any,
     Hashable,
     Literal,
     Mapping,
     Sequence,
     cast,
     no_type_check,
 )
 from warnings import warn
 
 import numpy as np
 import xarray as xr
-from numpy.typing import DTypeLike
 
 from . import convert
 from ._docstrings import docfiller_shared
-from ._typing import Dims, MomDims, Moments, T_CentralMoments
 from .abstract_central import CentralMomentsABC
 from .cached_decorators import gcached
 from .central import CentralMoments
 from .utils import _shape_reduce
 
+if TYPE_CHECKING:
+    from numpy.typing import DTypeLike
+
+    from ._typing import Dims, MomDims, Moments, T_CentralMoments
+
 
 # * Utilities
 def _select_axis_dim(
     dims: tuple[Hashable, ...],
     axis: int | str | None = None,
     dim: Hashable | None = None,
     default_axis: int | None = None,
```

### Comparing `cmomy-0.2.2/src/cmomy.egg-info/SOURCES.txt` & `cmomy-0.3.0/src/cmomy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 .cruft.json
+.editorconfig
 .gitattributes
 .gitignore
+.markdownlint.yaml
 .pre-commit-config.yaml
+.prettierrc.yaml
 AUTHORS.md
+CHANGELOG.md
 CONTRIBUTING.md
-HISTORY.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 commands.sh
 conftest.py
 environment.yaml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+changelog.d/20230424_125230_william.krekelberg_update_cruft.md
+changelog.d/README.txt
+changelog.d/templates/new_fragment.md.j2
+changelog.d/templates/auto-changelog/macros.jinja2
+changelog.d/templates/auto-changelog/template.jinja2
 docs/Makefile
 docs/authors.md
+docs/changelog.md
 docs/conf.py
 docs/contributing.md
-docs/example.md
-docs/history.md
+docs/example_for_readme.md
 docs/index.md
 docs/installation.md
 docs/license.md
 docs/make.bat
+docs/navigation.md
 docs/spelling_wordlist.txt
-docs/_build/html/_sources/reference/api-baseclasses.rst
-docs/_build/html/_sources/reference/api-modules.rst
-docs/_build/html/_sources/reference/api-public.rst
-docs/_build/html/_sources/reference/generated/cmomy.CentralMoments.rst
-docs/_build/html/_sources/reference/generated/cmomy.central_moments.rst
-docs/_build/html/_sources/reference/generated/cmomy.convert.rst
-docs/_build/html/_sources/reference/generated/cmomy.resample.rst
-docs/_build/html/_sources/reference/generated/cmomy.xCentralMoments.rst
-docs/_build/html/_sources/reference/generated/cmomy.xcentral_moments.rst
-docs/_build/html/_static/file.png
-docs/_build/html/_static/minus.png
-docs/_build/html/_static/plus.png
-docs/_build/html/_static/images/logo_colab.png
 docs/_static/css/nist-combined.css
 docs/_static/js/leave_notice.js
 docs/_static/js/nist-header-footer.js
 docs/_templates/class-individual-pages.rst
 docs/_templates/module-custom.rst
 docs/_templates/module-single.rst
 docs/_templates/module-template.rst
@@ -51,39 +47,43 @@
 docs/_templates/autodocsumm/class.rst
 docs/_templates/autodocsumm/module-inherit.rst
 docs/_templates/autodocsumm/module-noindex.rst
 docs/_templates/autodocsumm/module.rst
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
-docs/notebooks/motivation.ipynb
-docs/notebooks/usage_notebook.ipynb
+docs/examples/create-symlinks.sh
+docs/examples/index.md
+docs/examples/usage/motivation.ipynb
+docs/examples/usage/usage_notebook.ipynb
 docs/reference/api-baseclasses.rst
 docs/reference/api-modules.rst
 docs/reference/api-public.rst
 docs/reference/index.md
-docs/reference/generated/cmomy.CentralMoments.rst
-docs/reference/generated/cmomy.central_moments.rst
-docs/reference/generated/cmomy.convert.rst
-docs/reference/generated/cmomy.resample.rst
-docs/reference/generated/cmomy.xCentralMoments.rst
-docs/reference/generated/cmomy.xcentral_moments.rst
 environment/dev-extras.yaml
 environment/dev.yaml
 environment/dist-conda.yaml
 environment/dist-pypi.yaml
 environment/docs-extras.yaml
 environment/docs.yaml
+environment/lint-extras.yaml
+environment/lint.yaml
 environment/test-extras.yaml
 environment/test.yaml
-examples/bootstrap.ipynb
-examples/central_moments.ipynb
-examples/example_usage.ipynb
-examples/parallel_test.ipynb
-examples/test_accumulator.ipynb
+environment/tools.yaml
+examples/README.md
+examples/archived/bootstrap.ipynb
+examples/archived/central_moments.ipynb
+examples/archived/example_usage.ipynb
+examples/archived/parallel_test.ipynb
+examples/archived/test_accumulator.ipynb
+examples/usage/motivation.ipynb
+examples/usage/usage_notebook.ipynb
+scripts/docs-examples-symlinks.sh
+scripts/tox-ipykernel-display-name.sh
 src/cmomy/__init__.py
 src/cmomy/_docstrings.py
 src/cmomy/_formatting.py
 src/cmomy/_resample.py
 src/cmomy/_testing.py
 src/cmomy/_typing.py
 src/cmomy/abstract_central.py
@@ -94,14 +94,20 @@
 src/cmomy/options.py
 src/cmomy/pusher_interface.py
 src/cmomy/pushers.py
 src/cmomy/py.typed
 src/cmomy/resample.py
 src/cmomy/utils.py
 src/cmomy/xcentral.py
+src/cmomy.egg-info/PKG-INFO
+src/cmomy.egg-info/SOURCES.txt
+src/cmomy.egg-info/dependency_links.txt
+src/cmomy.egg-info/not-zip-safe
+src/cmomy.egg-info/requires.txt
+src/cmomy.egg-info/top_level.txt
 src/cmomy/_docfiller/__init__.py
 src/cmomy/_docfiller/docfiller.py
 src/cmomy/_docfiller/docscrape.py
 src/cmomy/tests/__init__.py
 src/cmomy/tests/conftest.py
 src/cmomy/tests/test_central.py
 src/cmomy/tests/test_central_2.py
```

### Comparing `cmomy-0.2.2/tox.ini` & `cmomy-0.3.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-skipsdist=True
+isolated_build = True
 requires = tox-conda
 envlist =
         # test
         py3{8, 9, 10}-tests
 
 
 [base]
@@ -12,14 +12,15 @@
 build_python = python3.10
 conda_env            = {toxinidir}/environment.yaml
 conda_env_dev        = {toxinidir}/environment/dev.yaml
 conda_env_test       = {toxinidir}/environment/test.yaml
 conda_env_docs       = {toxinidir}/environment/docs.yaml
 conda_env_dist_pypi  = {toxinidir}/environment/dist-pypi.yaml
 conda_env_dist_conda = {toxinidir}/environment/dist-conda.yaml
+conda_env_lint       = {toxinidir}/environment/lint.yaml
 conda_channels =
     wpk-nist
     conda-forge
 conda_deps_test =
 allowlist_externals =
     bash
     open
@@ -43,15 +44,25 @@
 allowlist_externals =
     {[base]allowlist_externals}
 commands =
     {[base]commands_test_check}
     pytest {posargs}
 
 
-# Build documentation
+[testenv:dev]
+description =
+    Create development environment.
+usedevelop = True
+basepython = {[base]build_python}
+conda_env = {[base]conda_env_dev}
+envdir = {toxworkdir}/dev
+commands =
+    {posargs:bash -ec 'conda list'}
+
+
 [testenv:docs-{build, release, clean, command, spelling, live, open, make}]
 description =
     build: build documentation.
     release: create documentation branch.
     clean: clean build.
     spelling: run spell checking on documentation and docstrings.
     command: run arbitrary command
@@ -62,63 +73,59 @@
 basepython = {[base]build_python}
 conda_env  = {[base]conda_env_docs}
 changedir  = {toxinidir}/docs
 commands =
     build: bash -c "echo $PWD"
     build: make {posargs:html}
     open: open {toxinidir}/docs/_build/html/index.html
-    release: ghp-import -n {posargs:-m 'update docs'} -b nist-pages {toxinidir}/docs/_build/html
+    release: ghp-import -o -n {posargs:-m 'update docs'} -b nist-pages {toxinidir}/docs/_build/html
     clean: make allclean
     spelling: make spelling
     command: {posargs}
     live: make livehtml
     make: make {posargs}
 
-# create pypi dist
+
 [testenv:dist-pypi-{build, testrelease, release}]
 description  =
     build: build distribution.
     testrelease: upload to testpypi
     release: upload to pypi
 skip_install = True
 envdir       = {toxworkdir}/dist-pypi
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_pypi}
 changedir    = {toxinidir}
 commands     =
     build: rm -rf {toxinidir}/dist
     build: python -m build --outdir "{toxinidir}/dist/"
-
     testrelease: twine upload --repository testpypi {toxinidir}/dist/*
     release: twine upload {toxinidir}/dist/*
 
 
-# create conda dist
 [testenv:dist-conda-{recipe, build, command}]
 description  =
-    recipe: build conda recipe using grayskull
+    recipe: build conda recipe using grayskull (can optionally pass a local sdist)
     build: build conda distribution
     command: run arbitrary command
 skip_install = True
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
 changedir    = {toxinidir}/dist-conda
 commands     =
     recipe: rm -rf {toxinidir}/dist-conda/{[base]package_name}
     recipe: grayskull pypi {posargs:{[base]package_name}}
     recipe: cat {[base]package_name}/meta.yaml
-
     build: rm -rf build
     build: mkdir -p build
     build: conda mambabuild --output-folder=build --no-anaconda-upload .
     command: {posargs:python}
 
 
-# test pypi/conda install from local/remote
 [testenv:test-dist-{pypi, conda}-{local,remote}-py3{8,9,10}]
 conda_channels =
     {[base]conda_channels}
 description  =
     Test install from
     pypi: pypi
     conda: conda
@@ -132,14 +139,25 @@
     conda-remote: {[base]package_name}
     conda-local: {posargs}
 deps =
     pypi-remote: {[base]package_name}
     pypi-local: {posargs}
 
 
-# Test pip installed dependencies
 [testenv:test-pip-py3{8,9,10}]
 description  =
     Test package against pip installed packages
 usedevelop   = True
 extras = test
 conda_env    = {toxinidir}/environment/test-extras.yaml
+
+
+[testenv:lint-{mypy,command}]
+description =
+    Run mypy on code. (run with tox -e lint -- --no-incremental to rebuild cache).
+conda_env = {[base]conda_env_lint}
+usedevelop = True
+envdir     = {toxworkdir}/lint
+basepython = {[base]build_python}
+commands =
+         mypy: mypy --color-output {posargs}
+         command: {posargs}
```

