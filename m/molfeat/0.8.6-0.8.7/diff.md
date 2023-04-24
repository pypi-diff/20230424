# Comparing `tmp/molfeat-0.8.6.tar.gz` & `tmp/molfeat-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.8.6.tar", last modified: Mon Apr 10 17:36:02 2023, max compression
+gzip compressed data, was "molfeat-0.8.7.tar", last modified: Mon Apr 24 16:37:54 2023, max compression
```

## Comparing `molfeat-0.8.6.tar` & `molfeat-0.8.7.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-10 17:34:46.000000 molfeat-0.8.6/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-10 17:34:46.000000 molfeat-0.8.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-10 17:34:46.000000 molfeat-0.8.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-10 17:34:46.000000 molfeat-0.8.6/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-10 17:34:46.000000 molfeat-0.8.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-10 17:34:46.000000 molfeat-0.8.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-10 17:34:46.000000 molfeat-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-10 17:36:02.965476 molfeat-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-10 17:34:46.000000 molfeat-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.949476 molfeat-0.8.6/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.953476 molfeat-0.8.6/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 17:34:46.000000 molfeat-0.8.6/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-10 17:34:46.000000 molfeat-0.8.6/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-10 17:34:46.000000 molfeat-0.8.6/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33689 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.961476 molfeat-0.8.6/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25556 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-10 17:34:46.000000 molfeat-0.8.6/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.957476 molfeat-0.8.6/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:35:52.000000 molfeat-0.8.6/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 17:36:02.000000 molfeat-0.8.6/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-10 17:34:46.000000 molfeat-0.8.6/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-10 17:34:46.000000 molfeat-0.8.6/plugin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-10 17:34:46.000000 molfeat-0.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-10 17:34:46.000000 molfeat-0.8.6/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:36:02.965476 molfeat-0.8.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:36:02.965476 molfeat-0.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-10 17:34:46.000000 molfeat-0.8.6/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.472288 molfeat-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-24 16:37:36.000000 molfeat-0.8.7/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.444288 molfeat-0.8.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.444288 molfeat-0.8.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.448288 molfeat-0.8.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-24 16:35:03.000000 molfeat-0.8.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 16:35:03.000000 molfeat-0.8.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 16:37:36.000000 molfeat-0.8.7/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 16:37:36.000000 molfeat-0.8.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-24 16:37:36.000000 molfeat-0.8.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-24 16:35:03.000000 molfeat-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-24 16:37:54.472288 molfeat-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-24 16:35:03.000000 molfeat-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.448288 molfeat-0.8.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.440288 molfeat-0.8.7/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.452288 molfeat-0.8.7/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.456288 molfeat-0.8.7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-24 16:35:03.000000 molfeat-0.8.7/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-24 16:35:03.000000 molfeat-0.8.7/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-24 16:35:03.000000 molfeat-0.8.7/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.456288 molfeat-0.8.7/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.460288 molfeat-0.8.7/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22266 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33499 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.464288 molfeat-0.8.7/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.468288 molfeat-0.8.7/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.468288 molfeat-0.8.7/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.468288 molfeat-0.8.7/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-24 16:35:03.000000 molfeat-0.8.7/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.456288 molfeat-0.8.7/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:37:45.000000 molfeat-0.8.7/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 16:37:54.000000 molfeat-0.8.7/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.472288 molfeat-0.8.7/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 16:35:03.000000 molfeat-0.8.7/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 16:35:03.000000 molfeat-0.8.7/plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-24 16:35:03.000000 molfeat-0.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 16:35:03.000000 molfeat-0.8.7/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:37:54.472288 molfeat-0.8.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:37:54.472288 molfeat-0.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 16:35:03.000000 molfeat-0.8.7/tests/test_viz.py
```

### Comparing `molfeat-0.8.6/.authors.yml` & `molfeat-0.8.7/.authors.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 - name: maclandrol
   email: emmanuel.noutahi@hotmail.ca
-  num_commits: 34
+  num_commits: 0
   first_commit: 2021-04-06 11:53:10
 - name: Cas Wognum
   email: caswognum@outlook.com
   aliases:
   - cwognum
-  num_commits: 30
+  num_commits: 0
   first_commit: 2023-03-20 13:05:13
 - name: Hadrien Mary
   email: hadrien.mary@gmail.com
   alternate_emails:
   - hadim@users.noreply.github.com
-  num_commits: 23
+  num_commits: 0
   first_commit: 2023-03-21 12:50:42
 - name: Therence
   email: 38595485+Therence1@users.noreply.github.com
-  num_commits: 2
+  num_commits: 0
   first_commit: 2023-03-26 23:33:17
 - name: Honore Hounwanou
   email: mercuryseries@gmail.com
-  num_commits: 3
+  num_commits: 0
   first_commit: 2023-04-03 19:51:15
 - name: Saurav Maheshkar
   github: SauravMaheshkar
   email: sauravvmaheshkar@gmail.com
-  num_commits: 1
+  num_commits: 0
   first_commit: 2023-04-04 07:44:44
+- name: rbyrne-momatx
+  email: 113197924+rbyrne-momatx@users.noreply.github.com
+  num_commits: 0
+  first_commit: 2023-04-22 17:53:52
```

### Comparing `molfeat-0.8.6/.github/CODE_OF_CONDUCT.md` & `molfeat-0.8.7/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.8.7/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.8.7/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.8.7/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.8.7/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.8.7/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.github/workflows/doc.yml` & `molfeat-0.8.7/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.github/workflows/test.yml` & `molfeat-0.8.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.gitignore` & `molfeat-0.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/.mailmap` & `molfeat-0.8.7/.mailmap`

 * *Files 7% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 
 Cas Wognum <caswognum@outlook.com> cwognum <caswognum@outlook.com>
 Hadrien Mary <hadrien.mary@gmail.com> Hadrien Mary <hadim@users.noreply.github.com>
 Honore Hounwanou <mercuryseries@gmail.com>
 Saurav Maheshkar <sauravvmaheshkar@gmail.com>
 Therence <38595485+Therence1@users.noreply.github.com>
 maclandrol <emmanuel.noutahi@hotmail.ca>
+rbyrne-momatx <113197924+rbyrne-momatx@users.noreply.github.com>
```

### Comparing `molfeat-0.8.6/CHANGELOG.rst` & `molfeat-0.8.7/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,42 @@
 ==================
 molfeat Change Log
 ==================
 
 .. current developments
 
+v0.8.7
+====================
+
+**Added:**
+
+* Support for `ignore_padding` in Graphormer
+* More flexibility overall for graphormer embeddings
+
+**Changed:**
+
+* Phased out rdchem.Mol, rdchem.Atom and rdkit.Bond in favor of datamol versions
+* Fully automated release process.
+
+**Fixed:**
+
+* Random logging in cache coming from testing if an input is a molecule
+* Some small typos in doc strings
+* Naming of JTVAE models
+* Fix issue #37 by making WeaveFeaturizer faster
+* Usage card for rdkit and fingerprints/descriptors featurizers
+
+**Authors:**
+
+* Hadrien Mary
+* maclandrol
+* rbyrne-momatx
+
+
+
 v0.8.6
 ====================
 
 **Added:**
 
 * Support for batch transformation in `MoleculeTransformer` for calculators that implements `batch_compute`
```

### Comparing `molfeat-0.8.6/LICENSE` & `molfeat-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/PKG-INFO` & `molfeat-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.6
+Version: 0.8.7
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -39,15 +39,15 @@
 
 <p align="center">
     <b>molfeat - the hub for all your molecular featurizers </b> <br />
 </p>
 <p align="center">
   <a href="https://molfeat-docs.datamol.io/" target="_blank">
       Docs
-  </a> | 
+  </a> |
   <a href="https://molfeat.datamol.io/" target="_blank">
       Homepage
   </a>
 </p>
 
 ---
 
@@ -68,52 +68,50 @@
 Molfeat is a hub of molecular featurizers. It supports a wide variety of out-of-the-box molecular featurizers and can be easily extended to include your own custom featurizers.
 
 - 🚀 Fast, with a simple and efficient API.
 - 🔄 Unify pre-trained molecular embeddings and hand-crafted featurizers in a single package.
 - ➕ Easily add your own featurizers through plugins.
 - 📈 Benefit from increased performance through a trouble-free caching system.
 
-Visit our website at https://molfeat.datamol.io.
+Visit our website at <https://molfeat.datamol.io>.
 
 ## Installation
 
 ### Installing Molfeat
 
 Use mamba:
 
 ```bash
 mamba install -c conda-forge molfeat
 ```
 
 _**Tips:** You can replace `mamba` by `conda`._
 
