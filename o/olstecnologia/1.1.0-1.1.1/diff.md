# Comparing `tmp/olstecnologia-1.1.0.tar.gz` & `tmp/olstecnologia-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olstecnologia-1.1.0.tar", max compression
+gzip compressed data, was "olstecnologia-1.1.1.tar", max compression
```

## Comparing `olstecnologia-1.1.0.tar` & `olstecnologia-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.0/olstecnologia/__init__.py
--rw-r--r--   0        0        0     6394 2023-04-24 19:40:00.245544 olstecnologia-1.1.0/olstecnologia/app.py
--rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.0/olstecnologia/config/__init__.py
--rw-r--r--   0        0        0     1836 2023-04-17 11:29:49.555822 olstecnologia-1.1.0/olstecnologia/config/database.py
--rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.0/olstecnologia/config/fbclient.dll
--rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.0/olstecnologia/features/__init__.py
--rw-r--r--   0        0        0     7979 2023-04-24 19:55:32.427961 olstecnologia-1.1.0/olstecnologia/features/update_addres_feature.py
--rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.0/olstecnologia/services/__init__.py
--rw-r--r--   0        0        0     6259 2023-04-24 19:38:29.262036 olstecnologia-1.1.0/olstecnologia/services/check_db_service.py
--rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.0/olstecnologia/services/connection_service.py
--rw-r--r--   0        0        0     6522 2023-04-24 19:54:50.040979 olstecnologia-1.1.0/olstecnologia/services/services_service.py
--rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.0/olstecnologia/services/utils_service.py
--rw-r--r--   0        0        0      711 2023-04-24 20:02:31.000796 olstecnologia-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.0/README.md
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 olstecnologia-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.1.1/olstecnologia/__init__.py
+-rw-r--r--   0        0        0     6394 2023-04-24 19:40:00.245544 olstecnologia-1.1.1/olstecnologia/app.py
+-rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.1.1/olstecnologia/config/__init__.py
+-rw-r--r--   0        0        0     1836 2023-04-17 11:29:49.555822 olstecnologia-1.1.1/olstecnologia/config/database.py
+-rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.1.1/olstecnologia/config/fbclient.dll
+-rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.1.1/olstecnologia/features/__init__.py
+-rw-r--r--   0        0        0     7979 2023-04-24 19:55:32.427961 olstecnologia-1.1.1/olstecnologia/features/update_addres_feature.py
+-rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.1.1/olstecnologia/services/__init__.py
+-rw-r--r--   0        0        0     6187 2023-04-24 20:04:24.783157 olstecnologia-1.1.1/olstecnologia/services/check_db_service.py
+-rw-r--r--   0        0        0      551 2023-04-24 19:55:17.355831 olstecnologia-1.1.1/olstecnologia/services/connection_service.py
+-rw-r--r--   0        0        0     6522 2023-04-24 19:54:50.040979 olstecnologia-1.1.1/olstecnologia/services/services_service.py
+-rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.1.1/olstecnologia/services/utils_service.py
+-rw-r--r--   0        0        0      711 2023-04-24 20:04:39.053510 olstecnologia-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.1.1/README.md
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 olstecnologia-1.1.1/PKG-INFO
```

### Comparing `olstecnologia-1.1.0/olstecnologia/app.py` & `olstecnologia-1.1.1/olstecnologia/app.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.0/olstecnologia/config/database.py` & `olstecnologia-1.1.1/olstecnologia/config/database.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.0/olstecnologia/config/fbclient.dll` & `olstecnologia-1.1.1/olstecnologia/config/fbclient.dll`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.0/olstecnologia/features/update_addres_feature.py` & `olstecnologia-1.1.1/olstecnologia/features/update_addres_feature.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.0/olstecnologia/services/check_db_service.py` & `olstecnologia-1.1.1/olstecnologia/services/check_db_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from sqlalchemy import text, create_engine, inspect, select, MetaData, Table
+from sqlalchemy import MetaData, Table
 from olstecnologia.services.utils_service import colors
 from tqdm import tqdm
-import urllib.parse
-import ipdb
 
 # Inspecionar o banco e pegar as tabelas.
 # Ler cada tabela procurando o erro
     # encontrando erro vericar as colunas Adicionar no errors o nome da tabela
         # Verica cada coluna para ver qual que tem erro.
             # achando a coluna com erro, adicionar no dict da tabela criada e verificar as linhas
                 # achando a liha com erro verificar cada digito.
```

### Comparing `olstecnologia-1.1.0/olstecnologia/services/connection_service.py` & `olstecnologia-1.1.1/olstecnologia/services/connection_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.0/olstecnologia/services/services_service.py` & `olstecnologia-1.1.1/olstecnologia/services/services_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.0/olstecnologia/services/utils_service.py` & `olstecnologia-1.1.1/olstecnologia/services/utils_service.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-1.1.0/pyproject.toml` & `olstecnologia-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olstecnologia"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = ["Julio Pereira <juliopereira.dev@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlalchemy-firebird = "^0.7.6"
```

### Comparing `olstecnologia-1.1.0/PKG-INFO` & `olstecnologia-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olstecnologia
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 Author: Julio Pereira
 Author-email: juliopereira.dev@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fdb (>=2.0.2,<3.0.0)
```

