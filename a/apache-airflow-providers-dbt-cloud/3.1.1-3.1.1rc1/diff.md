# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.1.1.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.1.1.tar", last modified: Fri Apr 21 19:37:04 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.1.1rc1.tar", last modified: Fri Apr 21 19:48:19 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.1.1.tar` & `apache-airflow-providers-dbt-cloud-3.1.1rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:37:03.000000 apache-airflow-providers-dbt-cloud-3.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9993 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8439 2023-04-21 19:37:03.000000 apache-airflow-providers-dbt-cloud-3.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-04-21 19:37:03.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12832 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5341 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4841 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9993 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1887 2023-04-21 19:37:04.000000 apache-airflow-providers-dbt-cloud-3.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-04-21 19:37:03.000000 apache-airflow-providers-dbt-cloud-3.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9999 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8442 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12832 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5341 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9999 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/LICENSE` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.1.1
+Version: 3.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.1``
+Release: ``3.1.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/README.rst` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.1``
+Release: ``3.1.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.1.1
+Version: 3.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.1``
+Release: ``3.1.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -44,21 +44,21 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
 	apache-airflow-providers-http
-	apache-airflow>=2.3.0
+	apache-airflow>=2.3.0.dev0
 	asgiref
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.dbt.cloud.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dbt.cloud
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1/setup.py` & `apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.py`

 * *Files identical despite different names*

