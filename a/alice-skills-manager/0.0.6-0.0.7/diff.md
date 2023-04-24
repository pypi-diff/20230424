# Comparing `tmp/alice-skills-manager-0.0.6.tar.gz` & `tmp/alice-skills-manager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alice-skills-manager-0.0.6.tar", last modified: Mon Apr 24 05:01:10 2023, max compression
+gzip compressed data, was "alice-skills-manager-0.0.7.tar", last modified: Mon Apr 24 20:54:05 2023, max compression
```

## Comparing `alice-skills-manager-0.0.6.tar` & `alice-skills-manager-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 05:01:10.984717 alice-skills-manager-0.0.6/
--rw-rw-rw-   0        0        0       61 2023-04-22 22:22:23.000000 alice-skills-manager-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      617 2023-04-24 05:01:10.984717 alice-skills-manager-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice-skills-manager-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 05:01:10.975420 alice-skills-manager-0.0.6/alice_skills_manager.egg-info/
--rw-rw-rw-   0        0        0      617 2023-04-24 05:01:10.000000 alice-skills-manager-0.0.6/alice_skills_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-04-24 05:01:10.000000 alice-skills-manager-0.0.6/alice_skills_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 05:01:10.000000 alice-skills-manager-0.0.6/alice_skills_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 05:01:10.000000 alice-skills-manager-0.0.6/alice_skills_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-04-24 05:01:10.000000 alice-skills-manager-0.0.6/alice_skills_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-24 05:01:10.000000 alice-skills-manager-0.0.6/alice_skills_manager.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 05:01:10.982716 alice-skills-manager-0.0.6/asm/
--rw-rw-rw-   0        0        0      156 2023-04-22 21:56:13.000000 alice-skills-manager-0.0.6/asm/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-04-22 21:57:43.000000 alice-skills-manager-0.0.6/asm/__main__.py
--rw-rw-rw-   0        0        0    20216 2023-04-22 21:57:47.000000 alice-skills-manager-0.0.6/asm/alice_skills_manager.py
--rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice-skills-manager-0.0.6/asm/exceptions.py
--rw-rw-rw-   0        0        0    19210 2023-04-22 21:56:47.000000 alice-skills-manager-0.0.6/asm/skill_entry.py
--rw-rw-rw-   0        0        0     6598 2023-04-22 21:56:27.000000 alice-skills-manager-0.0.6/asm/skill_repo.py
--rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice-skills-manager-0.0.6/asm/skill_state.py
--rw-rw-rw-   0        0        0     2993 2023-04-22 21:56:45.000000 alice-skills-manager-0.0.6/asm/util.py
--rw-rw-rw-   0        0        0       42 2023-04-24 05:01:10.984717 alice-skills-manager-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1948 2023-04-24 05:01:07.000000 alice-skills-manager-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.152964 alice-skills-manager-0.0.7/
+-rw-rw-rw-   0        0        0       61 2023-04-22 22:22:23.000000 alice-skills-manager-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      572 2023-04-24 20:54:05.152455 alice-skills-manager-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2023-04-21 23:05:03.000000 alice-skills-manager-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.138179 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/
+-rw-rw-rw-   0        0        0      572 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-24 20:54:04.000000 alice-skills-manager-0.0.7/alice_skills_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.146313 alice-skills-manager-0.0.7/asm/
+-rw-rw-rw-   0        0        0      156 2023-04-22 21:56:13.000000 alice-skills-manager-0.0.7/asm/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-04-22 21:57:43.000000 alice-skills-manager-0.0.7/asm/__main__.py
+-rw-rw-rw-   0        0        0    20216 2023-04-22 21:57:47.000000 alice-skills-manager-0.0.7/asm/alice_skills_manager.py
+-rw-rw-rw-   0        0        0     2202 2023-04-21 22:58:17.000000 alice-skills-manager-0.0.7/asm/exceptions.py
+-rw-rw-rw-   0        0        0    19210 2023-04-22 21:56:47.000000 alice-skills-manager-0.0.7/asm/skill_entry.py
+-rw-rw-rw-   0        0        0     6598 2023-04-22 21:56:27.000000 alice-skills-manager-0.0.7/asm/skill_repo.py
+-rw-rw-rw-   0        0        0     2623 2023-04-21 23:04:58.000000 alice-skills-manager-0.0.7/asm/skill_state.py
+-rw-rw-rw-   0        0        0     2993 2023-04-22 21:56:45.000000 alice-skills-manager-0.0.7/asm/util.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 20:54:05.153474 alice-skills-manager-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1840 2023-04-24 05:16:49.000000 alice-skills-manager-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:54:05.151438 alice-skills-manager-0.0.7/tests/
+-rw-rw-rw-   0        0        0    16155 2023-04-22 21:57:22.000000 alice-skills-manager-0.0.7/tests/test_alice_skills_manager.py
+-rw-rw-rw-   0        0        0     1453 2023-04-22 21:57:14.000000 alice-skills-manager-0.0.7/tests/test_main.py
+-rw-rw-rw-   0        0        0     2727 2023-04-22 21:56:58.000000 alice-skills-manager-0.0.7/tests/test_skill_entry.py
+-rw-rw-rw-   0        0        0     1957 2023-04-22 21:56:53.000000 alice-skills-manager-0.0.7/tests/test_skill_repo.py
```

### Comparing `alice-skills-manager-0.0.6/README.md` & `alice-skills-manager-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/asm/__main__.py` & `alice-skills-manager-0.0.7/asm/__main__.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/asm/alice_skills_manager.py` & `alice-skills-manager-0.0.7/asm/alice_skills_manager.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/asm/exceptions.py` & `alice-skills-manager-0.0.7/asm/exceptions.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/asm/skill_entry.py` & `alice-skills-manager-0.0.7/asm/skill_entry.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/asm/skill_repo.py` & `alice-skills-manager-0.0.7/asm/skill_repo.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/asm/skill_state.py` & `alice-skills-manager-0.0.7/asm/skill_state.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/asm/util.py` & `alice-skills-manager-0.0.7/asm/util.py`

 * *Files identical despite different names*

### Comparing `alice-skills-manager-0.0.6/setup.py` & `alice-skills-manager-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from setuptools import setup
+from setuptools import setup, find_packages
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
@@ -16,33 +16,29 @@
 #         requirements = f.read().splitlines()
 #         if 'ALICE_LOOSE_REQUIREMENTS' in os.environ:
 #             print('USING LOOSE REQUIREMENTS!')
 #             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
 #         return [pkg for pkg in requirements
 #                 if pkg.strip() and not pkg.startswith("#")]
 
-install_requires=[line.strip() for line in open('requirements/requirements.txt')]
-
-
 setup(
     name='alice-skills-manager',
-    version='0.0.6',
-    packages=['asm'],
+    version='0.0.7',
+    packages=find_packages(),
     install_requires=[line.strip() for line in open('requirements/requirements.txt')],
     package_data={'': package_files('asm')},
     # tests_require=required('requirements/tests.txt'),
     python_requires='>=3.6',
     url='https://github.com/Alice-IA/alice-skills-manager',
     license='Apache-2.0',
     author='Alice-IA',
     author_email='yuiassistant@gmail.com',
     description='Alice Skills Manager',
     classifiers=[
         'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     entry_points={
```

