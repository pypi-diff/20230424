# Comparing `tmp/git_notion_pretty-1.0.2.tar.gz` & `tmp/git_notion_pretty-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_notion_pretty-1.0.2.tar", last modified: Mon Apr 24 15:17:20 2023, max compression
+gzip compressed data, was "git_notion_pretty-1.0.3.tar", last modified: Mon Apr 24 15:47:22 2023, max compression
```

## Comparing `git_notion_pretty-1.0.2.tar` & `git_notion_pretty-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:17:20.776964 git_notion_pretty-1.0.2/
--rw-r--r--   0 liz        (501) staff       (20)     1065 2023-04-23 16:02:09.000000 git_notion_pretty-1.0.2/LICENSE
--rw-r--r--   0 liz        (501) staff       (20)     3342 2023-04-24 15:17:20.777024 git_notion_pretty-1.0.2/PKG-INFO
--rw-r--r--   0 liz        (501) staff       (20)     2597 2023-04-24 15:13:30.000000 git_notion_pretty-1.0.2/README.md
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:17:20.775665 git_notion_pretty-1.0.2/git_notion_pretty/
--rw-r--r--   0 liz        (501) staff       (20)      133 2023-04-24 15:17:05.000000 git_notion_pretty-1.0.2/git_notion_pretty/__init__.py
--rw-r--r--   0 liz        (501) staff       (20)      901 2023-04-24 15:16:08.000000 git_notion_pretty-1.0.2/git_notion_pretty/cli.py
--rw-r--r--   0 liz        (501) staff       (20)     5397 2023-04-24 14:55:17.000000 git_notion_pretty-1.0.2/git_notion_pretty/git_notion.py
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:17:20.776562 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/
--rw-r--r--   0 liz        (501) staff       (20)     3342 2023-04-24 15:17:20.000000 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/PKG-INFO
--rw-r--r--   0 liz        (501) staff       (20)      436 2023-04-24 15:17:20.000000 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/SOURCES.txt
--rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 15:17:20.000000 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/dependency_links.txt
--rw-r--r--   0 liz        (501) staff       (20)       65 2023-04-24 15:17:20.000000 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/entry_points.txt
--rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/not-zip-safe
--rw-r--r--   0 liz        (501) staff       (20)       38 2023-04-24 15:17:20.000000 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/requires.txt
--rw-r--r--   0 liz        (501) staff       (20)       18 2023-04-24 15:17:20.000000 git_notion_pretty-1.0.2/git_notion_pretty.egg-info/top_level.txt
--rw-r--r--   0 liz        (501) staff       (20)      568 2023-04-24 15:17:20.777302 git_notion_pretty-1.0.2/setup.cfg
--rw-r--r--   0 liz        (501) staff       (20)     1648 2023-04-24 15:17:05.000000 git_notion_pretty-1.0.2/setup.py
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:17:20.776692 git_notion_pretty-1.0.2/tests/
--rw-r--r--   0 liz        (501) staff       (20)      664 2023-04-24 14:53:53.000000 git_notion_pretty-1.0.2/tests/test_git_notion.py
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:47:22.936951 git_notion_pretty-1.0.3/
+-rw-r--r--   0 liz        (501) staff       (20)     1065 2023-04-23 16:02:09.000000 git_notion_pretty-1.0.3/LICENSE
+-rw-r--r--   0 liz        (501) staff       (20)     3342 2023-04-24 15:47:22.937019 git_notion_pretty-1.0.3/PKG-INFO
+-rw-r--r--   0 liz        (501) staff       (20)     2597 2023-04-24 15:13:30.000000 git_notion_pretty-1.0.3/README.md
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:47:22.935772 git_notion_pretty-1.0.3/git_notion_pretty/
+-rw-r--r--   0 liz        (501) staff       (20)      133 2023-04-24 15:47:08.000000 git_notion_pretty-1.0.3/git_notion_pretty/__init__.py
+-rw-r--r--   0 liz        (501) staff       (20)      901 2023-04-24 15:16:08.000000 git_notion_pretty-1.0.3/git_notion_pretty/cli.py
+-rw-r--r--   0 liz        (501) staff       (20)     5397 2023-04-24 14:55:17.000000 git_notion_pretty-1.0.3/git_notion_pretty/git_notion.py
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:47:22.936665 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/
+-rw-r--r--   0 liz        (501) staff       (20)     3342 2023-04-24 15:47:22.000000 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/PKG-INFO
+-rw-r--r--   0 liz        (501) staff       (20)      436 2023-04-24 15:47:22.000000 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/SOURCES.txt
+-rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 15:47:22.000000 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/dependency_links.txt
+-rw-r--r--   0 liz        (501) staff       (20)       65 2023-04-24 15:47:22.000000 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/entry_points.txt
+-rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/not-zip-safe
+-rw-r--r--   0 liz        (501) staff       (20)       28 2023-04-24 15:47:22.000000 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/requires.txt
+-rw-r--r--   0 liz        (501) staff       (20)       18 2023-04-24 15:47:22.000000 git_notion_pretty-1.0.3/git_notion_pretty.egg-info/top_level.txt
+-rw-r--r--   0 liz        (501) staff       (20)      568 2023-04-24 15:47:22.937296 git_notion_pretty-1.0.3/setup.cfg
+-rw-r--r--   0 liz        (501) staff       (20)     1648 2023-04-24 15:47:08.000000 git_notion_pretty-1.0.3/setup.py
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:47:22.936807 git_notion_pretty-1.0.3/tests/
+-rw-r--r--   0 liz        (501) staff       (20)      664 2023-04-24 14:53:53.000000 git_notion_pretty-1.0.3/tests/test_git_notion.py
```

### Comparing `git_notion_pretty-1.0.2/LICENSE` & `git_notion_pretty-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `git_notion_pretty-1.0.2/PKG-INFO` & `git_notion_pretty-1.0.3/git_notion_pretty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: git_notion_pretty
-Version: 1.0.2
+Name: git-notion-pretty
+Version: 1.0.3
 Summary: Syncs GitHub Markdown files to Notion
 Home-page: https://github.com/Harbor-Systems/git-notion
 Author: NarekA
 License: MIT license
 Keywords: git_notion_pretty
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `git_notion_pretty-1.0.2/README.md` & `git_notion_pretty-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `git_notion_pretty-1.0.2/git_notion_pretty/cli.py` & `git_notion_pretty-1.0.3/git_notion_pretty/cli.py`

 * *Files identical despite different names*

