# Comparing `tmp/deepthulac-0.0.5.tar.gz` & `tmp/deepthulac-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepthulac-0.0.5.tar", last modified: Thu Mar 16 08:42:09 2023, max compression
+gzip compressed data, was "deepthulac-0.0.6.tar", last modified: Mon Apr 24 06:43:44 2023, max compression
```

## Comparing `deepthulac-0.0.5.tar` & `deepthulac-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:09.706250 deepthulac-0.0.5/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1063 2022-11-01 11:55:55.000000 deepthulac-0.0.5/LICENSE
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-03-16 08:42:09.642250 deepthulac-0.0.5/PKG-INFO
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1856 2023-03-16 08:01:08.000000 deepthulac-0.0.5/README.md
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:07.430269 deepthulac-0.0.5/deepthulac/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       34 2023-03-16 08:38:22.000000 deepthulac-0.0.5/deepthulac/__init__.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:07.966264 deepthulac-0.0.5/deepthulac/eval/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:36:21.000000 deepthulac-0.0.5/deepthulac/eval/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3721 2023-03-16 07:33:33.000000 deepthulac-0.0.5/deepthulac/eval/cases.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    13748 2023-03-15 18:30:08.000000 deepthulac-0.0.5/deepthulac/eval/test.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     4199 2023-02-17 12:27:02.000000 deepthulac-0.0.5/deepthulac/eval/third_party_api.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:08.102263 deepthulac-0.0.5/deepthulac/legacy/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11114 2023-02-08 11:48:00.000000 deepthulac-0.0.5/deepthulac/legacy/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      190 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/__main__.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:08.434260 deepthulac-0.0.5/deepthulac/legacy/base/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2117 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/base/AlphaBeta.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7965 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/base/Dat.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       67 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/base/Node.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      137 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/base/WordWithTag.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/base/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1053 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/base/compatibility.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:08.702258 deepthulac-0.0.5/deepthulac/legacy/character/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2094 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/character/CBModel.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3995 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/character/CBNGramFeature.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7603 2023-03-01 15:26:39.000000 deepthulac-0.0.5/deepthulac/legacy/character/CBTaggingDecoder.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/character/__init__.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:09.106255 deepthulac-0.0.5/deepthulac/legacy/manage/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2792 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/Filter.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2550 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/Postprocesser.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     9839 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/Preprocesser.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1600 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/Punctuation.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1220 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/SoExtention.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5475 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/TimeWord.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      557 2023-01-16 16:22:28.000000 deepthulac-0.0.5/deepthulac/legacy/manage/verbword.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:09.574251 deepthulac-0.0.5/deepthulac/seg/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:29.000000 deepthulac-0.0.5/deepthulac/seg/__init__.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5188 2023-03-16 08:06:21.000000 deepthulac-0.0.5/deepthulac/seg/cut_sent.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    22309 2023-03-14 18:19:18.000000 deepthulac-0.0.5/deepthulac/seg/data_format.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11200 2023-02-17 17:07:25.000000 deepthulac-0.0.5/deepthulac/seg/eval.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    36406 2023-03-16 07:52:14.000000 deepthulac-0.0.5/deepthulac/seg/model.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3061 2023-02-17 16:50:59.000000 deepthulac-0.0.5/deepthulac/seg/post_process.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5843 2023-02-26 20:17:26.000000 deepthulac-0.0.5/deepthulac/seg/seg_utils.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5204 2023-03-16 07:30:09.000000 deepthulac-0.0.5/deepthulac/seg/train.py
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     8372 2023-03-13 16:45:01.000000 deepthulac-0.0.5/deepthulac/utils.py
-drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:42:07.766266 deepthulac-0.0.5/deepthulac.egg-info/
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-03-16 08:42:06.000000 deepthulac-0.0.5/deepthulac.egg-info/PKG-INFO
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1316 2023-03-16 08:42:07.000000 deepthulac-0.0.5/deepthulac.egg-info/SOURCES.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        1 2023-03-16 08:42:06.000000 deepthulac-0.0.5/deepthulac.egg-info/dependency_links.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       79 2023-03-16 08:42:06.000000 deepthulac-0.0.5/deepthulac.egg-info/requires.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       11 2023-03-16 08:42:06.000000 deepthulac-0.0.5/deepthulac.egg-info/top_level.txt
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       38 2023-03-16 08:42:09.706250 deepthulac-0.0.5/setup.cfg
--rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1521 2023-03-16 08:41:57.000000 deepthulac-0.0.5/setup.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.538138 deepthulac-0.0.6/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1063 2022-11-01 11:55:55.000000 deepthulac-0.0.6/LICENSE
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-04-24 06:43:44.534138 deepthulac-0.0.6/PKG-INFO
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1856 2023-03-16 08:01:08.000000 deepthulac-0.0.6/README.md
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.346139 deepthulac-0.0.6/deepthulac/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       34 2023-01-23 14:34:36.000000 deepthulac-0.0.6/deepthulac/__init__.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.374139 deepthulac-0.0.6/deepthulac/eval/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-03-16 08:36:21.000000 deepthulac-0.0.6/deepthulac/eval/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3851 2023-04-11 20:06:26.000000 deepthulac-0.0.6/deepthulac/eval/cases.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    38907 2023-03-05 17:38:25.000000 deepthulac-0.0.6/deepthulac/eval/old_model.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    13991 2023-03-21 07:52:38.000000 deepthulac-0.0.6/deepthulac/eval/test.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     4199 2023-02-17 12:27:02.000000 deepthulac-0.0.6/deepthulac/eval/third_party_api.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.382139 deepthulac-0.0.6/deepthulac/legacy/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11114 2023-02-08 11:48:00.000000 deepthulac-0.0.6/deepthulac/legacy/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      190 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/__main__.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.398139 deepthulac-0.0.6/deepthulac/legacy/base/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2117 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/AlphaBeta.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7965 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/Dat.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       67 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/Node.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      137 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/WordWithTag.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1053 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/base/compatibility.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.406139 deepthulac-0.0.6/deepthulac/legacy/character/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2094 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/character/CBModel.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3995 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/character/CBNGramFeature.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     7605 2023-04-24 06:29:06.000000 deepthulac-0.0.6/deepthulac/legacy/character/CBTaggingDecoder.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/character/__init__.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.430139 deepthulac-0.0.6/deepthulac/legacy/manage/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2792 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Filter.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     2550 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Postprocesser.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     9839 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Preprocesser.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1600 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/Punctuation.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1220 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/SoExtention.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5475 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/TimeWord.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      557 2023-01-16 16:22:28.000000 deepthulac-0.0.6/deepthulac/legacy/manage/verbword.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    30810 2023-02-26 16:12:20.000000 deepthulac-0.0.6/deepthulac/model_old.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.534138 deepthulac-0.0.6/deepthulac/seg/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        0 2023-01-16 16:22:29.000000 deepthulac-0.0.6/deepthulac/seg/__init__.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5188 2023-03-16 08:06:21.000000 deepthulac-0.0.6/deepthulac/seg/cut_sent.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    23373 2023-04-11 21:05:24.000000 deepthulac-0.0.6/deepthulac/seg/data_format.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    11200 2023-02-17 17:07:25.000000 deepthulac-0.0.6/deepthulac/seg/eval.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)    38541 2023-04-11 21:52:24.000000 deepthulac-0.0.6/deepthulac/seg/model.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     3144 2023-04-24 06:39:11.000000 deepthulac-0.0.6/deepthulac/seg/post_process.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5898 2023-04-12 19:02:05.000000 deepthulac-0.0.6/deepthulac/seg/seg_utils.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     5258 2023-03-21 07:39:11.000000 deepthulac-0.0.6/deepthulac/seg/train.py
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     8818 2023-03-19 21:55:47.000000 deepthulac-0.0.6/deepthulac/utils.py
+drwxrwxr-x   0 chengzhili  (1009) chengzhili  (1009)        0 2023-04-24 06:43:44.362139 deepthulac-0.0.6/deepthulac.egg-info/
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)      474 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/PKG-INFO
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1369 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/SOURCES.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)        1 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/dependency_links.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       79 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/requires.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       11 2023-04-24 06:43:44.000000 deepthulac-0.0.6/deepthulac.egg-info/top_level.txt
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)       38 2023-04-24 06:43:44.538138 deepthulac-0.0.6/setup.cfg
+-rw-rw-r--   0 chengzhili  (1009) chengzhili  (1009)     1521 2023-04-24 06:40:30.000000 deepthulac-0.0.6/setup.py
```

### Comparing `deepthulac-0.0.5/LICENSE` & `deepthulac-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/README.md` & `deepthulac-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/eval/cases.py` & `deepthulac-0.0.6/deepthulac/eval/cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,12 @@
 
 ancient_cases = [
     '必待一书毕然后方换一书，并不得兼读他书及省遍数。',
     '夫计谋欲密，攻敌欲疾，获若鹰击，战如河决，则兵未劳而敌自散，此用兵之势也。',
     '晋太元中，武陵人捕鱼为业，缘溪行，忘路之远近。忽逢桃花林，夹岸数百步，中无杂树，芳草鲜美，落英缤纷，渔人甚异之。复前行，欲穷其林。林尽水源，便得一山，山有小口，仿佛若有光，便舍船从口入。初极狭，才通人，复行数十步，豁然开朗。土地平旷，屋舍俨然，有良田美池桑竹之属。阡陌交通，鸡犬相闻。其中往来种作，男女衣著，悉如外人。黄发垂髫，并怡然自乐。'
     '见渔人，乃大惊，问所从来。具答之。便要还家，设酒杀鸡作食。村中闻有此人，咸来问讯。自云先世避秦时乱，率妻子邑人来此绝境，不复出焉，遂与外人间隔。问今是何世，乃不知有汉，无论魏晋。此人一一为具言所闻，皆叹惋。余人各复延至其家，皆出酒食。停数日，辞去。'
     '此中人语云，不足为外人道也。既出，得其船，便扶向路，处处志之。及郡下，诣太守说如此。太守即遣人随其往，寻向所志，遂迷不复得路。南阳刘子骥，高尚士也，闻之，欣然规往，未果。寻病终。后遂无问津者。'
+]
+
+pos_cases = [
+    '嘉平望日抵维扬晤裴岫云夫人不胜今昔之感余既匆匆南去夫人将之晋省赋此志别',
 ]
