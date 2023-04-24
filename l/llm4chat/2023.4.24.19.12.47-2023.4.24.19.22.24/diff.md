# Comparing `tmp/llm4chat-2023.4.24.19.12.47.tar.gz` & `tmp/llm4chat-2023.4.24.19.22.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4chat-2023.4.24.19.12.47.tar", last modified: Mon Apr 24 11:12:48 2023, max compression
+gzip compressed data, was "llm4chat-2023.4.24.19.22.24.tar", last modified: Mon Apr 24 11:22:24 2023, max compression
```

## Comparing `llm4chat-2023.4.24.19.12.47.tar` & `llm4chat-2023.4.24.19.22.24.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.205452 llm4chat-2023.4.24.19.12.47/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4chat-2023.4.24.19.12.47/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 11:12:48.205563 llm4chat-2023.4.24.19.12.47/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4chat-2023.4.24.19.12.47/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/README.rst
--rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 llm4chat-2023.4.24.19.12.47/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.173487 llm4chat-2023.4.24.19.12.47/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.177311 llm4chat-2023.4.24.19.12.47/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4chat-2023.4.24.19.12.47/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4chat-2023.4.24.19.12.47/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.196752 llm4chat-2023.4.24.19.12.47/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4chat-2023.4.24.19.12.47/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4chat-2023.4.24.19.12.47/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4chat-2023.4.24.19.12.47/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.197741 llm4chat-2023.4.24.19.12.47/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.199866 llm4chat-2023.4.24.19.12.47/llm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3528 2023-04-24 09:58:56.000000 llm4chat-2023.4.24.19.12.47/llm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      321 2023-04-24 10:13:55.000000 llm4chat-2023.4.24.19.12.47/llm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      766 2023-04-24 10:14:22.000000 llm4chat-2023.4.24.19.12.47/llm/applications/ann4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4chat-2023.4.24.19.12.47/llm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     1159 2023-04-24 10:42:45.000000 llm4chat-2023.4.24.19.12.47/llm/applications/crawler4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4chat-2023.4.24.19.12.47/llm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     2801 2023-04-24 11:12:46.000000 llm4chat-2023.4.24.19.12.47/llm/applications/qa.py
--rw-r--r--   0 betterme   (501) staff       (20)     1842 2023-04-21 11:25:02.000000 llm4chat-2023.4.24.19.12.47/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.200307 llm4chat-2023.4.24.19.12.47/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.201139 llm4chat-2023.4.24.19.12.47/llm/docutils/
--rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.19.12.47/llm/docutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4chat-2023.4.24.19.12.47/llm/docutils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.19.12.47/llm/docutils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.202126 llm4chat-2023.4.24.19.12.47/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4chat-2023.4.24.19.12.47/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4chat-2023.4.24.19.12.47/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4chat-2023.4.24.19.12.47/llm/kb/kbqa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.202649 llm4chat-2023.4.24.19.12.47/llm/knowledge_base/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4chat-2023.4.24.19.12.47/llm/knowledge_base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4chat-2023.4.24.19.12.47/llm/knowledge_base/lite.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4chat-2023.4.24.19.12.47/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.203122 llm4chat-2023.4.24.19.12.47/llm/textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.19.12.47/llm/textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      848 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.19.12.47/llm/textsplitter/chinese_text_splitter.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.203688 llm4chat-2023.4.24.19.12.47/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4chat-2023.4.24.19.12.47/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3941 2023-04-24 11:12:46.000000 llm4chat-2023.4.24.19.12.47/llm/uis/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     2995 2023-04-24 10:13:55.000000 llm4chat-2023.4.24.19.12.47/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.204897 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1452 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4chat-2023.4.24.19.12.47/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-24 11:12:48.205894 llm4chat-2023.4.24.19.12.47/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1514 2023-04-23 11:26:59.000000 llm4chat-2023.4.24.19.12.47/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.205275 llm4chat-2023.4.24.19.12.47/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.595384 llm4chat-2023.4.24.19.22.24/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4chat-2023.4.24.19.22.24/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 11:22:24.595498 llm4chat-2023.4.24.19.22.24/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4chat-2023.4.24.19.22.24/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/README.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 llm4chat-2023.4.24.19.22.24/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.584173 llm4chat-2023.4.24.19.22.24/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.586279 llm4chat-2023.4.24.19.22.24/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4chat-2023.4.24.19.22.24/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4chat-2023.4.24.19.22.24/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.22.24/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.22.24/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.22.24/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.22.24/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.590422 llm4chat-2023.4.24.19.22.24/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4chat-2023.4.24.19.22.24/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4chat-2023.4.24.19.22.24/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4chat-2023.4.24.19.22.24/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.590894 llm4chat-2023.4.24.19.22.24/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.591957 llm4chat-2023.4.24.19.22.24/llm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3528 2023-04-24 09:58:56.000000 llm4chat-2023.4.24.19.22.24/llm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      325 2023-04-24 11:17:43.000000 llm4chat-2023.4.24.19.22.24/llm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      766 2023-04-24 10:14:22.000000 llm4chat-2023.4.24.19.22.24/llm/applications/ann4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-24 11:20:53.000000 llm4chat-2023.4.24.19.22.24/llm/applications/chat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4chat-2023.4.24.19.22.24/llm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-04-24 11:20:53.000000 llm4chat-2023.4.24.19.22.24/llm/applications/crawler4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4chat-2023.4.24.19.22.24/llm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1842 2023-04-21 11:25:02.000000 llm4chat-2023.4.24.19.22.24/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.592369 llm4chat-2023.4.24.19.22.24/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.592787 llm4chat-2023.4.24.19.22.24/llm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.19.22.24/llm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4chat-2023.4.24.19.22.24/llm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.19.22.24/llm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.593224 llm4chat-2023.4.24.19.22.24/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4chat-2023.4.24.19.22.24/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4chat-2023.4.24.19.22.24/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4chat-2023.4.24.19.22.24/llm/kb/kbqa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.593485 llm4chat-2023.4.24.19.22.24/llm/knowledge_base/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4chat-2023.4.24.19.22.24/llm/knowledge_base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4chat-2023.4.24.19.22.24/llm/knowledge_base/lite.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4chat-2023.4.24.19.22.24/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.593754 llm4chat-2023.4.24.19.22.24/llm/textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.19.22.24/llm/textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      848 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.19.22.24/llm/textsplitter/chinese_text_splitter.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.594043 llm4chat-2023.4.24.19.22.24/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4chat-2023.4.24.19.22.24/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3915 2023-04-24 11:22:03.000000 llm4chat-2023.4.24.19.22.24/llm/uis/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2995 2023-04-24 10:13:55.000000 llm4chat-2023.4.24.19.22.24/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.594982 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 11:22:24.000000 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1454 2023-04-24 11:22:24.000000 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 11:22:24.000000 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-24 11:22:24.000000 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 11:22:24.000000 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-24 11:22:24.000000 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-24 11:22:24.000000 llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4chat-2023.4.24.19.22.24/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-24 11:22:24.595802 llm4chat-2023.4.24.19.22.24/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1514 2023-04-23 11:26:59.000000 llm4chat-2023.4.24.19.22.24/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:22:24.595266 llm4chat-2023.4.24.19.22.24/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.22.24/tox.ini
```

### Comparing `llm4chat-2023.4.24.19.12.47/.gitignore` & `llm4chat-2023.4.24.19.22.24/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/.travis.yml` & `llm4chat-2023.4.24.19.22.24/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/CONTRIBUTING.rst` & `llm4chat-2023.4.24.19.22.24/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/LICENSE` & `llm4chat-2023.4.24.19.22.24/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/Makefile` & `llm4chat-2023.4.24.19.22.24/Makefile`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/PKG-INFO` & `llm4chat-2023.4.24.19.22.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4chat
-Version: 2023.4.24.19.12.47
+Version: 2023.4.24.19.22.24
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4chat
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4chat-2023.4.24.19.12.47/README.md` & `llm4chat-2023.4.24.19.22.24/README.md`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/README.rst` & `llm4chat-2023.4.24.19.22.24/README.rst`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/data/医/500种中药现代研究.txt` & `llm4chat-2023.4.24.19.22.24/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/data/医/古今医统大全.txt` & `llm4chat-2023.4.24.19.22.24/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/data/姚明.txt` & `llm4chat-2023.4.24.19.22.24/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/data/王治郅.txt` & `llm4chat-2023.4.24.19.22.24/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/data/科比.txt` & `llm4chat-2023.4.24.19.22.24/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/docs/Makefile` & `llm4chat-2023.4.24.19.22.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/docs/README.md` & `llm4chat-2023.4.24.19.22.24/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/docs/conf.py` & `llm4chat-2023.4.24.19.22.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/docs/img.png` & `llm4chat-2023.4.24.19.22.24/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/docs/installation.rst` & `llm4chat-2023.4.24.19.22.24/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/docs/make.bat` & `llm4chat-2023.4.24.19.22.24/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/applications/Question2Answer.py` & `llm4chat-2023.4.24.19.22.24/llm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/applications/ann4qa.py` & `llm4chat-2023.4.24.19.22.24/llm/applications/ann4qa.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/applications/crawler4qa.py` & `llm4chat-2023.4.24.19.22.24/llm/applications/crawler4qa.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # @Software     : PyCharm
 # @Description  :
 
 
 from meutils.pipe import *
 from meutils.request_utils.crawler import Crawler
 
-from llm.applications.qa import QA
+from llm.applications import Chat
 
 
-class Crawler4QA(QA):
+class Crawler4QA(Chat):
 
     def __init__(self, chat_func):
         super().__init__(chat_func)
 
     def qa(self, query,
            url="https://top.baidu.com/board?tab=realtime",
            xpath='//*[@id="sanRoot"]/main/div[2]/div/div[2]/div[*]/div[2]/a/div[1]//text()', **kwargs):
```

