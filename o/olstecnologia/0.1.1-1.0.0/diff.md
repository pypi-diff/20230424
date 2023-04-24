# Comparing `tmp/olstecnologia-0.1.1.tar.gz` & `tmp/olstecnologia-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olstecnologia-0.1.1.tar", max compression
+gzip compressed data, was "olstecnologia-1.0.0.tar", max compression
```

## Comparing `olstecnologia-0.1.1.tar` & `olstecnologia-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,15 @@
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-0.1.1/olstecnologia/__init__.py
--rw-r--r--   0        0        0       63 2023-04-11 14:42:19.577223 olstecnologia-0.1.1/olstecnologia/app.py
--rw-r--r--   0        0        0       26 2023-04-06 11:58:53.547641 olstecnologia-0.1.1/olstecnologia/config/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-11 18:31:22.350517 olstecnologia-0.1.1/olstecnologia/config/database.py
--rw-r--r--   0        0        0      179 2023-04-10 17:58:30.917062 olstecnologia-0.1.1/olstecnologia/entities/__init__.py
--rw-r--r--   0        0        0      287 2023-04-10 17:56:32.173814 olstecnologia-0.1.1/olstecnologia/entities/bairro_entity.py
--rw-r--r--   0        0        0      132 2023-04-06 11:46:50.189344 olstecnologia-0.1.1/olstecnologia/entities/base_declative_entity.py
--rw-r--r--   0        0        0      323 2023-04-10 17:55:35.872698 olstecnologia-0.1.1/olstecnologia/entities/cidade_entity.py
--rw-r--r--   0        0        0      306 2023-04-10 17:56:13.452742 olstecnologia-0.1.1/olstecnologia/entities/logradouro_entity.py
--rw-r--r--   0        0        0     3254 2023-04-11 12:47:33.145374 olstecnologia-0.1.1/olstecnologia/entities/paciente_entity.py
--rw-r--r--   0        0        0      315 2023-04-10 17:59:00.227941 olstecnologia-0.1.1/olstecnologia/entities/rua_entity.py
--rw-r--r--   0        0        0       47 2023-04-11 11:19:34.706909 olstecnologia-0.1.1/olstecnologia/features/__int__.py
--rw-r--r--   0        0        0       48 2023-04-11 18:19:03.436972 olstecnologia-0.1.1/olstecnologia/features/atualiza_endereco/__init__.py
--rw-r--r--   0        0        0     3864 2023-04-11 18:30:45.661813 olstecnologia-0.1.1/olstecnologia/features/atualiza_endereco/atualiza_endereco.py
--rw-r--r--   0        0        0        0 2023-04-10 13:16:23.454502 olstecnologia-0.1.1/olstecnologia/services/__init__.py
--rw-r--r--   0        0        0      829 2023-04-11 13:34:43.232245 olstecnologia-0.1.1/olstecnologia/services/utils.py
--rw-r--r--   0        0        0      535 2023-04-11 18:32:17.216819 olstecnologia-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-0.1.1/README.md
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 olstecnologia-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-17 18:42:51.592799 olstecnologia-1.0.0/olstecnologia/__init__.py
+-rw-r--r--   0        0        0     6394 2023-04-24 19:40:00.245544 olstecnologia-1.0.0/olstecnologia/app.py
+-rw-r--r--   0        0        0       26 2023-04-17 11:23:57.131012 olstecnologia-1.0.0/olstecnologia/config/__init__.py
+-rw-r--r--   0        0        0     1836 2023-04-17 11:29:49.555822 olstecnologia-1.0.0/olstecnologia/config/database.py
+-rw-r--r--   0        0        0  1330176 2023-04-12 11:47:26.437495 olstecnologia-1.0.0/olstecnologia/config/fbclient.dll
+-rw-r--r--   0        0        0        0 2023-04-24 19:44:34.663276 olstecnologia-1.0.0/olstecnologia/features/__init__.py
+-rw-r--r--   0        0        0     7979 2023-04-24 17:40:59.208166 olstecnologia-1.0.0/olstecnologia/features/update_addres_feature.py
+-rw-r--r--   0        0        0      170 2023-04-17 19:35:08.114252 olstecnologia-1.0.0/olstecnologia/services/__init__.py
+-rw-r--r--   0        0        0     6259 2023-04-24 19:38:29.262036 olstecnologia-1.0.0/olstecnologia/services/check_db_service.py
+-rw-r--r--   0        0        0     2659 2023-04-17 19:55:30.611367 olstecnologia-1.0.0/olstecnologia/services/connection_service.py
+-rw-r--r--   0        0        0     6535 2023-04-24 19:34:53.382912 olstecnologia-1.0.0/olstecnologia/services/services_service.py
+-rw-r--r--   0        0        0     2117 2023-04-24 17:41:22.159646 olstecnologia-1.0.0/olstecnologia/services/utils_service.py
+-rw-r--r--   0        0        0      711 2023-04-24 19:41:43.366316 olstecnologia-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-1.0.0/README.md
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 olstecnologia-1.0.0/PKG-INFO
```