```

### Comparing `deepthulac-0.0.5/deepthulac/eval/test.py` & `deepthulac-0.0.6/deepthulac/eval/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,15 @@
 
         # seghard
         'seghard_hard_test_109.txt',
 
         # seg
         'seg_ours_test_2000.txt',
         'seg_oursseg_test_1614.txt',
+        'seg_zuozhuan-a_test_1594.txt',
         # 'seg_pku_test_1951.txt',
         'seg_msr_test_3985.txt',
         'seg_cityu_test_1492.txt',
         'seg_as_test_14432.txt',
         'seg_cbtsample_test_2000.txt',
         'seg_nlpccweibo_test_2052.txt',
 
@@ -261,15 +262,15 @@
         if fileformat in {'seghard', 'dict'} or (fileformat == 'seg' and gi):
             logging.info(f'{file}\tacc: {score[0]*100:.2f}\tacc/total: {score[1]}/{score[2]}')
         else:
             logging.info(f'{file}\tf1: {score[0]*100:.2f}\tp/r: {score[1]*100:.2f}/{score[2]*100:.2f}')
 
         scores[fileformat+'-gi' if gi else fileformat].append(f'{score[0]*100:.2f}')
 
-    table = PrettyTable(['pos', 'seghard', 'ours/oursseg/msr/cityu/as/cbt/nlpcc',  'dict', 'seg-gi'])
+    table = PrettyTable(['pos', 'seghard', 'ours/oursseg/zuozhuan/msr/cityu/as/cbt/nlpcc',  'dict', 'seg-gi'])
     table.add_row(['/'.join(scores['pos']), '/'.join(scores['seghard']), '/'.join(scores['seg']), '/'.join(scores['dict']), '/'.join(scores['seg-gi'])])
     logging.info(log_file+"\n"+str(table))
 
 # from deepthulac.eval.third_party_api import ltp_
 
 if __name__ == "__main__":
     from deepthulac.seg.model import LacModel