-_**Note:** We highly recommend using a [Conda Python distribution](https://github.com/conda-forge/miniforge) to install Molfeat. The package is also pip installable if you need it: `pip install molfeat`._ 
+_**Note:** We highly recommend using a [Conda Python distribution](https://github.com/conda-forge/miniforge) to install Molfeat. The package is also pip installable if you need it: `pip install molfeat`._
 
 ### Optional dependencies
-Not all featurizers in the Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them. 
+
+Not all featurizers in the Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them.
 
 - To install `dgl`: run `mamba install -c dglteam dgl`
-- To install `dgllife`:  run `mamba install -c conda-forge dgllife`
+- To install `dgllife`: run `mamba install -c conda-forge dgllife`
 - To install `fcd_torch`: run `mamba install -c conda-forge fcd_torch`
 - To install `pyg`: run `mamba install -c conda-forge pytorch_geometric`
 - To install `graphormer-pretrained`: run `mamba install -c conda-forge graphormer-pretrained`
-- To install `map4`: see https://github.com/reymond-group/map4
+- To install `map4`: see <https://github.com/reymond-group/map4>
 - To install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings >=0.2.2'`
 
-
 If you install Molfeat using pip, there are optional dependencies that can be installed with the main package. For example, `pip install "molfeat[all]"` allows installing all the compatible optional dependencies for small molecule featurization. There are other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/blob/main/pyproject.toml#L60) for more information.
 
-
 ### Installing Plugins
 
 The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](developers/create-plugin.md) your own plugins.
 
 However, this does imply that the installation of a plugin is plugin-dependent: please consult the relevant documentation to learn more.
 
-
 ## API tour
 
 ```python
 import datamol as dm
 from molfeat.calc import FPCalculator
 from molfeat.trans import MoleculeTransformer
 from molfeat.store.modelstore import ModelStore
@@ -153,17 +151,14 @@
 
 ## Changelogs
 
 See the latest changelogs at [CHANGELOG.rst](./CHANGELOG.rst).
 
 ## Maintainers
 
-* @cwognum
-* @maclandrol
-* @hadim
-
+- @cwognum
+- @maclandrol
+- @hadim
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.6 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.7 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -45,37 +45,38 @@
 badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/
 release.yml) Molfeat is a hub of molecular featurizers. It supports a wide
 variety of out-of-the-box molecular featurizers and can be easily extended to
 include your own custom featurizers. - ð Fast, with a simple and efficient
 API. - ð Unify pre-trained molecular embeddings and hand-crafted featurizers
 in a single package. - â Easily add your own featurizers through plugins. -
 ð Benefit from increased performance through a trouble-free caching system.
-Visit our website at https://molfeat.datamol.io. ## Installation ### Installing
-Molfeat Use mamba: ```bash mamba install -c conda-forge molfeat ``` _**Tips:**
-You can replace `mamba` by `conda`._ _**Note:** We highly recommend using a
-[Conda Python distribution](https://github.com/conda-forge/miniforge) to
-install Molfeat. The package is also pip installable if you need it: `pip
-install molfeat`._ ### Optional dependencies Not all featurizers in the Molfeat
-core package are supported by default. Some featurizers require additional
-dependencies. If you try to use a featurizer that requires additional
-dependencies, Molfeat will raise an error and tell you which dependencies are
-missing and how to install them. - To install `dgl`: run `mamba install -
-c dglteam dgl` - To install `dgllife`: run `mamba install -c conda-forge
-dgllife` - To install `fcd_torch`: run `mamba install -c conda-forge fcd_torch`
-- To install `pyg`: run `mamba install -c conda-forge pytorch_geometric` - To
-install `graphormer-pretrained`: run `mamba install -c conda-forge graphormer-
-pretrained` - To install `map4`: see https://github.com/reymond-group/map4 - To
-install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings
->=0.2.2'` If you install Molfeat using pip, there are optional dependencies
-that can be installed with the main package. For example, `pip install "molfeat
-[all]"` allows installing all the compatible optional dependencies for small
-molecule featurization. There are other options such as `molfeat[dgl]`,
-`molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat
-[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/
-blob/main/pyproject.toml#L60) for more information. ### Installing Plugins The
+Visit our website at
+molfeat.datamol.io>. ## Installation ### Installing Molfeat Use mamba: ```bash
+mamba install -c conda-forge molfeat ``` _**Tips:** You can replace `mamba` by
+`conda`._ _**Note:** We highly recommend using a [Conda Python distribution]
+(https://github.com/conda-forge/miniforge) to install Molfeat. The package is
+also pip installable if you need it: `pip install molfeat`._ ### Optional
+dependencies Not all featurizers in the Molfeat core package are supported by
+default. Some featurizers require additional dependencies. If you try to use a
+featurizer that requires additional dependencies, Molfeat will raise an error
+and tell you which dependencies are missing and how to install them. - To
+install `dgl`: run `mamba install -c dglteam dgl` - To install `dgllife`: run
+`mamba install -c conda-forge dgllife` - To install `fcd_torch`: run `mamba
+install -c conda-forge fcd_torch` - To install `pyg`: run `mamba install -
+c conda-forge pytorch_geometric` - To install `graphormer-pretrained`: run
+`mamba install -c conda-forge graphormer-pretrained` - To install `map4`: see
+github.com/reymond-group/map4> - To install `bio-embeddings`: run `mamba
+install -c conda-forge 'bio-embeddings >=0.2.2'` If you install Molfeat using
+pip, there are optional dependencies that can be installed with the main
+package. For example, `pip install "molfeat[all]"` allows installing all the
+compatible optional dependencies for small molecule featurization. There are
+other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat
+[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-
+dependencies](https://github.com/datamol-io/molfeat/blob/main/
+pyproject.toml#L60) for more information. ### Installing Plugins The
 functionality of Molfeat can be extended through plugins. The use of a plugin
 system ensures that the core package remains easy to install and as light as
 possible, while making it easy to extend its functionality with plug-and-play
 components. Additionally, it ensures that plugins can be developed
 independently from the core package, removing the bottleneck of a central party
 that reviews and approves new plugins. Consult the molfeat documentation for
 more details on how to [create](developers/create-plugin.md) your own plugins.
@@ -92,9 +93,9 @@
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
 contribute to `Molfeat` ## Changelogs See the latest changelogs at
-[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers * @cwognum * @maclandrol *
+[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers - @cwognum - @maclandrol -
 @hadim ## License Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `molfeat-0.8.6/README.md` & `molfeat-0.8.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 <p align="center">
     <b>molfeat - the hub for all your molecular featurizers </b> <br />
 </p>
 <p align="center">
   <a href="https://molfeat-docs.datamol.io/" target="_blank">
       Docs
-  </a> | 
+  </a> |
   <a href="https://molfeat.datamol.io/" target="_blank">
       Homepage
   </a>
 </p>
 
 ---
 
@@ -33,52 +33,50 @@
 Molfeat is a hub of molecular featurizers. It supports a wide variety of out-of-the-box molecular featurizers and can be easily extended to include your own custom featurizers.
 
 - 🚀 Fast, with a simple and efficient API.
 - 🔄 Unify pre-trained molecular embeddings and hand-crafted featurizers in a single package.
 - ➕ Easily add your own featurizers through plugins.
 - 📈 Benefit from increased performance through a trouble-free caching system.
 
-Visit our website at https://molfeat.datamol.io.
+Visit our website at <https://molfeat.datamol.io>.
 
 ## Installation
 
 ### Installing Molfeat
 
 Use mamba:
 
 ```bash
 mamba install -c conda-forge molfeat
 ```
 
 _**Tips:** You can replace `mamba` by `conda`._
 
-_**Note:** We highly recommend using a [Conda Python distribution](https://github.com/conda-forge/miniforge) to install Molfeat. The package is also pip installable if you need it: `pip install molfeat`._ 
+_**Note:** We highly recommend using a [Conda Python distribution](https://github.com/conda-forge/miniforge) to install Molfeat. The package is also pip installable if you need it: `pip install molfeat`._
 
 ### Optional dependencies
-Not all featurizers in the Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them. 
+
+Not all featurizers in the Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them.
 
 - To install `dgl`: run `mamba install -c dglteam dgl`
-- To install `dgllife`:  run `mamba install -c conda-forge dgllife`
+- To install `dgllife`: run `mamba install -c conda-forge dgllife`
 - To install `fcd_torch`: run `mamba install -c conda-forge fcd_torch`
 - To install `pyg`: run `mamba install -c conda-forge pytorch_geometric`
 - To install `graphormer-pretrained`: run `mamba install -c conda-forge graphormer-pretrained`
-- To install `map4`: see https://github.com/reymond-group/map4
+- To install `map4`: see <https://github.com/reymond-group/map4>
 - To install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings >=0.2.2'`
 
-
 If you install Molfeat using pip, there are optional dependencies that can be installed with the main package. For example, `pip install "molfeat[all]"` allows installing all the compatible optional dependencies for small molecule featurization. There are other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/blob/main/pyproject.toml#L60) for more information.
 
-
 ### Installing Plugins
 
 The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](developers/create-plugin.md) your own plugins.
 
 However, this does imply that the installation of a plugin is plugin-dependent: please consult the relevant documentation to learn more.
 
-
 ## API tour
 
 ```python
 import datamol as dm
 from molfeat.calc import FPCalculator
 from molfeat.trans import MoleculeTransformer
 from molfeat.store.modelstore import ModelStore
@@ -118,17 +116,14 @@
 
 ## Changelogs
 
 See the latest changelogs at [CHANGELOG.rst](./CHANGELOG.rst).
 
 ## Maintainers
 
-* @cwognum
-* @maclandrol
-* @hadim
-
+- @cwognum
+- @maclandrol
+- @hadim
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
-
-
```

#### html2text {}

```diff
@@ -25,37 +25,38 @@
 badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/
 release.yml) Molfeat is a hub of molecular featurizers. It supports a wide
 variety of out-of-the-box molecular featurizers and can be easily extended to
 include your own custom featurizers. - ð Fast, with a simple and efficient
 API. - ð Unify pre-trained molecular embeddings and hand-crafted featurizers
 in a single package. - â Easily add your own featurizers through plugins. -
 ð Benefit from increased performance through a trouble-free caching system.
-Visit our website at https://molfeat.datamol.io. ## Installation ### Installing
-Molfeat Use mamba: ```bash mamba install -c conda-forge molfeat ``` _**Tips:**
-You can replace `mamba` by `conda`._ _**Note:** We highly recommend using a
-[Conda Python distribution](https://github.com/conda-forge/miniforge) to
-install Molfeat. The package is also pip installable if you need it: `pip
-install molfeat`._ ### Optional dependencies Not all featurizers in the Molfeat
-core package are supported by default. Some featurizers require additional
-dependencies. If you try to use a featurizer that requires additional
-dependencies, Molfeat will raise an error and tell you which dependencies are
-missing and how to install them. - To install `dgl`: run `mamba install -
-c dglteam dgl` - To install `dgllife`: run `mamba install -c conda-forge
-dgllife` - To install `fcd_torch`: run `mamba install -c conda-forge fcd_torch`
-- To install `pyg`: run `mamba install -c conda-forge pytorch_geometric` - To
-install `graphormer-pretrained`: run `mamba install -c conda-forge graphormer-
-pretrained` - To install `map4`: see https://github.com/reymond-group/map4 - To
-install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings
->=0.2.2'` If you install Molfeat using pip, there are optional dependencies
-that can be installed with the main package. For example, `pip install "molfeat
-[all]"` allows installing all the compatible optional dependencies for small
-molecule featurization. There are other options such as `molfeat[dgl]`,
-`molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat
-[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/
-blob/main/pyproject.toml#L60) for more information. ### Installing Plugins The
+Visit our website at
+molfeat.datamol.io>. ## Installation ### Installing Molfeat Use mamba: ```bash
+mamba install -c conda-forge molfeat ``` _**Tips:** You can replace `mamba` by
+`conda`._ _**Note:** We highly recommend using a [Conda Python distribution]
+(https://github.com/conda-forge/miniforge) to install Molfeat. The package is
+also pip installable if you need it: `pip install molfeat`._ ### Optional
+dependencies Not all featurizers in the Molfeat core package are supported by
+default. Some featurizers require additional dependencies. If you try to use a
+featurizer that requires additional dependencies, Molfeat will raise an error
+and tell you which dependencies are missing and how to install them. - To
+install `dgl`: run `mamba install -c dglteam dgl` - To install `dgllife`: run
+`mamba install -c conda-forge dgllife` - To install `fcd_torch`: run `mamba
+install -c conda-forge fcd_torch` - To install `pyg`: run `mamba install -
+c conda-forge pytorch_geometric` - To install `graphormer-pretrained`: run
+`mamba install -c conda-forge graphormer-pretrained` - To install `map4`: see
+github.com/reymond-group/map4> - To install `bio-embeddings`: run `mamba
+install -c conda-forge 'bio-embeddings >=0.2.2'` If you install Molfeat using
+pip, there are optional dependencies that can be installed with the main
+package. For example, `pip install "molfeat[all]"` allows installing all the
+compatible optional dependencies for small molecule featurization. There are
+other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat
+[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-
+dependencies](https://github.com/datamol-io/molfeat/blob/main/
+pyproject.toml#L60) for more information. ### Installing Plugins The
 functionality of Molfeat can be extended through plugins. The use of a plugin
 system ensures that the core package remains easy to install and as light as
 possible, while making it easy to extend its functionality with plug-and-play
 components. Additionally, it ensures that plugins can be developed
 independently from the core package, removing the bottleneck of a central party
 that reviews and approves new plugins. Consult the molfeat documentation for
 more details on how to [create](developers/create-plugin.md) your own plugins.
@@ -72,9 +73,9 @@
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
 contribute to `Molfeat` ## Changelogs See the latest changelogs at
-[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers * @cwognum * @maclandrol *
+[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers - @cwognum - @maclandrol -
 @hadim ## License Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `molfeat-0.8.6/docs/api/molfeat.calc.md` & `molfeat-0.8.7/docs/api/molfeat.calc.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/assets/css/custom-molfeat.css` & `molfeat-0.8.7/docs/assets/css/custom-molfeat.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/assets/css/custom.css` & `molfeat-0.8.7/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/benchmark.ipynb` & `molfeat-0.8.7/docs/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/developers/contribute.md` & `molfeat-0.8.7/docs/developers/contribute.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/developers/create-plugin.md` & `molfeat-0.8.7/docs/developers/create-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/developers/register-plugin.md` & `molfeat-0.8.7/docs/developers/register-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/images/logo-black.png` & `molfeat-0.8.7/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/images/logo-black.svg` & `molfeat-0.8.7/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/images/logo-title.svg` & `molfeat-0.8.7/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/images/logo.png` & `molfeat-0.8.7/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/images/logo.svg` & `molfeat-0.8.7/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/index.md` & `molfeat-0.8.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/add_your_own.ipynb` & `molfeat-0.8.7/docs/tutorials/add_your_own.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/datacache.ipynb` & `molfeat-0.8.7/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/graphs.ipynb` & `molfeat-0.8.7/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/integrations.ipynb` & `molfeat-0.8.7/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.8.7/docs/tutorials/pyg_integration.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/save_and_load.ipynb` & `molfeat-0.8.7/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.8.7/docs/tutorials/transformer_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.8.7/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/docs/usage.md` & `molfeat-0.8.7/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/env.yml` & `molfeat-0.8.7/env.yml`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
   - pytorch >=1.10.2
   - scikit-learn
   - fcd_torch
 
   # Optional: featurizers
   - dgl
   - dgllife
-  - graphormer-pretrained >=0.2.2
+  - graphormer-pretrained >=0.2.3
   - transformers
   - tokenizers <0.13.2
   - biotite # required for ESM models
 
   # Optional: viz
   - nglview
   - ipywidgets
```

### Comparing `molfeat-0.8.6/mkdocs.yml` & `molfeat-0.8.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/calc/__init__.py` & `molfeat-0.8.7/molfeat/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/calc/_atom_bond_features.py` & `molfeat-0.8.7/molfeat/calc/_atom_bond_features.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Optional
 from typing import List
 from typing import Any
 
 
-import numpy as np
 import torch
+import numpy as np
+import datamol as dm
+
 from rdkit.Chem import rdchem
 from rdkit.Chem import AllChem
 from rdkit.Chem import GetSymmSSSR
 from rdkit.Chem.rdmolops import GetDistanceMatrix
 from rdkit.Chem.rdmolops import Get3DDistanceMatrix
 from molfeat.utils.commons import requires_conformer
 from molfeat.data import get_df as get_data
@@ -123,15 +125,15 @@
     rdchem.BondDir.NONE,
     rdchem.BondDir.ENDUPRIGHT,
     rdchem.BondDir.ENDDOWNRIGHT,
 ]
 
 
 def atom_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
     number: bool = False,
 ):
     """One hot encoding for the type of an atom.
 
     Args:
@@ -145,29 +147,29 @@
     """
     if allowable_set is None:
         allowable_set = ATOM_LIST if not number else list(range(1, 101))
     atom_val = atom.GetSymbol() if not number else atom.GetAtomicNum()
     return one_hot_encoding(atom_val, allowable_set, encode_unknown)
 
 
-def atom_number(atom: rdchem.Atom):
+def atom_number(atom: dm.Atom):
     """Get the atomic number for an atom.
 
     Args:
         atom : RDKit atom instance.
 
     Returns:
         list: List containing one int only.
 
     """
     return [atom.GetAtomicNum()]
 
 
 def atom_degree_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the degree of an atom.
 
     Result might be different if hydrogen have been added or not.
 
@@ -182,30 +184,30 @@
     """
     if allowable_set is None:
         allowable_set = ATOM_DEGREE_LIST
     return one_hot_encoding(atom.GetDegree(), allowable_set, encode_unknown)
 
 
 def atom_degree(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
 ):
     """Get the degree of an atom.
 
     Result might be different if hydrogen have been added or not.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.GetDegree()]
 
 
 def atom_total_degree_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the total degree of an atom including Hs.
 
     Args:
         atom: RDKit atom instance.
@@ -217,29 +219,29 @@
 
     """
     if allowable_set is None:
         allowable_set = ATOM_TOTAL_DEGREE_LIST
     return one_hot_encoding(atom.GetTotalDegree(), allowable_set, encode_unknown)
 
 
-def atom_total_degree(atom: rdchem.Atom):
+def atom_total_degree(atom: dm.Atom):
     """Get the total degree of an atom.
 
     Result might be different if hydrogen have been added or not.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.GetTotalDegree()]
 
 
 def atom_explicit_valence_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the explicit valence of an aotm.
 
     Args:
         atom: RDKit atom instance.
@@ -250,27 +252,27 @@
         list: List of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = EXPLICIT_VALENCE_LIST
     return one_hot_encoding(atom.GetExplicitValence(), allowable_set, encode_unknown)
 
 
-def atom_explicit_valence(atom: rdchem.Atom):
+def atom_explicit_valence(atom: dm.Atom):
     """Get the explicit valence of an atom.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.GetExplicitValence()]
 
 
 def atom_implicit_valence_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the implicit valence of an aotm.
 
     Args:
         atom: RDKit atom instance.
@@ -281,27 +283,27 @@
         list: List of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = IMPLICIT_VALENCE_LIST
     return one_hot_encoding(atom.GetImplicitValence(), allowable_set, encode_unknown)
 
 
-def atom_implicit_valence(atom: rdchem.Atom):
+def atom_implicit_valence(atom: dm.Atom):
     """Get the implicit valence of an atom.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.GetImplicitValence()]
 
 
 def atom_hybridization_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the hybridization of an atom.
 
     Args:
         atom: RDKit atom instance.
@@ -313,15 +315,15 @@
     """
     if allowable_set is None:
         allowable_set = HYBRIDIZATION_LIST
     return one_hot_encoding(atom.GetHybridization(), allowable_set, encode_unknown)
 
 
 def atom_total_num_H_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the total number of Hs of an atom.
 
      Args:
         atom: RDKit atom instance.
@@ -332,27 +334,27 @@
         list: List of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = ATOM_NUM_H_LIST
     return one_hot_encoding(atom.GetTotalNumHs(), allowable_set, encode_unknown)
 
 
-def atom_total_num_H(atom: rdchem.Atom):
+def atom_total_num_H(atom: dm.Atom):
     """Get the total number of Hs of an atom.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.GetTotalNumHs()]
 
 
 def atom_formal_charge_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the formal charge of an atom.
 
      Args:
         atom: RDKit atom instance.
@@ -363,26 +365,26 @@
         list: List of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = CHARGE_LIST
     return one_hot_encoding(atom.GetFormalCharge(), allowable_set, encode_unknown)
 
 
-def atom_formal_charge(atom: rdchem.Atom):
+def atom_formal_charge(atom: dm.Atom):
     """Get formal charge for an atom.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.GetFormalCharge()]
 
 
-def atom_partial_charge(atom: rdchem.Atom):
+def atom_partial_charge(atom: dm.Atom):
     """Get Gasteiger partial charge for an atom.
 
     This function requires calling ``AllChem.ComputeGasteigerCharges(mol)`` first to compute Gasteiger charges.
     Nan and infinite values are set to 0
 
     Args:
         atom: RDKit atom instance.
