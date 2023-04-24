# Comparing `tmp/aws_cfn_custom_resource_resolve_parser-0.2.1.tar.gz` & `tmp/aws_cfn_custom_resource_resolve_parser-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cfn_custom_resource_resolve_parser-0.2.1.tar", max compression
+gzip compressed data, was "aws_cfn_custom_resource_resolve_parser-0.2.2.tar", max compression
```

## Comparing `aws_cfn_custom_resource_resolve_parser-0.2.1.tar` & `aws_cfn_custom_resource_resolve_parser-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    16725 2021-04-04 09:27:49.733701 aws_cfn_custom_resource_resolve_parser-0.2.1/LICENSE
--rw-r--r--   0        0        0     1934 2021-04-04 08:02:22.355747 aws_cfn_custom_resource_resolve_parser-0.2.1/README.rst
--rw-r--r--   0        0        0     4510 2021-08-19 08:39:32.289061 aws_cfn_custom_resource_resolve_parser-0.2.1/aws_cfn_custom_resource_resolve_parser/__init__.py
--rw-r--r--   0        0        0     1851 2021-08-19 08:39:32.290061 aws_cfn_custom_resource_resolve_parser-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2676 2021-08-19 08:39:43.255594 aws_cfn_custom_resource_resolve_parser-0.2.1/setup.py
--rw-r--r--   0        0        0     2857 2021-08-19 08:39:43.255898 aws_cfn_custom_resource_resolve_parser-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-04-24 10:02:59.281226 aws_cfn_custom_resource_resolve_parser-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1934 2023-04-24 10:02:59.282226 aws_cfn_custom_resource_resolve_parser-0.2.2/README.rst
+-rw-r--r--   0        0        0     4347 2023-04-24 10:15:33.641432 aws_cfn_custom_resource_resolve_parser-0.2.2/aws_cfn_custom_resource_resolve_parser/__init__.py
+-rw-r--r--   0        0        0     1808 2023-04-24 10:15:33.641432 aws_cfn_custom_resource_resolve_parser-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 aws_cfn_custom_resource_resolve_parser-0.2.2/setup.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 aws_cfn_custom_resource_resolve_parser-0.2.2/PKG-INFO
```

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.1/LICENSE` & `aws_cfn_custom_resource_resolve_parser-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.1/README.rst` & `aws_cfn_custom_resource_resolve_parser-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.1/aws_cfn_custom_resource_resolve_parser/__init__.py` & `aws_cfn_custom_resource_resolve_parser-0.2.2/aws_cfn_custom_resource_resolve_parser/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import re
 
 from boto3.session import Session
 from botocore.exceptions import ClientError
 
 __author__ = """John Preston"""
 __email__ = "john@ews-network.net"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 
 SECRET_ARN_REGEXP = re.compile(
     r"(?:{{resolve:secretsmanager:)"
     r"(?P<arn>arn:(?P<partition>aws(?:-[a-z]+)?):secretsmanager:(?P<region>[a-z0-9-]+):"
     r"(?P<account_id>\d{12}):"
     r"(?:secret:(?P<secret_id>[a-z0-9A-Z-_./]+)))"
@@ -60,14 +60,15 @@
     """
     Function to parse the resolve string and return the parts of it of interest
 
     :param str resolve_str:
     :return: tuple of the secret, key and stage.
     :rtype: tuple
     """
+    secret = None
     key = None
     stage = None
     if SECRET_ARN_REGEXP.match(resolve_str):
         parts = SECRET_ARN_REGEXP.match(resolve_str)
         secret = parts.group("arn")
         if not secret:
             raise ValueError("Unable to find the secret ARN in", resolve_str)
@@ -83,31 +84,33 @@
     if parts:
         key = parts.group("secret_key")
         stage = parts.group("version")
 
     return secret, key, stage
 
 
-def retrieve_secret(secret, key=None, stage=None, session=None):
+def retrieve_secret(secret, key=None, stage=None, client=None, session=None):
     """
     Function to retrieve the secret. If key is provided, attempts to return only the key value.
     If stage is provided, retrieves the secret for given stage.
 
     :param str secret:
     :param str key:
     :param str stage:
+    :param boto3.client client:
     :param boto3.session.Session session:
     :return: The secret string or specific key of
     :raises: KeyError  if the key is provided but not present in secret
     :raises: ClientError in case of an error with boto3
     :raises: ResourceNotFoundException,ResourceNotFoundException if specific issue with secret retrieval
     """
-    if session is None:
-        session = Session()
-    client = session.client("secretsmanager")
+    if not client and session:
+        client = session.client("secretsmanager")
+    elif not client and not session:
+        client = Session().client("secretsmanager")
     try:
         get_secret_value_response = client.get_secret_value(
             SecretId=secret, VersionStage="AWSCURRENT" if not stage else stage
         )
         if keyisset("SecretString", get_secret_value_response):
             res = json.loads(get_secret_value_response["SecretString"])
         else:
@@ -115,33 +118,25 @@
                 base64.b64decode(get_secret_value_response["SecretBinary"])
             )
         if key and keypresent(key, res):
             return res[key]
         elif key and not keypresent(key, res):
             raise KeyError(f"Secret {secret} does not have a key {key}")
         return res
-    except (
-        client.exceptions.DecryptionFailure,
-        client.exceptions.ResourceNotFoundException,
-        client.exceptions.InvalidParameterException,
-        client.exceptions.ResourceNotFoundException,
-    ) as error:
+    except client.exceptions as error:
         print(error)
         raise
     except ClientError as error:
         print(error)
         raise
 
 
-def handle(resolve_str, session=None):
+def handle(resolve_str):
     """
     Main function.
 
     :param resolve_str:
-    :param boto3.session.Session session:
     :return:
     """
     parts = parse_secret_resolve_string(resolve_str)
-    secret = retrieve_secret(
-        secret=parts[0], key=parts[1], stage=parts[2], session=session
-    )
+    secret = retrieve_secret(parts[0], parts[1], parts[2])
     return secret
```

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.1/pyproject.toml` & `aws_cfn_custom_resource_resolve_parser-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 [tool.poetry]
 name = "aws_cfn_custom_resource_resolve_parser"
