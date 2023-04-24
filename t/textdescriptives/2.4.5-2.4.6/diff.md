# Comparing `tmp/textdescriptives-2.4.5.tar.gz` & `tmp/textdescriptives-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.4.5.tar", last modified: Wed Apr 19 20:55:45 2023, max compression
+gzip compressed data, was "textdescriptives-2.4.6.tar", last modified: Mon Apr 24 11:55:41 2023, max compression
```

## Comparing `textdescriptives-2.4.5.tar` & `textdescriptives-2.4.6.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1161 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2261 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1388 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)     6703 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23998 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9641 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3548 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2752 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/readability.rst
--rw-r--r--   0 root         (0) root         (0)      349 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    96689 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115780 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7465 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     8736 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     3059 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.573709 textdescriptives-2.4.5/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5353 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     7504 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5515 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     3380 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    22254 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10426 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     7713 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.573709 textdescriptives-2.4.5/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6042 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/extractors.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.573709 textdescriptives-2.4.5/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23998 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2365 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      493 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2821 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9305 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.485264 textdescriptives-2.4.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.461262 textdescriptives-2.4.6/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.465262 textdescriptives-2.4.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.465262 textdescriptives-2.4.6/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)     6856 2023-04-24 11:55:30.000000 textdescriptives-2.4.6/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23997 2023-04-24 11:55:41.485264 textdescriptives-2.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.469262 textdescriptives-2.4.6/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.473263 textdescriptives-2.4.6/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3548 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/readability.rst
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.473263 textdescriptives-2.4.6/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    96689 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7465 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.477263 textdescriptives-2.4.6/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9237 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-04-24 11:55:30.000000 textdescriptives-2.4.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 11:55:41.485264 textdescriptives-2.4.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.457262 textdescriptives-2.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.477263 textdescriptives-2.4.6/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.481263 textdescriptives-2.4.6/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5515 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    22254 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10426 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     7713 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.481263 textdescriptives-2.4.6/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6042 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.477263 textdescriptives-2.4.6/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23997 2023-04-24 11:55:41.000000 textdescriptives-2.4.6/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-04-24 11:55:41.000000 textdescriptives-2.4.6/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 11:55:41.000000 textdescriptives-2.4.6/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-24 11:55:41.000000 textdescriptives-2.4.6/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-24 11:55:41.000000 textdescriptives-2.4.6/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:55:41.485264 textdescriptives-2.4.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9305 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-24 11:55:29.000000 textdescriptives-2.4.6/tests/test_utils.py
```

### Comparing `textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.4.6/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.4.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/dependabot.yml` & `textdescriptives-2.4.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/workflows/dependabot_automerge.yml` & `textdescriptives-2.4.6/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/workflows/documentation.yml` & `textdescriptives-2.4.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/workflows/draft-pdf.yml` & `textdescriptives-2.4.6/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/workflows/release.yml` & `textdescriptives-2.4.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/workflows/stale.yml` & `textdescriptives-2.4.6/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.github/workflows/tests.yml` & `textdescriptives-2.4.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.gitignore` & `textdescriptives-2.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.pre-commit-config.yaml` & `textdescriptives-2.4.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/.zenodo.json` & `textdescriptives-2.4.6/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/CHANGELOG.md` & `textdescriptives-2.4.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.4.6 (2023-04-24)
+### Fix
+* Bump version ([`b59cdd1`](https://github.com/HLasse/TextDescriptives/commit/b59cdd17379c7c8460accccbb569283a1f2c8717))
+
 ## v2.4.5 (2023-04-19)
 ### Fix
 * Dep dist. test ([`a3b54a6`](https://github.com/HLasse/TextDescriptives/commit/a3b54a6b3e3d57acc140b0f9afd72406a88104f8))
 * Coherence model now handles empty strings as intended ([`abfa507`](https://github.com/HLasse/TextDescriptives/commit/abfa5071ba075f25ff8c170f5cee4f84ef648ea5))
 * Dep distance test ([`2bed2c1`](https://github.com/HLasse/TextDescriptives/commit/2bed2c194b98062aad66d6ca0985fb92af6be977))
 
 ### Documentation
```

### Comparing `textdescriptives-2.4.5/CITATION.cff` & `textdescriptives-2.4.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/CODE_OF_CONDUCT.md` & `textdescriptives-2.4.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/CONTRIBUTING.md` & `textdescriptives-2.4.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/LICENSE` & `textdescriptives-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/PKG-INFO` & `textdescriptives-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.4.5
+Version: 2.4.6
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -308,15 +308,14 @@
 ```
 |      | text                      | first_order_coherence | second_order_coherence | pos_prop_DET | pos_prop_NOUN | pos_prop_AUX | pos_prop_VERB | pos_prop_PUNCT | pos_prop_PRON | pos_prop_ADP | pos_prop_ADV | pos_prop_SCONJ | flesch_reading_ease | flesch_kincaid_grade |    smog | gunning_fog | automated_readability_index | coleman_liau_index |     lix |  rix | n_stop_words | alpha_ratio | mean_word_length | doc_length | proportion_ellipsis | proportion_bullet_points | duplicate_line_chr_fraction | duplicate_paragraph_chr_fraction | duplicate_5-gram_chr_fraction | duplicate_6-gram_chr_fraction | duplicate_7-gram_chr_fraction | duplicate_8-gram_chr_fraction | duplicate_9-gram_chr_fraction | duplicate_10-gram_chr_fraction | top_2-gram_chr_fraction | top_3-gram_chr_fraction | top_4-gram_chr_fraction | symbol_#_to_word_ratio | contains_lorem ipsum | passed_quality_check | dependency_distance_mean | dependency_distance_std | prop_adjacent_dependency_relation_mean | prop_adjacent_dependency_relation_std | token_length_mean | token_length_median | token_length_std | sentence_length_mean | sentence_length_median | sentence_length_std | syllables_per_token_mean | syllables_per_token_median | syllables_per_token_std | n_tokens | n_unique_tokens | proportion_unique_tokens | n_characters | n_sentences |
 | ---: | :------------------------ | --------------------: | ---------------------: | -----------: | ------------: | -----------: | ------------: | -------------: | ------------: | -----------: | -----------: | -------------: | ------------------: | -------------------: | ------: | ----------: | --------------------------: | -----------------: | ------: | ---: | -----------: | ----------: | ---------------: | ---------: | ------------------: | -----------------------: | --------------------------: | -------------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | -----------------------------: | ----------------------: | ----------------------: | ----------------------: | ---------------------: | :------------------- | :------------------- | -----------------------: | ----------------------: | -------------------------------------: | ------------------------------------: | ----------------: | ------------------: | ---------------: | -------------------: | ---------------------: | ------------------: | -----------------------: | -------------------------: | ----------------------: | -------: | --------------: | -----------------------: | -----------: | ----------: |
 |    0 | The world is changed(...) |              0.633002 |               0.573323 |     0.097561 |      0.121951 |    0.0731707 |      0.170732 |       0.146341 |      0.195122 |    0.0731707 |    0.0731707 |      0.0487805 |             107.879 |           -0.0485714 | 5.68392 |     3.94286 |                    -2.45429 |          -0.708571 | 12.7143 |  0.4 |           24 |    0.853659 |          2.95122 |         41 |                   0 |                        0 |                           0 |                                0 |                      0.232258 |                      0.232258 |                             0 |                             0 |                             0 |                              0 |               0.0580645 |                0.174194 |                       0 |                      0 | False                | False                |                  1.77524 |                0.553188 |                               0.457143 |                             0.0722806 |           3.28571 |                   3 |          1.54127 |                    7 |                      6 |             3.09839 |                  1.08571 |                          1 |                0.368117 |       35 |              23 |                 0.657143 |          121 |           5 |
 
 
 
-
 # 📖 Documentation
 
 TextDescriptives has a detailed documentation as well as a series of Jupyter notebook tutorials.
 All the tutorials are located in the `docs/tutorials` folder and can also be found on the documentation website.
 
 
 | Documentation              |                                                                                    |
```

### Comparing `textdescriptives-2.4.5/README.md` & `textdescriptives-2.4.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 ```
 |      | text                      | first_order_coherence | second_order_coherence | pos_prop_DET | pos_prop_NOUN | pos_prop_AUX | pos_prop_VERB | pos_prop_PUNCT | pos_prop_PRON | pos_prop_ADP | pos_prop_ADV | pos_prop_SCONJ | flesch_reading_ease | flesch_kincaid_grade |    smog | gunning_fog | automated_readability_index | coleman_liau_index |     lix |  rix | n_stop_words | alpha_ratio | mean_word_length | doc_length | proportion_ellipsis | proportion_bullet_points | duplicate_line_chr_fraction | duplicate_paragraph_chr_fraction | duplicate_5-gram_chr_fraction | duplicate_6-gram_chr_fraction | duplicate_7-gram_chr_fraction | duplicate_8-gram_chr_fraction | duplicate_9-gram_chr_fraction | duplicate_10-gram_chr_fraction | top_2-gram_chr_fraction | top_3-gram_chr_fraction | top_4-gram_chr_fraction | symbol_#_to_word_ratio | contains_lorem ipsum | passed_quality_check | dependency_distance_mean | dependency_distance_std | prop_adjacent_dependency_relation_mean | prop_adjacent_dependency_relation_std | token_length_mean | token_length_median | token_length_std | sentence_length_mean | sentence_length_median | sentence_length_std | syllables_per_token_mean | syllables_per_token_median | syllables_per_token_std | n_tokens | n_unique_tokens | proportion_unique_tokens | n_characters | n_sentences |
 | ---: | :------------------------ | --------------------: | ---------------------: | -----------: | ------------: | -----------: | ------------: | -------------: | ------------: | -----------: | -----------: | -------------: | ------------------: | -------------------: | ------: | ----------: | --------------------------: | -----------------: | ------: | ---: | -----------: | ----------: | ---------------: | ---------: | ------------------: | -----------------------: | --------------------------: | -------------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | -----------------------------: | ----------------------: | ----------------------: | ----------------------: | ---------------------: | :------------------- | :------------------- | -----------------------: | ----------------------: | -------------------------------------: | ------------------------------------: | ----------------: | ------------------: | ---------------: | -------------------: | ---------------------: | ------------------: | -----------------------: | -------------------------: | ----------------------: | -------: | --------------: | -----------------------: | -----------: | ----------: |
 |    0 | The world is changed(...) |              0.633002 |               0.573323 |     0.097561 |      0.121951 |    0.0731707 |      0.170732 |       0.146341 |      0.195122 |    0.0731707 |    0.0731707 |      0.0487805 |             107.879 |           -0.0485714 | 5.68392 |     3.94286 |                    -2.45429 |          -0.708571 | 12.7143 |  0.4 |           24 |    0.853659 |          2.95122 |         41 |                   0 |                        0 |                           0 |                                0 |                      0.232258 |                      0.232258 |                             0 |                             0 |                             0 |                              0 |               0.0580645 |                0.174194 |                       0 |                      0 | False                | False                |                  1.77524 |                0.553188 |                               0.457143 |                             0.0722806 |           3.28571 |                   3 |          1.54127 |                    7 |                      6 |             3.09839 |                  1.08571 |                          1 |                0.368117 |       35 |              23 |                 0.657143 |          121 |           5 |
 
 
 
-
 # 📖 Documentation
 
 TextDescriptives has a detailed documentation as well as a series of Jupyter notebook tutorials.
 All the tutorials are located in the `docs/tutorials` folder and can also be found on the documentation website.
 
 
 | Documentation              |                                                                                    |
```

### Comparing `textdescriptives-2.4.5/docs/Makefile` & `textdescriptives-2.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/_static/icon.png` & `textdescriptives-2.4.6/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/_static/icon_dark_old.png` & `textdescriptives-2.4.6/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/_static/icon_old.png` & `textdescriptives-2.4.6/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/coherence.rst` & `textdescriptives-2.4.6/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/conf.py` & `textdescriptives-2.4.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/dependencydistance.rst` & `textdescriptives-2.4.6/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/descriptivestats.rst` & `textdescriptives-2.4.6/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/faq.rst` & `textdescriptives-2.4.6/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/index.rst` & `textdescriptives-2.4.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/information_theory.rst` & `textdescriptives-2.4.6/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/installation.rst` & `textdescriptives-2.4.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/make.bat` & `textdescriptives-2.4.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/news.rst` & `textdescriptives-2.4.6/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/posstats.rst` & `textdescriptives-2.4.6/docs/posstats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/quality.rst` & `textdescriptives-2.4.6/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/readability.rst` & `textdescriptives-2.4.6/docs/readability.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.4.6/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.4.6/docs/tutorials/introductory_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/docs/usingthepackage.rst` & `textdescriptives-2.4.6/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/paper/paper.bib` & `textdescriptives-2.4.6/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/paper/paper.md` & `textdescriptives-2.4.6/paper/paper.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,23 +44,27 @@
 
 Implementations of the majority of the metrics included in `TextDescriptives` exist, but none as feature complete. The `textstat` library [@ward_textstat_2022] implements the same readability metrics, however, each metric has to be extracted one at a time with no interface for multiple extractions. `spacy-readability` [@holtzscher_spacy-readability_2019] adds readability metrics to `spaCy` pipelines, but does not work for new versions of `spaCy` (>=3.0.0). The `textacy` [@dewilde_textacy_2021] package has some overlap with `TextDescriptives`, but with a different focus. `TextDescriptives` focuses on document-level metrics, and includes a large number of metrics not included in `textacy` (dependency distance, coherence, and quality), whereas `textacy` includes components for preprocessing, information extraction, and visualization that are outside the scope of `TextDescriptives`. What sets `TextDescriptives` apart is the easy access to document-level metrics through a simple user-facing API and exhaustive documentation. 
 
 
 # Features & Functionality
 
 `TextDescriptives` is a Python package and provides the following `spaCy` pipeline components:
-`textdescriptives.descriptive_stats`: Calculates the total number of tokens, number of unique tokens, number of characters, and the proportion of unique tokens, as well as the mean, median, and standard deviation of token length, sentence length, and the number of syllables per token.
-`textdescriptives.readability`: Calculates the Gunning-Fog index, the SMOG index, Flesch reading ease, Flesch-Kincaid grade, the Automated Readability Index, the Coleman-Liau index, the Lix score, and the Rix score.
-`textdescriptives.dependency_distance`: Calculates the mean and standard deviation of the dependency distance (the average distance between a word and its head word), and the mean and the standard deviation of the proportion adjacent dependency relations on the sentence level. 
-`textdescriptives.pos_proportions`: Calculates the proportions of all part-of-speech tags in the documents. 
-`textdescriptives.coherence`: Calculates the first- and second-order coherence of the document based on word embedding similarity between sentences.
-`textdescriptives.quality`: Calculates the text-quality metrics proposed in @rae_scaling_2022 and @raffel_exploring_2020. These measures can be used for filtering out low-quality text prior to model training or text analysis. These include heuristics such as the number of stop words, ratio of words containing alphabetic characters, proportion of lines ending with an ellipsis, proportion of lines starting with a bullet point, ratio of symbols to words, and whether the document contains a specified string (e.g. “lorem ipsum”), as well as repetitious text metrics such as the proportion of lines that are duplicates, the proportion of paragraphs in a document that are duplicates, the proportion of n-gram duplicates, and the proportion of characters in a document that are contained within the top n-grams. 
 
+- `textdescriptives.descriptive_stats`: Calculates the total number of tokens, number of unique tokens, number of characters, and the proportion of unique tokens, as well as the mean, median, and standard deviation of token length, sentence length, and the number of syllables per token.
+- `textdescriptives.readability`: Calculates the Gunning-Fog index, the SMOG index, Flesch reading ease, Flesch-Kincaid grade, the Automated Readability Index, the Coleman-Liau index, the Lix score, and the Rix score.
+-`textdescriptives.dependency_distance`: Calculates the mean and standard deviation of the dependency distance (the average distance between a word and its head word), and the mean and the standard deviation of the proportion adjacent dependency relations on the sentence level. 
+- `textdescriptives.pos_proportions`: Calculates the proportions of all part-of-speech tags in the documents. 
+- `textdescriptives.coherence`: Calculates the first- and second-order coherence of the document based on word embedding similarity between sentences.
+- `textdescriptives.information_theory`: Calculates the Shannon entropy and the perplexitiy of the documents.
+- `textdescriptives.quality`: Calculates the text-quality metrics proposed in @rae_scaling_2022 and @raffel_exploring_2020. These measures can be used for filtering out low-quality text prior to model training or text analysis. These include heuristics such as the number of stop words, ratio of words containing alphabetic characters, proportion of lines ending with an ellipsis, proportion of lines starting with a bullet point, ratio of symbols to words, and whether the document contains a specified string (e.g. “lorem ipsum”), as well as repetitious text metrics such as the proportion of lines that are duplicates, the proportion of paragraphs in a document that are duplicates, the proportion of n-gram duplicates, and the proportion of characters in a document that are contained within the top n-grams. 
 
-All the components can be added to an existing `spaCy` pipeline with a single line of code, and jointly extracted to a dataframe or dictionary with a single call to `textdescriptives.extract_{df|dict}(doc)`.
+
+All the components can be added to an existing `spaCy` pipeline with a single line of code, and jointly extracted to a dataframe or dictionary with a single call to `textdescriptives.extract_{df|dict}(doc)`. 
+
+To assist users who lack coding experience and to showcase the tool's capabilities, the core features of TextDescriptives are available as a web app on [https://huggingface.co/spaces/HLasse/textdescriptives](https://huggingface.co/spaces/HLasse/textdescriptives). With the web app, users can extract metrics from their own texts and download the results in a .csv file format.
 
 # Example Use Cases
 
 Descriptive statistics can be used to summarize and understand data, such as by exploring patterns and relationships within the data, getting a better understanding of the data set, or identifying any changes in the distribution of the data. Readability metrics, which assess the clarity and ease of understanding of written text, have a variety of applications, including the design of educational materials and the improvement of legal or technical documents [@dubay_principles_2004]. Dependency distance can be used as a measure of language comprehension difficulty or of sentence complexity and has been used for analysing properties of natural language or for similar purposes as readability metrics [@gibson_how_2019; @liu_dependency_2008]. The proportions of different parts of speech in a document have been found to be predictive of certain mental disorders and can also be used to assess the quality and complexity of text [@tang_natural_2021]. Semantic coherence, or the logical connection between sentences, has primarily been used in the field of computational psychiatry to predict the onset of psychosis or schizophrenia [@parola_speech_2022; @bedi_automated_2015], but it also has other applications in the digital humanities.  Measures of text quality are useful cleaning and identifying low-quality data [@rae_scaling_2022; @raffel_exploring_2020]. 
 
 
 # Target Audience
```

### Comparing `textdescriptives-2.4.5/paper/paper_quarto.pdf` & `textdescriptives-2.4.6/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/paper/paper_quarto.qmd` & `textdescriptives-2.4.6/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/pyproject.toml` & `textdescriptives-2.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textdescriptives"
-version = "2.4.5"
+version = "2.4.6"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"},
              {name = "Kenneth Enevoldsen"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/coherence.py` & `textdescriptives-2.4.6/src/textdescriptives/components/coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.4.6/src/textdescriptives/components/dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.4.6/src/textdescriptives/components/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.4.6/src/textdescriptives/components/information_theory.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.4.6/src/textdescriptives/components/pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/quality.py` & `textdescriptives-2.4.6/src/textdescriptives/components/quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.4.6/src/textdescriptives/components/quality_data_classes.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/readability.py` & `textdescriptives-2.4.6/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/components/utils.py` & `textdescriptives-2.4.6/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/data/spam.csv` & `textdescriptives-2.4.6/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/extractors.py` & `textdescriptives-2.4.6/src/textdescriptives/extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/load_components.py` & `textdescriptives-2.4.6/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives/utils.py` & `textdescriptives-2.4.6/src/textdescriptives/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.4.6/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.4.5
+Version: 2.4.6
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -308,15 +308,14 @@
 ```
 |      | text                      | first_order_coherence | second_order_coherence | pos_prop_DET | pos_prop_NOUN | pos_prop_AUX | pos_prop_VERB | pos_prop_PUNCT | pos_prop_PRON | pos_prop_ADP | pos_prop_ADV | pos_prop_SCONJ | flesch_reading_ease | flesch_kincaid_grade |    smog | gunning_fog | automated_readability_index | coleman_liau_index |     lix |  rix | n_stop_words | alpha_ratio | mean_word_length | doc_length | proportion_ellipsis | proportion_bullet_points | duplicate_line_chr_fraction | duplicate_paragraph_chr_fraction | duplicate_5-gram_chr_fraction | duplicate_6-gram_chr_fraction | duplicate_7-gram_chr_fraction | duplicate_8-gram_chr_fraction | duplicate_9-gram_chr_fraction | duplicate_10-gram_chr_fraction | top_2-gram_chr_fraction | top_3-gram_chr_fraction | top_4-gram_chr_fraction | symbol_#_to_word_ratio | contains_lorem ipsum | passed_quality_check | dependency_distance_mean | dependency_distance_std | prop_adjacent_dependency_relation_mean | prop_adjacent_dependency_relation_std | token_length_mean | token_length_median | token_length_std | sentence_length_mean | sentence_length_median | sentence_length_std | syllables_per_token_mean | syllables_per_token_median | syllables_per_token_std | n_tokens | n_unique_tokens | proportion_unique_tokens | n_characters | n_sentences |
 | ---: | :------------------------ | --------------------: | ---------------------: | -----------: | ------------: | -----------: | ------------: | -------------: | ------------: | -----------: | -----------: | -------------: | ------------------: | -------------------: | ------: | ----------: | --------------------------: | -----------------: | ------: | ---: | -----------: | ----------: | ---------------: | ---------: | ------------------: | -----------------------: | --------------------------: | -------------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | ----------------------------: | -----------------------------: | ----------------------: | ----------------------: | ----------------------: | ---------------------: | :------------------- | :------------------- | -----------------------: | ----------------------: | -------------------------------------: | ------------------------------------: | ----------------: | ------------------: | ---------------: | -------------------: | ---------------------: | ------------------: | -----------------------: | -------------------------: | ----------------------: | -------: | --------------: | -----------------------: | -----------: | ----------: |
 |    0 | The world is changed(...) |              0.633002 |               0.573323 |     0.097561 |      0.121951 |    0.0731707 |      0.170732 |       0.146341 |      0.195122 |    0.0731707 |    0.0731707 |      0.0487805 |             107.879 |           -0.0485714 | 5.68392 |     3.94286 |                    -2.45429 |          -0.708571 | 12.7143 |  0.4 |           24 |    0.853659 |          2.95122 |         41 |                   0 |                        0 |                           0 |                                0 |                      0.232258 |                      0.232258 |                             0 |                             0 |                             0 |                              0 |               0.0580645 |                0.174194 |                       0 |                      0 | False                | False                |                  1.77524 |                0.553188 |                               0.457143 |                             0.0722806 |           3.28571 |                   3 |          1.54127 |                    7 |                      6 |             3.09839 |                  1.08571 |                          1 |                0.368117 |       35 |              23 |                 0.657143 |          121 |           5 |
 
 
 
-
 # 📖 Documentation
 
 TextDescriptives has a detailed documentation as well as a series of Jupyter notebook tutorials.
 All the tutorials are located in the `docs/tutorials` folder and can also be found on the documentation website.
 
 
 | Documentation              |                                                                                    |
```

### Comparing `textdescriptives-2.4.5/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.4.6/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/books.py` & `textdescriptives-2.4.6/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_coherence.py` & `textdescriptives-2.4.6/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_dependency_distance.py` & `textdescriptives-2.4.6/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_descriptive_stats.py` & `textdescriptives-2.4.6/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_extractors.py` & `textdescriptives-2.4.6/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_information.py` & `textdescriptives-2.4.6/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_load_components.py` & `textdescriptives-2.4.6/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_pos_proportions.py` & `textdescriptives-2.4.6/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_quality.py` & `textdescriptives-2.4.6/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_readability.py` & `textdescriptives-2.4.6/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.5/tests/test_utils.py` & `textdescriptives-2.4.6/tests/test_utils.py`

 * *Files identical despite different names*

