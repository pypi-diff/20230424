# Comparing `tmp/git_notion_pretty-1.0.0.tar.gz` & `tmp/git_notion_pretty-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_notion_pretty-1.0.0.tar", last modified: Mon Apr 24 14:59:14 2023, max compression
+gzip compressed data, was "git_notion_pretty-1.0.1.tar", last modified: Mon Apr 24 15:09:07 2023, max compression
```

## Comparing `git_notion_pretty-1.0.0.tar` & `git_notion_pretty-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 14:59:14.358118 git_notion_pretty-1.0.0/
--rw-r--r--   0 liz        (501) staff       (20)     1065 2023-04-23 16:02:09.000000 git_notion_pretty-1.0.0/LICENSE
--rw-r--r--   0 liz        (501) staff       (20)     3338 2023-04-24 14:59:14.358172 git_notion_pretty-1.0.0/PKG-INFO
--rw-r--r--   0 liz        (501) staff       (20)     2593 2023-04-24 14:53:02.000000 git_notion_pretty-1.0.0/README.md
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 14:59:14.357082 git_notion_pretty-1.0.0/git_notion_pretty/
--rw-r--r--   0 liz        (501) staff       (20)      126 2023-04-23 16:02:09.000000 git_notion_pretty-1.0.0/git_notion_pretty/__init__.py
--rw-r--r--   0 liz        (501) staff       (20)      880 2023-04-24 14:55:22.000000 git_notion_pretty-1.0.0/git_notion_pretty/cli.py
--rw-r--r--   0 liz        (501) staff       (20)     5397 2023-04-24 14:55:17.000000 git_notion_pretty-1.0.0/git_notion_pretty/git_notion.py
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 14:59:14.357881 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/
--rw-r--r--   0 liz        (501) staff       (20)     3338 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/PKG-INFO
--rw-r--r--   0 liz        (501) staff       (20)      436 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/SOURCES.txt
--rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/dependency_links.txt
--rw-r--r--   0 liz        (501) staff       (20)       65 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/entry_points.txt
--rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/not-zip-safe
--rw-r--r--   0 liz        (501) staff       (20)       38 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/requires.txt
--rw-r--r--   0 liz        (501) staff       (20)       18 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.0/git_notion_pretty.egg-info/top_level.txt
--rw-r--r--   0 liz        (501) staff       (20)      568 2023-04-24 14:59:14.358406 git_notion_pretty-1.0.0/setup.cfg
--rw-r--r--   0 liz        (501) staff       (20)     1648 2023-04-24 14:41:12.000000 git_notion_pretty-1.0.0/setup.py
-drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 14:59:14.358002 git_notion_pretty-1.0.0/tests/
--rw-r--r--   0 liz        (501) staff       (20)      664 2023-04-24 14:53:53.000000 git_notion_pretty-1.0.0/tests/test_git_notion.py
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:09:07.427386 git_notion_pretty-1.0.1/
+-rw-r--r--   0 liz        (501) staff       (20)     1065 2023-04-23 16:02:09.000000 git_notion_pretty-1.0.1/LICENSE
+-rw-r--r--   0 liz        (501) staff       (20)     3349 2023-04-24 15:09:07.427436 git_notion_pretty-1.0.1/PKG-INFO
+-rw-r--r--   0 liz        (501) staff       (20)     2604 2023-04-24 15:07:56.000000 git_notion_pretty-1.0.1/README.md
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:09:07.426074 git_notion_pretty-1.0.1/git_notion_pretty/
+-rw-r--r--   0 liz        (501) staff       (20)      133 2023-04-24 15:08:37.000000 git_notion_pretty-1.0.1/git_notion_pretty/__init__.py
+-rw-r--r--   0 liz        (501) staff       (20)      880 2023-04-24 14:55:22.000000 git_notion_pretty-1.0.1/git_notion_pretty/cli.py
+-rw-r--r--   0 liz        (501) staff       (20)     5397 2023-04-24 14:55:17.000000 git_notion_pretty-1.0.1/git_notion_pretty/git_notion.py
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:09:07.427062 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/
+-rw-r--r--   0 liz        (501) staff       (20)     3349 2023-04-24 15:09:07.000000 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/PKG-INFO
+-rw-r--r--   0 liz        (501) staff       (20)      436 2023-04-24 15:09:07.000000 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/SOURCES.txt
+-rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 15:09:07.000000 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/dependency_links.txt
+-rw-r--r--   0 liz        (501) staff       (20)       65 2023-04-24 15:09:07.000000 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/entry_points.txt
+-rw-r--r--   0 liz        (501) staff       (20)        1 2023-04-24 14:59:14.000000 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/not-zip-safe
+-rw-r--r--   0 liz        (501) staff       (20)       38 2023-04-24 15:09:07.000000 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/requires.txt
+-rw-r--r--   0 liz        (501) staff       (20)       18 2023-04-24 15:09:07.000000 git_notion_pretty-1.0.1/git_notion_pretty.egg-info/top_level.txt
+-rw-r--r--   0 liz        (501) staff       (20)      568 2023-04-24 15:09:07.427692 git_notion_pretty-1.0.1/setup.cfg
+-rw-r--r--   0 liz        (501) staff       (20)     1648 2023-04-24 15:08:37.000000 git_notion_pretty-1.0.1/setup.py
+drwxr-xr-x   0 liz        (501) staff       (20)        0 2023-04-24 15:09:07.427168 git_notion_pretty-1.0.1/tests/
+-rw-r--r--   0 liz        (501) staff       (20)      664 2023-04-24 14:53:53.000000 git_notion_pretty-1.0.1/tests/test_git_notion.py
```

### Comparing `git_notion_pretty-1.0.0/LICENSE` & `git_notion_pretty-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_notion_pretty-1.0.0/PKG-INFO` & `git_notion_pretty-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_notion_pretty
-Version: 1.0.0
+Version: 1.0.1
 Summary: Syncs GitHub Markdown files to Notion
 Home-page: https://github.com/Harbor-Systems/git-notion
 Author: NarekA
 License: MIT license
 Keywords: git_notion_pretty
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -106,12 +106,12 @@
 # To use the file name instead searching for and using the H1 header on the first line
 git-notion-pretty --use-file-name
 ```
 
 ## Pushing to PYPI
 
 ```bash