-version = "0.2.1"
+version = "0.2.2"
 description = "AWS CFN Custom Resource parser for dynamic values"
 authors = ["John Preston <john@ews-network.net>"]
 license = "MPL-2.0"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9"
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10"
 ]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-boto3 = "^1.18.0"
+python = "^3.8"
+boto3 = "^1.26"
 
-[tool.poetry.dev-dependencies]
-black = "^21.7b0"
-isort = "^5.9.3"
-placebo = "^0.9.0"
-pytest = "^6.2.4"
-coverage = "^5.5"
-Sphinx = "^4.1.0"
-sphinx-material = "^0.0.34"
-pre-commit = "^2.14.0"
-tbump = "^6.3.1"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+isort = "^5.12.0"
+placebo = "^0.10.0"
+pytest = "^7.3.1"
+coverage = "^7.2.3"
+Sphinx = "^6.2.0"
+sphinx-material = "^0.0.35"
+pre-commit = "^3.2.2"
+tbump = "^6.9.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
@@ -50,23 +49,23 @@
 known_first_party = "kelvin"
 
 
 [tool.tbump]
 github_url = "https://github.com/EWS-Network/aws_cfn_custom_resource_resolve_parser"
 
 [tool.tbump.version]
-current = "0.2.1"
+current = "0.2.2"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
-  (?:[-.](?P<rc>[\S]+))?
+  (?:(?P<rc>[\S]+))?
   '''
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
```

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.1/setup.py` & `aws_cfn_custom_resource_resolve_parser-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['aws_cfn_custom_resource_resolve_parser']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.18.0,<2.0.0']
+['boto3>=1.26,<2.0']
 
 setup_kwargs = {
     'name': 'aws-cfn-custom-resource-resolve-parser',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'AWS CFN Custom Resource parser for dynamic values',
     'long_description': '======================================\nAWS CFN Custom resource Resolve parser\n======================================\n\n\n.. image:: https://img.shields.io/pypi/v/aws_cfn_custom_resource_resolve_parser.svg\n        :target: https://pypi.python.org/pypi/aws_cfn_custom_resource_resolve_parser\n\n.. image:: https://readthedocs.org/projects/aws-cfn-custom-resource-resolve-parser/badge/?version=latest\n        :target: https://aws-cfn-custom-resource-resolve-parser.readthedocs.io/en/latest/?version=latest\n        :alt: Documentation Status\n\n\n----------------------------------------------------------------------------------------------------\nSmall lib to parse and retrieve secret from AWS Secrets manager using the CFN resolve format string\n----------------------------------------------------------------------------------------------------\n\nIntent\n=======\n\nCurrently in AWS CloudFormation, using **{{resolve}}** does not work for custom resources. Pending the feature being\nreleased, when the use of private resource types is not possible for the use-case, this small lib aims to allow\nparsing secrets so that you can today write your CFN templates with resolve.\n\nRequirements\n=============\n\nSadly, this means the lambda function using this library will still need IAM access directly, and cannot use the role\nused by CloudFormation on create/update currently.\n\nUsage\n=======\n\n.. code-block:: python\n\n    from aws_cfn_custom_resource_resolve_parser import handle\n    secret_string = r"{{resolve:secretsmanager:mysecret:SecretString:password}}"\n    secret_value = handle(secret_string)\n\n\n* Documentation: https://aws-cfn-custom-resource-resolve-parser.readthedocs.io.\n\nCredits\n-------\n\nThis package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage\n',
     'author': 'John Preston',
     'author_email': 'john@ews-network.net',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `aws_cfn_custom_resource_resolve_parser-0.2.1/PKG-INFO` & `aws_cfn_custom_resource_resolve_parser-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: aws-cfn-custom-resource-resolve-parser
-Version: 0.2.1
+Version: 0.2.2
 Summary: AWS CFN Custom Resource parser for dynamic values
 License: MPL-2.0
 Author: John Preston
 Author-email: john@ews-network.net
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: boto3 (>=1.18.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: boto3 (>=1.26,<2.0)
 Description-Content-Type: text/x-rst
 
 ======================================
 AWS CFN Custom resource Resolve parser
 ======================================
```

