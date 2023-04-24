# Comparing `tmp/colemen_volent-0.0.2.tar.gz` & `tmp/colemen_volent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colemen_volent-0.0.2.tar", last modified: Fri Apr 21 15:25:45 2023, max compression
+gzip compressed data, was "colemen_volent-0.0.3.tar", last modified: Mon Apr 24 13:21:43 2023, max compression
```

## Comparing `colemen_volent-0.0.2.tar` & `colemen_volent-0.0.3.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.354416 colemen_volent-0.0.2/
--rw-rw-rw-   0        0        0      469 2023-04-21 15:25:45.353416 colemen_volent-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.296415 colemen_volent-0.0.2/colemen_volent.egg-info/
--rw-rw-rw-   0        0        0      469 2023-04-21 15:25:45.000000 colemen_volent-0.0.2/colemen_volent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1485 2023-04-21 15:25:45.000000 colemen_volent-0.0.2/colemen_volent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:25:45.000000 colemen_volent-0.0.2/colemen_volent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 15:25:45.000000 colemen_volent-0.0.2/colemen_volent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 15:25:45.000000 colemen_volent-0.0.2/colemen_volent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 15:25:45.354416 colemen_volent-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-04-21 15:25:44.000000 colemen_volent-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.309416 colemen_volent-0.0.2/volent/
--rw-rw-rw-   0        0        0     5081 2023-04-18 20:41:28.000000 colemen_volent-0.0.2/volent/Column.py
--rw-rw-rw-   0        0        0     8710 2023-04-18 16:18:27.000000 colemen_volent-0.0.2/volent/Database.py
--rw-rw-rw-   0        0        0     5358 2023-04-21 13:44:38.000000 colemen_volent-0.0.2/volent/Field.py
--rw-rw-rw-   0        0        0    21054 2023-04-21 15:21:37.000000 colemen_volent-0.0.2/volent/Model.py
--rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.2/volent/NestedField.py
--rw-rw-rw-   0        0        0     2855 2023-04-21 13:13:13.000000 colemen_volent-0.0.2/volent/Relationship.py
--rw-rw-rw-   0        0        0    13985 2023-04-21 15:22:55.000000 colemen_volent-0.0.2/volent/Schema.py
--rw-rw-rw-   0        0        0     1478 2023-04-14 12:21:18.000000 colemen_volent-0.0.2/volent/UniqueConstraint.py
--rw-rw-rw-   0        0        0    11968 2023-04-21 14:11:15.000000 colemen_volent-0.0.2/volent/Volent.py
--rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.2/volent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.321415 colemen_volent-0.0.2/volent/data_types/
--rw-rw-rw-   0        0        0      831 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/BigInt.py
--rw-rw-rw-   0        0        0      650 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/Bool.py
--rw-rw-rw-   0        0        0     1695 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/Decimal.py
--rw-rw-rw-   0        0        0     1143 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/EncodedPrimary.py
--rw-rw-rw-   0        0        0      830 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/Integer.py
--rw-rw-rw-   0        0        0     1587 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/String.py
--rw-rw-rw-   0        0        0      864 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/TinyInt.py
--rw-rw-rw-   0        0        0     4404 2023-04-18 13:41:38.000000 colemen_volent-0.0.2/volent/data_types/TypeBase.py
--rw-rw-rw-   0        0        0      490 2023-04-11 19:39:38.000000 colemen_volent-0.0.2/volent/data_types/__init__.py
--rw-rw-rw-   0        0        0      873 2023-04-14 13:42:19.000000 colemen_volent-0.0.2/volent/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.326416 colemen_volent-0.0.2/volent/mixins/
--rw-rw-rw-   0        0        0    22731 2023-04-21 13:08:09.000000 colemen_volent-0.0.2/volent/mixins/DatabaseConnection.py
--rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.2/volent/mixins/EntityName.py
--rw-rw-rw-   0        0        0    17876 2023-04-18 14:57:37.000000 colemen_volent-0.0.2/volent/mixins/MySQLGeneratorMixin.py
--rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.2/volent/mixins/OrderedClass.py
--rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.2/volent/mixins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.333416 colemen_volent-0.0.2/volent/query/
--rw-rw-rw-   0        0        0     2805 2023-04-18 20:17:21.000000 colemen_volent-0.0.2/volent/query/Insert.py
--rw-rw-rw-   0        0        0    13456 2023-04-18 19:31:05.000000 colemen_volent-0.0.2/volent/query/Query.py
--rw-rw-rw-   0        0        0     6815 2023-04-21 15:25:12.000000 colemen_volent-0.0.2/volent/query/Select.py
--rw-rw-rw-   0        0        0     4240 2023-04-21 15:25:16.000000 colemen_volent-0.0.2/volent/query/Update.py
--rw-rw-rw-   0        0        0     2620 2023-04-18 18:54:55.000000 colemen_volent-0.0.2/volent/query/WhereMixin.py
--rw-rw-rw-   0        0        0      155 2023-04-18 19:08:07.000000 colemen_volent-0.0.2/volent/query/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.337417 colemen_volent-0.0.2/volent/settings/
--rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.2/volent/settings/__init__.py
--rw-rw-rw-   0        0        0     6137 2023-04-11 20:08:44.000000 colemen_volent-0.0.2/volent/settings/control.py
--rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.2/volent/settings/globe.py
--rw-rw-rw-   0        0        0     2165 2023-04-18 18:20:43.000000 colemen_volent-0.0.2/volent/settings/types.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:25:45.352416 colemen_volent-0.0.2/volent/validate/
--rw-rw-rw-   0        0        0     2426 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/CreditCardNumber.py
--rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/Email.py
--rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/Equal.py
--rw-rw-rw-   0        0        0     3391 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/IpAddress.py
--rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/Length.py
--rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/NoneOf.py
--rw-rw-rw-   0        0        0     2761 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/OneOf.py
--rw-rw-rw-   0        0        0     2237 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/PhoneNumber.py
--rw-rw-rw-   0        0        0     5757 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/Range.py
--rw-rw-rw-   0        0        0     2725 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/Regex.py
--rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/SocialSecurityNumber.py
--rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/StrongPassword.py
--rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.2/volent/validate/Validator.py
--rw-rw-rw-   0        0        0      615 2023-04-14 13:23:23.000000 colemen_volent-0.0.2/volent/validate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.533555 colemen_volent-0.0.3/
+-rw-rw-rw-   0        0        0      469 2023-04-24 13:21:43.533555 colemen_volent-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.165588 colemen_volent-0.0.3/colemen_volent.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1551 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 13:21:43.000000 colemen_volent-0.0.3/colemen_volent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:21:43.534555 colemen_volent-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-04-24 13:21:41.000000 colemen_volent-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.241587 colemen_volent-0.0.3/volent/
+-rw-rw-rw-   0        0        0     5081 2023-04-18 20:41:28.000000 colemen_volent-0.0.3/volent/Column.py
+-rw-rw-rw-   0        0        0     8710 2023-04-18 16:18:27.000000 colemen_volent-0.0.3/volent/Database.py
+-rw-rw-rw-   0        0        0     6358 2023-04-21 16:52:42.000000 colemen_volent-0.0.3/volent/Field.py
+-rw-rw-rw-   0        0        0    21054 2023-04-21 15:21:37.000000 colemen_volent-0.0.3/volent/Model.py
+-rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.3/volent/NestedField.py
+-rw-rw-rw-   0        0        0     2855 2023-04-21 13:13:13.000000 colemen_volent-0.0.3/volent/Relationship.py
+-rw-rw-rw-   0        0        0    16475 2023-04-21 16:50:12.000000 colemen_volent-0.0.3/volent/Schema.py
+-rw-rw-rw-   0        0        0     1478 2023-04-14 12:21:18.000000 colemen_volent-0.0.3/volent/UniqueConstraint.py
+-rw-rw-rw-   0        0        0    11968 2023-04-21 14:11:15.000000 colemen_volent-0.0.3/volent/Volent.py
+-rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.3/volent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.306591 colemen_volent-0.0.3/volent/data_types/
+-rw-rw-rw-   0        0        0      831 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/BigInt.py
+-rw-rw-rw-   0        0        0      650 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/Bool.py
+-rw-rw-rw-   0        0        0     1695 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/Decimal.py
+-rw-rw-rw-   0        0        0     1408 2023-04-21 16:46:29.000000 colemen_volent-0.0.3/volent/data_types/EncodedPrimary.py
+-rw-rw-rw-   0        0        0     1558 2023-04-21 16:38:30.000000 colemen_volent-0.0.3/volent/data_types/Integer.py
+-rw-rw-rw-   0        0        0     1587 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/String.py
+-rw-rw-rw-   0        0        0      864 2023-04-11 19:39:38.000000 colemen_volent-0.0.3/volent/data_types/TinyInt.py
+-rw-rw-rw-   0        0        0     4404 2023-04-18 13:41:38.000000 colemen_volent-0.0.3/volent/data_types/TypeBase.py
+-rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.0.3/volent/data_types/__init__.py
+-rw-rw-rw-   0        0        0      873 2023-04-14 13:42:19.000000 colemen_volent-0.0.3/volent/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.336555 colemen_volent-0.0.3/volent/mixins/
+-rw-rw-rw-   0        0        0    22731 2023-04-21 13:08:09.000000 colemen_volent-0.0.3/volent/mixins/DatabaseConnection.py
+-rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.3/volent/mixins/EntityName.py
+-rw-rw-rw-   0        0        0    17876 2023-04-18 14:57:37.000000 colemen_volent-0.0.3/volent/mixins/MySQLGeneratorMixin.py
+-rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.3/volent/mixins/OrderedClass.py
+-rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.3/volent/mixins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.379558 colemen_volent-0.0.3/volent/query/
+-rw-rw-rw-   0        0        0     2805 2023-04-18 20:17:21.000000 colemen_volent-0.0.3/volent/query/Insert.py
+-rw-rw-rw-   0        0        0    13462 2023-04-21 15:47:20.000000 colemen_volent-0.0.3/volent/query/Query.py
+-rw-rw-rw-   0        0        0     6815 2023-04-21 15:25:12.000000 colemen_volent-0.0.3/volent/query/Select.py
+-rw-rw-rw-   0        0        0     4240 2023-04-21 15:25:16.000000 colemen_volent-0.0.3/volent/query/Update.py
+-rw-rw-rw-   0        0        0     2620 2023-04-18 18:54:55.000000 colemen_volent-0.0.3/volent/query/WhereMixin.py
+-rw-rw-rw-   0        0        0      155 2023-04-18 19:08:07.000000 colemen_volent-0.0.3/volent/query/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.400555 colemen_volent-0.0.3/volent/settings/
+-rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.3/volent/settings/__init__.py
+-rw-rw-rw-   0        0        0     6137 2023-04-11 20:08:44.000000 colemen_volent-0.0.3/volent/settings/control.py
+-rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.3/volent/settings/globe.py
+-rw-rw-rw-   0        0        0     2165 2023-04-18 18:20:43.000000 colemen_volent-0.0.3/volent/settings/types.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:21:43.531557 colemen_volent-0.0.3/volent/validate/
+-rw-rw-rw-   0        0        0     2426 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/CreditCardNumber.py
+-rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Email.py
+-rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Equal.py
+-rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.0.3/volent/validate/FutureUnixDate.py
+-rw-rw-rw-   0        0        0     3391 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/IpAddress.py
+-rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Length.py
+-rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/NoneOf.py
+-rw-rw-rw-   0        0        0     2761 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/OneOf.py
+-rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.0.3/volent/validate/PastUnixDate.py
+-rw-rw-rw-   0        0        0     2237 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/PhoneNumber.py
+-rw-rw-rw-   0        0        0     5757 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Range.py
+-rw-rw-rw-   0        0        0     2725 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/Regex.py
+-rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/SocialSecurityNumber.py
+-rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.3/volent/validate/StrongPassword.py
+-rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.3/volent/validate/Validator.py
+-rw-rw-rw-   0        0        0      729 2023-04-21 16:11:07.000000 colemen_volent-0.0.3/volent/validate/__init__.py
```

### Comparing `colemen_volent-0.0.2/colemen_volent.egg-info/SOURCES.txt` & `colemen_volent-0.0.3/colemen_volent.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -38,18 +38,20 @@
 volent/settings/__init__.py
 volent/settings/control.py
 volent/settings/globe.py
 volent/settings/types.py
 volent/validate/CreditCardNumber.py
 volent/validate/Email.py
 volent/validate/Equal.py
