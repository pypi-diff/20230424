# Comparing `tmp/apache-airflow-providers-trino-5.0.0.tar.gz` & `tmp/apache-airflow-providers-trino-5.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-trino-5.0.0.tar", last modified: Fri Apr 21 19:38:56 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-trino-5.0.0rc1.tar", last modified: Fri Apr 21 19:50:11 2023, max compression
```

## Comparing `apache-airflow-providers-trino-5.0.0.tar` & `apache-airflow-providers-trino-5.0.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:38:54.000000 apache-airflow-providers-trino-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.0.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13318 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11747 2023-04-21 19:38:54.000000 apache-airflow-providers-trino-5.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-04-21 19:38:54.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9383 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/hooks/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/operators/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/transfers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4998 2023-04-21 10:05:41.000000 apache-airflow-providers-trino-5.0.0/airflow/providers/trino/transfers/gcs_to_trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13318 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      187 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-trino-5.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1890 2023-04-21 19:38:56.000000 apache-airflow-providers-trino-5.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1767 2023-04-21 19:38:54.000000 apache-airflow-providers-trino-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13324 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11750 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9383 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-04-21 10:05:41.000000 apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13324 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-trino-5.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-04-21 19:50:11.000000 apache-airflow-providers-trino-5.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-04-21 19:50:10.000000 apache-airflow-providers-trino-5.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-trino-5.0.0/LICENSE` & `apache-airflow-providers-trino-5.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/MANIFEST.in` & `apache-airflow-providers-trino-5.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/PKG-INFO` & `apache-airflow-providers-trino-5.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.0.0
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.0.0``
+Release: ``5.0.0rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.0.0/README.rst` & `apache-airflow-providers-trino-5.0.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.0.0``
+Release: ``5.0.0rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/get_provider_info.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/hooks/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/hooks/trino.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/hooks/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/operators/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/operators/trino.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/operators/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/transfers/__init__.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache-airflow-providers-trino-5.0.0rc1/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/PKG-INFO` & `apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.0.0
+Version: 5.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.0.0/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.0.0``
+Release: ``5.0.0rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-trino-5.0.0/apache_airflow_providers_trino.egg-info/SOURCES.txt` & `apache-airflow-providers-trino-5.0.0rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/pyproject.toml` & `apache-airflow-providers-trino-5.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.0.0/setup.cfg` & `apache-airflow-providers-trino-5.0.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

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
 	pandas>=0.17.1
 	trino>=0.318.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.trino.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.trino
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-trino-5.0.0/setup.py` & `apache-airflow-providers-trino-5.0.0rc1/setup.py`

 * *Files identical despite different names*