-bumpversion patch   # Look-up bumpversion
+python3 -m bumpversion patch   # Look-up bumpversion
 rm -rf dist/
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload dist/*
 ```
```

### Comparing `git_notion_pretty-1.0.0/README.md` & `git_notion_pretty-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,12 +85,12 @@
 # To use the file name instead searching for and using the H1 header on the first line
 git-notion-pretty --use-file-name
 ```
 
 ## Pushing to PYPI
 
 ```bash
-bumpversion patch   # Look-up bumpversion
+python3 -m bumpversion patch   # Look-up bumpversion
 rm -rf dist/
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload dist/*
 ```
```

### Comparing `git_notion_pretty-1.0.0/git_notion_pretty/cli.py` & `git_notion_pretty-1.0.1/git_notion_pretty/cli.py`

 * *Files identical despite different names*

### Comparing `git_notion_pretty-1.0.0/git_notion_pretty/git_notion.py` & `git_notion_pretty-1.0.1/git_notion_pretty/git_notion.py`

 * *Files identical despite different names*

### Comparing `git_notion_pretty-1.0.0/git_notion_pretty.egg-info/PKG-INFO` & `git_notion_pretty-1.0.1/git_notion_pretty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-notion-pretty
-Version: 1.0.0
+Version: 1.0.1
 Summary: Syncs GitHub Markdown files to Notion
 Home-page: https://github.com/Harbor-Systems/git-notion
 Author: NarekA
 License: MIT license
 Keywords: git_notion_pretty
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -106,12 +106,12 @@
 # To use the file name instead searching for and using the H1 header on the first line
 git-notion-pretty --use-file-name
 ```
 
 ## Pushing to PYPI
 
 ```bash
-bumpversion patch   # Look-up bumpversion
+python3 -m bumpversion patch   # Look-up bumpversion
 rm -rf dist/
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload dist/*
 ```
```

### Comparing `git_notion_pretty-1.0.0/setup.cfg` & `git_notion_pretty-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0
+current_version = 1.0.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `git_notion_pretty-1.0.0/setup.py` & `git_notion_pretty-1.0.1/setup.py`

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
-    version='1.0.0',
+    version='1.0.1',
     zip_safe=False,
 )
```

### Comparing `git_notion_pretty-1.0.0/tests/test_git_notion.py` & `git_notion_pretty-1.0.1/tests/test_git_notion.py`

 * *Files identical despite different names*