+volent/validate/FutureUnixDate.py
 volent/validate/IpAddress.py
 volent/validate/Length.py
 volent/validate/NoneOf.py
 volent/validate/OneOf.py
+volent/validate/PastUnixDate.py
 volent/validate/PhoneNumber.py
 volent/validate/Range.py
 volent/validate/Regex.py
 volent/validate/SocialSecurityNumber.py
 volent/validate/StrongPassword.py
 volent/validate/Validator.py
 volent/validate/__init__.py
```

### Comparing `colemen_volent-0.0.2/setup.py` & `colemen_volent-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from glob import glob
 from setuptools import setup, find_packages
 import colemen_utilities.build_utils.general as _gen
 
 
-VERSION='0.0.2'
+VERSION='0.0.3'
 DESCRIPTION = 'volent'
 LONG_DESCRIPTION = 'None'
 
 
 _root_path = f"{os.getcwd()}/volent"
 PY_MODULES = _gen.list_py_modules(
     _root_path,
```

### Comparing `colemen_volent-0.0.2/volent/Column.py` & `colemen_volent-0.0.3/volent/Column.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/Database.py` & `colemen_volent-0.0.3/volent/Database.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/Field.py` & `colemen_volent-0.0.3/volent/Field.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,24 +36,26 @@
     column:_t.column_type = None
 
 
     required:bool = False
     nullable:bool = True
     default = None
     validators = None
+    data_type:_t.type_base_type = None
 
 
     def __init__(
         self,
         column:str=None,
         required:bool=False,
         nullable:bool=True,
         empty_string_is_null:bool=True,
         default=_settings.types.no_default,
         validate=None,
+        data_type:_t.type_base_type=None
         ):
         '''
             Create a schema Field
             ----------
 
             Arguments
             -------------------------
@@ -85,14 +87,15 @@
             * @xxx [04-14-2023 08:24:58]: documentation for Field
         '''
         self.column = column
         self.default = default
         self.required = required
         self.nullable = nullable
         self.empty_string_is_null = empty_string_is_null
+        self.data_type = data_type
 
         self.validators = c.arr.force_list(validate,allow_nulls=False)
 
 
     @property
     def summary(self):
         '''
@@ -147,14 +150,42 @@
             `@created`: 03-25-2023 12:02:50
             `@memberOf`: Field
             `@property`: value
         '''
         value = self.column.value
         return value
 
+
+
+    def validate_value(self,value):
+        val = value
+        if self.data_type is not None:
+            if hasattr(self.data_type,"deserialized_value"):
+                val = self.data_type.deserialized_value(val)
+        # val = self.column.data_type.
+
+        if isinstance(val,self.data_type.python_data_type) is False:
+            if self.nullable is True and val is None:
+                pass
+            else:
+                raise ValidationError(f"{self.name} expects {self.data_type.python_data_type} types.",self.name)
+
+        # if self._less_than_data_len(val) is False:
+        #     raise ValidationError(f"{self.name} is too long.",self.name)
+
+
+
+        if self._is_null(val):
+            raise ValidationError(f"{self.name} cannot be null.",self.name)
+
+
+        for valid in self.validators:
+            val = valid(val,self.name)
+
+
     def validate(self):
         # val = self.value
         val = self.column.deserialized_value
         # val = self.column.data_type.
 
         if isinstance(val,self.column.data_type.python_data_type) is False:
             if self.column.is_primary is True:
```

### Comparing `colemen_volent-0.0.2/volent/Model.py` & `colemen_volent-0.0.3/volent/Model.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/NestedField.py` & `colemen_volent-0.0.3/volent/NestedField.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/Relationship.py` & `colemen_volent-0.0.3/volent/Relationship.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/Schema.py` & `colemen_volent-0.0.3/volent/Schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     _name:str = None
     _fields:Iterable[_t.field_type] = None
     _schema_description:str = None
     _schema_crud_type:str = None
 
     __unique_prop_keys = None
 
+    # _field_aliases = None
+
+
 
     def __init__(self,model:_t.model_type=None) -> None:
         from volent.Model import Model as _model
         if isinstance(model,_model):
             self.model = model
         else:
             if model is not None:
@@ -232,14 +235,44 @@
             `version`: 1.0
             `method_name`: __validate
             * @xxx [04-21-2023 07:44:01]: documentation for __validate
         '''
         for f in self.fields:
             f.validate()
 
+
+    def __validate_dict(self,data:dict):
+        '''
+            Execute the validation process on all fields associated to this schema
+            ----------
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-21-2023 07:43:15
+            `memberOf`: Schema
+            `version`: 1.0
+            `method_name`: __validate
+            * @xxx [04-21-2023 07:44:01]: documentation for __validate
+        '''
+        data = c.obj.keys_to_snake_case(data)
+        for f in self.fields:
+            value = None
+            if f.name not in data:
+                if f.required is True:
+                    raise ValueError(f"{f.name} is required.")
+                elif c.string.to_snake_case(f.name) in data:
+                    value = data[c.string.to_snake_case(f.name)]
+                else:
+                    continue
+            else:
+                value = data[f.name]
+            if value is not None:
+                f.validate_value(value)
+
     def get_field(self,name:str)->_t.field_type:
         '''
             Retrieve a field from this schema
             ----------
 
             Arguments
             -------------------------
@@ -297,15 +330,35 @@
                 continue
 
             col.column_value = data[col]
 
 
     def dump(self,model:_t.model_type=None,many=False)->dict:
         '''Dump the contents of the model(s) using the fields to filter.'''
-
+        
+        
+        if isinstance(model,(dict)):
+            data = self._correlate_to_dict(model)
+            self.__validate_dict(model)
+            out_data = {}
+            for f in self.fields:
+                if f.name in data:
+                    if hasattr(f.data_type,"serialized_value"):
+                        v = f.data_type.serialized_value(data[f.name])
+                        # print(f"v: {v}")
+                        out_data[f.name] = v
+                        continue
+                    out_data[f.name] = data[f.name]
+            if many:
+                out_data = c.arr.force_list(out_data)
+            return out_data
+        
+        
+        
+        
 
         if isinstance(model,(list)):
             result = []
             from volent.Model import Model as _model
             for mdl in model:
                 if isinstance(mdl,_model) is False:
                     c.con.log(f"The mdl is not an instance of model:{mdl}","magenta")
@@ -327,15 +380,14 @@
         data = {}
         for f in self.fields:
             data[f.name] = f.value
         if many:
             data = c.arr.force_list(data)
         return data
 
-
     def new(self)->_t.schema_type:
         '''
             Validate this schema's data and submit it to the model's table in the databse.
             ----------
 
             Return {schema}
             ----------------------
@@ -427,14 +479,31 @@
             props = dir(self)
             # # @Mstep [] find the props that exist on this instance and not on the base.
             value = c.arr.find_list_diff(props,df_props)
             self.__unique_prop_keys = value
 
         return value
 
+    def _correlate_to_dict(self,data:dict):
+        out_data = {}
+        data = c.obj.keys_to_snake_case(data)
+        # print(f"_correlate_to_dict: data:{data}")
+        for f in self.fields:
+            # snake_field = c.string.to_snake_case(f.name)
+            # print(f"_correlate_to_dict: snake_field:{snake_field}")
+            if f.name in data:
+                out_data[f.name] = data[f.name]
+                continue
+            # if snake_field in data:
+            #     print(f"snake case field match: {c.string.to_snake_case(f.name)}")
+            #     out_data[c.string.to_snake_case(f.name)] = data[c.string.to_snake_case(f.name)]
+            #     continue
+
+        return out_data
+
     def _correlate_to_columns(self):
         '''
             Iterate all fields to find their corresponding columns in the current model.
             ----------
 
             Meta
             ----------
```

### Comparing `colemen_volent-0.0.2/volent/UniqueConstraint.py` & `colemen_volent-0.0.3/volent/UniqueConstraint.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/Volent.py` & `colemen_volent-0.0.3/volent/Volent.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/data_types/BigInt.py` & `colemen_volent-0.0.3/volent/data_types/BigInt.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/data_types/Bool.py` & `colemen_volent-0.0.3/volent/data_types/Bool.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/data_types/Decimal.py` & `colemen_volent-0.0.3/volent/data_types/Decimal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/data_types/EncodedPrimary.py` & `colemen_volent-0.0.3/volent/data_types/Integer.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,38 +4,46 @@
 # pylint: disable=unused-import
 
 from dataclasses import dataclass
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
+from volent.exceptions import ValidationError
 from volent.data_types.TypeBase import TypeBase as _type_base
 
 @dataclass
-class EncodedPrimary(_type_base):
-
-
-
+class Integer(_type_base):
 
     def __init__(self,data_length:int=None) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
-        self.max_data_length = 65535
-        self.sql_type_name = "BIGINT"
-        self.python_data_type = (int,str)
+        self.max_data_length = 4294967295
+        self.sql_type_name = "INTEGER"
+        self.python_data_type = (int)
 
         self._validate_data_length(data_length)
 
 
-    def __serialize(self,value):
-        if isinstance(value,(str)):
-            return value
-        return c.string.string_encode_int(value)
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} : {self.data_length}>"
 
