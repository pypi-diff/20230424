# Comparing `tmp/cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7.tar.gz` & `tmp/cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/newrelic-observability-dashboards/dist/python/cdk-cloud", last modified: Fri Feb  3 16:13:18 2023, max compression
+gzip compressed data, was "/__w/cdk-cloudformation/cdk-cloudformation/packages/@cdk-cloudformation/newrelic-observability-dashboards/dist/python/cdk-cloud", last modified: Mon Apr 24 06:13:08 2023, max compression
```

## Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7.tar` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/
--rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/LICENSE
--rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/MANIFEST.in
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3084 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)     2124 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/README.md
--rw-r--r--   0 superchain  (1001) superchain  (1001)      236 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/pyproject.toml
--rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/setup.cfg
--rw-r--r--   0 superchain  (1001) superchain  (1001)     1967 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/setup.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     9007 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/
--rw-r--r--   0 superchain  (1001) superchain  (1001)      482 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/__init__.py
--rw-r--r--   0 superchain  (1001) superchain  (1001)    17368 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.0.0-alpha.7.jsii.tgz
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:13:10.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/py.typed
-drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/
--rw-r--r--   0 superchain  (1001) superchain  (1001)     3084 2023-02-03 16:13:17.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 superchain  (1001) superchain  (1001)      782 2023-02-03 16:13:18.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-02-03 16:13:17.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-02-03 16:13:17.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/requires.txt
--rw-r--r--   0 superchain  (1001) superchain  (1001)       53 2023-02-03 16:13:17.000000 cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/top_level.txt
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    11358 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/LICENSE
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       23 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/MANIFEST.in
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3115 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2124 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/README.md
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      234 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/pyproject.toml
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       38 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/setup.cfg
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     2017 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/setup.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     9007 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      482 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/__init__.py
+-rw-r--r--   0 superchain  (1001) superchain  (1001)    17384 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.1.0-alpha.7.jsii.tgz
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-24 06:13:02.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/py.typed
+drwxr-xr-x   0 superchain  (1001) superchain  (1001)        0 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/
+-rw-r--r--   0 superchain  (1001) superchain  (1001)     3115 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      782 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)        1 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)      113 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/requires.txt
+-rw-r--r--   0 superchain  (1001) superchain  (1001)       53 2023-04-24 06:13:08.000000 cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/top_level.txt
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/LICENSE` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/PKG-INFO` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-newrelic-observability-dashboards
-Version: 1.0.0a7
+Version: 1.1.0a7
 Summary: CRUD operations for New Relic Dashboards via the NerdGraph API
 Home-page: https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -55,15 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/README.md` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -32,13 +32,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/setup.py` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-cloudformation-newrelic-observability-dashboards",
-    "version": "1.0.0.a7",
+    "version": "1.1.0.a7",
     "description": "CRUD operations for New Relic Dashboards via the NerdGraph API",
     "license": "Apache-2.0",
     "url": "https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_cloudformation_newrelic_observability_dashboards",
         "cdk_cloudformation_newrelic_observability_dashboards._jsii"
     ],
     "package_data": {
         "cdk_cloudformation_newrelic_observability_dashboards._jsii": [
-            "newrelic-observability-dashboards@1.0.0-alpha.7.jsii.tgz"
+            "newrelic-observability-dashboards@1.1.0-alpha.7.jsii.tgz"
         ],
         "cdk_cloudformation_newrelic_observability_dashboards": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.63.0, <3.0.0",
-        "constructs>=10.1.239, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "aws-cdk-lib>=2.72.1, <3.0.0",
+        "constructs>=10.1.302, <11.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -33,15 +33,15 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
 '''
 import abc
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cdk-cloudformation-newrelic-observability-dashboards
-Version: 1.0.0a7
+Version: 1.1.0a7
 Summary: CRUD operations for New Relic Dashboards via the NerdGraph API
 Home-page: https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cloudformation.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # newrelic-observability-dashboards
 
-> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.0.0.
+> AWS CDK [L1 construct](https://docs.aws.amazon.com/cdk/latest/guide/constructs.html) and data structures for the [AWS CloudFormation Registry](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry.html) type `NewRelic::Observability::Dashboards` v1.1.0.
 
 ## Description
 
 CRUD operations for New Relic Dashboards via the NerdGraph API
 
 ## References
 
@@ -55,15 +55,13 @@
 
 You can find more information about activating this type in the [AWS CloudFormation documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/registry-public.html).
 
 ## Feedback
 
 This library is auto-generated and published to all supported programming languages by the [cdklabs/cdk-cloudformation](https://github.com/cdklabs/cdk-cloudformation) project based on the API schema published for `NewRelic::Observability::Dashboards`.
 
-* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.0.0).
+* Issues related to this generated library should be [reported here](https://github.com/cdklabs/cdk-cloudformation/issues/new?title=Issue+with+%40cdk-cloudformation%2Fnewrelic-observability-dashboards+v1.1.0).
 * Issues related to `NewRelic::Observability::Dashboards` should be reported to the [publisher](https://github.com/newrelic-experimental/newrelic-cloudformation-resource-providers-dashboards).
 
 ## License
 
 Distributed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-cloudformation-newrelic-observability-dashboards-1.0.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt` & `cdk-cloudformation-newrelic-observability-dashboards-1.1.0a7/src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cdk_cloudformation_newrelic_observability_dashboards/py.typed
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/PKG-INFO
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/SOURCES.txt
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/dependency_links.txt
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/requires.txt
 src/cdk_cloudformation_newrelic_observability_dashboards.egg-info/top_level.txt
 src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/__init__.py
-src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.0.0-alpha.7.jsii.tgz
+src/cdk_cloudformation_newrelic_observability_dashboards/_jsii/newrelic-observability-dashboards@1.1.0-alpha.7.jsii.tgz
```

