# Comparing `tmp/llm4chat-2023.4.24.18.52.28.tar.gz` & `tmp/llm4chat-2023.4.24.19.12.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4chat-2023.4.24.18.52.28.tar", last modified: Mon Apr 24 10:52:28 2023, max compression
+gzip compressed data, was "llm4chat-2023.4.24.19.12.47.tar", last modified: Mon Apr 24 11:12:48 2023, max compression
```

## Comparing `llm4chat-2023.4.24.18.52.28.tar` & `llm4chat-2023.4.24.19.12.47.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.752390 llm4chat-2023.4.24.18.52.28/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4chat-2023.4.24.18.52.28/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 10:52:28.752502 llm4chat-2023.4.24.18.52.28/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4chat-2023.4.24.18.52.28/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/README.rst
--rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 llm4chat-2023.4.24.18.52.28/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.740652 llm4chat-2023.4.24.18.52.28/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.742889 llm4chat-2023.4.24.18.52.28/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4chat-2023.4.24.18.52.28/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4chat-2023.4.24.18.52.28/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.18.52.28/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.18.52.28/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.18.52.28/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.18.52.28/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.747532 llm4chat-2023.4.24.18.52.28/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4chat-2023.4.24.18.52.28/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4chat-2023.4.24.18.52.28/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4chat-2023.4.24.18.52.28/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.748026 llm4chat-2023.4.24.18.52.28/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/llm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.748895 llm4chat-2023.4.24.18.52.28/llm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3528 2023-04-24 09:58:56.000000 llm4chat-2023.4.24.18.52.28/llm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      321 2023-04-24 10:13:55.000000 llm4chat-2023.4.24.18.52.28/llm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      766 2023-04-24 10:14:22.000000 llm4chat-2023.4.24.18.52.28/llm/applications/ann4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4chat-2023.4.24.18.52.28/llm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     1159 2023-04-24 10:42:45.000000 llm4chat-2023.4.24.18.52.28/llm/applications/crawler4qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4chat-2023.4.24.18.52.28/llm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     2700 2023-04-24 10:48:32.000000 llm4chat-2023.4.24.18.52.28/llm/applications/qa.py
--rw-r--r--   0 betterme   (501) staff       (20)     1842 2023-04-21 11:25:02.000000 llm4chat-2023.4.24.18.52.28/llm/chatllm.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.749278 llm4chat-2023.4.24.18.52.28/llm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/llm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/llm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/llm/clis/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.749667 llm4chat-2023.4.24.18.52.28/llm/docutils/
--rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.18.52.28/llm/docutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4chat-2023.4.24.18.52.28/llm/docutils/doc_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.18.52.28/llm/docutils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.750043 llm4chat-2023.4.24.18.52.28/llm/kb/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4chat-2023.4.24.18.52.28/llm/kb/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4chat-2023.4.24.18.52.28/llm/kb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4chat-2023.4.24.18.52.28/llm/kb/kbqa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.750313 llm4chat-2023.4.24.18.52.28/llm/knowledge_base/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4chat-2023.4.24.18.52.28/llm/knowledge_base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4chat-2023.4.24.18.52.28/llm/knowledge_base/lite.py
--rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4chat-2023.4.24.18.52.28/llm/qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.750591 llm4chat-2023.4.24.18.52.28/llm/textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.18.52.28/llm/textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      848 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.18.52.28/llm/textsplitter/chinese_text_splitter.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.750742 llm4chat-2023.4.24.18.52.28/llm/uis/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4chat-2023.4.24.18.52.28/llm/uis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2995 2023-04-24 10:13:55.000000 llm4chat-2023.4.24.18.52.28/llm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.751961 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 10:52:28.000000 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1431 2023-04-24 10:52:28.000000 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 10:52:28.000000 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-24 10:52:28.000000 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 10:52:28.000000 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-24 10:52:28.000000 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-24 10:52:28.000000 llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/top_level.txt
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4chat-2023.4.24.18.52.28/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-24 10:52:28.752812 llm4chat-2023.4.24.18.52.28/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1514 2023-04-23 11:26:59.000000 llm4chat-2023.4.24.18.52.28/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 10:52:28.752256 llm4chat-2023.4.24.18.52.28/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.18.52.28/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.205452 llm4chat-2023.4.24.19.12.47/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 llm4chat-2023.4.24.19.12.47/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 11:12:48.205563 llm4chat-2023.4.24.19.12.47/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1304 2023-04-20 12:13:34.000000 llm4chat-2023.4.24.19.12.47/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/README.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       47 2023-04-23 12:20:03.000000 llm4chat-2023.4.24.19.12.47/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.173487 llm4chat-2023.4.24.19.12.47/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.177311 llm4chat-2023.4.24.19.12.47/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 llm4chat-2023.4.24.19.12.47/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 llm4chat-2023.4.24.19.12.47/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 llm4chat-2023.4.24.19.12.47/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.196752 llm4chat-2023.4.24.19.12.47/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1315 2023-04-20 11:42:00.000000 llm4chat-2023.4.24.19.12.47/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 llm4chat-2023.4.24.19.12.47/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 llm4chat-2023.4.24.19.12.47/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.197741 llm4chat-2023.4.24.19.12.47/llm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.199866 llm4chat-2023.4.24.19.12.47/llm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3528 2023-04-24 09:58:56.000000 llm4chat-2023.4.24.19.12.47/llm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      321 2023-04-24 10:13:55.000000 llm4chat-2023.4.24.19.12.47/llm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      766 2023-04-24 10:14:22.000000 llm4chat-2023.4.24.19.12.47/llm/applications/ann4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-21 03:44:25.000000 llm4chat-2023.4.24.19.12.47/llm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1159 2023-04-24 10:42:45.000000 llm4chat-2023.4.24.19.12.47/llm/applications/crawler4qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 llm4chat-2023.4.24.19.12.47/llm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2801 2023-04-24 11:12:46.000000 llm4chat-2023.4.24.19.12.47/llm/applications/qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1842 2023-04-21 11:25:02.000000 llm4chat-2023.4.24.19.12.47/llm/chatllm.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.200307 llm4chat-2023.4.24.19.12.47/llm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/llm/clis/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.201139 llm4chat-2023.4.24.19.12.47/llm/docutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      295 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.19.12.47/llm/docutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 07:32:03.000000 llm4chat-2023.4.24.19.12.47/llm/docutils/doc_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 llm4chat-2023.4.24.19.12.47/llm/docutils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.202126 llm4chat-2023.4.24.19.12.47/llm/kb/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 llm4chat-2023.4.24.19.12.47/llm/kb/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-04-20 11:55:45.000000 llm4chat-2023.4.24.19.12.47/llm/kb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-04-21 03:56:52.000000 llm4chat-2023.4.24.19.12.47/llm/kb/kbqa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.202649 llm4chat-2023.4.24.19.12.47/llm/knowledge_base/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-21 03:47:12.000000 llm4chat-2023.4.24.19.12.47/llm/knowledge_base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      317 2023-04-21 04:31:21.000000 llm4chat-2023.4.24.19.12.47/llm/knowledge_base/lite.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2510 2023-04-20 12:07:40.000000 llm4chat-2023.4.24.19.12.47/llm/qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.203122 llm4chat-2023.4.24.19.12.47/llm/textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.19.12.47/llm/textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      848 2023-04-20 03:13:45.000000 llm4chat-2023.4.24.19.12.47/llm/textsplitter/chinese_text_splitter.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.203688 llm4chat-2023.4.24.19.12.47/llm/uis/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 llm4chat-2023.4.24.19.12.47/llm/uis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3941 2023-04-24 11:12:46.000000 llm4chat-2023.4.24.19.12.47/llm/uis/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2995 2023-04-24 10:13:55.000000 llm4chat-2023.4.24.19.12.47/llm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.204897 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     2123 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1452 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-04-24 11:12:48.000000 llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/top_level.txt
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 llm4chat-2023.4.24.19.12.47/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      390 2023-04-24 11:12:48.205894 llm4chat-2023.4.24.19.12.47/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1514 2023-04-23 11:26:59.000000 llm4chat-2023.4.24.19.12.47/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-24 11:12:48.205275 llm4chat-2023.4.24.19.12.47/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 llm4chat-2023.4.24.19.12.47/tox.ini
```

### Comparing `llm4chat-2023.4.24.18.52.28/.gitignore` & `llm4chat-2023.4.24.19.12.47/.gitignore`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/.travis.yml` & `llm4chat-2023.4.24.19.12.47/.travis.yml`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/CONTRIBUTING.rst` & `llm4chat-2023.4.24.19.12.47/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/LICENSE` & `llm4chat-2023.4.24.19.12.47/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/Makefile` & `llm4chat-2023.4.24.19.12.47/Makefile`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/PKG-INFO` & `llm4chat-2023.4.24.19.12.47/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4chat
-Version: 2023.4.24.18.52.28
+Version: 2023.4.24.19.12.47
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4chat
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4chat-2023.4.24.18.52.28/README.md` & `llm4chat-2023.4.24.19.12.47/README.md`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/README.rst` & `llm4chat-2023.4.24.19.12.47/README.rst`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/data/医/500种中药现代研究.txt` & `llm4chat-2023.4.24.19.12.47/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/data/医/古今医统大全.txt` & `llm4chat-2023.4.24.19.12.47/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/data/姚明.txt` & `llm4chat-2023.4.24.19.12.47/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/data/王治郅.txt` & `llm4chat-2023.4.24.19.12.47/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/data/科比.txt` & `llm4chat-2023.4.24.19.12.47/data/科比.txt`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/docs/Makefile` & `llm4chat-2023.4.24.19.12.47/docs/Makefile`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/docs/README.md` & `llm4chat-2023.4.24.19.12.47/docs/README.md`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/docs/conf.py` & `llm4chat-2023.4.24.19.12.47/docs/conf.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/docs/img.png` & `llm4chat-2023.4.24.19.12.47/docs/img.png`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/docs/installation.rst` & `llm4chat-2023.4.24.19.12.47/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/docs/make.bat` & `llm4chat-2023.4.24.19.12.47/docs/make.bat`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/applications/Question2Answer.py` & `llm4chat-2023.4.24.19.12.47/llm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/applications/ann4qa.py` & `llm4chat-2023.4.24.19.12.47/llm/applications/ann4qa.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/applications/crawler4qa.py` & `llm4chat-2023.4.24.19.12.47/llm/applications/crawler4qa.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/applications/qa.py` & `llm4chat-2023.4.24.19.12.47/llm/applications/qa.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,17 @@
             如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的相关信息"，不允许在答案中添加编造成分，答案请使用中文。
             已知内容: {context}
             问题: {question}
             """.strip()
 
         return prompt_template
 
+    def set_chat_kwargs(self, **kwargs):
+        self.chat_func = partial(self.chat_func, **kwargs)
+
 
 if __name__ == '__main__':
     from llm.utils import llm_load4chat
 
     chat_func = llm_load4chat(
         model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm",
         device='mps')
```

### Comparing `llm4chat-2023.4.24.18.52.28/llm/chatllm.py` & `llm4chat-2023.4.24.19.12.47/llm/chatllm.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/clis/cli.py` & `llm4chat-2023.4.24.19.12.47/llm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/docutils/doc_embedding.py` & `llm4chat-2023.4.24.19.12.47/llm/docutils/doc_embedding.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/kb/FaissANN.py` & `llm4chat-2023.4.24.19.12.47/llm/kb/FaissANN.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/qa.py` & `llm4chat-2023.4.24.19.12.47/llm/qa.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/textsplitter/chinese_text_splitter.py` & `llm4chat-2023.4.24.19.12.47/llm/textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm/utils.py` & `llm4chat-2023.4.24.19.12.47/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/PKG-INFO` & `llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm4chat
-Version: 2023.4.24.18.52.28
+Version: 2023.4.24.19.12.47
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/llm4gpt
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: llm4chat
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `llm4chat-2023.4.24.18.52.28/llm4chat.egg-info/SOURCES.txt` & `llm4chat-2023.4.24.19.12.47/llm4chat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 llm/kb/__init__.py
 llm/kb/kbqa.py
 llm/knowledge_base/__init__.py
 llm/knowledge_base/lite.py
 llm/textsplitter/__init__.py
 llm/textsplitter/chinese_text_splitter.py
 llm/uis/__init__.py
+llm/uis/gradio_ui.py
 llm4chat.egg-info/PKG-INFO
 llm4chat.egg-info/SOURCES.txt
 llm4chat.egg-info/dependency_links.txt
 llm4chat.egg-info/entry_points.txt
 llm4chat.egg-info/not-zip-safe
 llm4chat.egg-info/requires.txt
 llm4chat.egg-info/top_level.txt
```

### Comparing `llm4chat-2023.4.24.18.52.28/setup.py` & `llm4chat-2023.4.24.19.12.47/setup.py`

 * *Files identical despite different names*

### Comparing `llm4chat-2023.4.24.18.52.28/tests/test_llm4gpt.py` & `llm4chat-2023.4.24.19.12.47/tests/test_llm4gpt.py`

 * *Files identical despite different names*