-    def __deserialize(self,value):
+    def serialized_value(self,value):
         if isinstance(value,(int)):
             return value
-        return c.string.string_decode_int(value)
 
+        if isinstance(value,(str)):
+            if c.valid.numeric_only(value):
+                value = int(value)
+        if isinstance(value,(float)):
+            value = int(value)
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} : {self.data_length}>"
+        if isinstance(value,(int)) is False:
+            raise ValidationError(f"Failed to serialize {value} to integer.")
+
+        return value
+
+    def deserialized_value(self,value):
+        if isinstance(value,(int)):
+            return value
+        if isinstance(value,(int)) is False:
+            raise ValidationError(f"Failed to deserialize {value} to integer.")
```

### Comparing `colemen_volent-0.0.2/volent/data_types/Integer.py` & `colemen_volent-0.0.3/volent/data_types/TinyInt.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
 from volent.data_types.TypeBase import TypeBase as _type_base
 
 @dataclass
-class Integer(_type_base):
+class TinyInt(_type_base):
 
     def __init__(self,data_length:int=None) -> None:
         super().__init__(data_length)
         self.min_data_length = 0
-        self.max_data_length = 4294967295
-        self.sql_type_name = "INTEGER"
+        self.max_data_length = 255
+        self.sql_type_name = "TINYINT"
         self.python_data_type = (int)
 