@@ -290,14 +291,17 @@
     path = '/data03/private/chengzhili/segmentation/output/_good_checkpoint/sup_pretrain'
     path = '/data03/private/chengzhili/segmentation/output/seg_punc_dict/2023-03-05_01-51-41/9011200'
     path = 'output/seg_punc_dict/2023-03-05_02-06-24/9011200'
     path = 'output/bound_seg_punc_dict/2023-03-05_03-00-20/6553600'
     path = 'output/bound_seg_punc_dict/2023-03-05_03-03-24/8601600'
     path = 'output/seg_punc_dict_pretrain/2023-03-06_04-32-47/2867200'
     path = '/data03/private/chengzhili/segmentation/output/_good_checkpoint/sup_pretrain'
+    path = 'output/seg/2023-03-21_12-29-16 char-cm lr1e-4 best'
+    path = 'output/seg/2023-03-21_12-47-40 bert-base lr2e-5 best'
+    path = 'output/seg/2023-03-21_12-53-56 char-cm lr5e-5 best'
     # path = 'output/seg_punc_dict_pretrain/2023-03-06_04-31-08/3276800'
 
     #from ltp import LTP
     #ltp = LTP('LTP/base2', cache_dir='.cache', local_files_only=True)
 #
 #
     #def ltp_(task, sentences):
@@ -313,15 +317,15 @@
     # 测试的模型路径
     parser = argparse.ArgumentParser()
     parser.add_argument('--model_path', default=path, type=str)
     args = parser.parse_args()
     saved_path = args.model_path
 
     print('loading...')
-    device = 'cuda:3'  # 'cuda:5'
+    device = 'cuda:2'  # 'cuda:5'
     log_file = saved_path+'/test.log'
 
     def deepthulac_api(task, sents):
         # TODO: split_long的影响非常巨大，要把split_long的逻辑改一下，让split之后尽量长
         result = model.seg(sents, batch_size=64, split_long=False, post_vmvd=False, vote_pattern=None)  # seg_pos头也一样从pos里拿结果即可
         # logging.info(result[task]['labels']) # TODO: 改成全在这里logging
         # return result[task]['res']