@@ -394,15 +396,15 @@
         AllChem.ComputeGasteigerCharges(mol)
     gasteiger_charge = atom.GetProp("_GasteigerCharge")
     gasteiger_charge = np.nan_to_num(float(gasteiger_charge), posinf=0.0, neginf=0.0)
     return [float(gasteiger_charge)]
 
 
 def atom_num_radical_electrons_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the number of radical electrons of an atom.
 
      Args:
         atom: RDKit atom instance.
@@ -413,27 +415,27 @@
         list: List of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = RADICAL_ELECTRON_LIST
     return one_hot_encoding(atom.GetNumRadicalElectrons(), allowable_set, encode_unknown)
 
 
-def atom_num_radical_electrons(atom: rdchem.Atom):
+def atom_num_radical_electrons(atom: dm.Atom):
     """Get the number of radical electrons for an atom.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.GetNumRadicalElectrons()]
 
 
 def atom_is_aromatic_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for whether the atom is aromatic.
 
      Args:
         atom: RDKit atom instance.
@@ -444,28 +446,28 @@
         list: List of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = [False, True]
     return one_hot_encoding(atom.GetIsAromatic(), allowable_set, encode_unknown)
 
 
-def atom_is_aromatic(atom: rdchem.Atom):
+def atom_is_aromatic(atom: dm.Atom):
     """Get whether the atom is aromatic.
 
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one bool only.
     """
     return [atom.GetIsAromatic()]
 
 
 def atom_is_in_ring_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for whether the atom is in ring.
 
      Args:
         atom: RDKit atom instance.
@@ -476,27 +478,27 @@
         list: List of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = [False, True]
     return one_hot_encoding(atom.IsInRing(), allowable_set, encode_unknown)
 
 
-def atom_is_in_ring(atom: rdchem.Atom):
+def atom_is_in_ring(atom: dm.Atom):
     """Get whether the atom is in ring.
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one int only.
     """
     return [atom.IsInRing()]
 
 
 def atom_chiral_tag_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the chiral tag of an atom.
 
      Args:
         atom: RDKit atom instance.
@@ -508,15 +510,15 @@
     """
     if allowable_set is None:
         allowable_set = CHIRAL_TYPES
     return one_hot_encoding(atom.GetChiralTag(), allowable_set, encode_unknown)
 
 
 def atom_chirality_type_one_hot(
-    atom: rdchem.Atom,
+    atom: dm.Atom,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the chirality type of an atom.
 
      Args:
         atom: RDKit atom instance.
@@ -531,38 +533,38 @@
     if atom.HasProp("_CIPCode"):
         cip_code = atom.GetProp("_CIPCode")
     if allowable_set is None:
         allowable_set = ["R", "S"]
     return one_hot_encoding(cip_code, allowable_set, encode_unknown)
 
 
-def atom_mass(atom: rdchem.Atom, coeff: float = 1):
+def atom_mass(atom: dm.Atom, coeff: float = 1):
     """Get the mass of an atom and scale it.
 
     Args:
         atom: RDKit atom instance.
         coeff: scaling factor for the atom mass
     Returns:
         list: List containing one float only.
     """
     return [atom.GetMass() * coeff]
 
 
-def atom_is_chiral_center(atom: rdchem.Atom):
+def atom_is_chiral_center(atom: dm.Atom):
     """Get whether the atom is chiral center
 
     Args:
         atom: RDKit atom instance.
     Returns:
         list: List containing one bool only.
     """
     return [atom.HasProp("_ChiralityPossible")]
 
 
-def atom_extended_properties(atom: rdchem.Atom, dataset: str = "origin"):
+def atom_extended_properties(atom: dm.Atom, dataset: str = "origin"):
     """Get a full set of atom descriptors
 
     Args:
         atom: RDKit atom instance.
         dataset: which dataset to use to query the atom descriptor.
             One of 'origin', 'elements', 'elements_completed'. Default to "origin".
     Returns:
@@ -579,15 +581,15 @@
     feat = [0 for _ in range(feat_shape)]
     if atom.GetSymbol() in list(data.index):
         feat = list(data.loc[atom.GetSymbol()])
     return feat
 
 
 def bond_type_one_hot(
-    bond: rdchem.Bond,
+    bond: dm.Bond,
     allowable_set: Optional[List[Any]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the type of a bond.
 
     Args:
         bond: RDKit atom instance.
@@ -600,15 +602,15 @@
     """
     if allowable_set is None:
         allowable_set = BOND_TYPES
     return one_hot_encoding(bond.GetBondType(), allowable_set, encode_unknown)
 
 
 def bond_is_conjugated_one_hot(
-    bond: rdchem.Bond,
+    bond: dm.Bond,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for whether the bond is conjugated.
 
     Args:
         bond: RDKit bond instance.
@@ -619,27 +621,27 @@
         list: list of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = [False, True]
     return one_hot_encoding(bond.GetIsConjugated(), allowable_set, encode_unknown)
 
 
-def bond_is_conjugated(bond: rdchem.Bond):
+def bond_is_conjugated(bond: dm.Bond):
     """Get whether the bond is conjugated.
 
     Args:
         bond: RDKit bond instance.
     Returns:
         list: List containing one bool only.
     """
     return [bond.GetIsConjugated()]
 
 
 def bond_is_in_ring_one_hot(
-    bond: rdchem.Bond,
+    bond: dm.Bond,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for whether the bond is in a ring of any size.
 
     Args:
         bond: RDKit bond instance.
@@ -650,27 +652,27 @@
         list: list of boolean values where at most one value is True.
     """
     if allowable_set is None:
         allowable_set = [False, True]
     return one_hot_encoding(bond.IsInRing(), allowable_set, encode_unknown)
 
 
-def bond_is_in_ring(bond: rdchem.Bond):
+def bond_is_in_ring(bond: dm.Bond):
     """Get whether the bond is in ring.
 
     Args:
         bond: RDKit bond instance.
     Returns:
         list: List containing one bool only.
     """
     return [bond.IsInRing()]
 
 
 def bond_stereo_one_hot(
-    bond: rdchem.Bond,
+    bond: dm.Bond,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """One hot encoding for the stereo configuration of a bond.
 
     Args:
         bond: RDKit bond instance.
@@ -682,15 +684,15 @@
     """
     if allowable_set is None:
         allowable_set = BOND_STEREO
     return one_hot_encoding(bond.GetStereo(), allowable_set, encode_unknown)
 
 
 def bond_direction_one_hot(
-    bond: rdchem.Bond,
+    bond: dm.Bond,
     allowable_set: Optional[List[str]] = None,
     encode_unknown: bool = False,
 ):
     """Get a one hot encoding for the direction of a bond.
 
     Args:
         bond: RDKit bond instance.
@@ -702,56 +704,56 @@
 
     """
     if allowable_set is None:
         allowable_set = BOND_DIRECTION
     return one_hot_encoding(bond.GetBondDir(), allowable_set, encode_unknown)
 
 
-def pairwise_2D_dist(mol: rdchem.Mol):
+def pairwise_2D_dist(mol: dm.Mol):
     """Compute the pairwise distance between all pairs of atoms in 2D
 
     Args:
         mol: Input molecule
 
     Returns:
         dist: Matrix of size V^2, 1
     """
     mat = GetDistanceMatrix(mol)
     return mat.reshape(-1, 1)
 
 
 @requires_conformer
-def pairwise_3D_dist(mol: rdchem.Mol, conformer_id: int = -1):
+def pairwise_3D_dist(mol: dm.Mol, conformer_id: int = -1):
     """Compute the pairwise 3D distance between all pair of atoms
 
     Args:
         mol: Input molecule
         conformer_id: conformer id to use
 
     Returns:
         dist: Matrix of size V^2, 1
     """
     mat = Get3DDistanceMatrix(mol, confId=conformer_id)
     return mat.reshape(-1, 1)
 
 
-def pairwise_dist_indicator(mol: rdchem.Mol, max_distance: int = 7):
+def pairwise_dist_indicator(mol: dm.Mol, max_distance: int = 7):
     """Compute the pairwise distance matrix gated by a max distance for the weave featurizer
 
     Args:
         mol: input molecule
         max_distance: maximum distance to use for the thresholding
     """
     dist_mat = torch.from_numpy(pairwise_2D_dist(mol))
     # Elementwise compare if distance is bigger than 0, 1, ..., max_distance - 1
     dist_indicator = (dist_mat > torch.arange(0, max_distance).float()).float()
     return dist_indicator.numpy()
 
 
-def pairwise_bond_indicator(mol: rdchem.Mol, allowable_set: Optional[List[Any]] = None):
+def pairwise_bond_indicator(mol: dm.Mol, allowable_set: Optional[List[Any]] = None):
     """Compute the pairwise bond indicator for weave net
 
     Args:
         mol: input molecule
         allowable_set: bond type to consider
     """
     num_atoms = mol.GetNumAtoms()
@@ -766,15 +768,15 @@
         bond_indicators[begin_atom_idx, end_atom_idx] = bond_type_encoding
         bond_indicators[end_atom_idx, begin_atom_idx] = bond_type_encoding
     # Reshape from (V, V, num_bond_types) to (V^2, num_bond_types)
     bond_indicators = bond_indicators.reshape(-1, len(allowable_set))
     return bond_indicators.numpy()
 
 
-def pairwise_ring_membership(mol: rdchem.Mol):
+def pairwise_ring_membership(mol: dm.Mol):
     """Compute the joint ring membership of all atom pairs
 
     Args:
         mol: Input molecule
 
     Returns:
         ring_membership: Matrix of size V^2, 1
```

### Comparing `molfeat-0.8.6/molfeat/calc/_map4.py` & `molfeat-0.8.7/molfeat/calc/_map4.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Union
 
 import datamol as dm
-from rdkit.Chem import rdchem
 from loguru import logger
 from molfeat.utils import requires
 
 if requires.check("map4"):
     from map4 import MAP4Calculator
 else:
     MAP4Calculator = requires.mock("map4")
 
 
 def MAP4(
-    x: Union[rdchem.Mol, str],
+    x: Union[dm.Mol, str],
     dimensions: int = 2048,
     radius: int = 2,
     is_counted: bool = False,
     is_folded: bool = True,
     return_strings: bool = False,
     **kwargs,
 ):
```

### Comparing `molfeat-0.8.6/molfeat/calc/_mhfp.py` & `molfeat-0.8.7/molfeat/calc/_mhfp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Union
 
 import datamol as dm
 from rdkit.Chem.rdMHFPFingerprint import MHFPEncoder
-from rdkit.Chem import rdchem
 
 
 def MHFP(
-    x: Union[rdchem.Mol, str],
+    x: Union[dm.Mol, str],
     n_permutations: int = 128,
     radius: int = 3,
     min_radius: int = 1,
     rings: bool = True,
     isomeric: bool = False,
     kekulize: bool = False,
     seed: int = 0,
@@ -42,15 +41,15 @@
         kekulize=kekulize,
         min_radius=min_radius,
     )
     return encoded_fp
 
 
 def SECFP(
-    x: Union[rdchem.Mol, str],
+    x: Union[dm.Mol, str],
     n_permutations: int = 128,
     nBits: int = 2048,
     radius: int = 3,
     min_radius: int = 1,
     rings: bool = True,
     isomeric: bool = False,
     kekulize: bool = False,
```

### Comparing `molfeat-0.8.6/molfeat/calc/atom.py` & `molfeat-0.8.7/molfeat/calc/atom.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,24 @@
 
 from collections import defaultdict
 from functools import partial
 from functools import lru_cache
 
 import inspect
 import importlib
+import os
 import datamol as dm
 import numpy as np
-import os
 
 from rdkit import RDConfig
 from rdkit.Chem import AllChem
 from rdkit.Chem import ChemicalFeatures
 from rdkit.Chem import GetSymmSSSR
-from rdkit.Chem import rdchem
 
 from molfeat._version import __version__ as MOLFEAT_VERSION
-from molfeat.utils.commons import hex_to_fn
-from molfeat.utils.commons import fn_to_hex
 from molfeat.calc.base import SerializableCalculator
 from molfeat.calc._atom_bond_features import atom_one_hot
 from molfeat.calc._atom_bond_features import atom_degree_one_hot
 from molfeat.calc._atom_bond_features import atom_extended_properties
 from molfeat.calc._atom_bond_features import atom_implicit_valence_one_hot
 from molfeat.calc._atom_bond_features import atom_hybridization_one_hot
 from molfeat.calc._atom_bond_features import atom_is_aromatic
@@ -38,14 +35,16 @@
 from molfeat.calc._atom_bond_features import atom_chiral_tag_one_hot
 from molfeat.calc._atom_bond_features import atom_partial_charge
 from molfeat.calc._atom_bond_features import DGLLIFE_HYBRIDIZATION_LIST
 from molfeat.calc._atom_bond_features import DGLLIFE_WEAVE_ATOMS
 from molfeat.calc._atom_bond_features import DGLLIFE_WEAVE_CHIRAL_TYPES
 from molfeat.utils import datatype
 from molfeat.utils.commons import concat_dict
+from molfeat.utils.commons import hex_to_fn
+from molfeat.utils.commons import fn_to_hex
 
 
 class AtomCalculator(SerializableCalculator):
     """
     Base class for computing atom properties compatible with DGLLife
     """
 
@@ -72,15 +71,15 @@
         """
         Init function of the atom property calculator
 
         Args:
             featurizer_funcs : Mapping of feature name to the featurization function.
                 For compatibility a list of callable/function is still accepted, and the corresponding
                 featurizer name will be automatically generated. Each function is of signature
-                ``func(rdkit.Chem.rdchem.Atom) -> list or 1D numpy array``.
+                ``func(dm.Atom) -> list or 1D numpy array``.
             concat: Whether to concat all the data into a single value in the output dict
             name: Name of the key name of the concatenated features
         """
         self._input_kwargs = locals().copy()
         self._input_kwargs.pop("self")
         # we also remove the featurizer funcs
         self._input_kwargs.pop("featurizer_funcs", None)
@@ -189,15 +188,15 @@
             self._feat_sizes[feat_name] = len(self.featurizer_funcs[feat_name](atom))
         return self._feat_sizes[feat_name]
 
     def __len__(self):
         """Get length of the property estimator"""
         return sum(v for k, v in self._feat_sizes.items() if k != self.name)
 
-    def __call__(self, mol: Union[rdchem.Mol, str], dtype: Callable = None):
+    def __call__(self, mol: Union[dm.Mol, str], dtype: Callable = None):
         """
         Get rdkit basic descriptors for a molecule
 
         Args:
             mol: the molecule of interest
             dtype: requested data type
 
@@ -318,19 +317,26 @@
                     is_donor[u] = True
             elif feats.GetFamily() == "Acceptor":
                 nodes = feats.GetAtomIds()
                 for u in nodes:
                     is_acceptor[u] = True
         return is_donor, is_acceptor
 
-    @lru_cache
-    def _compute_weave_net_properties(self, mol: rdchem.Mol):
-        # Get information for donor and acceptor
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _feat_factory_cache():
+        """Build and cache chemical features caching for speed"""
         fdef_name = os.path.join(RDConfig.RDDataDir, "BaseFeatures.fdef")
         chem_feats = ChemicalFeatures.BuildFeatureFactory(fdef_name)
+        return chem_feats
+
+    @lru_cache
+    def _compute_weave_net_properties(self, mol: dm.Mol):
+        # Get information for donor and acceptor
+        chem_feats = self._feat_factory_cache()
         mol_feats = chem_feats.GetFeaturesForMol(mol)
         is_donor, is_acceptor = self._get_atom_state_info(mol_feats)
         sssr = GetSymmSSSR(mol)
         num_atoms = mol.GetNumAtoms()
         atom_features = []
         for i in range(num_atoms):
             cur_atom_props = [float(is_donor[i]), float(is_acceptor[i])]
@@ -340,21 +346,21 @@
                 ring_size = len(ring)
                 if i in ring and 3 <= ring_size <= 8:
                     count[ring_size - 3] += 1
             cur_atom_props.extend(count)
             atom_features.append(cur_atom_props)
         return atom_features
 
-    def atom_weave_props(self, atom: rdchem.Atom):
+    def atom_weave_props(self, atom: dm.Atom):
         """Get the WeaveNet properties for an atom"""
         mol = atom.GetOwningMol()
         feats = self._compute_weave_net_properties(mol)
         return feats[atom.GetIdx()]
 
-    def __call__(self, mol: Union[rdchem.Mol, str], dtype: Callable = None):
+    def __call__(self, mol: Union[dm.Mol, str], dtype: Callable = None):
         """
         Get rdkit basic descriptors for a molecule
 
         Args:
             mol: the molecule of interest
             dtype: requested data type
```

### Comparing `molfeat-0.8.6/molfeat/calc/base.py` & `molfeat-0.8.7/molfeat/calc/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/calc/bond.py` & `molfeat-0.8.7/molfeat/calc/bond.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from collections import defaultdict
 
 import importlib
 import inspect
 import datamol as dm
 import numpy as np
 
-from rdkit.Chem import rdchem
-
 from molfeat._version import __version__ as MOLFEAT_VERSION
 from molfeat.calc.base import SerializableCalculator
 from molfeat.calc._atom_bond_features import bond_type_one_hot
 from molfeat.calc._atom_bond_features import bond_is_conjugated
 from molfeat.calc._atom_bond_features import bond_is_in_ring
 from molfeat.calc._atom_bond_features import bond_direction_one_hot
 from molfeat.calc._atom_bond_features import bond_stereo_one_hot
@@ -174,15 +172,15 @@
             self._feat_sizes[feat_name] = len(self.featurizer_funcs[feat_name](bond))
         return self._feat_sizes[feat_name]
 
     def __len__(self):
         """Get length of the property estimator"""
         return sum(v for k, v in self._feat_sizes.items() if k != self.name)
 
-    def __call__(self, mol: Union[rdchem.Mol, str], dtype: Callable = None, **kwargs):
+    def __call__(self, mol: Union[dm.Mol, str], dtype: Callable = None, **kwargs):
         """Featurize all bonds in a molecule.
 
         Args:
             mol: the molecule of interest
             dtype: requested data type
 
         Returns:
@@ -347,15 +345,15 @@
                 self._feat_sizes[feat_name] = self.pairwise_atom_funcs[feat_name](
                     self._toy_mol
                 ).shape[-1]
             else:
                 raise ValueError(f"Feature name {feat_name} is not defined !")
         return self._feat_sizes[feat_name]
 
-    def __call__(self, mol: Union[rdchem.Mol, str], dtype: Callable = None, flat: bool = True):
+    def __call__(self, mol: Union[dm.Mol, str], dtype: Callable = None, flat: bool = True):
         """Featurize all bonds in a molecule.
 
         Args:
             mol: the molecule of interest
             dtype: requested data type
             flat: whether to return a collapsed N^2, M or a N, N, M matrix
```

### Comparing `molfeat-0.8.6/molfeat/calc/cats.py` & `molfeat-0.8.7/molfeat/calc/cats.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from collections import defaultdict as ddict
 import functools
 
 import datamol as dm
 import numpy as np
 
-from rdkit.Chem import rdchem
 from rdkit.Chem.rdmolops import GetDistanceMatrix
 from rdkit.Chem.rdmolops import Get3DDistanceMatrix
 
 from molfeat.utils.datatype import to_numpy
 from molfeat.calc.base import SerializableCalculator
 
 
@@ -150,15 +149,15 @@
         smarts_mols = ddict(list)
         for label, patterns in smarts_dict.items():
             patterns = [dm.from_smarts(patt) for patt in patterns]
             smarts_mols[label] = patterns
 
         return smarts_mols
 
-    def _get_pcore_group(self, mol: Union[rdchem.Mol, str]):
+    def _get_pcore_group(self, mol: Union[dm.Mol, str]):
         """
         Assign a PPP (potential pharmacophore points) to individual atoms of a molecule.
 
         !!! note
             The return value is a list of length `N_atoms` of the
             input molecule. The i'th element of the list contains
             a list of PPP labels that were identified for the i'th atom
```

### Comparing `molfeat-0.8.6/molfeat/calc/descriptors.py` & `molfeat-0.8.7/molfeat/calc/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import copy
 from typing import Union, List, Optional
 from collections import OrderedDict
 
-
 import datamol as dm
 import numpy as np
 
 from loguru import logger
-
 from rdkit.Chem.QED import properties
 from rdkit.Chem import Descriptors
 from rdkit.Chem import Descriptors3D
-from rdkit.Chem import rdchem
 from rdkit.Chem import FindMolChiralCenters
 from rdkit.Chem import rdPartialCharges
 from rdkit.Chem import rdMolDescriptors
 
-
 from molfeat.utils.commons import requires_conformer
 from molfeat.utils.commons import requires_standardization
 from molfeat.utils.datatype import to_numpy
 from molfeat.utils import requires
 from molfeat.calc.base import SerializableCalculator
 
 if requires.check("mordred"):
@@ -113,15 +109,15 @@
         state["_columns"] = self._columns
 
         # EN: set `avg_ipc` and `standardize`` default value to False for compat until next release
         state["avg_ipc"] = getattr(self, "avg_ipc", False)
         state["do_not_standardize"] = getattr(self, "do_not_standardize", False)
         return state
 
-    def _compute_extra_features(self, mol: Union[rdchem.Mol, str]):
+    def _compute_extra_features(self, mol: Union[dm.Mol, str]):
         """Compute the extra properties required for the augmented features version
 
         Args:
             mol: Input molecule
 
         Returns:
             props (dict): Dict of extra molecular properties
@@ -144,15 +140,15 @@
         return self._columns
 
     def __len__(self):
         """Return the length of the calculator"""
         return len(self._columns)
 
     @requires_standardization(disconnect_metals=True, remove_salt=True)
-    def __call__(self, mol: Union[rdchem.Mol, str]):
+    def __call__(self, mol: Union[dm.Mol, str]):
         r"""
         Get rdkit basic descriptors for a molecule
 
         Args:
             mol: the molecule of interest
 
         Returns:
@@ -244,15 +240,15 @@
         return state
 
     def __setstate__(self, state: dict):
         """Reload the class from pickling."""
         self.__dict__.update(state)
         self._init_calc()
 
-    def __call__(self, mol: Union[rdchem.Mol, str], conformer_id: Optional[int] = -1):
+    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1):
         r"""
         Get rdkit basic descriptors for a molecule
 
         Args:
             mol: the molecule of interest
             conformer_id (int, optional): Optional
 
@@ -330,15 +326,15 @@
 
     @property
     def columns(self):
         """Get the descriptors columns"""
         return self._columns
 
     @requires_conformer
-    def __call__(self, mol: Union[rdchem.Mol, str], conformer_id: Optional[int] = -1):
+    def __call__(self, mol: Union[dm.Mol, str], conformer_id: Optional[int] = -1):
         r"""
         Get rdkit 3D descriptors for a molecule
 
         Args:
             mol: the molecule of interest
             conformer_id (int, optional): Optional conformer id. Defaults to -1.
```

### Comparing `molfeat-0.8.6/molfeat/calc/fingerprints.py` & `molfeat-0.8.7/molfeat/calc/fingerprints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-#!
 from typing import Union
 from typing import Optional
 
 from functools import partial
 
 import copy
 import datamol as dm
 from rdkit.Avalon import pyAvalonTools
 from rdkit.Chem import rdMolDescriptors
 from rdkit.Chem import rdReducedGraphs
 from rdkit.Chem import rdmolops
-from rdkit.Chem import rdchem
 from rdkit.Chem.EState import Fingerprinter as EStateFingerprinter
 
 from loguru import logger
 from molfeat.calc._mhfp import SECFP
 from molfeat.calc._map4 import MAP4
 from molfeat.calc.base import SerializableCalculator
 from molfeat.utils.datatype import to_numpy, to_fp
@@ -289,15 +287,15 @@
             len_key = "dimensions"
             fplen = self.params[len_key]
         if len_key is not None and length:
             self.params[len_key] = length
             fplen = length
         return fplen
 
-    def __call__(self, mol: Union[rdchem.Mol, str], raw: bool = False):
+    def __call__(self, mol: Union[dm.Mol, str], raw: bool = False):
         r"""
         Compute the Fingerprint of a molecule
 
         Args:
             mol: the molecule of interest
             raw: whether to keep original datatype or convert to numpy. Useful for rdkit's similarity functions
```

### Comparing `molfeat-0.8.6/molfeat/calc/pharmacophore.py` & `molfeat-0.8.7/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/calc/shape.py` & `molfeat-0.8.7/molfeat/calc/shape.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/calc/skeys.py` & `molfeat-0.8.7/molfeat/calc/skeys.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 import pandas as pd
 import datamol as dm
 
 from collections import defaultdict as ddict
 from pathlib import Path
 from loguru import logger
 from rdkit import Chem
-from rdkit.Chem import rdchem
 from rdkit.Chem import rdMolDescriptors as Desc
 from rdkit.Chem.rdmolops import GetFormalCharge
 from rdkit.Chem.Scaffolds import MurckoScaffold
 from molfeat.calc.base import SerializableCalculator
 
 import molfeat
 
 
-def _is_ring_fully_conjugated(mol: rdchem.Mol, ring: list):
+def _is_ring_fully_conjugated(mol: dm.Mol, ring: list):
     """Check whether a ring is fully conjugated"""
     suppl = Chem.ResonanceMolSupplier(mol)
     first_idx_conj = -1
     first = True
     for i in range(len(ring)):
         atom_idx = ring[i]
         atom_conj_grp_idx = Chem.ResonanceMolSupplier.GetAtomConjGrpIdx(suppl, atom_idx)
@@ -34,15 +33,15 @@
             first = False
         else:
             if atom_conj_grp_idx != first_idx_conj:
                 return False
     return True
 
 
-def _n_multiple_bond_in_ring(mol: rdchem.Mol, ring: list):
+def _n_multiple_bond_in_ring(mol: dm.Mol, ring: list):
     """Get number of multiple bonds in a ring"""
     atom_i = -1
     atom_j = -1
     bond = None
     nr_multiple_bonds = 0
     multiple_bond_types = [2, 3, 12]
     for i in range(len(ring)):
@@ -53,25 +52,25 @@
             if bond is not None:
                 bond_type = Chem.Bond.GetBondType(bond)
                 if int(bond_type) in multiple_bond_types:
                     nr_multiple_bonds += 1
     return nr_multiple_bonds
 
 
-def _count_heteroatom_per_ring(mol: rdchem.Mol, rings: list):
+def _count_heteroatom_per_ring(mol: dm.Mol, rings: list):
     """Count number of heteroatoms in rings"""
     n_heteros = [0] * len(rings)
     for i, ring in enumerate(rings):
         for atom in ring:
             is_hetero = int(mol.GetAtomWithIdx(atom).GetAtomicNum() not in [1, 6])
             n_heteros[i] += is_hetero
     return n_heteros
 
 
-def _get_ring_system(mol: rdchem.Mol):
+def _get_ring_system(mol: dm.Mol):
     """Build ring systems in a molecule"""
     q = mol.GetRingInfo()
     simple_rings = q.AtomRings()
     rings = [set(r) for r in simple_rings]
     ring_map = [set([x]) for x in range(len(rings))]
     go_next = True
     while go_next:
@@ -87,15 +86,15 @@
                 ring_map.append(new_map)
 
                 go_next = True
                 break
     return list(simple_rings), rings, ring_map
 
 
-def _ring_atom_state(mol: rdchem.Mol):
+def _ring_atom_state(mol: dm.Mol):
     """Get the conjugated state of ring atoms"""
     ri = mol.GetRingInfo()
     ring_atom_conj_state = ddict(list)
     for ring in ri.AtomRings():
         state = _is_ring_fully_conjugated(mol, ring)
         for atom in ring:
             ring_atom_conj_state[atom].append(state)
@@ -187,173 +186,173 @@
     @classmethod
     def compute_normalization(cls, features: np.ndarray):
         """Normalize input features. The normalization parameters are
         computed by the scaffolds of 2.1M molecules from CHEMBL 29.
         """
         return (features - cls.NORM_PARAMS["mean"]) / cls.NORM_PARAMS["std"]
 
-    def n_atom_in_rings(self, mol: rdchem.Mol):
+    def n_atom_in_rings(self, mol: dm.Mol):
         """1. number of ring atoms"""
         sm = dm.from_smarts("[r]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_atom_in_conjugated_ring(self, mol: rdchem.Mol):
+    def n_atom_in_conjugated_ring(self, mol: dm.Mol):
         """2. number of atoms in conjugated rings"""
         ri = mol.GetRingInfo()
         n = 0
         for ring in ri.AtomRings():
             if _is_ring_fully_conjugated(mol, ring):
                 n += len(ring)
         return n
 
-    def n_atoms_not_in_conjugated_ring(self, mol: rdchem.Mol):
+    def n_atoms_not_in_conjugated_ring(self, mol: dm.Mol):
         """
         3. number of atoms not in conjugated rings
         (i.e. atoms in aliphatic rings and non-ring atoms)
         """
         # EN: replace conjugation by aromatic
         ri = mol.GetRingInfo()
         n = 0
         for ring in ri.AtomRings():
             if not _is_ring_fully_conjugated(mol, ring):
                 n += len(ring)
         return n
 
-    def n_atom_in_chain(self, mol: rdchem.Mol):
+    def n_atom_in_chain(self, mol: dm.Mol):
         """4. number atoms in chains (not counting double-connected exo-chain atoms)"""
         sm = dm.from_smarts("[!r;!$(*=[r])]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_atom_exocyclic(self, mol: rdchem.Mol):
+    def n_atom_exocyclic(self, mol: dm.Mol):
         """5. number of exocyclic atoms (connected by multiple bonds to a ring)"""
         sm = dm.from_smarts("[!r;!$(*-[r])&$(*~[r])]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_nitrogen(self, mol: rdchem.Mol):
+    def n_nitrogen(self, mol: dm.Mol):
         """6. number of nitrogen"""
         sm = dm.from_smarts("[#7]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_nitrogen_in_ring(self, mol: rdchem.Mol):
+    def n_nitrogen_in_ring(self, mol: dm.Mol):
         """7. number of nitrogen in rings"""
         sm = dm.from_smarts("[#7;r]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_oxygen(self, mol: rdchem.Mol):
+    def n_oxygen(self, mol: dm.Mol):
         """8. number of oxygen"""
         sm = dm.from_smarts("[#8]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_oxygen_in_ring(self, mol: rdchem.Mol):
+    def n_oxygen_in_ring(self, mol: dm.Mol):
         """9. number of oxygen in rings"""
         sm = dm.from_smarts("[#8]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_sulfur(self, mol: rdchem.Mol):
+    def n_sulfur(self, mol: dm.Mol):
         """10. number of sulfur atoms"""
         sm = dm.from_smarts("[#16]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_heteroatoms(self, mol: rdchem.Mol):
+    def n_heteroatoms(self, mol: dm.Mol):
         """11. number of heteroatoms"""
 
         sm = dm.from_smarts("[!#1&!#6]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_heteroatoms_in_ring(self, mol: rdchem.Mol):
+    def n_heteroatoms_in_ring(self, mol: dm.Mol):
         """12. number of heteroatoms in rings"""
         sm = dm.from_smarts("[!#1&!#6&r]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_atom_spiro_atoms(self, mol: rdchem.Mol):
+    def n_atom_spiro_atoms(self, mol: dm.Mol):
         """13. number of spiro atoms"""
         return Desc.CalcNumSpiroAtoms(mol)
 
-    def n_heteroatom_more_than_2_conn(self, mol: rdchem.Mol):
+    def n_heteroatom_more_than_2_conn(self, mol: dm.Mol):
         """14. number of heteroatoms with more than 2 connections"""
         sm = dm.from_smarts("[!#1;!#6;!D1!D0;!D2]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_carbon_atleast_2_heteroatoms(self, mol: rdchem.Mol):
+    def n_carbon_atleast_2_heteroatoms(self, mol: dm.Mol):
         """15. number of carbon atoms connected to at least 2 heteroatoms"""
         n_atoms = 0
         for atom in mol.GetAtoms():
             tmp = [x for x in atom.GetNeighbors() if x.GetAtomicNum() not in [1, 6]]
             n_atoms += len(tmp) >= 2
         return n_atoms
 
-    def n_atom_at_least_2_nei_more_than_2_conn(self, mol: rdchem.Mol):
+    def n_atom_at_least_2_nei_more_than_2_conn(self, mol: dm.Mol):
         """16. Number of atoms where at least 2 connected atoms have more than 2 connections"""
         n_atoms = 0
         for atom in mol.GetAtoms():
             tmp = [x for x in atom.GetNeighbors() if len(x.GetNeighbors()) > 2]
             n_atoms += len(tmp) > 2
         return n_atoms
 
-    def abs_scaffold_format_charge(self, mol: rdchem.Mol):
+    def abs_scaffold_format_charge(self, mol: dm.Mol):
         """17. absolute value of the scaffold formal charge"""
         charge = GetFormalCharge(mol)
         return abs(charge)
 
-    def n_bonds(self, mol: rdchem.Mol):
+    def n_bonds(self, mol: dm.Mol):
         """18. number of bonds"""
         return mol.GetNumBonds()
 
-    def n_multiple_non_conj_ring_bonds(self, mol: rdchem.Mol):
+    def n_multiple_non_conj_ring_bonds(self, mol: dm.Mol):
         """19. number of multiple, nonconjugated ring bonds"""
         extracted_rings = []
         nr_multiple_bonds_infcr = 0  # infcr: in not fully conjugated ring
         rings = Chem.GetSymmSSSR(mol)
         for i in range(len(rings)):
             extracted_rings.append(list(rings[i]))
         for ring in extracted_rings:
             if not _is_ring_fully_conjugated(mol, ring):
                 nr_multiple_bonds_infcr += _n_multiple_bond_in_ring(mol, ring)
         return nr_multiple_bonds_infcr
 
-    def n_bonds_2_heteroatoms(self, mol: rdchem.Mol):
+    def n_bonds_2_heteroatoms(self, mol: dm.Mol):
         """20. number of bonds connecting 2 heteroatoms"""
         sm = dm.from_smarts("[!#1&!#6]~[!#1&!#6]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_carbon_het_carbon_het_bonds(self, mol: rdchem.Mol):
+    def n_carbon_het_carbon_het_bonds(self, mol: dm.Mol):
         """21. number of bonds connecting 2 heteroatoms through 2 carbons"""
         sm = dm.from_smarts("[!#1&!#6]~[#6]~[#6]~[!#1&!#6]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_bonds_at_least_3_conn(self, mol: rdchem.Mol):
+    def n_bonds_at_least_3_conn(self, mol: dm.Mol):
         """22. number of bonds with at least 3 connections on both its atoms"""
         sm = dm.from_smarts("[$([!#1](~[!#1])(~[!#1])~[!#1])][$([!#1](~[!#1])(~[!#1])~[!#1])]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_exocyclic_single_bonds_carbon(self, mol: rdchem.Mol):
+    def n_exocyclic_single_bonds_carbon(self, mol: dm.Mol):
         """23. number of exocyclic single bonds where a ring atom is carbon"""
         sm = dm.from_smarts("[!R;!#1]-[#6;R]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_exocyclic_single_bonds_nitrogen(self, mol: rdchem.Mol):
+    def n_exocyclic_single_bonds_nitrogen(self, mol: dm.Mol):
         """24. number of exocyclic single bonds where a ring atom is nitrogen"""
         sm = dm.from_smarts("[!R;!#1]-[#7;R]")
         return len(mol.GetSubstructMatches(sm, uniquify=True))
 
-    def n_non_ring_bonds_2_conj_rings(self, mol: rdchem.Mol):
+    def n_non_ring_bonds_2_conj_rings(self, mol: dm.Mol):
         """25. number of non-ring bonds connecting 2 nonconjugated rings"""
         # EN: this is interpretated literally as bonds and not path
         ring_atom_conj_state = _ring_atom_state(mol)
         sm = dm.from_smarts("[R:1]!@[R:2]")
         bond_list = mol.GetSubstructMatches(sm, uniquify=True)
         result = 0
         for a_start, a_end in bond_list:
             s_state = ring_atom_conj_state.get(a_start)
             e_state = ring_atom_conj_state.get(a_end)
             if False in s_state and False in e_state:
                 result += 1
         return result
 
-    def n_non_ring_bonds_conj_nonconj_rings(self, mol: rdchem.Mol):
+    def n_non_ring_bonds_conj_nonconj_rings(self, mol: dm.Mol):
         """
         26. number of non-ring bonds connecting 2 rings,
         one of them conjugated and one non-conjugated
         """
         # EN: this is interpretated literally as bonds and not path
 
         ring_atom_conj_state = _ring_atom_state(mol)
@@ -363,15 +362,15 @@
         for a_start, a_end in bond_list:
             s_state = ring_atom_conj_state.get(a_start)
             e_state = ring_atom_conj_state.get(a_end)
             if (True in s_state and False in e_state) or (False in s_state and True in e_state):
                 result += 1
         return result
 
-    def n_bonds_atoms_with_at_least_one_nei_with_2_conn(self, mol: rdchem.Mol):
+    def n_bonds_atoms_with_at_least_one_nei_with_2_conn(self, mol: dm.Mol):
         """
         27. number of bonds where both atoms have at least one neighbor
         (not considering the bond atoms) with more than 2 connections
         """
         result = 0
         huge_conn = list(
             itertools.chain(*mol.GetSubstructMatches(dm.from_smarts("[*;!D0;!D1;!D2]"), uniquify=1))
@@ -384,134 +383,134 @@
             ]
             if any([x.GetIdx() in allowed_conn_table for x in a_start.GetNeighbors()]) and any(
                 [y.GetIdx() in allowed_conn_table for y in a_end.GetNeighbors()]
             ):
                 result += 1
         return result
 
-    def n_simple_rings(self, mol: rdchem.Mol):
+    def n_simple_rings(self, mol: dm.Mol):
         """28. number of simple rings"""
         ri = mol.GetRingInfo()
         return ri.NumRings()
 
-    def size_largest_ring(self, mol: rdchem.Mol):
+    def size_largest_ring(self, mol: dm.Mol):
         """29. Size of the largest ring"""
         ri = mol.GetRingInfo()
         max_ring_size = max((len(r) for r in ri.AtomRings()), default=0)
         return max_ring_size
 
-    def n_simple_rings_no_heteroatoms(self, mol: rdchem.Mol):
+    def n_simple_rings_no_heteroatoms(self, mol: dm.Mol):
         """30. number of simple rings with no heteroatoms"""
         ri = mol.GetRingInfo()
         n_heteros = _count_heteroatom_per_ring(mol, ri.AtomRings())
         return sum(1 for x in n_heteros if x == 0)
 
-    def n_simple_rings_1_heteroatoms(self, mol: rdchem.Mol):
+    def n_simple_rings_1_heteroatoms(self, mol: dm.Mol):
         """31. number of simple rings with 1 heteroatom"""
         ri = mol.GetRingInfo()
         n_heteros = _count_heteroatom_per_ring(mol, ri.AtomRings())
         return sum(1 for x in n_heteros if x == 1)
 
-    def n_simple_rings_2_heteroatoms(self, mol: rdchem.Mol):
+    def n_simple_rings_2_heteroatoms(self, mol: dm.Mol):
         """32. number of simple rings with 2 heteroatom"""
         ri = mol.GetRingInfo()
         n_heteros = _count_heteroatom_per_ring(mol, ri.AtomRings())
         return sum(1 for x in n_heteros if x == 2)
 
-    def n_simple_rings_at_least_3_heteroatoms(self, mol: rdchem.Mol):
+    def n_simple_rings_at_least_3_heteroatoms(self, mol: dm.Mol):
         """33. number of simple rings with 3 or more heteroatoms"""
         ri = mol.GetRingInfo()
         n_heteros = _count_heteroatom_per_ring(mol, ri.AtomRings())
         return sum(1 for x in n_heteros if x >= 3)
 
-    def n_simple_non_conj_5_atoms_rings(self, mol: rdchem.Mol):
+    def n_simple_non_conj_5_atoms_rings(self, mol: dm.Mol):
         """34. number of simple non-conjugated rings with 5 atoms"""
         ri = mol.GetRingInfo()
         n = 0
         for ring in ri.AtomRings():
             if not _is_ring_fully_conjugated(mol, ring) and len(ring) == 5:
                 n += 1
         return n
 
-    def n_simple_non_conj_6_atoms_rings(self, mol: rdchem.Mol):
+    def n_simple_non_conj_6_atoms_rings(self, mol: dm.Mol):
         """35. number of simple non-conjugated rings with 6 atoms"""
         ri = mol.GetRingInfo()
         n = 0
         for ring in ri.AtomRings():
             if not _is_ring_fully_conjugated(mol, ring) and len(ring) == 6:
                 n += 1
         return n
 
-    def n_ring_system(self, mol: rdchem.Mol):
+    def n_ring_system(self, mol: dm.Mol):
         """36. number of ring systems"""
         simple_rings, ring_system, _ = _get_ring_system(mol)
         return len(ring_system)
 
-    def n_ring_system_with_2_non_conj_simple_ring(self, mol: rdchem.Mol):
+    def n_ring_system_with_2_non_conj_simple_ring(self, mol: dm.Mol):
         """37. number of rings systems with 2 non-conjugated simple rings"""
         simple_rings, _, ring_map = _get_ring_system(mol)
         conj_rings_map = dict(
             (i, _is_ring_fully_conjugated(mol, x)) for i, x in enumerate(simple_rings)
         )
         result = 0
         for ring_set in ring_map:
             n_not_conj = sum(not conj_rings_map[rnum] for rnum in ring_set)
             result += n_not_conj == 2
         return result
 
-    def n_ring_system_with_2_conj_simple_ring(self, mol: rdchem.Mol):
+    def n_ring_system_with_2_conj_simple_ring(self, mol: dm.Mol):
         """38. number of rings systems with 2 conjugated simple rings"""
         simple_rings, _, ring_map = _get_ring_system(mol)
         conj_rings_map = dict(
             (i, _is_ring_fully_conjugated(mol, x)) for i, x in enumerate(simple_rings)
         )
         result = 0
         for ring_set in ring_map:
             n_conj = sum(conj_rings_map[rnum] for rnum in ring_set)
             result += n_conj == 2
         return result
 
-    def n_ring_system_with_conj_non_conj_simple_ring(self, mol: rdchem.Mol):
+    def n_ring_system_with_conj_non_conj_simple_ring(self, mol: dm.Mol):
         """39 number of ring system containing 2 simple rings, one conjugated and one nonconjugated"""
         simple_rings, _, ring_map = _get_ring_system(mol)
         conj_rings_map = dict(
             (i, _is_ring_fully_conjugated(mol, x)) for i, x in enumerate(simple_rings)
         )
         result = 0
         for ring_set in ring_map:
             if len(ring_set) == 2:
                 n_conj = sum(conj_rings_map[rnum] for rnum in ring_set)
                 result += n_conj == 1
         return result
 
-    def n_ring_system_with_3_conj_simple_ring(self, mol: rdchem.Mol):
+    def n_ring_system_with_3_conj_simple_ring(self, mol: dm.Mol):
         """40. number of rings systems with 3 conjugated simple rings"""
         simple_rings, _, ring_map = _get_ring_system(mol)
         conj_rings_map = dict(
             (i, _is_ring_fully_conjugated(mol, x)) for i, x in enumerate(simple_rings)
         )
         result = 0
         for ring_set in ring_map:
             n_conj = sum(conj_rings_map[rnum] for rnum in ring_set)
             result += n_conj == 3
         return result
 
-    def n_ring_system_with_3_non_conj_simple_ring(self, mol: rdchem.Mol):
+    def n_ring_system_with_3_non_conj_simple_ring(self, mol: dm.Mol):
         """41. number of rings systems with 3 non-conjugated simple rings"""
         simple_rings, _, ring_map = _get_ring_system(mol)
         conj_rings_map = dict(
             (i, _is_ring_fully_conjugated(mol, x)) for i, x in enumerate(simple_rings)
         )
         result = 0
         for ring_set in ring_map:
             n_not_conj = sum(not conj_rings_map[rnum] for rnum in ring_set)
             result += n_not_conj == 3
         return result
 
-    def n_ring_system_with_greater_one_conj_nonconj_simple_ring(self, mol: rdchem.Mol):
+    def n_ring_system_with_greater_one_conj_nonconj_simple_ring(self, mol: dm.Mol):
         """42. number of ring system containing 3 simple rings, at least one conjugated and one nonconjugated"""
         simple_rings, _, ring_map = _get_ring_system(mol)
         conj_rings_map = dict(
             (i, _is_ring_fully_conjugated(mol, x)) for i, x in enumerate(simple_rings)
         )
         result = 0
         for ring_set in ring_map:
@@ -521,15 +520,15 @@
         return result
 
     @property
     def columns(self):
         """Get the name of all the descriptors of this calculator"""
         return list(self.DESCRIPTORS)
 
-    def __call__(self, mol: Union[rdchem.Mol, str]):
+    def __call__(self, mol: Union[dm.Mol, str]):
         r"""
         Compute the Fingerprint of a molecule
 
         Args:
             mol: the molecule of interest
 
         Returns:
```

### Comparing `molfeat-0.8.6/molfeat/calc/tree.py` & `molfeat-0.8.7/molfeat/calc/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 from typing import List
 from typing import Union
 from typing import Tuple
 from typing import Optional
 from collections import defaultdict
 
 import os
-import copy
 import pathlib
 import platformdirs
 import fsspec
 import datamol as dm
 
 from loguru import logger
 from joblib import Memory
 from scipy.sparse import csr_matrix
 from scipy.sparse.csgraph import minimum_spanning_tree
-from rdkit.Chem import rdchem
 from rdkit.Chem import GetSymmSSSR
 from rdkit.Chem import MolFragmentToSmiles
 
 MAX_W = 1000
 MST_MAX_WEIGHT = 100
 
 
@@ -48,15 +46,15 @@
             self.tmp_dir = None
         memory = Memory(self.tmp_dir, verbose=1)
         if self.cache:
             self.decomposition_into_tree = memory.cache(
                 self.decomposition_into_tree, ignore=["self", "mol"]
             )
 
-    def decomposition_into_tree(self, mol: rdchem.Mol, inchikey: str = None):
+    def decomposition_into_tree(self, mol: dm.Mol, inchikey: str = None):
         """
         Find the maximum spanning tree over all the clusters of a molecule
 
         Args:
             mol: The molecule of interest
             inchikey: Optional inchi key of the molecule
 
@@ -147,15 +145,15 @@
         junc_tree = minimum_spanning_tree(clique_graph)
         row, col = junc_tree.nonzero()
         edges = [(row[i], col[i]) for i in range(len(row))]
         return cliques, edges, frags
 
     def __call__(
         self,
-        mol: Union[rdchem.Mol, str],
+        mol: Union[dm.Mol, str],
         as_smiles: bool = True,
     ):
         """
         Find the maximum spanning tree over all the clusters of a molecule
 
         Args:
             mol: the molecule of interest
@@ -165,25 +163,25 @@
         cliques, edges, frags = self.decomposition_into_tree(mol, dm.to_inchikey(mol))
         if not as_smiles:
             frags = [dm.to_mol(x) for x in frags]
         return cliques, edges, frags
 
     def get_vocab(
         self,
-        mol_list: List[Union[str, rdchem.Mol]],
+        mol_list: List[Union[str, dm.Mol]],
         output_file: Optional[os.PathLike] = None,
         log: bool = False,
     ):
         r"""
         Generate the list of all possible fragments given a set of molecules.
         This can be useful to build the vocabulary of fragments that can be found in a dataset of molecule
         before doing some learning.
 
         Args:
-            mol_list (Iterable[rdchem.Mo]): A collection of molecules
+            mol_list (Iterable[dm.Mol]): A collection of molecules
             output_file: path to a file that will be used to store the generated set of fragments.
             log (bool, optional): Whether to print intermediate results to stdout
 
         Returns:
             res (List[str]): List of the smiles of all fragments found in the molecule collection
         """
         res = set()
```

### Comparing `molfeat-0.8.6/molfeat/data/cats_features.fdef` & `molfeat-0.8.7/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/data/elements.xz` & `molfeat-0.8.7/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/data/elements_completed.xz` & `molfeat-0.8.7/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/data/origin.xz` & `molfeat-0.8.7/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/data/skey_parameters.csv` & `molfeat-0.8.7/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/plugins/entry_point.py` & `molfeat-0.8.7/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/plugins/factories.py` & `molfeat-0.8.7/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/store/loader.py` & `molfeat-0.8.7/molfeat/store/loader.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/store/modelcard.py` & `molfeat-0.8.7/molfeat/store/modelcard.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Args:
         card: model card to use
     """
     if card.group == "all" and card.type != "pretrained":
         import_statement = "from molfeat.trans import MoleculeTransformer"
         loader_statement = f"MoleculeTransformer(featurizer='{card.name}')"
     elif card.group in ["rdkit", "fp"]:
-        import_statement = f"from molfeat.trans import FPVecTransformer"
+        import_statement = f"from molfeat.trans.fp import FPVecTransformer"
         loader_statement = f"FPVecTransformer(kind='{card.name}')"
     elif card.group == "dgllife":
         import_statement = "from molfeat.trans.pretrained import PretrainedDGLTransformer"
         loader_statement = f"PretrainedDGLTransformer(kind='{card.name}')"
     elif card.group == "graphormer":
         import_statement = "from molfeat.trans.pretrained import GraphormerTransformer"
         loader_statement = f"GraphormerTransformer(kind='{card.name}')"
```

### Comparing `molfeat-0.8.6/molfeat/store/modelstore.py` & `molfeat-0.8.7/molfeat/store/modelstore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/trans/base.py` & `molfeat-0.8.7/molfeat/trans/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import yaml
 import fsspec
 import pandas as pd
 import datamol as dm
 import numpy as np
 
-from rdkit.Chem import rdchem
 from sklearn.base import TransformerMixin
 from sklearn.base import BaseEstimator
 from loguru import logger
 
 from molfeat._version import __version__ as MOLFEAT_VERSION
 
 from molfeat.calc import get_calculator
@@ -219,15 +218,15 @@
 
     def __setstate__(self, state):
         state.pop("callbacks", None)
         self.__dict__.update(state)
         self.__dict__["parallel_kwargs"] = state.get("parallel_kwargs", {})
         self._update_params()
 
-    def fit(self, X: List[Union[rdchem.Mol, str]], y: Optional[list] = None, **fit_params):
+    def fit(self, X: List[Union[dm.Mol, str]], y: Optional[list] = None, **fit_params):
         """Fit the current transformer on given dataset.
 
         The goal of fitting is for example to identify nan columns values
         that needs to be removed from the dataset
 
         Args:
             X: input list of molecules
@@ -241,21 +240,21 @@
         if lengths:
             # we will ignore all nan
             feats = datatype.to_numpy([f for f in feats if not datatype.is_null(f)])
             self.cols_to_keep = (~np.any(np.isnan(feats), axis=0)).nonzero()[0]
         self._fitted = True
         return self
 
-    def _transform(self, mol: rdchem.Mol):
+    def _transform(self, mol: dm.Mol):
         r"""
         Compute features for a single molecule.
         This method would potentially need to be reimplemented by child classes
 
         Args:
-            mol (rdchem.Mol): molecule to transform into features
+            mol (dm.Mol): molecule to transform into features
 
         Returns
             feat: featurized input molecule
 
         """
         feat = None
         try:
@@ -265,15 +264,15 @@
         except Exception as e:
             if self.verbose:
                 logger.error(e)
         return feat
 
     def transform(
         self,
-        mols: List[Union[rdchem.Mol, str]],
+        mols: List[Union[dm.Mol, str]],
         ignore_errors: bool = False,
         **kwargs,
     ):
         r"""
         Compute the features for a set of molecules.
 
         !!! note
@@ -288,15 +287,15 @@
             ignore_errors (bool, optional): Whether to silently ignore errors
 
 
         Returns:
             features: a list of features for each molecule in the input set
         """
         # Convert single mol to iterable format
-        if isinstance(mols, (str, rdchem.Mol)) or not isinstance(mols, Iterable):
+        if isinstance(mols, (str, dm.Mol)) or not isinstance(mols, Iterable):
             mols = [mols]
 
         def _to_mol(x):
             return dm.to_mol(x) if x else None
 
         parallel_kwargs = getattr(self, "parallel_kwargs", {})
 
@@ -347,15 +346,15 @@
                 f"Cannot auto-determine length of this MolTransformer: {self.__class__.__name__}"
             )
 
         return cur_length
 
     def __call__(
         self,
-        mols: List[Union[rdchem.Mol, str]],
+        mols: List[Union[dm.Mol, str]],
         enforce_dtype: bool = True,
         ignore_errors: bool = False,
         **kwargs,
     ):
         r"""
         Calculate features for molecules. Using __call__, instead of transform.
         If ignore_error is True, a list of features and valid ids are returned.
@@ -426,15 +425,15 @@
         if columns is not None and cols_to_keep is not None and len(cols_to_keep) > 0:
             columns = [columns[i] for i in cols_to_keep]
         return columns
 
     @staticmethod
     def batch_transform(
         transformer: Callable,
-        mols: List[Union[rdchem.Mol, str]],
+        mols: List[Union[dm.Mol, str]],
         batch_size: int = 256,
         n_jobs: Optional[int] = None,
         concatenate: bool = True,
         progress: bool = True,
         leave_progress: bool = False,
         **parallel_kwargs,
     ):
@@ -630,26 +629,26 @@
         if args.get("bond_featurizer") is not None:
             if not args.get("_bond_featurizer_is_pickled"):
                 klass_name = args["bond_featurizer"].get("name")
                 args["bond_featurizer"] = BOND_FEATURIZER_MAPPING_REVERSE[
                     klass_name
                 ].from_state_dict(args["bond_featurizer"])
             else:
-                # buffer = io.BytesIO(bytes.fromhex(args["bond_featurizer"]))
-                # args["bond_featurizer"] = joblib.load(buffer)
                 args["bond_featurizer"] = hex_to_fn(args["bond_featurizer"])
             args.pop("_bond_featurizer_is_pickled", None)
         ## Deal with custom featurizer
         if "featurizer" in args:
             if args.get("_featurizer_is_pickled") is True:
-                # buffer = io.BytesIO(bytes.fromhex(args["featurizer"]))
-                # args["featurizer"] = joblib.load(buffer)
                 args["featurizer"] = hex_to_fn(args["featurizer"])
                 args.pop("_featurizer_is_pickled")
-            elif not isinstance(args["featurizer"], str):
+            elif (
+                isinstance(args["featurizer"], Mapping)
+                and args["featurizer"].get("name") in _CALCULATORS
+            ):
+                # we have found a known calculator
                 klass_name = args["featurizer"].get("name")
                 args["featurizer"] = _CALCULATORS[klass_name].from_state_dict(args["featurizer"])
                 args.pop("_featurizer_is_pickled")
 
         if override_args is not None:
             args.update(override_args)
 
@@ -750,20 +749,20 @@
             self.length = len(self.base_featurizer)
         else:
             raise AttributeError(
                 "The cache is empty and the base featurizer is not specified. It's impossible"
                 " to determine the length of the featurizer."
             )
 
-    def _transform(self, mol: rdchem.Mol):
+    def _transform(self, mol: dm.Mol):
         r"""
         Return precomputed feature for a single molecule
 
         Args:
-            mol (rdchem.Mol): molecule to transform into features
+            mol (dm.Mol): molecule to transform into features
 
         Returns
             feat: featurized input molecule
 
         """
         feat = self.cache.get(mol)
         # if feat is None and we have an existing featurizer, we can update the cache
```

### Comparing `molfeat-0.8.6/molfeat/trans/concat.py` & `molfeat-0.8.7/molfeat/trans/concat.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import List
 from typing import Any
 
 import numpy as np
 import pandas as pd
 import datamol as dm
 
-from rdkit.Chem import rdchem
 from sklearn.base import BaseEstimator
 from molfeat.trans.fp import FPVecTransformer
 from molfeat.utils import datatype
 
 
 class FeatConcat(list, BaseEstimator):
     r"""
@@ -146,15 +145,15 @@
             if fp_columns is None:
                 fp_out, _ = fp([tmp_mol])
                 fp_out = np.asarray(fp_out)
                 fp_columns = [f"{fp_name}:{ind}" for ind in range(fp_out.shape[-1])]
             columns.extend(fp_columns)
         return columns
 
-    def transform(self, mols: List[Union[rdchem.Mol, str]], **kwargs):
+    def transform(self, mols: List[Union[dm.Mol, str]], **kwargs):
         r"""
         Calls the ``FPVecTransformer.transform`` for each transformer in
         the current list, and concatenates the resulting fingerprints.
 
         Args:
             mols: List of SMILES or molecules
             kwargs: named parameters for transform (see below)
@@ -172,15 +171,15 @@
             fps.append(out)
         fps = pd.concat(fps, axis=1)
         fps.columns = self.columns
         return fps.values
 
     def __call__(
         self,
-        mols: List[Union[rdchem.Mol, str]],
+        mols: List[Union[dm.Mol, str]],
         enforce_dtype: bool = False,
         ignore_errors: bool = False,
         **kwargs,
     ):
         r"""
         Calls each of the internal transformer and concatenate results only on valid indices.
 
@@ -213,15 +212,15 @@
             fps = datatype.cast(fps, dtype=self.dtype, columns=self.columns)
         if not ignore_errors:
             return fps
         return fps, list(valid_idx)
 
     def fit_transform(
         self,
-        mols: List[Union[str, rdchem.Mol]],
+        mols: List[Union[str, dm.Mol]],
         y: Optional[Iterable] = None,
         fit_kwargs: Dict = None,
         trans_kwargs: Dict = None,
     ):
         r"""
         Calls the ``self.fit`` followed by the ``fit.transform`` for each transfomer in
         the current list, and concatenates the resulting fingerprints.
@@ -239,15 +238,15 @@
                 molecules that have been successfully featurized.
         """
         fit_kwargs = {} if fit_kwargs is None else fit_kwargs
         trans_kwargs = {} if trans_kwargs is None else trans_kwargs
         self.fit(mols, y=y, **fit_kwargs)
         return self.transform(mols, **trans_kwargs)
 
-    def fit(self, X: List[Union[rdchem.Mol, str]], y=None, **kwargs):
+    def fit(self, X: List[Union[dm.Mol, str]], y=None, **kwargs):
         r"""
         Calls the ``FPVecTransformer.fit`` for each transformer in the current list.
 
         Args:
             X: input list of molecules
             y (list, optional): Optional list of molecular properties. Defaults to None.
```

### Comparing `molfeat-0.8.6/molfeat/trans/fp.py` & `molfeat-0.8.7/molfeat/trans/fp.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
 import re
 import copy
 import numpy as np
-from rdkit.Chem import rdchem
+import datamol as dm
 
 from molfeat.calc import get_calculator, FP_FUNCS
 from molfeat.trans.base import MoleculeTransformer
 from molfeat.utils import datatype
 from molfeat.utils.commons import _parse_to_evaluable_str
 
-
 _UNSERIALIZABLE_FPS = []
 
 
 class FPVecTransformer(MoleculeTransformer):
     r"""
     Molecular fingerprinter that computes various fingerprints and descriptors regularly used in QSAR modeling.
 
@@ -225,15 +224,15 @@
             _parse_to_evaluable_str(self.kind),
             _parse_to_evaluable_str(self.length),
             _parse_to_evaluable_str(self.occ_threshold),
             _parse_to_evaluable_str(self.del_invariant),
             _parse_to_evaluable_str(self.dtype),
         )
 
-    def fit(self, X: List[Union[rdchem.Mol, str]], y: Optional[list] = None, **fit_params):
+    def fit(self, X: List[Union[dm.Mol, str]], y: Optional[list] = None, **fit_params):
         """Fit the current transformer on given dataset.
 
         The goal of fitting is for example to identify nan columns values
         that needs to be removed from the dataset
 
         Args:
             X: input list of molecules
```

### Comparing `molfeat-0.8.6/molfeat/trans/graph/adj.py` & `molfeat-0.8.7/molfeat/trans/graph/adj.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import List
 from typing import Union
 
 import torch
 import datamol as dm
 import numpy as np
 import torch.nn.functional as F
+
 from loguru import logger
-from rdkit.Chem import rdchem
 from rdkit.Chem.rdmolops import GetAdjacencyMatrix
 from rdkit.Chem.rdmolops import GetDistanceMatrix
 from rdkit.Chem.rdmolops import Get3DDistanceMatrix
 from molfeat.trans.base import MoleculeTransformer
 from molfeat.utils import datatype
 from molfeat.utils import requires
 from molfeat.utils.commons import requires_conformer
```

### Comparing `molfeat-0.8.6/molfeat/trans/graph/tree.py` & `molfeat-0.8.7/molfeat/trans/graph/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import Optional
 
 import os
 import torch
 import numpy as np
 import datamol as dm
 from loguru import logger
-from rdkit.Chem import rdchem
 from molfeat.calc.tree import TreeDecomposer
 from molfeat.trans.base import MoleculeTransformer
 from molfeat.utils import datatype
 from molfeat.utils.commons import one_hot_encoding
 from molfeat.utils import requires
 
 if requires.check("dgl"):
@@ -81,15 +80,15 @@
         Returns:
             size: vocab size
         """
         return self._vocab_size
 
     def fit(
         self,
-        X: List[Union[rdchem.Mol, str]],
+        X: List[Union[dm.Mol, str]],
         y: Optional[list] = None,
         output_file: Optional[os.PathLike] = None,
         **fit_params,
     ):
         """Fit the current transformer on given dataset.
 
         The goal of fitting is for example to identify nan columns values
@@ -112,21 +111,21 @@
         self._fitted = True
 
         # save the vocab in the state
         self._input_args["vocab"] = self.vocab
 
         return self
 
-    def _transform(self, mol: rdchem.Mol):
+    def _transform(self, mol: dm.Mol):
         r"""
         Compute features for a single molecule.
         This method would potentially need to be reimplemented by child classes
 
         Args:
-            mol (rdchem.Mol): molecule to transform into features
+            mol (dm.Mol): molecule to transform into features
 
         Returns
             feat: featurized input molecule
 
         """
         if not self._fitted:
             raise ValueError(
```

### Comparing `molfeat-0.8.6/molfeat/trans/pretrained/base.py` & `molfeat-0.8.7/molfeat/trans/pretrained/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from collections.abc import Iterable
 from functools import lru_cache
 
 import copy
 import datamol as dm
 
 from loguru import logger
-from rdkit.Chem import rdchem
 from molfeat.utils.commons import _parse_to_evaluable_str
 from molfeat.trans.base import MoleculeTransformer
 from molfeat.utils.cache import DataCache
 from molfeat.store.loader import PretrainedModel
 
 
 class PretrainedMolTransformer(MoleculeTransformer):
@@ -71,21 +70,21 @@
     def _get_param_names(self):
         """Get parameter names for the estimator"""
         out = self._input_params.keys()
         out = [x for x in out if x != "featurizer"]
         return out
 
     def _embed(self, smiles: str, **kwargs):
-        """Internal molecular embedding
+        """Compute molecular embeddings for input list of smiles
         This functiom takes a list of smiles or molecules and return the featurization
         corresponding to the inputs.  In `transform` and `_transform`, this function is
         called after calling `_convert`
 
         Args:
-            smiles: input smiless
+            smiles: input smiles
         """
         raise NotImplementedError
 
     def _preload(self):
         """Preload the pretrained model for later queries"""
         if self.featurizer is not None and isinstance(self.featurizer, PretrainedModel):
             self.featurizer = self.featurizer.load()
@@ -132,21 +131,21 @@
         if self.precompute_cache not in [False, None]:
             try:
                 self.transform(inputs)
             except:
                 pass
         return out
 
-    def _transform(self, mol: rdchem.Mol, **kwargs):
+    def _transform(self, mol: dm.Mol, **kwargs):
         r"""
         Compute features for a single molecule.
         This method would potentially need to be reimplemented by any child class
 
         Args:
-            mol (rdchem.Mol): molecule to transform into features
+            mol (dm.Mol): molecule to transform into features
 
         Returns
             feat: featurized input molecule
 
         """
         feat = None
         if self.precompute_cache is not None:
```

### Comparing `molfeat-0.8.6/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.8.7/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Load one of the pretrained DGL models for molecular embedding:
     """
     AVAILABLE_MODELS = [
         "gin_supervised_contextpred",
         "gin_supervised_infomax",
         "gin_supervised_edgepred",
         "gin_supervised_masking",
-        "JTVAE_ZINC_no_kl",
+        "jtvae_zinc_no_kl",
     ]
 
     def __init__(
         self,
         name: str,
         cache_path: Optional[os.PathLike] = None,
         store: Optional[ModelStore] = None,
```

### Comparing `molfeat-0.8.6/molfeat/trans/pretrained/fcd.py` & `molfeat-0.8.7/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.8.7/molfeat/trans/pretrained/hf_transformers.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/trans/struct/esm.py` & `molfeat-0.8.7/molfeat/trans/struct/esm.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/trans/struct/prot1D.py` & `molfeat-0.8.7/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/cache.py` & `molfeat-0.8.7/molfeat/utils/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import itertools
 import random
 import multiprocessing as mp
 
 import pandas.errors
 
 from functools import partial
-from rdkit.Chem import rdchem
 from molfeat.utils import commons
 from molfeat.utils import datatype
 
 
 class MolToKey:
     """Convert a molecule to a key"""
 
@@ -62,25 +61,24 @@
             self.hash_fn = hash_fn
             self.hash_name = None
 
             if self.hash_fn is None:
                 self.hash_fn = dm.unique_id
                 self.hash_name = "dm.unique_id"
 
-    def __call__(self, mol: rdchem.Mol):
+    def __call__(self, mol: dm.Mol):
         """Convert a molecule object to a key that can be used for the cache system
 
         Args:
             mol: input molecule object
         """
-        is_mol = dm.to_mol(mol) is not None
-
-        if is_mol and self.hash_fn is not None:
-            return self.hash_fn(mol)
-
+        with dm.without_rdkit_log():
+            is_mol = dm.to_mol(mol) is not None
+            if is_mol and self.hash_fn is not None:
+                return self.hash_fn(mol)
         return mol
 
     def to_state_dict(self):
         """Serialize MolToKey to a state dict."""
 
         if self.hash_name is None:
             raise ValueError(
@@ -156,25 +154,26 @@
             key: input key to set
             item: value of the key to set
         """
         self.update({key: item})
 
     def __call__(
         self,
-        mols: List[Union[rdchem.Mol, str]],
+        mols: List[Union[dm.Mol, str]],
         featurizer: Any,
         enforce_dtype=True,
         **transform_kwargs,
     ):
         """
         Compute the features for a list of molecules and save them to the cache
 
         Args:
             mols: list of molecule to preprocess
             featurizer: input featurizer to use to compute the molecular representation. Should implement a `__call__` method.
+            enforce_dtype: whether to ensure the featurizer dtype is returned
             transformer_kwargs: keyword arguments to pass to the transformer.
 
         !!! note
             Parquet format does not support tensor datatype, so you should ensure that the output of
             the featurizer is a numpy array in that case
 
         Returns:
@@ -199,15 +198,15 @@
                 mol_queries.append(m)
         if len(mol_queries) > 0:
             features = featurizer(
                 mol_queries,
                 **transform_kwargs,
             )
             dtype = getattr(featurizer, "dtype", None)
-            if dtype is not None:
+            if dtype is not None and enforce_dtype:
                 features = datatype.cast(features, dtype=dtype)
             for key, feat in zip(unseen_ids, features):
                 self[key] = feat
             self._sync_cache()
         return self.fetch(mols)
 
     def clear(self, *args, **kwargs):
@@ -243,33 +242,35 @@
         return dict(self.items())
 
     def _sync_cache(self):
         ...
 
     def fetch(
         self,
-        mols: List[Union[rdchem.Mol, str]],
+        mols: List[Union[dm.Mol, str]],
     ):
-        """Get the representation for a single
+        """Get the cached representation for a list of input molecules
 
         Args:
             mols: list of molecules
         """
         if isinstance(mols, str) or not isinstance(mols, Iterable):
             mols = [mols]
 
-        converter = copy.deepcopy(self.mol_hasher)
-        mol_ids = dm.parallelized(
-            converter,
-            mols,
-            n_jobs=self.n_jobs,
-            progress=self.verbose,
-            tqdm_kwargs=dict(leave=False),
+        # copy if possible to prevent parallel issues
+        try:
+            cacher = copy.deepcopy(self)
+            n_jobs = self.n_jobs
+        except:
+            # cannot parallelize process, ensure n_jobs is 0
+            cacher = self
+            n_jobs = 0
+        return dm.parallelized(
+            cacher.get, mols, n_jobs=n_jobs, progress=self.verbose, tqdm_kwargs=dict(leave=False)
         )
-        return [self.get(mol_id) for mol_id in mol_ids]
 
     @abc.abstractclassmethod
     def load_from_file(cls, filepath: Union[os.PathLike, str], **kwargs):
         """Load a cache from a file (including remote file)
 
         Args:
             filepath: path to the file to load
@@ -768,15 +769,15 @@
 
     def to_dict(self):
         """Convert current cache to a dictionary"""
         return dict(self.items())
 
     def fetch(
         self,
-        mols: List[Union[rdchem.Mol, str]],
+        mols: List[Union[dm.Mol, str]],
     ):
         """Get the representation for a single
 
         Args:
             mols: list of molecules
         """
         if isinstance(mols, str) or not isinstance(mols, Iterable):
```

### Comparing `molfeat-0.8.6/molfeat/utils/commons.py` & `molfeat-0.8.7/molfeat/utils/commons.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/const.py` & `molfeat-0.8.7/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/converters.py` & `molfeat-0.8.7/molfeat/utils/converters.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/datatype.py` & `molfeat-0.8.7/molfeat/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/log.py` & `molfeat-0.8.7/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/parsing.py` & `molfeat-0.8.7/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/pooler.py` & `molfeat-0.8.7/molfeat/utils/pooler.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         """
         x = torch.as_tensor(x)
         if mask is None:
             mask = torch.ones_like(x)
         if indices is not None:
             mask[:, indices] = 0
         neg_inf = torch.finfo(x.dtype).min
+        if mask.ndim == 2:
+            mask = mask.unsqueeze(-1)  # B, S, 1
         if self.name == "clf":
             return x[:, 0, :]
         if self.name == "max":
             tmp = x.masked_fill(mask, neg_inf)
             return torch.max(tmp, dim=self.dim)[0]
         elif self.name in ["mean", "avg"]:
             return torch.sum(x * mask, dim=self.dim) / mask.sum(self.dim)
```

### Comparing `molfeat-0.8.6/molfeat/utils/requires.py` & `molfeat-0.8.7/molfeat/utils/requires.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/utils/state.py` & `molfeat-0.8.7/molfeat/utils/state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat/viz.py` & `molfeat-0.8.7/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/molfeat.egg-info/PKG-INFO` & `molfeat-0.8.7/molfeat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.6
+Version: 0.8.7
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
@@ -39,15 +39,15 @@
 
 <p align="center">
     <b>molfeat - the hub for all your molecular featurizers </b> <br />
 </p>
 <p align="center">
   <a href="https://molfeat-docs.datamol.io/" target="_blank">
       Docs
-  </a> | 
+  </a> |
   <a href="https://molfeat.datamol.io/" target="_blank">
       Homepage
   </a>
 </p>
 
 ---
 
@@ -68,52 +68,50 @@
 Molfeat is a hub of molecular featurizers. It supports a wide variety of out-of-the-box molecular featurizers and can be easily extended to include your own custom featurizers.
 
 - 🚀 Fast, with a simple and efficient API.
 - 🔄 Unify pre-trained molecular embeddings and hand-crafted featurizers in a single package.
 - ➕ Easily add your own featurizers through plugins.
 - 📈 Benefit from increased performance through a trouble-free caching system.
 
-Visit our website at https://molfeat.datamol.io.
+Visit our website at <https://molfeat.datamol.io>.
 
 ## Installation
 
 ### Installing Molfeat
 
 Use mamba:
 
 ```bash
 mamba install -c conda-forge molfeat
 ```
 
 _**Tips:** You can replace `mamba` by `conda`._
 
-_**Note:** We highly recommend using a [Conda Python distribution](https://github.com/conda-forge/miniforge) to install Molfeat. The package is also pip installable if you need it: `pip install molfeat`._ 
+_**Note:** We highly recommend using a [Conda Python distribution](https://github.com/conda-forge/miniforge) to install Molfeat. The package is also pip installable if you need it: `pip install molfeat`._
 
 ### Optional dependencies
-Not all featurizers in the Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them. 
+
+Not all featurizers in the Molfeat core package are supported by default. Some featurizers require additional dependencies. If you try to use a featurizer that requires additional dependencies, Molfeat will raise an error and tell you which dependencies are missing and how to install them.
 
 - To install `dgl`: run `mamba install -c dglteam dgl`
-- To install `dgllife`:  run `mamba install -c conda-forge dgllife`
+- To install `dgllife`: run `mamba install -c conda-forge dgllife`
 - To install `fcd_torch`: run `mamba install -c conda-forge fcd_torch`
 - To install `pyg`: run `mamba install -c conda-forge pytorch_geometric`
 - To install `graphormer-pretrained`: run `mamba install -c conda-forge graphormer-pretrained`
-- To install `map4`: see https://github.com/reymond-group/map4
+- To install `map4`: see <https://github.com/reymond-group/map4>
 - To install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings >=0.2.2'`
 
-
 If you install Molfeat using pip, there are optional dependencies that can be installed with the main package. For example, `pip install "molfeat[all]"` allows installing all the compatible optional dependencies for small molecule featurization. There are other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/blob/main/pyproject.toml#L60) for more information.
 
-
 ### Installing Plugins
 
 The functionality of Molfeat can be extended through plugins. The use of a plugin system ensures that the core package remains easy to install and as light as possible, while making it easy to extend its functionality with plug-and-play components. Additionally, it ensures that plugins can be developed independently from the core package, removing the bottleneck of a central party that reviews and approves new plugins. Consult the molfeat documentation for more details on how to [create](developers/create-plugin.md) your own plugins.
 
 However, this does imply that the installation of a plugin is plugin-dependent: please consult the relevant documentation to learn more.
 
-
 ## API tour
 
 ```python
 import datamol as dm
 from molfeat.calc import FPCalculator
 from molfeat.trans import MoleculeTransformer
 from molfeat.store.modelstore import ModelStore
@@ -153,17 +151,14 @@
 
 ## Changelogs
 
 See the latest changelogs at [CHANGELOG.rst](./CHANGELOG.rst).
 
 ## Maintainers
 
-* @cwognum
-* @maclandrol
-* @hadim
-
+- @cwognum
+- @maclandrol
+- @hadim
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
-
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.6 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.7 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
@@ -45,37 +45,38 @@
 badge.svg)](https://github.com/datamol-io/molfeat/actions/workflows/
 release.yml) Molfeat is a hub of molecular featurizers. It supports a wide
 variety of out-of-the-box molecular featurizers and can be easily extended to
 include your own custom featurizers. - ð Fast, with a simple and efficient
 API. - ð Unify pre-trained molecular embeddings and hand-crafted featurizers
 in a single package. - â Easily add your own featurizers through plugins. -
 ð Benefit from increased performance through a trouble-free caching system.
-Visit our website at https://molfeat.datamol.io. ## Installation ### Installing
-Molfeat Use mamba: ```bash mamba install -c conda-forge molfeat ``` _**Tips:**
-You can replace `mamba` by `conda`._ _**Note:** We highly recommend using a
-[Conda Python distribution](https://github.com/conda-forge/miniforge) to
-install Molfeat. The package is also pip installable if you need it: `pip
-install molfeat`._ ### Optional dependencies Not all featurizers in the Molfeat
-core package are supported by default. Some featurizers require additional
-dependencies. If you try to use a featurizer that requires additional
-dependencies, Molfeat will raise an error and tell you which dependencies are
-missing and how to install them. - To install `dgl`: run `mamba install -
-c dglteam dgl` - To install `dgllife`: run `mamba install -c conda-forge
-dgllife` - To install `fcd_torch`: run `mamba install -c conda-forge fcd_torch`
-- To install `pyg`: run `mamba install -c conda-forge pytorch_geometric` - To
-install `graphormer-pretrained`: run `mamba install -c conda-forge graphormer-
-pretrained` - To install `map4`: see https://github.com/reymond-group/map4 - To
-install `bio-embeddings`: run `mamba install -c conda-forge 'bio-embeddings
->=0.2.2'` If you install Molfeat using pip, there are optional dependencies
-that can be installed with the main package. For example, `pip install "molfeat
-[all]"` allows installing all the compatible optional dependencies for small
-molecule featurization. There are other options such as `molfeat[dgl]`,
-`molfeat[graphormer]`, `molfeat[transformer]`, `molfeat[viz]`, and `molfeat
-[fcd]`. See the [optional-dependencies](https://github.com/datamol-io/molfeat/
-blob/main/pyproject.toml#L60) for more information. ### Installing Plugins The
+Visit our website at
+molfeat.datamol.io>. ## Installation ### Installing Molfeat Use mamba: ```bash
+mamba install -c conda-forge molfeat ``` _**Tips:** You can replace `mamba` by
+`conda`._ _**Note:** We highly recommend using a [Conda Python distribution]
+(https://github.com/conda-forge/miniforge) to install Molfeat. The package is
+also pip installable if you need it: `pip install molfeat`._ ### Optional
+dependencies Not all featurizers in the Molfeat core package are supported by
+default. Some featurizers require additional dependencies. If you try to use a
+featurizer that requires additional dependencies, Molfeat will raise an error
+and tell you which dependencies are missing and how to install them. - To
+install `dgl`: run `mamba install -c dglteam dgl` - To install `dgllife`: run
+`mamba install -c conda-forge dgllife` - To install `fcd_torch`: run `mamba
+install -c conda-forge fcd_torch` - To install `pyg`: run `mamba install -
+c conda-forge pytorch_geometric` - To install `graphormer-pretrained`: run
+`mamba install -c conda-forge graphormer-pretrained` - To install `map4`: see
+github.com/reymond-group/map4> - To install `bio-embeddings`: run `mamba
+install -c conda-forge 'bio-embeddings >=0.2.2'` If you install Molfeat using
+pip, there are optional dependencies that can be installed with the main
+package. For example, `pip install "molfeat[all]"` allows installing all the
+compatible optional dependencies for small molecule featurization. There are
+other options such as `molfeat[dgl]`, `molfeat[graphormer]`, `molfeat
+[transformer]`, `molfeat[viz]`, and `molfeat[fcd]`. See the [optional-
+dependencies](https://github.com/datamol-io/molfeat/blob/main/
+pyproject.toml#L60) for more information. ### Installing Plugins The
 functionality of Molfeat can be extended through plugins. The use of a plugin
 system ensures that the core package remains easy to install and as light as
 possible, while making it easy to extend its functionality with plug-and-play
 components. Additionally, it ensures that plugins can be developed
 independently from the core package, removing the bottleneck of a central party
 that reviews and approves new plugins. Consult the molfeat documentation for
 more details on how to [create](developers/create-plugin.md) your own plugins.
@@ -92,9 +93,9 @@
 List all available featurizers store = ModelStore() store.available_models #
 Find a featurizer and learn how to use it model_card = store.search
 (name="ChemBERTa-77M-MLM")[0] model_card.usage() ``` ## How to cite Please cite
 Molfeat if you use it in your research: [![DOI](https://zenodo.org/badge/
 613548667.svg)](https://zenodo.org/badge/latestdoi/613548667). ## Contribute
 See [developers](docs/developers/) for a comprehensive guide on how to
 contribute to `Molfeat` ## Changelogs See the latest changelogs at
-[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers * @cwognum * @maclandrol *
+[CHANGELOG.rst](./CHANGELOG.rst). ## Maintainers - @cwognum - @maclandrol -
 @hadim ## License Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `molfeat-0.8.6/molfeat.egg-info/SOURCES.txt` & `molfeat-0.8.7/molfeat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/pyproject.toml` & `molfeat-0.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_atom_bond_calculator.py` & `molfeat-0.8.7/tests/test_atom_bond_calculator.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_descriptors.py` & `molfeat-0.8.7/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_fp.py` & `molfeat-0.8.7/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_graphs.py` & `molfeat-0.8.7/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_pharmacophore.py` & `molfeat-0.8.7/tests/test_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_pretrained.py` & `molfeat-0.8.7/tests/test_pretrained.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import unittest as ut
 import time
 import numpy as np
 import datamol as dm
-import torch
 import pytest
 import tempfile
 import joblib
 from molfeat.trans.pretrained import GraphormerTransformer
 from molfeat.trans.pretrained import PretrainedDGLTransformer
 from molfeat.trans.pretrained import PretrainedHFTransformer
 from molfeat.utils import requires
-from molfeat.utils.cache import DataCache
 
 
 @pytest.mark.xfail(
     not requires.check("graphormer_pretrained"), reason="3rd party module graphormer is missing"
 )
 class TestGraphormerTransformer(ut.TestCase):
     r"""Test cases for FingerprintsTransformer"""
@@ -24,43 +22,68 @@
         "C[C@@H]([NH3+])Cc1c2ccoc2c(Br)c2ccoc12",
     ]
 
     def test_graphormer_pickling(self):
         transf = GraphormerTransformer(dtype=np.float32, pooling="sum")
         with tempfile.NamedTemporaryFile(delete=True) as pickled_file:
             joblib.dump(transf, pickled_file.name)
-            trans2 = joblib.load(pickled_file.name)
+            transf2 = joblib.load(pickled_file.name)
         ori_feat = transf(dm.freesolv().smiles.values[:10])
-        reloaded_feat = trans2(dm.freesolv().smiles.values[:10])
+        reloaded_feat = transf2(dm.freesolv().smiles.values[:10])
         np.testing.assert_array_equal(ori_feat, reloaded_feat)
 
     def test_graphormer(self):
         transf = GraphormerTransformer(dtype=np.float32, pooling="sum")
-        trans2 = GraphormerTransformer(dtype=np.float32, pooling="mean")
+        transf2 = GraphormerTransformer(dtype=np.float32, pooling="mean")
+        transf3 = GraphormerTransformer(dtype=np.float32, pooling="mean", concat_layers=[-1, -2])
         fps = transf(self.smiles, enforce_dtype=True)
         fps2 = transf(self.smiles, enforce_dtype=True)
-        fps3 = trans2(self.smiles, enforce_dtype=True)
+        fps3 = transf2(self.smiles, enforce_dtype=True)
+        fps4 = transf3(self.smiles, enforce_dtype=True)
         self.assertEqual(len(fps), 3)
         self.assertEqual(len(transf), fps[0].shape[-1])
+        # concatenated layer should be twice bigger
+        self.assertEqual(len(transf3), fps[0].shape[-1] * 2)
         np.testing.assert_array_equal(fps, fps2)
-        node_per_mol = np.rint(fps / fps3)
-        node_per_mol = np.unique(node_per_mol)
-        self.assertLessEqual(len(node_per_mol), 2)
+        # first layer should be equal to the mean pooling
+        np.testing.assert_array_equal(fps3, fps4[:, : fps[0].shape[-1]])
+        n_atoms = np.asarray([dm.descriptors.n_heavy_atoms(dm.to_mol(x)) for x in self.smiles])
+        n_atoms += 1  # we add the virtual node that is connected to all other nodes.
+        np.testing.assert_allclose(fps, fps3 * n_atoms[:, None], atol=1e-5)
+
+    def test_graphormer_pooling(self):
+        transf = GraphormerTransformer(dtype=np.float32, pooling="mean", ignore_padding=True)
+        transf2 = GraphormerTransformer(
+            dtype=np.float32, pooling="mean", max_length=100, ignore_padding=True
+        )
+        transf3 = GraphormerTransformer(
+            dtype=np.float32, pooling="virtual", max_length=100, ignore_padding=True
+        )
+        transf4 = GraphormerTransformer(
+            dtype=np.float32, pooling="virtual", max_length=50, ignore_padding=True
+        )
+        fps = transf(self.smiles, enforce_dtype=True)
+        fps2 = transf2(self.smiles, enforce_dtype=True)
+        fps3 = transf3(self.smiles, enforce_dtype=True)
+        fps4 = transf4(self.smiles, enforce_dtype=True)
+
+        np.testing.assert_allclose(fps, fps2, atol=1e-5)
+        np.testing.assert_allclose(fps3, fps4, atol=1e-5)
 
     def test_graphormer_cache(self):
         transf = GraphormerTransformer(
             dtype=np.float32, pooling="mean", max_length=25, precompute_cache=True
         )
         t0 = time.time()
         time_buffer = 1
         fps = transf.transform(self.smiles)
         ori_run = time.time() - t0
         fps2 = transf.transform(self.smiles)
         cached_run = time.time() - t0 - ori_run
-        np.testing.assert_array_equal(fps, fps2)
+        np.testing.assert_allclose(fps, fps2, atol=1e-5)
         # add buffers
         self.assertLessEqual(cached_run, ori_run + time_buffer)
 
 
 class TestDGLTransformer(ut.TestCase):
     r"""Test cases for FingerprintsTransformer"""
     smiles = [
@@ -69,17 +92,17 @@
         "C[C@@H]([NH3+])Cc1c2ccoc2c(Br)c2ccoc12",
     ]
 
     def test_dgl_pickling(self):
         transf = PretrainedDGLTransformer(dtype=np.float32, pooling="sum")
         with tempfile.NamedTemporaryFile(delete=True) as pickled_file:
             joblib.dump(transf, pickled_file.name)
-            trans2 = joblib.load(pickled_file.name)
+            transf2 = joblib.load(pickled_file.name)
         ori_feat = transf(dm.freesolv().smiles.values[:10])
-        reloaded_feat = trans2(dm.freesolv().smiles.values[:10])
+        reloaded_feat = transf2(dm.freesolv().smiles.values[:10])
         np.testing.assert_array_equal(ori_feat, reloaded_feat)
 
     def test_dgl_pretrained(self):
         transf = PretrainedDGLTransformer(dtype=np.float32, pooling="sum")
         fps = transf(self.smiles, enforce_dtype=True)
         fps2 = transf(self.smiles, enforce_dtype=True)
         self.assertEqual(len(fps), 3)
@@ -110,17 +133,17 @@
         "C[C@@H]([NH3+])Cc1c2ccoc2c(Br)c2ccoc12",
     ]
 
     def test_hgf_pickling(self):
         transf = PretrainedHFTransformer(dtype=np.float32, pooling="sum")
         with tempfile.NamedTemporaryFile(delete=True) as pickled_file:
             joblib.dump(transf, pickled_file.name)
-            trans2 = joblib.load(pickled_file.name)
+            transf2 = joblib.load(pickled_file.name)
         ori_feat = transf(dm.freesolv().smiles.values[:10])
-        reloaded_feat = trans2(dm.freesolv().smiles.values[:10])
+        reloaded_feat = transf2(dm.freesolv().smiles.values[:10])
         np.testing.assert_array_equal(ori_feat, reloaded_feat)
 
     def test_hgf_pretrained(self):
         transf = PretrainedHFTransformer(dtype=np.float32, pooling="sum")
         fps = transf(self.smiles, enforce_dtype=True)
         fps2 = transf(self.smiles, enforce_dtype=True)
         self.assertEqual(len(fps), 3)
```

### Comparing `molfeat-0.8.6/tests/test_prot_embed.py` & `molfeat-0.8.7/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_state.py` & `molfeat-0.8.7/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.6/tests/test_utils.py` & `molfeat-0.8.7/tests/test_utils.py`

 * *Files identical despite different names*