-        self._validate_data_length(data_length)
+        self._validate_data_length(data_length,_settings.control.varchar_default_length)
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.data_length}>"
```

### Comparing `colemen_volent-0.0.2/volent/data_types/String.py` & `colemen_volent-0.0.3/volent/data_types/String.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/data_types/TypeBase.py` & `colemen_volent-0.0.3/volent/data_types/TypeBase.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/exceptions.py` & `colemen_volent-0.0.3/volent/exceptions.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/mixins/DatabaseConnection.py` & `colemen_volent-0.0.3/volent/mixins/DatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/mixins/EntityName.py` & `colemen_volent-0.0.3/volent/mixins/EntityName.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/mixins/MySQLGeneratorMixin.py` & `colemen_volent-0.0.3/volent/mixins/MySQLGeneratorMixin.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/mixins/OrderedClass.py` & `colemen_volent-0.0.3/volent/mixins/OrderedClass.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/query/Insert.py` & `colemen_volent-0.0.3/volent/query/Insert.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/query/Query.py` & `colemen_volent-0.0.3/volent/query/Query.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 @dataclass
 class Query(metaclass=OrderedClass):
     main = None
     # database:_t.database_type = None
     model:_t.model_type = None
     '''A reference to the model instance this query is referencing.'''
 