### Comparing `llm4chat-2023.4.24.19.12.47/llm/applications/qa.py` & `llm4chat-2023.4.24.19.22.24/llm/applications/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # @Software     : PyCharm
 # @Description  :
 import types
 from meutils.pipe import *
 from meutils.decorators import clear_cuda_cache
 
 
-class QA(object):
+class Chat(object):
 
     def __init__(self, chat_func, prompt_template=None):
         self.chat_func = chat_func
 
         self.history = []
         self.knowledge_base = None
 
@@ -73,11 +73,11 @@
 if __name__ == '__main__':
     from llm.utils import llm_load4chat
 
     chat_func = llm_load4chat(
         model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm",
         device='mps')
 
-    qa = QA(chat_func=chat_func)
+    qa = Chat(chat_func=chat_func)
 
     for i, _ in qa(query='提取关键词', knowledge_base='我今天去听了周杰伦的演唱会'):
         print(i, flush=True)
```

### Comparing `llm4chat-2023.4.24.19.12.47/llm/chatllm.py` & `llm4chat-2023.4.24.19.22.24/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/clis/cli.py` & `llm4chat-2023.4.24.19.22.24/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/docutils/doc_embedding.py` & `llm4chat-2023.4.24.19.22.24/llm/docutils/doc_embedding.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/kb/FaissANN.py` & `llm4chat-2023.4.24.19.22.24/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/qa.py` & `llm4chat-2023.4.24.19.22.24/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/textsplitter/chinese_text_splitter.py` & `llm4chat-2023.4.24.19.22.24/llm/textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm/uis/gradio_ui.py` & `llm4chat-2023.4.24.19.22.24/llm/uis/gradio_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 from meutils.pipe import *
 from transformers import AutoModel, AutoTokenizer
 import gradio as gr
 import mdtex2html
 
 MODEL = '/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm'
 
