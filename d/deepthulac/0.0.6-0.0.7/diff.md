# Comparing `tmp/deepthulac-0.0.6.tar.gz` & `tmp/deepthulac-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepthulac-0.0.6.tar", last modified: Mon Apr 24 06:43:44 2023, max compression
+gzip compressed data, was "deepthulac-0.0.7.tar", last modified: Mon Apr 24 06:50:14 2023, max compression
```

## Comparing `deepthulac-0.0.6.tar` & `deepthulac-0.0.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.538138 deepthulac-0.0.6/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1063 2022-11-01 11:55:55.000000 deepthulac-0.0.6/LICENSE
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-04-24 06:43:44.534138 deepthulac-0.0.6/PKG-INFO
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1856 2023-03-16 08:01:08.000000 deepthulac-0.0.6/README.md
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.346139 deepthulac-0.0.6/deepthulac/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       34 2023-01-23 14:34:36.000000 deepthulac-0.0.6/deepthulac/__init__.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.374139 deepthulac-0.0.6/deepthulac/eval/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:36:21.000000 deepthulac-0.0.6/deepthulac/eval/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3851 2023-04-11 20:06:26.000000 deepthulac-0.0.6/deepthulac/eval/cases.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    38907 2023-03-05 17:38:25.000000 deepthulac-0.0.6/deepthulac/eval/old_model.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    13991 2023-03-21 07:52:38.000000 deepthulac-0.0.6/deepthulac/eval/test.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     4199 2023-02-17 12:27:02.000000 deepthulac-0.0.6/deepthulac/eval/third_party_api.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.382139 deepthulac-0.0.6/deepthulac/legacy/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11114 2023-02-08 11:48:00.000000 deepthulac-0.0.6/deepthulac/legacy/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      190 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/__main__.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.398139 deepthulac-0.0.6/deepthulac/legacy/base/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2117 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/AlphaBeta.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7965 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/Dat.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       67 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/Node.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      137 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/WordWithTag.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1053 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/compatibility.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.406139 deepthulac-0.0.6/deepthulac/legacy/character/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2094 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/character/CBModel.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3995 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/character/CBNGramFeature.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7605 2023-04-24 06:29:06.000000 deepthulac-0.0.6/deepthulac/legacy/character/CBTaggingDecoder.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/character/__init__.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.430139 deepthulac-0.0.6/deepthulac/legacy/manage/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2792 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Filter.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2550 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Postprocesser.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     9839 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Preprocesser.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1600 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Punctuation.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1220 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/SoExtention.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5475 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/TimeWord.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      557 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/verbword.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    30810 2023-02-26 16:12:20.000000 deepthulac-0.0.6/deepthulac/model_old.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.534138 deepthulac-0.0.6/deepthulac/seg/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:29.000000 deepthulac-0.0.6/deepthulac/seg/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5188 2023-03-16 08:06:21.000000 deepthulac-0.0.6/deepthulac/seg/cut_sent.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    23373 2023-04-11 21:05:24.000000 deepthulac-0.0.6/deepthulac/seg/data_format.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11200 2023-02-17 17:07:25.000000 deepthulac-0.0.6/deepthulac/seg/eval.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    38541 2023-04-11 21:52:24.000000 deepthulac-0.0.6/deepthulac/seg/model.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3144 2023-04-24 06:39:11.000000 deepthulac-0.0.6/deepthulac/seg/post_process.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5898 2023-04-12 19:02:05.000000 deepthulac-0.0.6/deepthulac/seg/seg_utils.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5258 2023-03-21 07:39:11.000000 deepthulac-0.0.6/deepthulac/seg/train.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     8818 2023-03-19 21:55:47.000000 deepthulac-0.0.6/deepthulac/utils.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.362139 deepthulac-0.0.6/deepthulac.egg-info/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/PKG-INFO
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1369 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/SOURCES.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        1 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/dependency_links.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       79 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/requires.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       11 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/top_level.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       38 2023-04-24 06:43:44.538138 deepthulac-0.0.6/setup.cfg
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1521 2023-04-24 06:40:30.000000 deepthulac-0.0.6/setup.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:14.508907 deepthulac-0.0.7/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1063 2022-11-01 11:55:55.000000 deepthulac-0.0.7/LICENSE
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-04-24 06:50:14.432907 deepthulac-0.0.7/PKG-INFO
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1856 2023-03-16 08:01:08.000000 deepthulac-0.0.7/README.md
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:12.096915 deepthulac-0.0.7/deepthulac/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       34 2023-01-23 14:34:36.000000 deepthulac-0.0.7/deepthulac/__init__.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:12.724913 deepthulac-0.0.7/deepthulac/eval/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:36:21.000000 deepthulac-0.0.7/deepthulac/eval/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3851 2023-04-11 20:06:26.000000 deepthulac-0.0.7/deepthulac/eval/cases.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    38907 2023-03-05 17:38:25.000000 deepthulac-0.0.7/deepthulac/eval/old_model.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    13991 2023-03-21 07:52:38.000000 deepthulac-0.0.7/deepthulac/eval/test.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     4199 2023-02-17 12:27:02.000000 deepthulac-0.0.7/deepthulac/eval/third_party_api.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:12.864913 deepthulac-0.0.7/deepthulac/legacy/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11114 2023-02-08 11:48:00.000000 deepthulac-0.0.7/deepthulac/legacy/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      190 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/__main__.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:13.200911 deepthulac-0.0.7/deepthulac/legacy/base/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2117 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/base/AlphaBeta.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7965 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/base/Dat.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       67 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/base/Node.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      137 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/base/WordWithTag.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/base/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1053 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/base/compatibility.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:13.468911 deepthulac-0.0.7/deepthulac/legacy/character/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2094 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/character/CBModel.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3995 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/character/CBNGramFeature.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7605 2023-04-24 06:29:06.000000 deepthulac-0.0.7/deepthulac/legacy/character/CBTaggingDecoder.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/character/__init__.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:13.872909 deepthulac-0.0.7/deepthulac/legacy/manage/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2792 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/Filter.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2550 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/Postprocesser.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     9839 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/Preprocesser.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1600 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/Punctuation.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1220 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/SoExtention.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5475 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/TimeWord.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      557 2023-01-16 16:22:28.000000 deepthulac-0.0.7/deepthulac/legacy/manage/verbword.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    30810 2023-02-26 16:12:20.000000 deepthulac-0.0.7/deepthulac/model_old.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:14.356908 deepthulac-0.0.7/deepthulac/seg/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:29.000000 deepthulac-0.0.7/deepthulac/seg/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5188 2023-03-16 08:06:21.000000 deepthulac-0.0.7/deepthulac/seg/cut_sent.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    23373 2023-04-11 21:05:24.000000 deepthulac-0.0.7/deepthulac/seg/data_format.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11200 2023-02-17 17:07:25.000000 deepthulac-0.0.7/deepthulac/seg/eval.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    38541 2023-04-11 21:52:24.000000 deepthulac-0.0.7/deepthulac/seg/model.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3149 2023-04-24 06:47:36.000000 deepthulac-0.0.7/deepthulac/seg/post_process.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5898 2023-04-12 19:02:05.000000 deepthulac-0.0.7/deepthulac/seg/seg_utils.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5258 2023-03-21 07:39:11.000000 deepthulac-0.0.7/deepthulac/seg/train.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     8818 2023-03-19 21:55:47.000000 deepthulac-0.0.7/deepthulac/utils.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:50:12.432914 deepthulac-0.0.7/deepthulac.egg-info/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-04-24 06:50:11.000000 deepthulac-0.0.7/deepthulac.egg-info/PKG-INFO
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1369 2023-04-24 06:50:11.000000 deepthulac-0.0.7/deepthulac.egg-info/SOURCES.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        1 2023-04-24 06:50:11.000000 deepthulac-0.0.7/deepthulac.egg-info/dependency_links.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       79 2023-04-24 06:50:11.000000 deepthulac-0.0.7/deepthulac.egg-info/requires.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       11 2023-04-24 06:50:11.000000 deepthulac-0.0.7/deepthulac.egg-info/top_level.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       38 2023-04-24 06:50:14.508907 deepthulac-0.0.7/setup.cfg
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1521 2023-04-24 06:50:02.000000 deepthulac-0.0.7/setup.py
```

### Comparing `deepthulac-0.0.6/LICENSE` & `deepthulac-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/README.md` & `deepthulac-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/eval/cases.py` & `deepthulac-0.0.7/deepthulac/eval/cases.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/eval/old_model.py` & `deepthulac-0.0.7/deepthulac/eval/old_model.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/eval/test.py` & `deepthulac-0.0.7/deepthulac/eval/test.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/eval/third_party_api.py` & `deepthulac-0.0.7/deepthulac/eval/third_party_api.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/__init__.py` & `deepthulac-0.0.7/deepthulac/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/base/AlphaBeta.py` & `deepthulac-0.0.7/deepthulac/legacy/base/AlphaBeta.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/base/Dat.py` & `deepthulac-0.0.7/deepthulac/legacy/base/Dat.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/base/compatibility.py` & `deepthulac-0.0.7/deepthulac/legacy/base/compatibility.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/character/CBModel.py` & `deepthulac-0.0.7/deepthulac/legacy/character/CBModel.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/character/CBNGramFeature.py` & `deepthulac-0.0.7/deepthulac/legacy/character/CBNGramFeature.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/character/CBTaggingDecoder.py` & `deepthulac-0.0.7/deepthulac/legacy/character/CBTaggingDecoder.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/manage/Filter.py` & `deepthulac-0.0.7/deepthulac/legacy/manage/Filter.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/manage/Postprocesser.py` & `deepthulac-0.0.7/deepthulac/legacy/manage/Postprocesser.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/manage/Preprocesser.py` & `deepthulac-0.0.7/deepthulac/legacy/manage/Preprocesser.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/manage/Punctuation.py` & `deepthulac-0.0.7/deepthulac/legacy/manage/Punctuation.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/manage/SoExtention.py` & `deepthulac-0.0.7/deepthulac/legacy/manage/SoExtention.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/manage/TimeWord.py` & `deepthulac-0.0.7/deepthulac/legacy/manage/TimeWord.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/legacy/manage/verbword.py` & `deepthulac-0.0.7/deepthulac/legacy/manage/verbword.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/model_old.py` & `deepthulac-0.0.7/deepthulac/model_old.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/seg/cut_sent.py` & `deepthulac-0.0.7/deepthulac/seg/cut_sent.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/seg/data_format.py` & `deepthulac-0.0.7/deepthulac/seg/data_format.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/seg/eval.py` & `deepthulac-0.0.7/deepthulac/seg/eval.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/seg/model.py` & `deepthulac-0.0.7/deepthulac/seg/model.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/seg/post_process.py` & `deepthulac-0.0.7/deepthulac/seg/post_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     segs[i] = cand
                     del segs[i+1:i+j+2]
                     break
             i += 1
         return segs
 
     def adjust_seg(self, pred_segs, num_workers=12):