### Comparing `git_notion_pretty-1.0.2/git_notion_pretty/git_notion.py` & `git_notion_pretty-1.0.3/git_notion_pretty/git_notion.py`

 * *Files identical despite different names*

### Comparing `git_notion_pretty-1.0.2/git_notion_pretty.egg-info/PKG-INFO` & `git_notion_pretty-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: git-notion-pretty
-Version: 1.0.2
+Name: git_notion_pretty
+Version: 1.0.3
 Summary: Syncs GitHub Markdown files to Notion
 Home-page: https://github.com/Harbor-Systems/git-notion
 Author: NarekA
 License: MIT license
 Keywords: git_notion_pretty
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `git_notion_pretty-1.0.2/setup.cfg` & `git_notion_pretty-1.0.3/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.2
+current_version = 1.0.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `git_notion_pretty-1.0.2/setup.py` & `git_notion_pretty-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     long_description_content_type='text/markdown',
     name='git_notion_pretty',
     packages=find_packages(include=['git_notion_pretty', 'git_notion_pretty.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Harbor-Systems/git-notion',
-    version='1.0.2',
+    version='1.0.3',
     zip_safe=False,
 )
```

### Comparing `git_notion_pretty-1.0.2/tests/test_git_notion.py` & `git_notion_pretty-1.0.3/tests/test_git_notion.py`

 * *Files identical despite different names*

