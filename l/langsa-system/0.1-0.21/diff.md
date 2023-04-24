# Comparing `tmp/langsa_system-0.1.tar.gz` & `tmp/langsa_system-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsa_system-0.1.tar", last modified: Mon Apr 24 14:17:32 2023, max compression
+gzip compressed data, was "langsa_system-0.21.tar", last modified: Mon Apr 24 13:59:29 2023, max compression
```

## Comparing `langsa_system-0.1.tar` & `langsa_system-0.21.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:17:32.457641 langsa_system-0.1/
--rw-rw-rw-   0        0        0    35823 2023-04-04 10:37:11.000000 langsa_system-0.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-24 14:17:32.457641 langsa_system-0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11534 2023-04-04 10:57:40.000000 langsa_system-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 14:17:32.456489 langsa_system-0.1/langsa_system.egg-info/
--rw-rw-rw-   0        0        0      273 2023-04-24 14:17:32.000000 langsa_system-0.1/langsa_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-24 14:17:32.000000 langsa_system-0.1/langsa_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:17:32.000000 langsa_system-0.1/langsa_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:17:32.000000 langsa_system-0.1/langsa_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 14:17:32.457641 langsa_system-0.1/setup.cfg
--rw-rw-rw-   0        0        0      555 2023-04-24 14:17:15.000000 langsa_system-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:59:29.004444 langsa_system-0.21/
+-rw-rw-rw-   0        0        0    35823 2023-04-04 10:37:11.000000 langsa_system-0.21/LICENSE
+-rw-rw-rw-   0        0        0      274 2023-04-24 13:59:29.004444 langsa_system-0.21/PKG-INFO
+-rw-rw-rw-   0        0        0    11534 2023-04-04 10:57:40.000000 langsa_system-0.21/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:59:29.004444 langsa_system-0.21/langsa_system.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-04-24 13:59:28.000000 langsa_system-0.21/langsa_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-24 13:59:28.000000 langsa_system-0.21/langsa_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:59:28.000000 langsa_system-0.21/langsa_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:59:28.000000 langsa_system-0.21/langsa_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:59:29.004444 langsa_system-0.21/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-04-24 13:31:40.000000 langsa_system-0.21/setup.py
```

### Comparing `langsa_system-0.1/LICENSE` & `langsa_system-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `langsa_system-0.1/README.md` & `langsa_system-0.21/README.md`

 * *Files identical despite different names*