-        res = [_adjust_seg(pred_seg) for pred_seg in pred_segs]
+        res = [self._adjust_seg(pred_seg) for pred_seg in pred_segs]
         return res
         from multiprocessing import Pool
         with Pool(num_workers) as p:
             res = p.map(self._adjust_seg, pred_segs)
         return res
```

### Comparing `deepthulac-0.0.6/deepthulac/seg/seg_utils.py` & `deepthulac-0.0.7/deepthulac/seg/seg_utils.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/seg/train.py` & `deepthulac-0.0.7/deepthulac/seg/train.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac/utils.py` & `deepthulac-0.0.7/deepthulac/utils.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/deepthulac.egg-info/SOURCES.txt` & `deepthulac-0.0.7/deepthulac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.6/setup.py` & `deepthulac-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         print("requirements:", ret)
     return ret
 
 
 setup(
     name='deepthulac',
     # packages = ['deepthulac'], # this must be the same as the name above
-    version='0.0.6',
+    version='0.0.7',
     description='A High-Performance Lexical Analyzer for Chinese',
     author='THUNLP',
     url='https://github.com/thunlp/DeepTHULAC',
     author_email='chengzl22@mails.tsinghua.edu.cn',
     download_url='https://github.com/thunlp/DeepTHULAC/archive/master.zip',
     classifiers=[
         "Programming Language :: Python :: 3",
```