```

### Comparing `deepthulac-0.0.5/deepthulac/eval/third_party_api.py` & `deepthulac-0.0.6/deepthulac/eval/third_party_api.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/__init__.py` & `deepthulac-0.0.6/deepthulac/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/base/AlphaBeta.py` & `deepthulac-0.0.6/deepthulac/legacy/base/AlphaBeta.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/base/Dat.py` & `deepthulac-0.0.6/deepthulac/legacy/base/Dat.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/base/compatibility.py` & `deepthulac-0.0.6/deepthulac/legacy/base/compatibility.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/character/CBModel.py` & `deepthulac-0.0.6/deepthulac/legacy/character/CBModel.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/character/CBNGramFeature.py` & `deepthulac-0.0.6/deepthulac/legacy/character/CBNGramFeature.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/character/CBTaggingDecoder.py` & `deepthulac-0.0.6/deepthulac/legacy/character/CBTaggingDecoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
         for i in range(self.len):
             if(i not in self.result):
                 self.result[i] = 0
             if((i == self.len-1) or (self.labelInfo[self.result[i]][0] == '2') or (self.labelInfo[self.result[i]][0] == '3')):
                 ts.append((self.sequence[offset:i+1], self.separator, self.labelInfo[self.result[i]][1:-1]))
                 offset = i + 1
-        print(ts)
+        # print(ts)
         return 1, ts
 
     def get_seg_result(self):
         segged = []
         offset = 0
         for i in range(self.len):
             if((i == 0) or (self.labelInfo[self.result[i]][0] == '0') or (self.labelInfo[self.result[i]][0] == '3')):
```

### Comparing `deepthulac-0.0.5/deepthulac/legacy/manage/Filter.py` & `deepthulac-0.0.6/deepthulac/legacy/manage/Filter.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/manage/Postprocesser.py` & `deepthulac-0.0.6/deepthulac/legacy/manage/Postprocesser.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/manage/Preprocesser.py` & `deepthulac-0.0.6/deepthulac/legacy/manage/Preprocesser.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/manage/Punctuation.py` & `deepthulac-0.0.6/deepthulac/legacy/manage/Punctuation.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/manage/SoExtention.py` & `deepthulac-0.0.6/deepthulac/legacy/manage/SoExtention.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/manage/TimeWord.py` & `deepthulac-0.0.6/deepthulac/legacy/manage/TimeWord.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/legacy/manage/verbword.py` & `deepthulac-0.0.6/deepthulac/legacy/manage/verbword.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/seg/cut_sent.py` & `deepthulac-0.0.6/deepthulac/seg/cut_sent.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/seg/data_format.py` & `deepthulac-0.0.6/deepthulac/seg/data_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import functools
 from torch.utils.data import DataLoader, IterableDataset
 import re
 from typing import List, Callable, Optional
 from typeguard import typechecked
 from tqdm import tqdm
 from deepthulac.seg.cut_sent import split_sentence
-from deepthulac.utils import load_lines, parallel_run, store_lines, load_json, store_json, timer, log
+from deepthulac.utils import get_dinfo, load_lines, parallel_run, store_lines, load_json, store_json, timer, log
 from deepthulac.seg.seg_utils import *
 import os
 from distutils.version import StrictVersion
 import platform
 if StrictVersion(platform.python_version()) >= StrictVersion('3.8'):
     from typing import Literal
 else:
     from typing_extensions import Literal
 import random
 import logging
