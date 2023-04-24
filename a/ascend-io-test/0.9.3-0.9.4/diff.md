# Comparing `tmp/ascend_io_test-0.9.3.tar.gz` & `tmp/ascend_io_test-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascend_io_test-0.9.3.tar", max compression
+gzip compressed data, was "ascend_io_test-0.9.4.tar", max compression
```

## Comparing `ascend_io_test-0.9.3.tar` & `ascend_io_test-0.9.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-17 13:04:31.076182 ascend_io_test-0.9.3/LICENSE
--rw-r--r--   0        0        0     4263 2023-04-17 13:04:31.076182 ascend_io_test-0.9.3/README.rst
--rw-r--r--   0        0        0      326 2023-04-17 13:04:31.076182 ascend_io_test-0.9.3/ascend_io_test/framework/__init__.py
--rw-r--r--   0        0        0     5011 2023-04-17 13:04:31.076182 ascend_io_test-0.9.3/ascend_io_test/framework/ascend_pyspark_transform.py
--rw-r--r--   0        0        0     1773 2023-04-17 13:04:31.076182 ascend_io_test-0.9.3/ascend_io_test/framework/ascend_python_bytestream_read_connector.py
--rw-r--r--   0        0        0     4601 2023-04-17 13:04:31.076182 ascend_io_test-0.9.3/ascend_io_test/framework/ascend_python_read_connector.py
--rw-r--r--   0        0        0     1091 2023-04-17 13:04:31.076182 ascend_io_test-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 ascend_io_test-0.9.3/setup.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ascend_io_test-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 18:04:53.673318 ascend_io_test-0.9.4/LICENSE
+-rw-r--r--   0        0        0     4440 2023-04-24 18:04:53.673318 ascend_io_test-0.9.4/README.rst
+-rw-r--r--   0        0        0      326 2023-04-24 18:04:53.673318 ascend_io_test-0.9.4/ascend_io_test/framework/__init__.py
+-rw-r--r--   0        0        0     5011 2023-04-24 18:04:53.673318 ascend_io_test-0.9.4/ascend_io_test/framework/ascend_pyspark_transform.py
+-rw-r--r--   0        0        0     1773 2023-04-24 18:04:53.673318 ascend_io_test-0.9.4/ascend_io_test/framework/ascend_python_bytestream_read_connector.py
+-rw-r--r--   0        0        0     4848 2023-04-24 18:04:53.673318 ascend_io_test-0.9.4/ascend_io_test/framework/ascend_python_read_connector.py
+-rw-r--r--   0        0        0     1091 2023-04-24 18:04:53.673318 ascend_io_test-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     5361 1970-01-01 00:00:00.000000 ascend_io_test-0.9.4/setup.py
+-rw-r--r--   0        0        0     5725 1970-01-01 00:00:00.000000 ascend_io_test-0.9.4/PKG-INFO
```

### Comparing `ascend_io_test-0.9.3/LICENSE` & `ascend_io_test-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ascend_io_test-0.9.3/README.rst` & `ascend_io_test-0.9.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 
 This package helps developers who are writing custom python for Ascend.io automated pipelines by providing a local
 testing framework. Local testing speeds the development of python pipeline code. The local framework exercises the
 code as if the code was running directly in the platform while giving you access to patching and mocking frameworks.
 
 Documentation, including examples, is located in our `Ascend Developer Hub <https://developer.ascend.io>`_.
 
