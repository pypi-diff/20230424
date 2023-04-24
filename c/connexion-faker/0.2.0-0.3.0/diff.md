# Comparing `tmp/connexion-faker-0.2.0.tar.gz` & `tmp/connexion_faker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connexion-faker-0.2.0.tar", max compression
+gzip compressed data, was "connexion_faker-0.3.0.tar", max compression
```

## Comparing `connexion-faker-0.2.0.tar` & `connexion_faker-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-05-16 19:09:19.859835 connexion-faker-0.2.0/LICENSE
--rw-r--r--   0        0        0       22 2022-05-16 19:09:19.859835 connexion-faker-0.2.0/connexion_faker/__init__.py
--rw-r--r--   0        0        0      783 2022-05-16 19:09:19.859835 connexion-faker-0.2.0/connexion_faker/aiohttp.py
--rw-r--r--   0        0        0     2523 2022-05-16 19:09:19.859835 connexion-faker-0.2.0/connexion_faker/base.py
--rw-r--r--   0        0        0      846 2022-05-16 19:09:19.859835 connexion-faker-0.2.0/connexion_faker/django.py
--rw-r--r--   0        0        0      769 2022-05-16 19:09:19.863835 connexion-faker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      858 2022-05-16 19:09:27.635013 connexion-faker-0.2.0/setup.py
--rw-r--r--   0        0        0      828 2022-05-16 19:09:27.635263 connexion-faker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-24 14:54:31.544743 connexion_faker-0.3.0/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-24 14:54:31.544743 connexion_faker-0.3.0/connexion_faker/__init__.py
+-rw-r--r--   0        0        0      783 2023-04-24 14:54:31.548743 connexion_faker-0.3.0/connexion_faker/aiohttp.py
+-rw-r--r--   0        0        0     2523 2023-04-24 14:54:31.548743 connexion_faker-0.3.0/connexion_faker/base.py
+-rw-r--r--   0        0        0      846 2023-04-24 14:54:31.548743 connexion_faker-0.3.0/connexion_faker/django.py
+-rw-r--r--   0        0        0      829 2023-04-24 14:54:31.548743 connexion_faker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1007 1970-01-01 00:00:00.000000 connexion_faker-0.3.0/PKG-INFO
```

### Comparing `connexion-faker-0.2.0/LICENSE` & `connexion_faker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connexion-faker-0.2.0/connexion_faker/aiohttp.py` & `connexion_faker-0.3.0/connexion_faker/aiohttp.py`

 * *Files identical despite different names*

### Comparing `connexion-faker-0.2.0/connexion_faker/base.py` & `connexion_faker-0.3.0/connexion_faker/base.py`

 * *Files identical despite different names*

### Comparing `connexion-faker-0.2.0/connexion_faker/django.py` & `connexion_faker-0.3.0/connexion_faker/django.py`

 * *Files identical despite different names*

### Comparing `connexion-faker-0.2.0/pyproject.toml` & `connexion_faker-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "connexion-faker"
-version = "0.2.0"
+version = "0.3.0"
 description = "Auto-generate mocks from your Connexion API using OpenAPI"
 authors = ["Erle Carrara <carrara.erle@gmail.com>"]
+repository = "https://github.com/buserbrasil/connexion-faker"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 connexion = "^2.9.0"
-Faker = "<14"
+Faker = "*"
 aiohttp = {version = "^3.0", optional = true}
 aiohttp_jinja2 = {version = "^1.0", optional = true}
 Django = {version = "^4.0.2", optional = true}
 django-connexion = {version = "^0", optional = true}
 
 [tool.poetry.extras]
 aiohttp = ["aiohttp", "aiohttp_jinja2"]
```

