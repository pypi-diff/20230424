# Comparing `tmp/zope.container-5.0.tar.gz` & `tmp/zope.container-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.container-5.0.tar", last modified: Tue Jan 24 13:31:53 2023, max compression
+gzip compressed data, was "zope.container-5.1.tar", last modified: Mon Apr 24 06:17:20 2023, max compression
```

## Comparing `zope.container-5.0.tar` & `zope.container-5.1.tar`

### file list

```diff
@@ -1,76 +1,88 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-01-24 13:31:53.984976 zope.container-5.0/
--rw-r--r--   0 mac        (513) staff       (20)      588 2023-01-24 13:31:46.000000 zope.container-5.0/.coveragerc
--rwxr-xr-x   0 mac        (513) staff       (20)     1919 2023-01-24 13:31:46.000000 zope.container-5.0/.manylinux-install.sh
--rwxr-xr-x   0 mac        (513) staff       (20)      509 2023-01-24 13:31:46.000000 zope.container-5.0/.manylinux.sh
--rw-r--r--   0 mac        (513) staff       (20)    10955 2023-01-24 13:31:46.000000 zope.container-5.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      799 2023-01-24 13:31:46.000000 zope.container-5.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-01-24 13:31:46.000000 zope.container-5.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-01-24 13:31:46.000000 zope.container-5.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      495 2023-01-24 13:31:46.000000 zope.container-5.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    13844 2023-01-24 13:31:53.985134 zope.container-5.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1428 2023-01-24 13:31:46.000000 zope.container-5.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)     1777 2023-01-24 13:31:46.000000 zope.container-5.0/appveyor.yml
--rw-r--r--   0 mac        (513) staff       (20)      192 2023-01-24 13:31:46.000000 zope.container-5.0/compat.cfg
--rw-r--r--   0 mac        (513) staff       (20)       87 2023-01-24 13:31:46.000000 zope.container-5.0/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-01-24 13:31:53.968642 zope.container-5.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     6790 2023-01-24 13:31:46.000000 zope.container-5.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      688 2023-01-24 13:31:46.000000 zope.container-5.0/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-01-24 13:31:46.000000 zope.container-5.0/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)     9909 2023-01-24 13:31:46.000000 zope.container-5.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)       51 2023-01-24 13:31:46.000000 zope.container-5.0/docs/constraints.rst
--rw-r--r--   0 mac        (513) staff       (20)      843 2023-01-24 13:31:46.000000 zope.container-5.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     6715 2023-01-24 13:31:46.000000 zope.container-5.0/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)       57 2023-01-24 13:31:46.000000 zope.container-5.0/docs/narrative.rst
--rw-r--r--   0 mac        (513) staff       (20)      541 2023-01-24 13:31:53.985815 zope.container-5.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     7627 2023-01-24 13:31:46.000000 zope.container-5.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-01-24 13:31:53.961135 zope.container-5.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-01-24 13:31:53.968939 zope.container-5.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-01-24 13:31:53.977899 zope.container-5.0/src/zope/container/
--rw-r--r--   0 mac        (513) staff       (20)       61 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1157 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/_compat.h
--rw-r--r--   0 mac        (513) staff       (20)     3799 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/_proxy.py
--rw-r--r--   0 mac        (513) staff       (20)     6302 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/_util.py
--rw-r--r--   0 mac        (513) staff       (20)     9769 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/_zope_container_contained.c
--rw-r--r--   0 mac        (513) staff       (20)     3364 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/btree.py
--rw-r--r--   0 mac        (513) staff       (20)     3431 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/configure.zcml
--rw-r--r--   0 mac        (513) staff       (20)    13964 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/constraints.py
--rw-r--r--   0 mac        (513) staff       (20)     3826 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/constraints.rst
--rw-r--r--   0 mac        (513) staff       (20)    30150 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/contained.py
--rw-r--r--   0 mac        (513) staff       (20)     3693 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/directory.py
--rw-r--r--   0 mac        (513) staff       (20)     2829 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/find.py
--rw-r--r--   0 mac        (513) staff       (20)     1620 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/folder.py
--rw-r--r--   0 mac        (513) staff       (20)      892 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/i18n.py
--rw-r--r--   0 mac        (513) staff       (20)     9918 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     7836 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/ordered.py
--rw-r--r--   0 mac        (513) staff       (20)     2898 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/sample.py
--rw-r--r--   0 mac        (513) staff       (20)     1430 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/size.py
--rw-r--r--   0 mac        (513) staff       (20)     3274 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-01-24 13:31:53.984714 zope.container-5.0/src/zope/container/tests/
--rw-r--r--   0 mac        (513) staff       (20)       61 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      665 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/constraints_example.py
--rw-r--r--   0 mac        (513) staff       (20)     1625 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/directory.rst
--rw-r--r--   0 mac        (513) staff       (20)     8128 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_btree.py
--rw-r--r--   0 mac        (513) staff       (20)     1567 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_compile_flags.py
--rw-r--r--   0 mac        (513) staff       (20)     2345 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_constraints.py
--rw-r--r--   0 mac        (513) staff       (20)     9309 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_contained.py
--rw-r--r--   0 mac        (513) staff       (20)     5648 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_contained_zodb.py
--rw-r--r--   0 mac        (513) staff       (20)     2325 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_containertraversable.py
--rw-r--r--   0 mac        (513) staff       (20)     4216 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_containertraverser.py
--rw-r--r--   0 mac        (513) staff       (20)     1559 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_dependencies.py
--rw-r--r--   0 mac        (513) staff       (20)     1862 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_directory.py
--rw-r--r--   0 mac        (513) staff       (20)     5810 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_find.py
--rw-r--r--   0 mac        (513) staff       (20)      777 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_folder.py
--rw-r--r--   0 mac        (513) staff       (20)    12638 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_icontainer.py
--rw-r--r--   0 mac        (513) staff       (20)     4179 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_ordered.py
--rw-r--r--   0 mac        (513) staff       (20)     2345 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/tests/test_size.py
--rw-r--r--   0 mac        (513) staff       (20)     4295 2023-01-24 13:31:46.000000 zope.container-5.0/src/zope/container/traversal.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-01-24 13:31:53.971124 zope.container-5.0/src/zope.container.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    13844 2023-01-24 13:31:53.000000 zope.container-5.0/src/zope.container.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2011 2023-01-24 13:31:53.000000 zope.container-5.0/src/zope.container.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-01-24 13:31:53.000000 zope.container-5.0/src/zope.container.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-01-24 13:31:53.000000 zope.container-5.0/src/zope.container.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-01-24 13:31:53.000000 zope.container-5.0/src/zope.container.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      593 2023-01-24 13:31:53.000000 zope.container-5.0/src/zope.container.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-01-24 13:31:53.000000 zope.container-5.0/src/zope.container.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1397 2023-01-24 13:31:46.000000 zope.container-5.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.596571 zope.container-5.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      588 2023-04-24 06:17:20.000000 zope.container-5.1/.coveragerc
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)     2183 2023-04-24 06:17:20.000000 zope.container-5.1/.manylinux-install.sh
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2023-04-24 06:17:20.000000 zope.container-5.1/.manylinux.sh
+-rw-r--r--   0 m.howitz   (502) staff       (20)      128 2023-04-24 06:17:20.000000 zope.container-5.1/.readthedocs.yaml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11103 2023-04-24 06:17:20.000000 zope.container-5.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      799 2023-04-24 06:17:20.000000 zope.container-5.1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-04-24 06:17:20.000000 zope.container-5.1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-04-24 06:17:20.000000 zope.container-5.1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      644 2023-04-24 06:17:20.000000 zope.container-5.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13992 2023-04-24 06:17:20.596651 zope.container-5.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1428 2023-04-24 06:17:20.000000 zope.container-5.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1943 2023-04-24 06:17:20.000000 zope.container-5.1/appveyor.yml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      192 2023-04-24 06:17:20.000000 zope.container-5.1/compat.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)        8 2023-04-24 06:17:20.000000 zope.container-5.1/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.588684 zope.container-5.1/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6790 2023-04-24 06:17:20.000000 zope.container-5.1/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      688 2023-04-24 06:17:20.000000 zope.container-5.1/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-04-24 06:17:20.000000 zope.container-5.1/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9909 2023-04-24 06:17:20.000000 zope.container-5.1/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       51 2023-04-24 06:17:20.000000 zope.container-5.1/docs/constraints.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      885 2023-04-24 06:17:20.000000 zope.container-5.1/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6715 2023-04-24 06:17:20.000000 zope.container-5.1/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)       57 2023-04-24 06:17:20.000000 zope.container-5.1/docs/narrative.rst
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.584748 zope.container-5.1/include/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.588957 zope.container-5.1/include/persistent/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1464 2023-04-24 06:17:20.000000 zope.container-5.1/include/persistent/_compat.h
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.589104 zope.container-5.1/include/persistent/persistent/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5105 2023-04-24 06:17:20.000000 zope.container-5.1/include/persistent/persistent/cPersistence.h
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2640 2023-04-24 06:17:20.000000 zope.container-5.1/include/persistent/ring.h
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.584815 zope.container-5.1/include/zope.proxy/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.584880 zope.container-5.1/include/zope.proxy/zope/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.589434 zope.container-5.1/include/zope.proxy/zope/proxy/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    27350 2023-04-24 06:17:20.000000 zope.container-5.1/include/zope.proxy/zope/proxy/_zope_proxy_proxy.c
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1457 2023-04-24 06:17:20.000000 zope.container-5.1/include/zope.proxy/zope/proxy/proxy.h
+-rw-r--r--   0 m.howitz   (502) staff       (20)      542 2023-04-24 06:17:20.596962 zope.container-5.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4402 2023-04-24 06:17:20.000000 zope.container-5.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.585125 zope.container-5.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.589564 zope.container-5.1/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.593771 zope.container-5.1/src/zope/container/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1157 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/_compat.h
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3799 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/_proxy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6302 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/_util.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9791 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/_zope_container_contained.c
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3364 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/btree.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3431 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13964 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/constraints.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3826 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/constraints.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)    30150 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/contained.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3693 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/directory.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2829 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/find.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1620 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/folder.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      892 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/i18n.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9918 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7836 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/ordered.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2898 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/sample.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1430 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/size.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3274 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.596439 zope.container-5.1/src/zope/container/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       61 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      665 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/constraints_example.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1625 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/directory.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8128 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_btree.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1567 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_compile_flags.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2345 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_constraints.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9309 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_contained.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5648 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_contained_zodb.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2325 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_containertraversable.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4216 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_containertraverser.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1559 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_dependencies.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1862 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_directory.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5810 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_find.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      777 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_folder.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12638 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_icontainer.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4179 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_ordered.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2345 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/tests/test_size.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4295 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope/container/traversal.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-24 06:17:20.590549 zope.container-5.1/src/zope.container.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13992 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope.container.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2217 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope.container.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope.container.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope.container.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope.container.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      593 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope.container.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-24 06:17:20.000000 zope.container-5.1/src/zope.container.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1439 2023-04-24 06:17:20.000000 zope.container-5.1/tox.ini
```

### Comparing `zope.container-5.0/.coveragerc` & `zope.container-5.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/.manylinux-install.sh` & `zope.container-5.1/.manylinux-install.sh`

 * *Files 9% similar despite different names*

```diff
@@ -24,33 +24,40 @@
 ls -ld /cache/pip
 
 # We need some libraries because we build wheels from scratch:
 yum -y install libffi-devel
 
 tox_env_map() {
     case $1 in
+        *"cp312"*) echo 'py312';;
         *"cp37"*) echo 'py37';;
         *"cp38"*) echo 'py38';;
         *"cp39"*) echo 'py39';;
         *"cp310"*) echo 'py310';;
         *"cp311"*) echo 'py311';;
         *) echo 'py';;
     esac
 }
 
 # Compile wheels
 for PYBIN in /opt/python/*/bin; do
     if \
+       [[ "${PYBIN}" == *"cp312"* ]] || \
        [[ "${PYBIN}" == *"cp311"* ]] || \
        [[ "${PYBIN}" == *"cp37"* ]] || \
        [[ "${PYBIN}" == *"cp38"* ]] || \
        [[ "${PYBIN}" == *"cp39"* ]] || \
        [[ "${PYBIN}" == *"cp310"* ]] ; then
-        "${PYBIN}/pip" install -e /io/
-        "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        if [[ "${PYBIN}" == *"cp312"* ]] ; then
+            "${PYBIN}/pip" install --pre -e /io/
+            "${PYBIN}/pip" wheel /io/ --pre -w wheelhouse/
+        else
+            "${PYBIN}/pip" install -e /io/
+            "${PYBIN}/pip" wheel /io/ -w wheelhouse/
+        fi
         if [ `uname -m` == 'aarch64' ]; then
           cd /io/
           ${PYBIN}/pip install tox
           TOXENV=$(tox_env_map "${PYBIN}")
           ${PYBIN}/tox -e ${TOXENV}
           cd ..
         fi
```

### Comparing `zope.container-5.0/CHANGES.rst` & `zope.container-5.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+5.1 (2023-04-24)
+================
+
+- Drop using ``setup_requires`` due to constant problems on GHA.
+
+- Add preliminary support for Python 3.12a7.
+
+
 5.0 (2023-01-24)
 ================
 
 - Build Linux binary wheels for Python 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `zope.container-5.0/CONTRIBUTING.md` & `zope.container-5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/LICENSE.txt` & `zope.container-5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/PKG-INFO` & `zope.container-5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.container
-Version: 5.0
+Version: 5.1
 Summary: Zope Container
 Home-page: https://github.com/zopefoundation/zope.container
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopecontainer.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.container/issues
@@ -68,14 +68,22 @@
 Documentation is hosted at https://zopecontainer.readthedocs.io
 
 
 =========
  Changes
 =========
 
+5.1 (2023-04-24)
+================
+
+- Drop using ``setup_requires`` due to constant problems on GHA.
+
+- Add preliminary support for Python 3.12a7.
+
+
 5.0 (2023-01-24)
 ================
 
 - Build Linux binary wheels for Python 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `zope.container-5.0/README.rst` & `zope.container-5.1/README.rst`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/appveyor.yml` & `zope.container-5.1/appveyor.yml`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
   matrix:
     - python: 37-x64
     - python: 38-x64
     - python: 39-x64
     - python: 310-x64
     - python: 311-x64
+    # `multibuild` cannot install non-final versions as they are not on
+    # ftp.python.org, so we skip Python 3.11 until its final release:
+    # - python: 312-x64
 
 install:
   - "SET PYTHONVERSION=%PYTHON%"
   - "SET PATH=C:\\Python%PYTHON%;c:\\Python%PYTHON%\\scripts;%PATH%"
   - ps: |
       $env:PYTHON = "C:\\Python${env:PYTHON}"
       if (-not (Test-Path $env:PYTHON)) {
```

### Comparing `zope.container-5.0/docs/Makefile` & `zope.container-5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/docs/api.rst` & `zope.container-5.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/docs/conf.py` & `zope.container-5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/docs/index.rst` & `zope.container-5.1/docs/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ================
  zope.container
 ================
 
-.. image:: https://travis-ci.org/zopefoundation/zope.container.png?branch=master
-        :target: https://travis-ci.org/zopefoundation/zope.container
+.. image:: https://github.com/zopefoundation/zope.container/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.container/actions/workflows/tests.yml
 
 .. image:: https://readthedocs.org/projects/zopecontainer/badge/?version=latest
         :target: http://zopecontainer.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 This package define interfaces of container components, and provides
 container implementations such as a :class:`~.BTreeContainer` and
```

### Comparing `zope.container-5.0/docs/make.bat` & `zope.container-5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/setup.cfg` & `zope.container-5.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	.meta.toml
 	docs/_build/html/_sources/*
 
 [isort]
 force_single_line = True
 combine_as_imports = True
 sections = FUTURE,STDLIB,THIRDPARTY,ZOPE,FIRSTPARTY,LOCALFOLDER
-known_third_party = six, docutils, pkg_resources
+known_third_party = docutils, pkg_resources, pytz
 known_zope = 
 known_first_party = 
 default_section = ZOPE
 line_length = 79
 lines_after_imports = 2
 
 [egg_info]
```

### Comparing `zope.container-5.0/src/zope/container/_compat.h` & `zope.container-5.1/src/zope/container/_compat.h`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/_proxy.py` & `zope.container-5.1/src/zope/container/_proxy.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/_util.py` & `zope.container-5.1/src/zope/container/_util.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/_zope_container_contained.c` & `zope.container-5.1/src/zope/container/_zope_container_contained.c`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  The proxy will only be unghostified if you need to access one of the
  attributes provided by the proxy.
 
  */
 
 
 #include "Python.h"