+Release Notes
+-------------
+
+-------------
+0.9.4
+-------------
+* Add ``skip_read_bytes`` to ``AscendPythonReadConnector`` so tests can skip reading data
+
+
+Example
+------------
 Here is a basic python transformation test case example. The python code under test is located in a file
 with the name ``my_python_transform.py`` and imported with the name ``my_python_transform``. Other variables,
 imports, and code are omitted for brevity::
 
     @AscendPySparkTransform(spark=spark_session,
                             module=my_python_transform,
                             schema=input_schema,
@@ -65,13 +76,14 @@
 
 Write some tests. When your test cases are complete, pushing the code to the platform is simple with
 the `CLI <https://pypi.org/project/ascend-io-cli/>`_. For example::
 
     ascend apply data-flow MY_DATASERVICE MY_DATA_FLOW
 
 
+
 ---------------
 Read the Docs
 ---------------
 * `Ascend Developer Hub <https://developer.ascend.io>`_
 * `Ascend.io <https://www.ascend.io>`_
 * `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_
```

### Comparing `ascend_io_test-0.9.3/ascend_io_test/framework/ascend_pyspark_transform.py` & `ascend_io_test-0.9.4/ascend_io_test/framework/ascend_pyspark_transform.py`

 * *Files identical despite different names*

### Comparing `ascend_io_test-0.9.3/ascend_io_test/framework/ascend_python_bytestream_read_connector.py` & `ascend_io_test-0.9.4/ascend_io_test/framework/ascend_python_bytestream_read_connector.py`

 * *Files identical despite different names*

### Comparing `ascend_io_test-0.9.3/ascend_io_test/framework/ascend_python_read_connector.py` & `ascend_io_test-0.9.4/ascend_io_test/framework/ascend_python_read_connector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 import inspect
 import logging
 from datetime import datetime
 from typing import Any, Optional, Dict
+from collections import deque
 
 import pytest as pytest
 
 __all__ = ['AscendPythonReadConnector']
 
 
 def _get_method(module, name):
@@ -23,95 +24,99 @@
 
   return result
 
 
 class MetadataSupport:
   def __init__(self,
                name,
-               is_prefix,
                fingerprint,
-               last_modified=None,
-               byte_count=0,
-               record_count=0,
-               details=None,
-               version: int = 0,
+               is_prefix,
                ):
-    if details is None:
-      details = dict()
     self.name: str = name
-    self.is_prefix: bool = is_prefix
     self.fingerprint: str = fingerprint
-    self.last_modified: Optional[datetime] = last_modified
-    self.byte_count: Optional[int] = byte_count
-    self.record_count: Optional[int] = record_count
-    self.details: Optional[Dict[str, Any]] = details
-    self.version: int = version
+    self.is_prefix: bool = is_prefix
 
   def to_dict(self):
     return dict((k, v) for k, v in self.__dict__.items() if v is not None)
 
 
 class AscendPythonReadConnector:
   """This decorator automates the testing of read connectors by wrapping the read connector module
   in code that operates as if it was running in the platform"""
 
   def __init__(self,
                module=None,
                credentials=None,
                name=None,
                patches=None,
+               skip_read_bytes=False,
                ):
     if patches is None:
       patches = []
     self.credentials = credentials
     self.module = module
     self.name = name
     self.def_context = _get_method(module, 'context')
     self.def_list_objects = _get_method(module, 'list_objects')
     self.def_read_bytes = _get_method(module, 'read_bytes')
     self.def_read_spark_dataframe = _get_method(module, 'read_spark_dataframe')
     self.def_read_pandas_dataframe = _get_method(module, 'read_pandas_dataframe')
     self.patches = patches
+    self.skip_read_bytes = skip_read_bytes
 
     # inject pytest fixtures if they were applied to the global method
     caller_globals = inspect.stack()[1][0].f_globals
     caller_globals['context_result'] = _result_fixture('function', None)
     caller_globals['list_objects_result'] = _result_fixture('function', None)
     caller_globals['read_bytes_result'] = _result_fixture('function', None)
     caller_globals['mock_results'] = _result_fixture('function', None)
 
+  def __process_list_objects(self, context, metadata):
+        depth = 0
+        queue = deque([(context, metadata, depth)])
+        results = []
+
+        while queue:
+            current_context, current_metadata, current_depth = queue.popleft()
+            for item in self.def_list_objects(current_context, current_metadata):
+                logging.debug('partition level: %s meta: %s', current_depth, item)
+                results.append(item)
+                if item["is_prefix"]:
+                    queue.append((current_context, item, current_depth + 1))
+
+        return results
+
   def __call__(self, func):
     @functools.wraps(func)
     def wrapper(*args: Any, **kwargs: Any):
       logging.debug('calling the wrapper')
 
       # patch as requested
       patched = [m.start() for m in self.patches]
       context_result = self.def_context(self.credentials)
       context_result = context_result if context_result else {}
 
-      # TODO: implement some meaningful metadata
-      if self.name:
-        context_result['name'] = self.name
-      list_objects_result = [o for o in self.def_list_objects(context_result, {})]
+      # get the list objects/partitions
+      list_objects_result = [o for o in self.__process_list_objects(context_result, {})]
 
       read_bytes_result = []
-      for result in list_objects_result:
-        if self.def_read_bytes:
-          assert not self.def_read_spark_dataframe
-          assert not self.def_read_pandas_dataframe
-          read_bytes_result = (list(b for b in self.def_read_bytes(context_result, MetadataSupport(**result).to_dict())))
-        elif self.def_read_spark_dataframe:
-          assert not self.def_read_bytes
-          assert not self.def_read_pandas_dataframe
-          read_bytes_result = self.def_read_spark_dataframe(context_result, MetadataSupport(**result).to_dict())
-        elif self.def_read_pandas_dataframe:
-          assert not self.def_read_bytes
-          assert not self.def_read_spark_dataframe
-          read_bytes_result = self.def_read_pandas_dataframe(context_result, MetadataSupport(**result).to_dict())
+      if not self.skip_read_bytes:
+        for result in list_objects_result:
+          if self.def_read_bytes:
+            assert not self.def_read_spark_dataframe
+            assert not self.def_read_pandas_dataframe
+            read_bytes_result = (list(b for b in self.def_read_bytes(context_result, MetadataSupport(**result).to_dict())))
+          elif self.def_read_spark_dataframe:
+            assert not self.def_read_bytes
+            assert not self.def_read_pandas_dataframe
+            read_bytes_result = self.def_read_spark_dataframe(context_result, MetadataSupport(**result).to_dict())
+          elif self.def_read_pandas_dataframe:
+            assert not self.def_read_bytes
+            assert not self.def_read_spark_dataframe
+            read_bytes_result = self.def_read_pandas_dataframe(context_result, MetadataSupport(**result).to_dict())
 
       logging.debug('read connector interface calls complete')
       # write the data back to the test method for assertion
       full_args = inspect.getfullargspec(func)
       if 'context_result' in full_args.args:
         kwargs['context_result'] = context_result
       if 'list_objects_result' in full_args.args:
```

### Comparing `ascend_io_test-0.9.3/pyproject.toml` & `ascend_io_test-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ascend-io-test"
-version = "0.9.3"
+version = "0.9.4"
 description = "The Ascend Python Test Framework"
 license = "Apache-2.0"
 authors = ["Ascend.io Engineering <support@ascend.io>"]
 maintainers = ["Ascend.io Engineering <support@ascend.io>"]
 readme = "README.rst"
 homepage = "https://www.ascend.io"
 documentation = "https://developer.ascend.io"
```

### Comparing `ascend_io_test-0.9.3/setup.py` & `ascend_io_test-0.9.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pyspark>=3.3.1,<4.0.0', 'pytest-mock>=3.10.0,<4.0.0', 'pytest>=7.2.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'ascend-io-test',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'The Ascend Python Test Framework',
-    'long_description': '========================\nAscend.io Test Framework\n========================\n\nThis package helps developers who are writing custom python for Ascend.io automated pipelines by providing a local\ntesting framework. Local testing speeds the development of python pipeline code. The local framework exercises the\ncode as if the code was running directly in the platform while giving you access to patching and mocking frameworks.\n\nDocumentation, including examples, is located in our `Ascend Developer Hub <https://developer.ascend.io>`_.\n\nHere is a basic python transformation test case example. The python code under test is located in a file\nwith the name ``my_python_transform.py`` and imported with the name ``my_python_transform``. Other variables,\nimports, and code are omitted for brevity::\n\n    @AscendPySparkTransform(spark=spark_session,\n                            module=my_python_transform,\n                            schema=input_schema,\n                            data=[(123, \'NORMAL\', today, today + datetime.timedelta(days=1))],\n                            credentials=test_creds,\n                            discover_schema=True,\n                            patches=[patch(\'requests.post\', return_value=Mock(status_code=200,\n                                                                              text=\'{"internalReportIds":"REPORT_A"}\')),\n                                     patch(\'requests.get\', return_value=Mock(status_code=200,\n                                                                             text=\'{"status":"SUCCESS", "downloadLink": "https://test.my.download"}\')),\n                                     patch(\'pandas.read_csv\', return_value=build_mock_csv()),\n                                     ], )\n    def test_normal_loading_process_single_record(input_dataframe, transform_result: DataFrame, mock_results: List[Mock]):\n      """Check that a normal call does the work properly.\n            Assert values are correct.\n            Assert mock services are called."""\n      assert input_dataframe\n      assert transform_result\n      assert transform_result.count() == 3\n      dataset = transform_result.collect()\n      # check field mapping\n      assert dataset[0][\'CUSTOMER_ID\'] == \'101\'\n      assert dataset[1][\'CUSTOMER_ID\'] == \'102\'\n      assert dataset[2][\'CUSTOMER_ID\'] == \'103\'\n      assert dataset[0][\'YOUR_NAME\'] == "customerName.one"\n      assert dataset[0][\'THE_OBJECTIVE\'] == "customerBudget.one"\n      assert dataset[0][\'AD_ID\'] == "tempId.one"\n      assert dataset[0][\'AD_NAME\'] == "myName.one"\n      assert dataset[0][\'GEO_LOC\'] == "geo_location.one"\n      assert dataset[0][\'ORDER_ID\'] == "orderId.test"\n      assert dataset[0][\'ORDER_NAME\'] == "orderName.test"\n      assert dataset[0][\'DT\'] == "__time.one"\n      assert dataset[0][\'AUDIO_IMPRESSIONS\'] == 1\n      assert transform_result.columns.__contains__(\'RUN_ID\')\n      assert transform_result.columns.__contains__(\'REPORT_START_DT\')\n      assert transform_result.columns.__contains__(\'REPORT_END_DT\')\n      assert transform_result.columns.__contains__(\'record_number\')\n      # check mocks were properly called\n      mock_results[0].assert_called_once()\n      mock_results[1].assert_called_once_with(f"https://custom.io/v1/async-query/REPORT_A",\n                                              headers={\'agency\': \'12\', \'x-api-key\': \'key\', \'Content-Type\': \'application/json\'})\n      mock_results[2].assert_called_once_with("https://test.my.download", header=0, skip_blank_lines=True)\n\n\nDecorators are available for all types of Ascend python implementation strategies. Testing scenarios are only limited\nby your creativity and desire to produce high quality code.\n\nDownload your pipelines using the `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_ like this::\n\n    ascend download data-flow MY_DATASERVICE MY_DATA_FLOW\n\nWrite some tests. When your test cases are complete, pushing the code to the platform is simple with\nthe `CLI <https://pypi.org/project/ascend-io-cli/>`_. For example::\n\n    ascend apply data-flow MY_DATASERVICE MY_DATA_FLOW\n\n\n---------------\nRead the Docs\n---------------\n* `Ascend Developer Hub <https://developer.ascend.io>`_\n* `Ascend.io <https://www.ascend.io>`_\n* `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_\n',
+    'long_description': '========================\nAscend.io Test Framework\n========================\n\nThis package helps developers who are writing custom python for Ascend.io automated pipelines by providing a local\ntesting framework. Local testing speeds the development of python pipeline code. The local framework exercises the\ncode as if the code was running directly in the platform while giving you access to patching and mocking frameworks.\n\nDocumentation, including examples, is located in our `Ascend Developer Hub <https://developer.ascend.io>`_.\n\nRelease Notes\n-------------\n\n-------------\n0.9.4\n-------------\n* Add ``skip_read_bytes`` to ``AscendPythonReadConnector`` so tests can skip reading data\n\n\nExample\n------------\nHere is a basic python transformation test case example. The python code under test is located in a file\nwith the name ``my_python_transform.py`` and imported with the name ``my_python_transform``. Other variables,\nimports, and code are omitted for brevity::\n\n    @AscendPySparkTransform(spark=spark_session,\n                            module=my_python_transform,\n                            schema=input_schema,\n                            data=[(123, \'NORMAL\', today, today + datetime.timedelta(days=1))],\n                            credentials=test_creds,\n                            discover_schema=True,\n                            patches=[patch(\'requests.post\', return_value=Mock(status_code=200,\n                                                                              text=\'{"internalReportIds":"REPORT_A"}\')),\n                                     patch(\'requests.get\', return_value=Mock(status_code=200,\n                                                                             text=\'{"status":"SUCCESS", "downloadLink": "https://test.my.download"}\')),\n                                     patch(\'pandas.read_csv\', return_value=build_mock_csv()),\n                                     ], )\n    def test_normal_loading_process_single_record(input_dataframe, transform_result: DataFrame, mock_results: List[Mock]):\n      """Check that a normal call does the work properly.\n            Assert values are correct.\n            Assert mock services are called."""\n      assert input_dataframe\n      assert transform_result\n      assert transform_result.count() == 3\n      dataset = transform_result.collect()\n      # check field mapping\n      assert dataset[0][\'CUSTOMER_ID\'] == \'101\'\n      assert dataset[1][\'CUSTOMER_ID\'] == \'102\'\n      assert dataset[2][\'CUSTOMER_ID\'] == \'103\'\n      assert dataset[0][\'YOUR_NAME\'] == "customerName.one"\n      assert dataset[0][\'THE_OBJECTIVE\'] == "customerBudget.one"\n      assert dataset[0][\'AD_ID\'] == "tempId.one"\n      assert dataset[0][\'AD_NAME\'] == "myName.one"\n      assert dataset[0][\'GEO_LOC\'] == "geo_location.one"\n      assert dataset[0][\'ORDER_ID\'] == "orderId.test"\n      assert dataset[0][\'ORDER_NAME\'] == "orderName.test"\n      assert dataset[0][\'DT\'] == "__time.one"\n      assert dataset[0][\'AUDIO_IMPRESSIONS\'] == 1\n      assert transform_result.columns.__contains__(\'RUN_ID\')\n      assert transform_result.columns.__contains__(\'REPORT_START_DT\')\n      assert transform_result.columns.__contains__(\'REPORT_END_DT\')\n      assert transform_result.columns.__contains__(\'record_number\')\n      # check mocks were properly called\n      mock_results[0].assert_called_once()\n      mock_results[1].assert_called_once_with(f"https://custom.io/v1/async-query/REPORT_A",\n                                              headers={\'agency\': \'12\', \'x-api-key\': \'key\', \'Content-Type\': \'application/json\'})\n      mock_results[2].assert_called_once_with("https://test.my.download", header=0, skip_blank_lines=True)\n\n\nDecorators are available for all types of Ascend python implementation strategies. Testing scenarios are only limited\nby your creativity and desire to produce high quality code.\n\nDownload your pipelines using the `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_ like this::\n\n    ascend download data-flow MY_DATASERVICE MY_DATA_FLOW\n\nWrite some tests. When your test cases are complete, pushing the code to the platform is simple with\nthe `CLI <https://pypi.org/project/ascend-io-cli/>`_. For example::\n\n    ascend apply data-flow MY_DATASERVICE MY_DATA_FLOW\n\n\n\n---------------\nRead the Docs\n---------------\n* `Ascend Developer Hub <https://developer.ascend.io>`_\n* `Ascend.io <https://www.ascend.io>`_\n* `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_\n',
     'author': 'Ascend.io Engineering',
     'author_email': 'support@ascend.io',
     'maintainer': 'Ascend.io Engineering',
     'maintainer_email': 'support@ascend.io',
     'url': 'https://www.ascend.io',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ascend_io_test-0.9.3/PKG-INFO` & `ascend_io_test-0.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascend-io-test
-Version: 0.9.3
+Version: 0.9.4
 Summary: The Ascend Python Test Framework
 Home-page: https://www.ascend.io
 License: Apache-2.0
 Keywords: ascend,pipeline,data,automation,platform
 Author: Ascend.io Engineering
 Author-email: support@ascend.io
 Maintainer: Ascend.io Engineering
@@ -35,14 +35,25 @@
 
 This package helps developers who are writing custom python for Ascend.io automated pipelines by providing a local
 testing framework. Local testing speeds the development of python pipeline code. The local framework exercises the
 code as if the code was running directly in the platform while giving you access to patching and mocking frameworks.
 
 Documentation, including examples, is located in our `Ascend Developer Hub <https://developer.ascend.io>`_.
 
+Release Notes
+-------------
+
+-------------
+0.9.4
+-------------
+* Add ``skip_read_bytes`` to ``AscendPythonReadConnector`` so tests can skip reading data
+
+
+Example
+------------
 Here is a basic python transformation test case example. The python code under test is located in a file
 with the name ``my_python_transform.py`` and imported with the name ``my_python_transform``. Other variables,
 imports, and code are omitted for brevity::
 
     @AscendPySparkTransform(spark=spark_session,
                             module=my_python_transform,
                             schema=input_schema,
@@ -96,14 +107,15 @@
 
 Write some tests. When your test cases are complete, pushing the code to the platform is simple with
 the `CLI <https://pypi.org/project/ascend-io-cli/>`_. For example::
 
     ascend apply data-flow MY_DATASERVICE MY_DATA_FLOW
 
 
+
 ---------------
 Read the Docs
 ---------------
 * `Ascend Developer Hub <https://developer.ascend.io>`_
 * `Ascend.io <https://www.ascend.io>`_
 * `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_
```