-    crud_type:str = None
+    query_crud_type:str = None
     data:dict = None
     database:_t.database_type = None
     '''A reference to the database instance used to execute this query.'''
 
     _selects:Iterable[str] = None
     _wheres:Iterable[str] = None
     _count:bool = False
```

### Comparing `colemen_volent-0.0.2/volent/query/Select.py` & `colemen_volent-0.0.3/volent/query/Select.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/query/Update.py` & `colemen_volent-0.0.3/volent/query/Update.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/query/WhereMixin.py` & `colemen_volent-0.0.3/volent/query/WhereMixin.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/settings/control.py` & `colemen_volent-0.0.3/volent/settings/control.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/settings/types.py` & `colemen_volent-0.0.3/volent/settings/types.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/CreditCardNumber.py` & `colemen_volent-0.0.3/volent/validate/CreditCardNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/Email.py` & `colemen_volent-0.0.3/volent/validate/Email.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/Equal.py` & `colemen_volent-0.0.3/volent/validate/Equal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/IpAddress.py` & `colemen_volent-0.0.3/volent/validate/IpAddress.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/Length.py` & `colemen_volent-0.0.3/volent/validate/Length.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/NoneOf.py` & `colemen_volent-0.0.3/volent/validate/NoneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/OneOf.py` & `colemen_volent-0.0.3/volent/validate/OneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/PhoneNumber.py` & `colemen_volent-0.0.3/volent/validate/PhoneNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/Range.py` & `colemen_volent-0.0.3/volent/validate/Range.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/Regex.py` & `colemen_volent-0.0.3/volent/validate/Regex.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/SocialSecurityNumber.py` & `colemen_volent-0.0.3/volent/validate/SocialSecurityNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/StrongPassword.py` & `colemen_volent-0.0.3/volent/validate/StrongPassword.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/Validator.py` & `colemen_volent-0.0.3/volent/validate/Validator.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.2/volent/validate/__init__.py` & `colemen_volent-0.0.3/volent/validate/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 from volent.validate.Equal import Equal
 from volent.validate.NoneOf import NoneOf
 from volent.validate.Range import Range
 from volent.validate.IpAddress import IpAddress
 from volent.validate.CreditCardNumber import CreditCardNumber
 from volent.validate.PhoneNumber import PhoneNumber
 from volent.validate.SocialSecurityNumber import SocialSecurityNumber
-from volent.validate.StrongPassword import StrongPassword
+from volent.validate.StrongPassword import StrongPassword
+from volent.validate.FutureUnixDate import FutureUnixDate
+from volent.validate.PastUnixDate import PastUnixDate
```