-#include "cPersistence.h"
+#include "persistent/cPersistence.h"
 #include "_compat.h"
 
 static PyObject *str_p_deactivate;
 
 /* Now things get weird. We use _zope_proxy_proxy.c like a complex macro.
    To do so, we define things that zope.proxy/proxy.h would define, and
    suppress inclusion of that file, and then include the complete .c file. */
@@ -72,15 +72,15 @@
 
 #define OBJECT(O) ((PyObject*)(O))
 #define Proxy_GET_OBJECT(ob)   (((ProxyObject *)(ob))->proxy_object)
 
 #define CLEAR(O) Py_CLEAR(O)
 
 /* Incude the proxy C source */
-#include "_zope_proxy_proxy.c"
+#include "zope/proxy/_zope_proxy_proxy.c"
 
 #define MAKE_PYSTRING(s) PyUnicode_FromString(s)
 #define MAKE_STRING(name) PyBytes_AS_STRING(PyUnicode_AsUTF8String(name))
 
 #define SPECIAL(NAME) (                        \
     *(NAME) == '_' &&                          \
       (((NAME)[1] == 'p' && (NAME)[2] == '_')  \
```

### Comparing `zope.container-5.0/src/zope/container/btree.py` & `zope.container-5.1/src/zope/container/btree.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/configure.zcml` & `zope.container-5.1/src/zope/container/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/constraints.py` & `zope.container-5.1/src/zope/container/constraints.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/constraints.rst` & `zope.container-5.1/src/zope/container/constraints.rst`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/contained.py` & `zope.container-5.1/src/zope/container/contained.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/directory.py` & `zope.container-5.1/src/zope/container/directory.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/find.py` & `zope.container-5.1/src/zope/container/find.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/folder.py` & `zope.container-5.1/src/zope/container/folder.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/i18n.py` & `zope.container-5.1/src/zope/container/i18n.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/interfaces.py` & `zope.container-5.1/src/zope/container/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/ordered.py` & `zope.container-5.1/src/zope/container/ordered.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/sample.py` & `zope.container-5.1/src/zope/container/sample.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/size.py` & `zope.container-5.1/src/zope/container/size.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/testing.py` & `zope.container-5.1/src/zope/container/testing.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/constraints_example.py` & `zope.container-5.1/src/zope/container/tests/constraints_example.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/directory.rst` & `zope.container-5.1/src/zope/container/tests/directory.rst`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_btree.py` & `zope.container-5.1/src/zope/container/tests/test_btree.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_compile_flags.py` & `zope.container-5.1/src/zope/container/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_constraints.py` & `zope.container-5.1/src/zope/container/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_contained.py` & `zope.container-5.1/src/zope/container/tests/test_contained.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_contained_zodb.py` & `zope.container-5.1/src/zope/container/tests/test_contained_zodb.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_containertraversable.py` & `zope.container-5.1/src/zope/container/tests/test_containertraversable.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_containertraverser.py` & `zope.container-5.1/src/zope/container/tests/test_containertraverser.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_dependencies.py` & `zope.container-5.1/src/zope/container/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_directory.py` & `zope.container-5.1/src/zope/container/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_find.py` & `zope.container-5.1/src/zope/container/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_folder.py` & `zope.container-5.1/src/zope/container/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_icontainer.py` & `zope.container-5.1/src/zope/container/tests/test_icontainer.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_ordered.py` & `zope.container-5.1/src/zope/container/tests/test_ordered.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/tests/test_size.py` & `zope.container-5.1/src/zope/container/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope/container/traversal.py` & `zope.container-5.1/src/zope/container/traversal.py`

 * *Files identical despite different names*

### Comparing `zope.container-5.0/src/zope.container.egg-info/PKG-INFO` & `zope.container-5.1/src/zope.container.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.container
-Version: 5.0
+Version: 5.1
 Summary: Zope Container
 Home-page: https://github.com/zopefoundation/zope.container
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zopecontainer.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.container/issues
@@ -68,14 +68,22 @@
 Documentation is hosted at https://zopecontainer.readthedocs.io
 
 
 =========
  Changes
 =========
 
+5.1 (2023-04-24)
+================
+
+- Drop using ``setup_requires`` due to constant problems on GHA.
+
+- Add preliminary support for Python 3.12a7.
+
+
 5.0 (2023-01-24)
 ================
 
 - Build Linux binary wheels for Python 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `zope.container-5.0/src/zope.container.egg-info/requires.txt` & `zope.container-5.1/src/zope.container.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-persistent>=4.1.0
-zope.proxy>=4.1.5
 BTrees
+persistent>=4.1.0
 zope.cachedescriptors
 zope.component
 zope.deferredimport
 zope.dottedname
 zope.event
 zope.filerepresentation
 zope.i18nmessageid
 zope.interface
 zope.lifecycleevent>=3.5.2
 zope.location>=3.5.4
+zope.proxy>=4.1.5
 zope.publisher
 zope.schema
 zope.security
 zope.size
 zope.traversing>=4.0.0a1
 setuptools
```

### Comparing `zope.container-5.0/tox.ini` & `zope.container-5.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/c-code
 [tox]
-minversion = 3.18
+minversion = 4.0
 envlist =
     lint
     py37,py37-pure
     py38,py38-pure
     py39,py39-pure
     py310,py310-pure
     py311,py311-pure
+    py312,py312-pure
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
+pip_pre = py312: true
 deps =
 setenv =
     pure: PURE_PYTHON=1
     !pure-!pypy3: PURE_PYTHON=0
     ZOPE_INTERFACE_STRICT_IRO=1
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
```