-from llm.utils import llm_load
+from llm.utils import llm_load, llm_load4chat
+from llm.applications import Chat
 
-model, tokenizer = llm_load(MODEL)
+chat_func = llm_load4chat(MODEL, device='mps')
 
-#
-# from llm.utils import llm_load4chat
-#
-# chat = llm_load4chat(MODEL, device='mps')
+qa = Chat(chat_func)
 
 """Override Chatbot.postprocess"""
 
 
 def postprocess(self, y):
     if y is None:
         return []
@@ -70,22 +68,21 @@
                     line = line.replace(")", "&#41;")
                     line = line.replace("$", "&#36;")
                 lines[i] = "<br>" + line
     text = "".join(lines)
     return text
 
 
-def predict(input, chatbot, max_length, top_p, temperature, history):
+def predict(input, chatbot, max_length, top_p, temperature, history, knowledge_base=''):
     chatbot.append((parse_text(input), ""))
-    print(chatbot)
 
-    for response, history in model.stream_chat(tokenizer, input, history, max_length=max_length, top_p=top_p,
-                                               temperature=temperature):
-        chatbot[-1] = (parse_text(input), parse_text(response))
+    qa.set_chat_kwargs(max_length=max_length, top_p=top_p, temperature=temperature)
 
+    for response, history in qa(query=input, knowledge_base=knowledge_base):
+        chatbot[-1] = (parse_text(input), parse_text(response))
         yield chatbot, history
 
 
 def reset_user_input():
     return gr.update(value='')
```

### Comparing `llm4chat-2023.4.24.19.12.47/llm/utils.py` & `llm4chat-2023.4.24.19.22.24/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/PKG-INFO` & `llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4chat
-Version: 2023.4.24.19.12.47
+Version: 2023.4.24.19.22.24
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4chat
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/SOURCES.txt` & `llm4chat-2023.4.24.19.22.24/llm4chat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 llm/__init__.py
 llm/chatllm.py
 llm/qa.py
 llm/utils.py
 llm/applications/Question2Answer.py
 llm/applications/__init__.py
 llm/applications/ann4qa.py
+llm/applications/chat.py
 llm/applications/chatpdf.py
 llm/applications/crawler4qa.py
 llm/applications/pipeline.py
-llm/applications/qa.py
 llm/clis/README.md
 llm/clis/__init__.py
 llm/clis/cli.py
 llm/docutils/__init__.py
 llm/docutils/doc_embedding.py
 llm/docutils/doc_parse.py
 llm/kb/FaissANN.py
```

### Comparing `llm4chat-2023.4.24.19.12.47/setup.py` & `llm4chat-2023.4.24.19.22.24/setup.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.19.12.47/tests/test_llm4gpt.py` & `llm4chat-2023.4.24.19.22.24/tests/test_llm4gpt.py`

 * *Files identical despite different names*

