# Comparing `tmp/apache-airflow-providers-snowflake-4.0.5.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.0.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-snowflake-4.0.5.tar", last modified: Fri Apr 21 19:38:49 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-snowflake-4.0.5rc1.tar", last modified: Fri Apr 21 19:50:04 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.0.5.tar` & `apache-airflow-providers-snowflake-4.0.5rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:38:47.000000 apache-airflow-providers-snowflake-4.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.0.5/NOTICE
--rw-r--r--   0 root         (0) root         (0)    18293 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16711 2023-04-21 19:38:47.000000 apache-airflow-providers-snowflake-4.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-04-21 19:38:47.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17835 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/hooks/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15192 2023-03-10 19:32:05.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5973 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     4998 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/utils/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18293 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1079 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      217 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:38:48.000000 apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-snowflake-4.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1946 2023-04-21 19:38:49.000000 apache-airflow-providers-snowflake-4.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-04-21 19:38:47.000000 apache-airflow-providers-snowflake-4.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.0.5rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:50:03.000000 apache-airflow-providers-snowflake-4.0.5rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.0.5rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    18299 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16714 2023-04-21 19:50:03.000000 apache-airflow-providers-snowflake-4.0.5rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-04-21 19:50:03.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17835 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/hooks/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15192 2023-03-10 19:32:05.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5973 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/utils/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18299 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-snowflake-4.0.5rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-04-21 19:50:04.000000 apache-airflow-providers-snowflake-4.0.5rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-04-21 19:50:03.000000 apache-airflow-providers-snowflake-4.0.5rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.0.5/LICENSE` & `apache-airflow-providers-snowflake-4.0.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/MANIFEST.in` & `apache-airflow-providers-snowflake-4.0.5rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/PKG-INFO` & `apache-airflow-providers-snowflake-4.0.5rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.0.5
+Version: 4.0.5rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.0.5/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.0.5``
+Release: ``4.0.5rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.0.5/README.rst` & `apache-airflow-providers-snowflake-4.0.5rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.0.5``
+Release: ``4.0.5rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.0.5rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.0.5
+Version: 4.0.5rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.0.5/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.0.5``
+Release: ``4.0.5rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.0.5/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.0.5rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/pyproject.toml` & `apache-airflow-providers-snowflake-4.0.5rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.0.5/setup.cfg` & `apache-airflow-providers-snowflake-4.0.5rc1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
-	apache-airflow>=2.3.0
+	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.3.0.dev0
 	snowflake-connector-python>=2.4.1
 	snowflake-sqlalchemy>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.0.5/setup.py` & `apache-airflow-providers-snowflake-4.0.5rc1/setup.py`

 * *Files identical despite different names*

