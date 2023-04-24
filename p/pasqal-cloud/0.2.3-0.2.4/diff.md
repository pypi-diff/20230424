# Comparing `tmp/pasqal-cloud-0.2.3.tar.gz` & `tmp/pasqal-cloud-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.2.3.tar", last modified: Thu Apr 20 09:10:35 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.2.4.tar", last modified: Mon Apr 24 09:26:10 2023, max compression
```

## Comparing `pasqal-cloud-0.2.3.tar` & `pasqal-cloud-0.2.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.422105 pasqal-cloud-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-20 09:10:35.422105 pasqal-cloud-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.414105 pasqal-cloud-0.2.3/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.414105 pasqal-cloud-0.2.3/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.418105 pasqal-cloud-0.2.3/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.418105 pasqal-cloud-0.2.3/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.414105 pasqal-cloud-0.2.3/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-20 09:10:35.000000 pasqal-cloud-0.2.3/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 09:10:35.000000 pasqal-cloud-0.2.3/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:10:35.000000 pasqal-cloud-0.2.3/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-20 09:10:35.000000 pasqal-cloud-0.2.3/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 09:10:35.000000 pasqal-cloud-0.2.3/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.418105 pasqal-cloud-0.2.3/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.418105 pasqal-cloud-0.2.3/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.418105 pasqal-cloud-0.2.3/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.418105 pasqal-cloud-0.2.3/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-20 09:10:35.422105 pasqal-cloud-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.422105 pasqal-cloud-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:35.422105 pasqal-cloud-0.2.3/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-20 09:10:23.000000 pasqal-cloud-0.2.3/tests/test_doubles/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.342655 pasqal-cloud-0.2.4/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.342655 pasqal-cloud-0.2.4/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.342655 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 09:26:10.000000 pasqal-cloud-0.2.4/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:26:10.346655 pasqal-cloud-0.2.4/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 09:25:58.000000 pasqal-cloud-0.2.4/tests/test_doubles/authentication.py
```

### Comparing `pasqal-cloud-0.2.3/LICENSE` & `pasqal-cloud-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/PKG-INFO` & `pasqal-cloud-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.3
+Version: 0.2.4
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.2.3/README.md` & `pasqal-cloud-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/__init__.py` & `pasqal-cloud-0.2.4/pasqal_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/_version.py` & `pasqal-cloud-0.2.4/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/authentication.py` & `pasqal-cloud-0.2.4/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/batch.py` & `pasqal-cloud-0.2.4/pasqal_cloud/batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/client.py` & `pasqal-cloud-0.2.4/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.2.4/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.2.4/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/errors.py` & `pasqal-cloud-0.2.4/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/job.py` & `pasqal-cloud-0.2.4/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.2.4/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.2.4/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.3
+Version: 0.2.4
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pasqal-cloud-0.2.3/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.2.4/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/sdk/setup.py` & `pasqal-cloud-0.2.4/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/setup.py` & `pasqal-cloud-0.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     # TODO:
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
     url="https://github.com/pasqal-io/pasqal-cloud",
     install_requires=[
-        "auth0-python==3.23.1",
-        "requests==2.25.1",
-        "pyjwt[crypto]==2.5.0",
+        "auth0-python >= 3.23.1, <4.0.0 ",
+        "requests>=2.25.1, <3.0.0",
+        "pyjwt[crypto]>=2.5.0, <3.0.0",
     ],
     extras_require={
         "dev": {
             "black==20.8b1",
             "flake8==3.9.0",
             "flake8-import-order==0.18.1",
             "mypy==0.982",
```

### Comparing `pasqal-cloud-0.2.3/tests/conftest.py` & `pasqal-cloud-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/tests/test_batch.py` & `pasqal-cloud-0.2.4/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/tests/test_client.py` & `pasqal-cloud-0.2.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.2.4/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/tests/test_config.py` & `pasqal-cloud-0.2.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/tests/test_device_specs.py` & `pasqal-cloud-0.2.4/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.3/tests/test_doubles/authentication.py` & `pasqal-cloud-0.2.4/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