-
+from deepthulac.utils import timer
 
 class LacDataset(IterableDataset):
     @typechecked
     def __init__(self, corpus_name: str, path: str, line_processor: Callable, lines_num: int = 0, file_order_reverse=False):
         """流式处理的数据集初始化
 
         Args:
@@ -39,25 +39,42 @@
         if lines_num == 0 or lines_num > total:
             lines_num = total
         self.line_processor = line_processor
         self.lines_num = lines_num
         self.corpus_name = corpus_name
 
     def __iter__(self):
+        import time
         index = -1
+        
         for file in self.files:
             logging.info(f'{file} start')
             with open(file, 'r', encoding='utf-8') as f:
+                start_time = time.perf_counter()
                 for line in f:
                     index += 1
                     if index == self.lines_num:
                         return
+
+                    # print(index, end=' ')
+                    """
+                    if index%(32*8)==0:
+                        end_time = time.perf_counter()
+                        total_time = end_time - start_time
+                        start_time=end_time
+                        #print()
+                        print(get_dinfo().local_rank, total_time)"""
                     # print(self.line_processor(line.strip('\n')))
-                    train_sample = self.line_processor(line.strip('\n'))
+                    train_sample = self.line_processor(line.strip('\n')) # 这个处理很快, 主要是collate非常慢
+                    # print(train_sample)
                     if train_sample:
+                        # chars = np.array([ord(x) for x in train_sample[0]])
+                        # labels = np.array([ord(x) for x in train_sample[1]])
+                        # yield chars
+                        # yield (chars, )+(self.corpus_name, )
                         yield train_sample+(self.corpus_name, )
             logging.info(f'{file} end')
 
     def __len__(self):
         return self.lines_num
 
 
@@ -439,22 +456,31 @@
         format_raw('data_raw/seg_pku_test.txt')
         format_raw('data_raw/seg_msr_train.txt')
         format_raw('data_raw/seg_msr_test.txt')
 
     @timer
     def test_lacdataset():
         path = 'data/seg_ours_train_1611208.txt'
-        dataset = LacDataset(path, seg_line_processor, lines_num=0)
+        dataset = LacDataset('seg', path, seg_line_processor, lines_num=0)
         dataloader = DataLoader(dataset, batch_size=1, num_workers=1)
-        print(next(iter(dataloader.dataset)))
+        # print(next(iter(dataloader.dataset)))
         for batch in dataloader:
             pass
             # print(batch)
         print(len(dataloader))
 
+    
+    format_raw('data_raw/pos_guiyuan_train.txt')
+    exit(0)
+    format_raw('data_raw/seg_zuozhuan-a_test.txt')
+    format_raw('data_raw/seg_zuozhuan-b_test.txt')
+    exit(0)
+    test_lacdataset()
+    exit(0)
+
     # seg_remove_punc('data_raw/seg_zuozhuan_train.txt', 'zuozhuan')
     format_raw('data_raw/seg_zuozhuan-rm_train.txt')
     exit(0)
     format_raw('data_raw/seg_zuozhuan_train.txt')
     exit(0)
     # format_all()
     # format_all()
```

### Comparing `deepthulac-0.0.5/deepthulac/seg/eval.py` & `deepthulac-0.0.6/deepthulac/seg/eval.py`

 * *Files identical despite different names*

### Comparing `deepthulac-0.0.5/deepthulac/seg/model.py` & `deepthulac-0.0.6/deepthulac/seg/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from tqdm import tqdm
 import logging
 from munch import Munch
 from transformers import AutoTokenizer, AutoModel, BertTokenizer, BertConfig
 from torch.utils.data import DataLoader
 from deepthulac.seg.post_process import UserDict, adjust_pos
 from deepthulac.seg.seg_utils import *
-from deepthulac.seg.cut_sent import restore_batch, split_batch, split_batch_with_group_texts
+from deepthulac.seg.cut_sent import restore_batch, split_batch_with_group_texts
 from deepthulac.seg.data_format import make_pair
 from deepthulac.utils import DistributedInfo, load_yaml, store_yaml
 from deepthulac.eval.cases import *
 import torch.nn.functional as F
 
 import functools
 import random
@@ -213,15 +213,16 @@
 class LacModel(nn.Module):
     def __init__(self, config, dinfo, pretrained_path):
         # pretrained_path is pretrained model path or huggingface model or checkpoint
         bert = AutoModel.from_pretrained(pretrained_path)
         custom = os.path.exists(pretrained_path)
         if custom:
             self.pretrained_path = pretrained_path
-            tokenizer = BertTokenizer.from_pretrained(f'{self.pretrained_path}/vocab.txt')
+            # tokenizer = BertTokenizer.from_pretrained(f'{self.pretrained_path}/vocab.txt')
+            tokenizer = AutoTokenizer.from_pretrained(f'{self.pretrained_path}', trust_remote_code=True) # 这个我自己写了tokenizer
         else:
             tokenizer = AutoTokenizer.from_pretrained(config.pretrained_bert_model)
         super(LacModel, self).__init__()
 
         self.bert = bert
         self.tokenizer: AutoTokenizer = tokenizer
         if 'heads' not in config:
@@ -389,14 +390,15 @@
         device = self.dinfo.device
         for i in range(len(batch)):
             if isinstance(batch[i], torch.Tensor):
                 batch[i] = batch[i].to(device)
         return batch
 
     def collate_fn(self, task, batch):
+        # NOTE: 目前collate非常慢，影响到多卡训练了，瓶颈在一张卡collate上，要阻止只让一个卡collate
         # STEP1: tokens和labels都变成id
         sent_only = (task == 'any')  # none表示没有真实label标签, 数据集只有文本输入
         if sent_only:
             sents, corpus_names = [x[0] for x in batch], [x[1] for x in batch]
         else:
             sents, labels, corpus_names = [x[0] for x in batch], [x[1] for x in batch], [x[2] for x in batch]  # "李学勤", ['S', 'B', 'E'] -> [101, 3330, 2110, 1249]
             labels = [[parse_label2id(t, self.heads[task].label2id) for t in tag] for tag in labels]
@@ -496,30 +498,34 @@
         warmup_steps = warmup_steps if type(warmup_steps) == int else int(warmup_steps * steps_per_epoch)  # 2 * len(train_loader)
         logging.info(f'warmup_steps: {warmup_steps}')
         lr_scheduler = get_cosine_schedule_with_warmup(optimizer, num_warmup_steps=warmup_steps, num_training_steps=training_steps)
 
         accelerator = self.dinfo.accelerator
         is_main = self.dinfo.is_main
         if accelerator:
-            # model, optimizer, lr_scheduler = accelerator.prepare(model, optimizer, lr_scheduler)
-            model, optimizer = accelerator.prepare(model, optimizer)
+            model, optimizer, lr_scheduler = accelerator.prepare(model, optimizer, lr_scheduler)
+            # model, optimizer = accelerator.prepare(model, optimizer)
             for idx, loader in enumerate(train_loaders):
                 train_loaders[idx] = accelerator.prepare(loader)
                 train_loaders[idx].task = loader.task
 
         def save_checkpoint(path):
             if accelerator:
                 accelerator.unwrap_model(model).save(path)
             else:
                 model.save(path)
             logging.info("best model saved.")
 
         def evaluate_all():  # 以最后一个dev_loader的指标为准
             examples = self.seg(hard_cases+funny_cases+long_cases+ancient_cases, batch_size=1, split_long=False)['seg']['res']
             logging.info('\n'+'\n'.join(['/'.join(segs) for segs in examples]))
+            if 'pos' in self.heads:
+                examples = self.seg(pos_cases, batch_size=1, split_long=False)['pos']['res']
+                logging.info('\n'+'\n'.join(['/'.join(segs) for segs in examples]))
+                
             for dev_loader in dev_loaders:
                 score = evaluator(dev_loader, self, save_result=False, saved_path=model_dir)
             return score
 
         if is_main:
             best_f1 = evaluate_all()
 
@@ -556,41 +562,64 @@
                     input_ids, labels, sents = self.batch_to_device(batch_samples)
 
                 if teacher_model:
                     teacher_input_ids, _, _ = self.batch_to_device(next(train_loader_teacher))
                     assert torch.equal(teacher_input_ids.gt(0).sum(-1), input_ids.gt(0).sum(-1))  # 内容token的长度一样
                 else:
                     teacher_input_ids = None
-
-                loss = model(train_loaders[train_idx].task, input_ids, labels=labels, teacher_model=teacher_model, teacher_input_ids=teacher_input_ids)[0]
-                train_losses += loss.item()
-                model.zero_grad()
                 if accelerator:
-                    accelerator.backward(loss)
+                    if accelerator.sync_gradients:
+                        bar.update()
+                    with accelerator.accumulate(model):
+                        loss = model(train_loaders[train_idx].task, input_ids, labels=labels, teacher_model=teacher_model, teacher_input_ids=teacher_input_ids)[0]
+                        train_losses += loss.item()
+                        model.zero_grad()
+                        continue
+                        loss.backward() # BUG: 极其慢
+                    # accelerator.backward(loss)
+                    continue
+                    nn.utils.clip_grad_norm_(parameters=model.parameters(), max_norm=clip_grad)  # gradient clipping
+                    optimizer.step()  # 更新参数
+                    lr_scheduler.step()
+                    with accelerator.accumulate(model):
+                        loss = model(train_loaders[train_idx].task, input_ids, labels=labels, teacher_model=teacher_model, teacher_input_ids=teacher_input_ids)[0]
+                        train_losses += loss.item()
+                        model.zero_grad()
+                        continue
+                        accelerator.backward(loss) # BUG: 极其慢 # https://huggingface.co/docs/accelerate/concept_guides/gradient_synchronization
+                        continue
+                        nn.utils.clip_grad_norm_(parameters=model.parameters(), max_norm=clip_grad)  # gradient clipping
+                        optimizer.step()  # 更新参数
+                        lr_scheduler.step()
+                        # optimizer.zero_grad()
+                    continue
+                    accelerator.wait_for_everyone()
+                    continue
                 else:
+                    loss = model(train_loaders[train_idx].task, input_ids, labels=labels, teacher_model=teacher_model, teacher_input_ids=teacher_input_ids)[0]
+                    train_losses += loss.item()
+                    model.zero_grad()
                     loss.backward()
-                nn.utils.clip_grad_norm_(parameters=model.parameters(), max_norm=clip_grad)  # gradient clipping
-                optimizer.step()  # 更新参数
-                lr_scheduler.step()
-                bar.update()
+                    nn.utils.clip_grad_norm_(parameters=model.parameters(), max_norm=clip_grad)  # gradient clipping
+                    optimizer.step()  # 更新参数
+                    lr_scheduler.step()
+                    bar.update()
 
-                if accelerator:
-                    accelerator.wait_for_everyone()
                 if i in eval_steps and is_main:
                     logging.info(f'lr: {round(lr_scheduler.get_last_lr()[0],7)*1e5:.2f}e-5')
                     save_checkpoint(str(model_dir)+'/'+str(i*batch_size))
                     evaluate_all()
 
             if is_main:
                 train_loss = float(train_losses) / steps_per_epoch
                 logging.info(f"epoch: {epoch}, train loss: {train_loss}")
                 f1 = evaluate_all()
                 if f1 - best_f1 > 1e-5:
                     best_f1 = f1
-                    save_checkpoint(model_dir)
+                save_checkpoint(model_dir)
         if is_main:
             logging.info("--Complete trainning--")
 
     def add_user_dict(self, file: str):
         self.post_process = UserDict(file)
 
     def save(self, path: str):
@@ -598,21 +627,21 @@
         logger.info(f"save model to {path}")
         store_yaml(self.model_config, os.path.join(path, "config.yaml"))
         self.bert.config.save_pretrained(path)
         self.tokenizer.save_vocabulary(path)
         torch.save(self.state_dict(), os.path.join(path, 'pytorch_model.bin'))
 
     @classmethod
-    def load(cls, path: str = '', device: Union[str, torch.device] = 'cpu', use_f16=False, cache_dir=None):
+    def load(cls, path: str = '', device: Union[str, torch.device, DistributedInfo] = 'cpu', use_f16=False, cache_dir=None):
         from transformers import logging
         from huggingface_hub import snapshot_download
         logging.set_verbosity_error()
         if not path:
             path = snapshot_download(repo_id="chengzl18/deepthulac-seg", cache_dir=cache_dir)
-        dinfo = DistributedInfo(device=device)
+        dinfo = device if isinstance(device, DistributedInfo) else DistributedInfo(device=device)
         config = load_yaml(os.path.join(path, "config.yaml"))
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             model = cls(config, dinfo, pretrained_path=path)
         # TODO: 这还需要load和todevice吗
         model.load_state_dict(torch.load(os.path.join(path, 'pytorch_model.bin'), map_location=dinfo.device))
         model.to(device=dinfo.device)
```

### Comparing `deepthulac-0.0.5/deepthulac/seg/post_process.py` & `deepthulac-0.0.6/deepthulac/seg/post_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
                     segs[i] = cand
                     del segs[i+1:i+j+2]
                     break
             i += 1
         return segs
 
     def adjust_seg(self, pred_segs, num_workers=12):
+        res = [_adjust_seg(pred_seg) for pred_seg in pred_segs]
+        return res
         from multiprocessing import Pool
         with Pool(num_workers) as p:
             res = p.map(self._adjust_seg, pred_segs)
         return res
 
 
 def _adjust_pos(poss):
```

### Comparing `deepthulac-0.0.5/deepthulac/seg/seg_utils.py` & `deepthulac-0.0.6/deepthulac/seg/seg_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,9 +161,10 @@
     if t == 'U':  # 未知标签，不进行loss计算。NOTE: U这个标签只会在训练时出现并使用，即config文件里不允许出现U标签，U表示该位置不计算loss，并不表示一种分类
         return -1
     elif t in label2id:  # 正常标签
         return label2id.get(t)
     else:  # NOTE 约定用/分隔表示partial label
         partial = [0] * len(label2id)
         for label in t.split('/'):
+            print('ERROR', label, label2id.get(label))
             partial[label2id.get(label)] = 1
         return partial_label2id(partial)
```

### Comparing `deepthulac-0.0.5/deepthulac/seg/train.py` & `deepthulac-0.0.6/deepthulac/seg/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,31 +29,34 @@
         print_green(saved_path)
         log_dir = saved_path + '/train.log'
         set_logger(log_dir)
         logging.info(' '.join(sys.argv[:]))
     else:
         saved_path = None
 
+    if dinfo.accelerator:
+        config.batch_size *= dinfo.world_size
+
     data_strategy = getattr(config, 'data_strategy', 'shuffle_batches')
     train_loaders = []
     batch_order, loop_times, repeat_times = [], 0, []
     for i, dataset in enumerate(config.train_datasets):
         dataset_config = config.train_datasets[dataset]
         dataset_config.name = dataset
         dataset_config.split = 'train'
         dataset_config.samples_num = 1600 if config.part_data else 0
         train_loader = build_dataloader(dataset_config, config.heads, batch_size=config.batch_size)
         train_loaders.append(train_loader)
-        if data_strategy=='continuous_batches':
+        if data_strategy == 'continuous_batches':
             continuous_batches = dataset_config.continuous_batches
             batch_order.extend([i]*continuous_batches)
             loop_times = max(loop_times, math.ceil(len(train_loader)/continuous_batches))
-        elif data_strategy=='shuffle_batches':
+        elif data_strategy == 'shuffle_batches':
             batch_order.extend([i]*len(train_loader)*dataset_config.repeat_times)
-        elif data_strategy=='shuffle_samples':
+        elif data_strategy == 'shuffle_samples':
             repeat_times.append(dataset_config.repeat_times)
     if data_strategy == 'continuous_batches':
         batch_order = batch_order * loop_times
     elif data_strategy == 'shuffle_batches':
         random.shuffle(batch_order)
     elif data_strategy == 'shuffle_samples':
         train_loaders = [build_mixed_dataloader(train_loaders, repeat_times)]
@@ -65,29 +68,29 @@
         dataset_config.name = dataset
         dataset_config.split = 'test'
         dataset_config.samples_num = 60 if config.part_data else 120  # 这个会影响训练过程中的eval和最终eval结果不一样的问题
         dev_loader = build_dataloader(dataset_config, config.heads, batch_size=config.batch_size)
         dev_loaders.append(dev_loader)
 
     log('loading model')
-    
+
     if hasattr(config, 'load_seg_pretrain'):
-        load_path = config.load_seg_pretrain # +'/'+config.saved_path.split('/')[-1]
+        load_path = config.load_seg_pretrain
         if not os.path.exists(load_path):
             seg_pretrain = LacModel.load(config.load_seg_pretrain)
             model = LacModel(config, DistributedInfo(device='cpu'), config.pretrained_bert_model)
             model.bert = seg_pretrain.bert
             model.seg_head = seg_pretrain.seg_head
             model.heads['seg'] = model.seg_head
             model.save(load_path)
         model = LacModel.load(load_path, dinfo.device)
         model.model_config = config
+        model.dinfo = dinfo
     else:
         model = LacModel(config, dinfo, config.pretrained_bert_model)
-        
 
     # model = LacModel.load(path, 'cuda:0', use_f16=False) # 加载训练好的模型
     evaluator = functools.partial(SegEvaluator.eval_model, split_long=False)
     log('training')
 
     model.fit(config, train_loaders, dev_loaders, saved_path, evaluator, batch_order)
```

### Comparing `deepthulac-0.0.5/deepthulac/utils.py` & `deepthulac-0.0.6/deepthulac/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,18 @@
     device: Union[str, torch.device] = 'cuda'
 
 
 def init_distributed():
     global dinfo
     if "LOCAL_RANK" in os.environ:
         # split the batches of the original data loader across devices, batch_size= gpu_num * per_gpu_batch_size
-        accelerator = Accelerator(split_batches=True, kwargs_handlers=[DistributedDataParallelKwargs(find_unused_parameters=True)])
+        # 如果没有用find_unused_parameters=True，那么如果有模块没用上，就会报错，https://github.com/pytorch/pytorch/issues/43259
+        # 如果split_batches=True分发数据用了太多的时间，split batches总是会让主进程分合数据
+        # 默认Iterable dispatch_batches=True，我们改成了false，因为split_batches=True, 我们就不要让主进程再去dispatch_batches了。
+        accelerator = Accelerator(split_batches=True, dispatch_batches=False, kwargs_handlers=[DistributedDataParallelKwargs(find_unused_parameters=True)])
         dinfo = DistributedInfo(accelerator, accelerator.num_processes, accelerator.process_index, accelerator.is_local_main_process, accelerator.device)
         dinfo.world_size = accelerator.num_processes
         dinfo.local_rank = accelerator.process_index
 
     else:
         dinfo = DistributedInfo()
     return dinfo
```

### Comparing `deepthulac-0.0.5/deepthulac.egg-info/SOURCES.txt` & `deepthulac-0.0.6/deepthulac.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.md
 setup.py
 deepthulac/__init__.py
+deepthulac/model_old.py
 deepthulac/utils.py
 deepthulac.egg-info/PKG-INFO
 deepthulac.egg-info/SOURCES.txt
 deepthulac.egg-info/dependency_links.txt
 deepthulac.egg-info/requires.txt
 deepthulac.egg-info/top_level.txt
 deepthulac/eval/__init__.py
 deepthulac/eval/cases.py
+deepthulac/eval/old_model.py
 deepthulac/eval/test.py
 deepthulac/eval/third_party_api.py
 deepthulac/legacy/__init__.py
 deepthulac/legacy/__main__.py
 deepthulac/legacy/base/AlphaBeta.py
 deepthulac/legacy/base/Dat.py
 deepthulac/legacy/base/Node.py
```

### Comparing `deepthulac-0.0.5/setup.py` & `deepthulac-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         print("requirements:", ret)
     return ret
 
 
 setup(
     name='deepthulac',
     # packages = ['deepthulac'], # this must be the same as the name above
-    version='0.0.5',
+    version='0.0.6',
     description='A High-Performance Lexical Analyzer for Chinese',
     author='THUNLP',
     url='https://github.com/thunlp/DeepTHULAC',
     author_email='chengzl22@mails.tsinghua.edu.cn',
     download_url='https://github.com/thunlp/DeepTHULAC/archive/master.zip',
     classifiers=[
         "Programming Language :: Python :: 3",
```

