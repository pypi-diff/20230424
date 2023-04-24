# Comparing `tmp/cloud-radar-0.6.3.tar.gz` & `tmp/cloud_radar-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-radar-0.6.3.tar", max compression
+gzip compressed data, was "cloud_radar-0.6.4.tar", max compression
```

## Comparing `cloud-radar-0.6.3.tar` & `cloud_radar-0.6.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11357 2022-10-02 09:43:03.219390 cloud-radar-0.6.3/LICENSE.txt
--rw-r--r--   0        0        0    12781 2022-10-02 09:43:03.219390 cloud-radar-0.6.3/README.md
--rw-r--r--   0        0        0     1449 2022-10-02 09:43:11.763454 cloud-radar-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-02 09:43:03.223390 cloud-radar-0.6.3/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2022-10-02 09:43:03.223390 cloud-radar-0.6.3/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2022-10-02 09:43:03.223390 cloud-radar-0.6.3/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2022-10-02 09:43:03.223390 cloud-radar-0.6.3/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2022-10-02 09:43:03.223390 cloud-radar-0.6.3/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0     7924 2022-10-02 09:43:03.223390 cloud-radar-0.6.3/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    23903 2022-10-02 09:43:03.223390 cloud-radar-0.6.3/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    13974 1970-01-01 00:00:00.000000 cloud-radar-0.6.3/setup.py
--rw-r--r--   0        0        0    13930 1970-01-01 00:00:00.000000 cloud-radar-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/LICENSE.txt
+-rw-r--r--   0        0        0    12792 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/README.md
+-rw-r--r--   0        0        0     1431 2023-04-24 00:45:28.601597 cloud_radar-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0     8886 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24195 2023-04-24 00:45:18.349485 cloud_radar-0.6.4/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    13992 1970-01-01 00:00:00.000000 cloud_radar-0.6.4/PKG-INFO
```

### Comparing `cloud-radar-0.6.3/LICENSE.txt` & `cloud_radar-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud-radar-0.6.3/README.md` & `cloud_radar-0.6.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 * [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [python-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-the-badge
 [version-shield]: https://img.shields.io/pypi/v/cloud-radar?label=latest&style=for-the-badge
 [pypi-url]: https://pypi.org/project/cloud-radar/
-[test-shield]: https://img.shields.io/github/workflow/status/DontShaveTheYak/cloud-radar/Tests?label=Tests&style=for-the-badge
+[test-shield]: https://img.shields.io/github/actions/workflow/status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-badge
 [test-url]: https://github.com/DontShaveTheYak/cloud-radar/actions?query=workflow%3ATests+branch%3Amaster
 [codecov-shield]: https://img.shields.io/codecov/c/gh/DontShaveTheYak/cloud-radar?color=green&style=for-the-badge&token=NE5C92139X
 [codecov-url]: https://codecov.io/gh/DontShaveTheYak/cloud-radar
 [contributors-shield]: https://img.shields.io/github/contributors/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
 [contributors-url]: https://github.com/DontShaveTheYak/cloud-radar/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
 [forks-url]: https://github.com/DontShaveTheYak/cloud-radar/network/members
```

### Comparing `cloud-radar-0.6.3/pyproject.toml` & `cloud_radar-0.6.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.6.3"
+version = "0.6.4"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
@@ -21,24 +21,23 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 taskcat = "^0.9.20"
 cfn-flip = "^1.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
-coverage = {extras = ["toml"], version = "^6.4"}
+coverage = {extras = ["toml"], version = "^7.0.0"}
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.6.1"
-black = "^22.1.0"
+black = "^23.0.0"
 flake8 = "^5.0.0"
 flake8-black = "^0.3.0"
 flake8-import-order = "^0.18.1"
-flake8-bugbear = "^22.0.0"
-mypy = "^0.981"
-codecov = "^2.1.10"
+flake8-bugbear = "^23.0.0"
+mypy = "^1.0.0"
 types-requests = "^2.28.11"
 types-PyYAML = "^6.0.12"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.run]
```

### Comparing `cloud-radar-0.6.3/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.6.4/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud-radar-0.6.3/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.6.4/src/cloud_radar/cf/unit/_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         tmp_str = dump_yaml(tmp_yaml)
 
         template = yaml.load(tmp_str, Loader=yaml.FullLoader)
 
         return cls(template, imports)
 
     def render(
-        self, params: Dict[str, str] = None, region: Union[str, None] = None
+        self, params: Optional[Dict[str, str]] = None, region: Optional[str] = None
     ) -> dict:
         """Solves all conditionals, references and pseudo variables using
         the passed in parameters. After rendering the template all resources
         that wouldn't get deployed because of a condtion statement are removed.
 
         Args:
             params (dict, optional): Parameter names and values to be used when rendering.
@@ -103,85 +103,96 @@
             self.Region = region
 
         self.template = yaml.load(self.raw, Loader=yaml.FullLoader)
         self.set_parameters(params)
 
         add_metadata(self.template, self.Region)
 
-        if "Conditions" in self.template:
-            self.template["Conditions"] = self.resolve_values(
-                self.template["Conditions"], functions.CONDITIONS, solve_conditions=True
-            )
-
         self.resolve_values(
-            self.template, functions.ALL_FUNCTIONS, solve_conditions=False
+            self.template,
+            functions.ALL_FUNCTIONS,
         )
 
         resources = self.template["Resources"]
         for r_name, r_value in list(resources.items()):
-
             if "Condition" not in r_value:
                 continue
 
             keep_resource = r_value["Condition"]
 
             if not keep_resource:
                 del self.template["Resources"][r_name]
                 continue
 
         return self.template
 
     def resolve_values(
-        self, data: Any, allowed_func: functions.Dispatch, solve_conditions=False
+        self,
+        data: Any,
+        allowed_func: functions.Dispatch,
     ) -> Any:
         """Recurses through a Cloudformation template. Solving all
         references and variables along the way.
 
         Args:
             data (Any): Could be a dict, list, str or int.
 
         Returns:
             Any: Return the rendered data structure.
         """
 
         if isinstance(data, dict):
             for key, value in data.items():
-
                 if key == "Ref":
                     return functions.ref(self, value)
 
+                # This takes care of keys that not intrinsic functions,
+                #  except for the condition func
+                if "Fn::" not in key and key != "Condition":
+                    data[key] = self.resolve_values(
+                        value,
+                        allowed_func,
+                    )
+                    continue
+
+                # Takes care of the tricky 'Condition' key
                 if key == "Condition":
+                    # This takes care of conditional resources
+                    if "Properties" in data:
+                        data[key] = functions.condition(self, value)
+                        continue
 
-                    if solve_conditions:
+                    # If it's an intrinsic func
+                    if is_condition_func(value):
                         return functions.condition(self, value)
 
-                    data[key] = functions.condition(self, value)
-                    continue
-
-                if "Fn::" not in key:
+                    # Normal key like in an IAM role
                     data[key] = self.resolve_values(
-                        value, allowed_func, solve_conditions
+                        value,
+                        allowed_func,
                     )
                     continue
 
                 if key not in allowed_func:
                     raise ValueError(f"{key} with value ({value}) not allowed here")
 
                 value = self.resolve_values(
                     value,
                     functions.ALLOWED_FUNCTIONS[key],
-                    solve_conditions,
                 )
 
                 return allowed_func[key](self, value)
 
             return data
         elif isinstance(data, list):
             return [
-                self.resolve_values(item, allowed_func, solve_conditions)
+                self.resolve_values(
+                    item,
+                    allowed_func,
+                )
                 for item in data
             ]
         else:
             return data
 
     def set_parameters(self, parameters: Union[Dict[str, str], None] = None) -> None:
         """Sets the parameters for a template using the provided parameters or
@@ -236,7 +247,25 @@
 
     metadata = {"Cloud-Radar": {"Region": region}}
 
     if "Metadata" not in template:
         template["Metadata"] = {}
 
     template["Metadata"].update(metadata)
+
+
+# All the other Cloudformation intrinsic functions start with `Fn:` but for some reason
+# the Condition function does not. This can be problem because
+#  `Condition` is a valid key in an IAM policy but its value is always a Map.
+def is_condition_func(value: Any) -> bool:
+    """Checks if the 'Condition' key is a instrinsic function.
+
+    Args:
+        value (Any): The value of the 'Condition' key.
+
+    Returns:
+        bool: True if we think this `Condition` key is an instrinsic function.
+    """
+    if isinstance(value, str):
+        return True
+
+    return False
```

### Comparing `cloud-radar-0.6.3/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.6.4/src/cloud_radar/cf/unit/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     if not isinstance(name, str):
         raise TypeError(
             f"Fn::Condition - The value must be a String, not {type(name).__name__}."
         )
 
     if name not in template.template["Conditions"]:
         raise KeyError(
-            f"Fn::Condition - Unable to find condition '{name}' in template."
+            f"Fn::Condition - Unable to find condition {name!r} in template."
         )
 
     condition_value = template.template["Conditions"][name]
 
     if not isinstance(condition_value, bool):
         condition_value: bool = template.resolve_values(  # type: ignore
             condition_value, allowed_func=ALLOWED_NESTED_CONDITIONS
@@ -714,19 +714,20 @@
         # we don't want to update the class var for every run.
         if pseudo == "Region":
             return template.template["Metadata"]["Cloud-Radar"]["Region"]
         try:
             return getattr(template, pseudo)
         except AttributeError:
             raise ValueError(
-                f"Unrecognized AWS Pseduo variable: '{var_name}'."
+                f"Unrecognized AWS Pseduo variable: {var_name!r}."
             ) from None
 
-    if var_name in template.template["Parameters"]:
-        return template.template["Parameters"][var_name]["Value"]
+    if "Parameters" in template.template:
+        if var_name in template.template["Parameters"]:
+            return template.template["Parameters"][var_name]["Value"]
 
     if var_name in template.template["Resources"]:
         return var_name
 
     raise Exception(f"Fn::Ref - {var_name} is not a valid Resource or Parameter.")
 
 
@@ -804,17 +805,20 @@
 
 ALLOWED_NESTED_CONDITIONS: Dispatch = {
     "Fn::FindInMap": find_in_map,
     "Ref": ref,
     **CONDITIONS,
 }
 
+# Cloudformation only allows certain functions to be called from inside
+# other functions. The keys are the function name and the values are the
+# functions that are allowed to be nested inside it.
 ALLOWED_FUNCTIONS: Dict[str, Dispatch] = {
     "Fn::And": ALLOWED_NESTED_CONDITIONS,
-    "Fn::Equals": ALLOWED_NESTED_CONDITIONS,
+    "Fn::Equals": {**ALLOWED_NESTED_CONDITIONS, "Fn::Join": join, "Fn::Select": select},
     "Fn::If": {
         "Fn::Base64": base64,
         "Fn::FindInMap": find_in_map,
         "Fn::GetAtt": get_att,
         "Fn::GetAZs": get_azs,
         "Fn::If": if_,
         "Fn::Join": join,
```

### Comparing `cloud-radar-0.6.3/setup.py` & `cloud_radar-0.6.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,362 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cloud-radar
+Version: 0.6.4
+Summary: Run functional tests on cloudformation stacks.
+Home-page: https://github.com/DontShaveTheYak/cloud-radar
+License: Apache-2.0
+Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
+Author: Levi Blaney
+Author-email: shadycuz@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: cfn-flip (>=1.2.3,<2.0.0)
+Requires-Dist: taskcat (>=0.9.20,<0.10.0)
+Project-URL: Repository, https://github.com/DontShaveTheYak/cloud-radar
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+<!-- PROJECT SHIELDS -->
+<!--
+*** I'm using markdown "reference style" links for readability.
+*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
+*** See the bottom of this document for the declaration of the reference variables
+*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
+*** https://www.markdownguide.org/basic-syntax/#reference-style-links
+-->
+[![Python][python-shield]][pypi-url]
+[![Latest][version-shield]][pypi-url]
+[![Tests][test-shield]][test-url]
+[![Coverage][codecov-shield]][codecov-url]
+[![License][license-shield]][license-url]
+<!-- [![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url] -->
 
-packages = \
-['cloud_radar', 'cloud_radar.cf', 'cloud_radar.cf.e2e', 'cloud_radar.cf.unit']
+<!-- PROJECT LOGO -->
+<br />
+<p align="center">
+  <!-- <a href="https://github.com/DontShaveTheYak/cloud-radar">
+    <img src="images/logo.png" alt="Logo" width="80" height="80">
+  </a> -->
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cfn-flip>=1.2.3,<2.0.0', 'taskcat>=0.9.20,<0.10.0']
-
-setup_kwargs = {
-    'name': 'cloud-radar',
-    'version': '0.6.3',
-    'description': 'Run functional tests on cloudformation stacks.',
-    'long_description': '<!-- PROJECT SHIELDS -->\n<!--\n*** I\'m using markdown "reference style" links for readability.\n*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).\n*** See the bottom of this document for the declaration of the reference variables\n*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.\n*** https://www.markdownguide.org/basic-syntax/#reference-style-links\n-->\n[![Python][python-shield]][pypi-url]\n[![Latest][version-shield]][pypi-url]\n[![Tests][test-shield]][test-url]\n[![Coverage][codecov-shield]][codecov-url]\n[![License][license-shield]][license-url]\n<!-- [![Contributors][contributors-shield]][contributors-url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url] -->\n\n<!-- PROJECT LOGO -->\n<br />\n<p align="center">\n  <!-- <a href="https://github.com/DontShaveTheYak/cloud-radar">\n    <img src="images/logo.png" alt="Logo" width="80" height="80">\n  </a> -->\n\n  <h3 align="center">Cloud-Radar</h3>\n\n  <p align="center">\n    Write unit and functional tests for AWS Cloudformation.\n    <!-- <br />\n    <a href="https://github.com/DontShaveTheYak/cloud-radar"><strong>Explore the docs »</strong></a>\n    <br /> -->\n    <br />\n    <!-- <a href="https://github.com/DontShaveTheYak/cloud-radar">View Demo</a>\n    · -->\n    <a href="https://github.com/DontShaveTheYak/cloud-radar/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/DontShaveTheYak/cloud-radar/issues">Request Feature</a>\n    ·\n    <a href="https://la-tech.co/post/hypermodern-cloudformation/getting-started/">Guide</a>\n  </p>\n</p>\n\n\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary>Table of Contents</summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#built-with">Built With</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#roadmap">Roadmap</a></li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#license">License</a></li>\n    <li><a href="#contact">Contact</a></li>\n    <li><a href="#acknowledgements">Acknowledgements</a></li>\n  </ol>\n</details>\n\n## About The Project\n\n<!-- [![Product Name Screen Shot][product-screenshot]](https://example.com) -->\n\nCloud-Radar is a python module that allows testing of Cloudformation Templates/Stacks using Python.\n\n### Unit Testing\n\nYou can now unit test the logic contained inside your Cloudformation template. Cloud-Radar takes your template, the desired region and some parameters. We render the template into its final state and pass it back to you.\n\nYou can Test:\n* That Conditionals in your template evaluate to the correct value.\n* Conditional resources were created or not.\n* That resources have the correct properties.\n* That resources are named as expected because of `!Sub`.\n\nYou can test all this locally without worrying about AWS Credentials.\n\n### Functional Testing\n\nThis project is a wrapper around Taskcat. Taskcat is a great tool for ensuring your Cloudformation Template can be deployed in multiple AWS Regions. Cloud-Radar enhances Taskcat by making it easier to write more complete functional tests.\n\nHere\'s How:\n* You can interact with the deployed resources directly with tools you already know like boto3.\n* You can control the lifecycle of the stack. This allows testing if resources were retained after the stacks were deleted.\n* You can run tests without hardcoding them in a taskcat config file.\n\nThis project is new and it\'s possible not all features or functionality of Taskcat/Cloudformation are supported (see [Roadmap](#roadmap)). If you find something missing or have a use case that isn\'t covered then please let me know =)\n\n### Built With\n\n* [Taskcat](https://github.com/aws-quickstart/taskcat)\n* [cfn_tools from cfn-flip](https://github.com/awslabs/aws-cfn-template-flip)\n\n## Getting Started\n\nCloud-Radar is available as an easy to install pip package.\n\n### Prerequisites\n\nCloud-Radar requires python >= 3.8\n\n### Installation\n\n1. Install with pip.\n   ```sh\n   pip install cloud-radar\n   ```\n\n## Usage\n<details>\n<summary>Unit Testing <span style=\'font-size: .67em\'>(Click to expand)</span></summary>\n\nUsing Cloud-Radar starts by importing it into your test file or framework. We will use this [Template](./tests/templates/log_bucket/log_bucket.yaml) as an example.\n\n```python\nfrom pathlib import Path\nfrom cloud_radar.cf.unit import Template\n\ntemplate_path = Path("tests/templates/log_bucket/log_bucket.yaml")\n\n# template_path can be a str or a Path object\ntemplate = Template.from_yaml(template_path.resolve())\n\nparams = {"BucketPrefix": "testing", "KeepBucket": "TRUE"}\n\n# parameters and region are optional arguments.\nresult = template.render(params, region="us-west-2")\n\nassert "LogsBucket" not in result["Resources"]\n\nbucket = result["Resources"]["RetainLogsBucket"]\n\nassert "DeletionPolicy" in bucket\n\nassert bucket["DeletionPolicy"] == "Retain"\n\nbucket_name = bucket["Properties"]["BucketName"]\n\nassert "us-west-2" in bucket_name\n```\n\nThe AWS pseudo variables are all class attributes and can be modified before rendering a template.\n```python\n# The value of \'AWS::AccountId\' in !Sub "My AccountId is ${AWS::AccountId}" can be changed:\nTemplate.AccountId = \'8675309\'\n```\n_Note: Region should only be changed to change the default value. To change the region during testing pass the desired region to render(region=\'us-west-2\')_\n\nThe default values for psedo variables:\n\n| Name             | Default Value   |\n| ---------------- | --------------- |\n| AccountId        | "555555555555"  |\n| NotificationARNs | []              |\n| **NoValue**      | ""              |\n| **Partition**    | "aws"           |\n| Region           | "us-east-1"     |\n| **StackId**      | ""              |\n| **StackName**    | ""              |\n| **URLSuffix**    | "amazonaws.com" |\n_Note: Bold variables are not fully impletmented yet see the [Roadmap](#roadmap)_\n\nA real unit testing example using Pytest can be seen [here](./tests/test_cf/test_examples/test_unit.py)\n\n</details>\n\n<details>\n<summary>Functional Testing <span style=\'font-size: .67em\'>(Click to expand)</span></summary>\nUsing Cloud-Radar starts by importing it into your test file or framework.\n\n```python\nfrom pathlib import Path\n\nfrom cloud_radar.cf.e2e import Stack\n\n# Stack is a context manager that makes sure your stacks are deleted after testing.\ntemplate_path = Path("tests/templates/log_bucket/log_bucket.yaml")\nparams = {"BucketPrefix": "testing", "KeepBucket": "False"}\nregions = [\'us-west-2\']\n\n# template_path can be a string or a Path object.\n# params can be optional if all your template params have default values\n# regions can be optional, default region is \'us-east-1\'\nwith Stack(template_path, params, regions) as stacks:\n    # Stacks will be created and returned as a list in the stacks variable.\n\n    for stack in stacks:\n        # stack will be an instance of Taskcat\'s Stack class.\n        # It has all the expected properties like parameters, outputs and resources\n\n        print(f"Testing {stack.name}")\n\n        bucket_name = ""\n\n        for output in stack.outputs:\n\n            if output.key == "LogsBucketName":\n                bucket_name = output.value\n                break\n\n        assert "logs" in bucket_name\n\n        assert stack.region.name in bucket_name\n\n        print(f"Created bucket: {bucket_name}")\n\n# Once the test is over then all resources will be deleted from your AWS account.\n```\n\nYou can use taskcat [tokens](https://aws.amazon.com/blogs/infrastructure-and-automation/a-deep-dive-into-testing-with-taskcat/) in your parameter values.\n\n```python\nparameters = {\n  "BucketPrefix": "taskcat-$[taskcat_random-string]",\n  "KeepBucket": "FALSE",\n}\n```\n\nYou can skip the context manager. Here is an example for `unittest`\n\n```python\nimport unittest\n\nfrom cloud-radar.cf.e2e import Stack\n\nclass TestLogBucket(unittest.TestCase):\n    @classmethod\n    def setUpClass(cls):\n        template_path = Path("tests/templates/log_bucket/log_bucket.yaml")\n        cls.test = Stack(template_path)\n        cls.test.create()\n\n    @classmethod\n    def tearDownClass(cls):\n        cls.test.delete()\n\n    def test_bucket(self):\n        stacks = self.__class__.test.stacks\n\n        for stack in stacks:\n            # Test\n```\n\nAll the properties and methods of a [stack instance](https://github.com/aws-quickstart/taskcat/blob/main/taskcat/_cfn/stack.py#L188).\n\nA real functional testing example using Pytest can be seen [here](./tests/test_cf/test_examples/test_functional.py)\n\n</details>\n\n## Roadmap\n\n### Project\n- Python 3.7 support\n- Add Logging\n- Add Logo\n- Make it easier to interact with stack resources.\n  * Getting a resource for testing should be as easy as `stack.Resources(\'MyResource)` or `template.Resources(\'MyResource\')`\n- Easier to pick regions for testing\n\n### Unit\n- Add full functionality to pseudo variables.\n  * Variables like `Partition`, `URLSuffix` should change if the region changes.\n  * Variables like `StackName` and `StackId` should have a better default than ""\n- Handle References to resources that shouldn\'t exist.\n  * It\'s currently possible that a `!Ref` to a Resource stays in the final template even if that resource is later removed because of a conditional.\n- Handle function order\n  * Some functions are only allowed in [certain parts](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-conditions.html) of the template.\n\n### Functional\n- Add the ability to update a stack instance to Taskcat.\n\nSee the [open issues](https://github.com/DontShaveTheYak/cloud-radar/issues) for a list of proposed features (and known issues).\n\n## Contributing\n\nContributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.\n\nThis project uses poetry to manage dependencies and pre-commit to run formatting, linting and tests. You will need to have both installed to your system as well as python 3.9.\n\n1. Fork the Project\n2. Setup environment (`poetry install`)\n3. Setup commit hooks (`pre-commit install`)\n2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/AmazingFeature`)\n5. Open a Pull Request\n\n## License\n\nDistributed under the Apache-2.0 License. See [LICENSE.txt](./LICENSE.txt) for more information.\n\n## Contact\n\nLevi - [@shady_cuz](https://twitter.com/shady_cuz)\n\n<!-- ACKNOWLEDGEMENTS -->\n## Acknowledgements\n* [Taskcat](https://aws-quickstart.github.io/taskcat/)\n* [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)\n* [Best-README-Template](https://github.com/othneildrew/Best-README-Template)\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[python-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-the-badge\n[version-shield]: https://img.shields.io/pypi/v/cloud-radar?label=latest&style=for-the-badge\n[pypi-url]: https://pypi.org/project/cloud-radar/\n[test-shield]: https://img.shields.io/github/workflow/status/DontShaveTheYak/cloud-radar/Tests?label=Tests&style=for-the-badge\n[test-url]: https://github.com/DontShaveTheYak/cloud-radar/actions?query=workflow%3ATests+branch%3Amaster\n[codecov-shield]: https://img.shields.io/codecov/c/gh/DontShaveTheYak/cloud-radar?color=green&style=for-the-badge&token=NE5C92139X\n[codecov-url]: https://codecov.io/gh/DontShaveTheYak/cloud-radar\n[contributors-shield]: https://img.shields.io/github/contributors/DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n[contributors-url]: https://github.com/DontShaveTheYak/cloud-radar/graphs/contributors\n[forks-shield]: https://img.shields.io/github/forks/DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n[forks-url]: https://github.com/DontShaveTheYak/cloud-radar/network/members\n[stars-shield]: https://img.shields.io/github/stars/DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n[stars-url]: https://github.com/DontShaveTheYak/cloud-radar/stargazers\n[issues-shield]: https://img.shields.io/github/issues/DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n[issues-url]: https://github.com/DontShaveTheYak/cloud-radar/issues\n[license-shield]: https://img.shields.io/github/license/DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n[license-url]: https://github.com/DontShaveTheYak/cloud-radar/blob/master/LICENSE.txt\n[product-screenshot]: images/screenshot.png\n',
-    'author': 'Levi Blaney',
-    'author_email': 'shadycuz@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DontShaveTheYak/cloud-radar',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+  <h3 align="center">Cloud-Radar</h3>
+
+  <p align="center">
+    Write unit and functional tests for AWS Cloudformation.
+    <!-- <br />
+    <a href="https://github.com/DontShaveTheYak/cloud-radar"><strong>Explore the docs »</strong></a>
+    <br /> -->
+    <br />
+    <!-- <a href="https://github.com/DontShaveTheYak/cloud-radar">View Demo</a>
+    · -->
+    <a href="https://github.com/DontShaveTheYak/cloud-radar/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/DontShaveTheYak/cloud-radar/issues">Request Feature</a>
+    ·
+    <a href="https://la-tech.co/post/hypermodern-cloudformation/getting-started/">Guide</a>
+  </p>
+</p>
+
+
+
+<!-- TABLE OF CONTENTS -->
+<details open="open">
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#roadmap">Roadmap</a></li>
+    <li><a href="#contributing">Contributing</a></li>
+    <li><a href="#license">License</a></li>
+    <li><a href="#contact">Contact</a></li>
+    <li><a href="#acknowledgements">Acknowledgements</a></li>
+  </ol>
+</details>
+
+## About The Project
+
+<!-- [![Product Name Screen Shot][product-screenshot]](https://example.com) -->
+
+Cloud-Radar is a python module that allows testing of Cloudformation Templates/Stacks using Python.
+
+### Unit Testing
+
+You can now unit test the logic contained inside your Cloudformation template. Cloud-Radar takes your template, the desired region and some parameters. We render the template into its final state and pass it back to you.
+
+You can Test:
+* That Conditionals in your template evaluate to the correct value.
+* Conditional resources were created or not.
+* That resources have the correct properties.
+* That resources are named as expected because of `!Sub`.
+
+You can test all this locally without worrying about AWS Credentials.
+
+### Functional Testing
+
+This project is a wrapper around Taskcat. Taskcat is a great tool for ensuring your Cloudformation Template can be deployed in multiple AWS Regions. Cloud-Radar enhances Taskcat by making it easier to write more complete functional tests.
+
+Here's How:
+* You can interact with the deployed resources directly with tools you already know like boto3.
+* You can control the lifecycle of the stack. This allows testing if resources were retained after the stacks were deleted.
+* You can run tests without hardcoding them in a taskcat config file.
+
+This project is new and it's possible not all features or functionality of Taskcat/Cloudformation are supported (see [Roadmap](#roadmap)). If you find something missing or have a use case that isn't covered then please let me know =)
+
+### Built With
+
+* [Taskcat](https://github.com/aws-quickstart/taskcat)
+* [cfn_tools from cfn-flip](https://github.com/awslabs/aws-cfn-template-flip)
+
+## Getting Started
+
+Cloud-Radar is available as an easy to install pip package.
+
+### Prerequisites
+
+Cloud-Radar requires python >= 3.8
+
+### Installation
+
+1. Install with pip.
+   ```sh
+   pip install cloud-radar
+   ```
+
+## Usage
+<details>
+<summary>Unit Testing <span style='font-size: .67em'>(Click to expand)</span></summary>
+
+Using Cloud-Radar starts by importing it into your test file or framework. We will use this [Template](./tests/templates/log_bucket/log_bucket.yaml) as an example.
+
+```python
+from pathlib import Path
+from cloud_radar.cf.unit import Template
+
+template_path = Path("tests/templates/log_bucket/log_bucket.yaml")
+
+# template_path can be a str or a Path object
+template = Template.from_yaml(template_path.resolve())
+
+params = {"BucketPrefix": "testing", "KeepBucket": "TRUE"}
+
+# parameters and region are optional arguments.
+result = template.render(params, region="us-west-2")
+
+assert "LogsBucket" not in result["Resources"]
+
+bucket = result["Resources"]["RetainLogsBucket"]
+
+assert "DeletionPolicy" in bucket
+
+assert bucket["DeletionPolicy"] == "Retain"
+
+bucket_name = bucket["Properties"]["BucketName"]
+
+assert "us-west-2" in bucket_name
+```
+
+The AWS pseudo variables are all class attributes and can be modified before rendering a template.
+```python
+# The value of 'AWS::AccountId' in !Sub "My AccountId is ${AWS::AccountId}" can be changed:
+Template.AccountId = '8675309'
+```
+_Note: Region should only be changed to change the default value. To change the region during testing pass the desired region to render(region='us-west-2')_
+
+The default values for psedo variables:
+
+| Name             | Default Value   |
+| ---------------- | --------------- |
+| AccountId        | "555555555555"  |
+| NotificationARNs | []              |
+| **NoValue**      | ""              |
+| **Partition**    | "aws"           |
+| Region           | "us-east-1"     |
+| **StackId**      | ""              |
+| **StackName**    | ""              |
+| **URLSuffix**    | "amazonaws.com" |
+_Note: Bold variables are not fully impletmented yet see the [Roadmap](#roadmap)_
+
+A real unit testing example using Pytest can be seen [here](./tests/test_cf/test_examples/test_unit.py)
+
+</details>
+
+<details>
+<summary>Functional Testing <span style='font-size: .67em'>(Click to expand)</span></summary>
+Using Cloud-Radar starts by importing it into your test file or framework.
+
+```python
+from pathlib import Path
+
+from cloud_radar.cf.e2e import Stack
+
+# Stack is a context manager that makes sure your stacks are deleted after testing.
+template_path = Path("tests/templates/log_bucket/log_bucket.yaml")
+params = {"BucketPrefix": "testing", "KeepBucket": "False"}
+regions = ['us-west-2']
+
+# template_path can be a string or a Path object.
+# params can be optional if all your template params have default values
+# regions can be optional, default region is 'us-east-1'
+with Stack(template_path, params, regions) as stacks:
+    # Stacks will be created and returned as a list in the stacks variable.
+
+    for stack in stacks:
+        # stack will be an instance of Taskcat's Stack class.
+        # It has all the expected properties like parameters, outputs and resources
+
+        print(f"Testing {stack.name}")
+
+        bucket_name = ""
+
+        for output in stack.outputs:
+
+            if output.key == "LogsBucketName":
+                bucket_name = output.value
+                break
+
+        assert "logs" in bucket_name
+
+        assert stack.region.name in bucket_name
+
+        print(f"Created bucket: {bucket_name}")
+
+# Once the test is over then all resources will be deleted from your AWS account.
+```
+
+You can use taskcat [tokens](https://aws.amazon.com/blogs/infrastructure-and-automation/a-deep-dive-into-testing-with-taskcat/) in your parameter values.
+
+```python
+parameters = {
+  "BucketPrefix": "taskcat-$[taskcat_random-string]",
+  "KeepBucket": "FALSE",
 }
+```
+
+You can skip the context manager. Here is an example for `unittest`
+
+```python
+import unittest
+
+from cloud-radar.cf.e2e import Stack
+
+class TestLogBucket(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        template_path = Path("tests/templates/log_bucket/log_bucket.yaml")
+        cls.test = Stack(template_path)
+        cls.test.create()
+
+    @classmethod
+    def tearDownClass(cls):
+        cls.test.delete()
+
+    def test_bucket(self):
+        stacks = self.__class__.test.stacks
+
+        for stack in stacks:
+            # Test
+```
+
+All the properties and methods of a [stack instance](https://github.com/aws-quickstart/taskcat/blob/main/taskcat/_cfn/stack.py#L188).
+
+A real functional testing example using Pytest can be seen [here](./tests/test_cf/test_examples/test_functional.py)
+
+</details>
+
+## Roadmap
+
+### Project
+- Python 3.7 support
+- Add Logging
+- Add Logo
+- Make it easier to interact with stack resources.
+  * Getting a resource for testing should be as easy as `stack.Resources('MyResource)` or `template.Resources('MyResource')`
+- Easier to pick regions for testing
+
+### Unit
+- Add full functionality to pseudo variables.
+  * Variables like `Partition`, `URLSuffix` should change if the region changes.
+  * Variables like `StackName` and `StackId` should have a better default than ""
+- Handle References to resources that shouldn't exist.
+  * It's currently possible that a `!Ref` to a Resource stays in the final template even if that resource is later removed because of a conditional.
+- Handle function order
+  * Some functions are only allowed in [certain parts](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-conditions.html) of the template.
+
+### Functional
+- Add the ability to update a stack instance to Taskcat.
+
+See the [open issues](https://github.com/DontShaveTheYak/cloud-radar/issues) for a list of proposed features (and known issues).
+
+## Contributing
+
+Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+This project uses poetry to manage dependencies and pre-commit to run formatting, linting and tests. You will need to have both installed to your system as well as python 3.9.
+
+1. Fork the Project
+2. Setup environment (`poetry install`)
+3. Setup commit hooks (`pre-commit install`)
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## License
+
+Distributed under the Apache-2.0 License. See [LICENSE.txt](./LICENSE.txt) for more information.
+
+## Contact
+
+Levi - [@shady_cuz](https://twitter.com/shady_cuz)
+
+<!-- ACKNOWLEDGEMENTS -->
+## Acknowledgements
+* [Taskcat](https://aws-quickstart.github.io/taskcat/)
+* [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)
+* [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
 
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[python-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-the-badge
+[version-shield]: https://img.shields.io/pypi/v/cloud-radar?label=latest&style=for-the-badge
+[pypi-url]: https://pypi.org/project/cloud-radar/
+[test-shield]: https://img.shields.io/github/actions/workflow/status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-badge
+[test-url]: https://github.com/DontShaveTheYak/cloud-radar/actions?query=workflow%3ATests+branch%3Amaster
+[codecov-shield]: https://img.shields.io/codecov/c/gh/DontShaveTheYak/cloud-radar?color=green&style=for-the-badge&token=NE5C92139X
+[codecov-url]: https://codecov.io/gh/DontShaveTheYak/cloud-radar
+[contributors-shield]: https://img.shields.io/github/contributors/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
+[contributors-url]: https://github.com/DontShaveTheYak/cloud-radar/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
+[forks-url]: https://github.com/DontShaveTheYak/cloud-radar/network/members
+[stars-shield]: https://img.shields.io/github/stars/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
+[stars-url]: https://github.com/DontShaveTheYak/cloud-radar/stargazers
+[issues-shield]: https://img.shields.io/github/issues/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
+[issues-url]: https://github.com/DontShaveTheYak/cloud-radar/issues
+[license-shield]: https://img.shields.io/github/license/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
+[license-url]: https://github.com/DontShaveTheYak/cloud-radar/blob/master/LICENSE.txt
+[product-screenshot]: images/screenshot.png
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,186 +1,161 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['cloud_radar', 'cloud_radar.cf', 'cloud_radar.cf.e2e',
-'cloud_radar.cf.unit'] package_data = \ {'': ['*']} install_requires = \ ['cfn-
-flip>=1.2.3,<2.0.0', 'taskcat>=0.9.20,<0.10.0'] setup_kwargs = { 'name':
-'cloud-radar', 'version': '0.6.3', 'description': 'Run functional tests on
-cloudformation stacks.', 'long_description': '\n\n[![Python][python-shield]]
-[pypi-url]\n[![Latest][version-shield]][pypi-url]\n[![Tests][test-shield]]
-[test-url]\n[![Coverage][codecov-shield]][codecov-url]\n[![License][license-
-shield]][license-url]\n\n\n\n
-\n
-                                    \n \n\n
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.6.4 Summary: Run functional
+tests on cloudformation stacks. Home-page: https://github.com/DontShaveTheYak/
+cloud-radar License: Apache-2.0 Keywords: aws,cloudformation,cloud-
+radar,testing,taskcat,cloud,radar Author: Levi Blaney Author-email:
+shadycuz@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
+:: 2 - Pre-Alpha Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Testing Requires-Dist: cfn-flip (>=1.2.3,<2.0.0) Requires-Dist: taskcat
+(>=0.9.20,<0.10.0) Project-URL: Repository, https://github.com/DontShaveTheYak/
+cloud-radar Description-Content-Type: text/markdown   [![Python][python-
+shield]][pypi-url] [![Latest][version-shield]][pypi-url] [![Tests][test-
+shield]][test-url] [![Coverage][codecov-shield]][codecov-url] [![License]
+[license-shield]][license-url]
                              **** Cloud-Radar ****
-\n\n
-       \n Write unit and functional tests for AWS Cloudformation.\n \n
-            \n \n Report_Bug\n Â·\n Request_Feature\n Â·\n Guide\n
-\n
-\n\n\n\n\n\n Table of Contents\n
-   1. \n
-   2. \n About_The_Project\n
-          o \n
+           Write unit and functional tests for AWS Cloudformation.
+                     Report_Bug Â· Request_Feature Â· Guide
+  Table of Contents
+   1. About_The_Project
           o Built_With
-          o \n
-      \n
-   3. \n
-   4. \n Getting_Started\n
-          o \n
+   2. Getting_Started
           o Prerequisites
-          o \n
           o Installation
-          o \n
-      \n
-   5. \n
-   6. Usage
-   7. \n
-   8. Roadmap
-   9. \n
-  10. Contributing
-  11. \n
-  12. License
-  13. \n
-  14. Contact
-  15. \n
-  16. Acknowledgements
-  17. \n
-\n\n\n## About The Project\n\n\n\nCloud-Radar is a python module that allows
-testing of Cloudformation Templates/Stacks using Python.\n\n### Unit
-Testing\n\nYou can now unit test the logic contained inside your Cloudformation
-template. Cloud-Radar takes your template, the desired region and some
-parameters. We render the template into its final state and pass it back to
-you.\n\nYou can Test:\n* That Conditionals in your template evaluate to the
-correct value.\n* Conditional resources were created or not.\n* That resources
-have the correct properties.\n* That resources are named as expected because of
-`!Sub`.\n\nYou can test all this locally without worrying about AWS
-Credentials.\n\n### Functional Testing\n\nThis project is a wrapper around
-Taskcat. Taskcat is a great tool for ensuring your Cloudformation Template can
-be deployed in multiple AWS Regions. Cloud-Radar enhances Taskcat by making it
-easier to write more complete functional tests.\n\nHere\'s How:\n* You can
-interact with the deployed resources directly with tools you already know like
-boto3.\n* You can control the lifecycle of the stack. This allows testing if
-resources were retained after the stacks were deleted.\n* You can run tests
-without hardcoding them in a taskcat config file.\n\nThis project is new and
-it\'s possible not all features or functionality of Taskcat/Cloudformation are
-supported (see [Roadmap](#roadmap)). If you find something missing or have a
-use case that isn\'t covered then please let me know =)\n\n### Built With\n\n*
-[Taskcat](https://github.com/aws-quickstart/taskcat)\n* [cfn_tools from cfn-
-flip](https://github.com/awslabs/aws-cfn-template-flip)\n\n## Getting
-Started\n\nCloud-Radar is available as an easy to install pip package.\n\n###
-Prerequisites\n\nCloud-Radar requires python >= 3.8\n\n### Installation\n\n1.
-Install with pip.\n ```sh\n pip install cloud-radar\n ```\n\n## Usage\n\nUnit
-Testing
-67em\'>(Click to expand)\n\nUsing Cloud-Radar starts by importing it into your
-test file or framework. We will use this [Template](./tests/templates/
-log_bucket/log_bucket.yaml) as an example.\n\n```python\nfrom pathlib import
-Path\nfrom cloud_radar.cf.unit import Template\n\ntemplate_path = Path("tests/
-templates/log_bucket/log_bucket.yaml")\n\n# template_path can be a str or a
-Path object\ntemplate = Template.from_yaml(template_path.resolve())\n\nparams =
-{"BucketPrefix": "testing", "KeepBucket": "TRUE"}\n\n# parameters and region
-are optional arguments.\nresult = template.render(params, region="us-west-
-2")\n\nassert "LogsBucket" not in result["Resources"]\n\nbucket = result
-["Resources"]["RetainLogsBucket"]\n\nassert "DeletionPolicy" in
-bucket\n\nassert bucket["DeletionPolicy"] == "Retain"\n\nbucket_name = bucket
-["Properties"]["BucketName"]\n\nassert "us-west-2" in bucket_name\n```\n\nThe
-AWS pseudo variables are all class attributes and can be modified before
-rendering a template.\n```python\n# The value of \'AWS::AccountId\' in !Sub "My
-AccountId is ${AWS::AccountId}" can be changed:\nTemplate.AccountId =
-\'8675309\'\n```\n_Note: Region should only be changed to change the default
-value. To change the region during testing pass the desired region to render
-(region=\'us-west-2\')_\n\nThe default values for psedo variables:\n\n| Name |
-Default Value |\n| ---------------- | --------------- |\n| AccountId |
-"555555555555" |\n| NotificationARNs | [] |\n| **NoValue** | "" |\n|
-**Partition** | "aws" |\n| Region | "us-east-1" |\n| **StackId** | "" |\n|
-**StackName** | "" |\n| **URLSuffix** | "amazonaws.com" |\n_Note: Bold
-variables are not fully impletmented yet see the [Roadmap](#roadmap)_\n\nA real
-unit testing example using Pytest can be seen [here](./tests/test_cf/
-test_examples/test_unit.py)\n\n\n\n\nFunctional Testing
-67em\'>(Click to expand)\nUsing Cloud-Radar starts by importing it into your
-test file or framework.\n\n```python\nfrom pathlib import Path\n\nfrom
-cloud_radar.cf.e2e import Stack\n\n# Stack is a context manager that makes sure
-your stacks are deleted after testing.\ntemplate_path = Path("tests/templates/
-log_bucket/log_bucket.yaml")\nparams = {"BucketPrefix": "testing",
-"KeepBucket": "False"}\nregions = [\'us-west-2\']\n\n# template_path can be a
-string or a Path object.\n# params can be optional if all your template params
-have default values\n# regions can be optional, default region is \'us-east-
-1\'\nwith Stack(template_path, params, regions) as stacks:\n # Stacks will be
-created and returned as a list in the stacks variable.\n\n for stack in stacks:
-\n # stack will be an instance of Taskcat\'s Stack class.\n # It has all the
-expected properties like parameters, outputs and resources\n\n print(f"Testing
-{stack.name}")\n\n bucket_name = ""\n\n for output in stack.outputs:\n\n if
-output.key == "LogsBucketName":\n bucket_name = output.value\n break\n\n assert
-"logs" in bucket_name\n\n assert stack.region.name in bucket_name\n\n print
-(f"Created bucket: {bucket_name}")\n\n# Once the test is over then all
-resources will be deleted from your AWS account.\n```\n\nYou can use taskcat
-[tokens](https://aws.amazon.com/blogs/infrastructure-and-automation/a-deep-
-dive-into-testing-with-taskcat/) in your parameter
-values.\n\n```python\nparameters = {\n "BucketPrefix": "taskcat-$
-[taskcat_random-string]",\n "KeepBucket": "FALSE",\n}\n```\n\nYou can skip the
-context manager. Here is an example for `unittest`\n\n```python\nimport
-unittest\n\nfrom cloud-radar.cf.e2e import Stack\n\nclass TestLogBucket
-(unittest.TestCase):\n @classmethod\n def setUpClass(cls):\n template_path =
-Path("tests/templates/log_bucket/log_bucket.yaml")\n cls.test = Stack
-(template_path)\n cls.test.create()\n\n @classmethod\n def tearDownClass(cls):
-\n cls.test.delete()\n\n def test_bucket(self):\n stacks =
-self.__class__.test.stacks\n\n for stack in stacks:\n # Test\n```\n\nAll the
-properties and methods of a [stack instance](https://github.com/aws-quickstart/
-taskcat/blob/main/taskcat/_cfn/stack.py#L188).\n\nA real functional testing
+   3. Usage
+   4. Roadmap
+   5. Contributing
+   6. License
+   7. Contact
+   8. Acknowledgements
+ ## About The Project  Cloud-Radar is a python module that allows testing of
+Cloudformation Templates/Stacks using Python. ### Unit Testing You can now unit
+test the logic contained inside your Cloudformation template. Cloud-Radar takes
+your template, the desired region and some parameters. We render the template
+into its final state and pass it back to you. You can Test: * That Conditionals
+in your template evaluate to the correct value. * Conditional resources were
+created or not. * That resources have the correct properties. * That resources
+are named as expected because of `!Sub`. You can test all this locally without
+worrying about AWS Credentials. ### Functional Testing This project is a
+wrapper around Taskcat. Taskcat is a great tool for ensuring your
+Cloudformation Template can be deployed in multiple AWS Regions. Cloud-Radar
+enhances Taskcat by making it easier to write more complete functional tests.
+Here's How: * You can interact with the deployed resources directly with tools
+you already know like boto3. * You can control the lifecycle of the stack. This
+allows testing if resources were retained after the stacks were deleted. * You
+can run tests without hardcoding them in a taskcat config file. This project is
+new and it's possible not all features or functionality of Taskcat/
+Cloudformation are supported (see [Roadmap](#roadmap)). If you find something
+missing or have a use case that isn't covered then please let me know =) ###
+Built With * [Taskcat](https://github.com/aws-quickstart/taskcat) * [cfn_tools
+from cfn-flip](https://github.com/awslabs/aws-cfn-template-flip) ## Getting
+Started Cloud-Radar is available as an easy to install pip package. ###
+Prerequisites Cloud-Radar requires python >= 3.8 ### Installation 1. Install
+with pip. ```sh pip install cloud-radar ``` ## Usage  Unit Testing (Click to
+expand) Using Cloud-Radar starts by importing it into your test file or
+framework. We will use this [Template](./tests/templates/log_bucket/
+log_bucket.yaml) as an example. ```python from pathlib import Path from
+cloud_radar.cf.unit import Template template_path = Path("tests/templates/
+log_bucket/log_bucket.yaml") # template_path can be a str or a Path object
+template = Template.from_yaml(template_path.resolve()) params =
+{"BucketPrefix": "testing", "KeepBucket": "TRUE"} # parameters and region are
+optional arguments. result = template.render(params, region="us-west-2") assert
+"LogsBucket" not in result["Resources"] bucket = result["Resources"]
+["RetainLogsBucket"] assert "DeletionPolicy" in bucket assert bucket
+["DeletionPolicy"] == "Retain" bucket_name = bucket["Properties"]["BucketName"]
+assert "us-west-2" in bucket_name ``` The AWS pseudo variables are all class
+attributes and can be modified before rendering a template. ```python # The
+value of 'AWS::AccountId' in !Sub "My AccountId is ${AWS::AccountId}" can be
+changed: Template.AccountId = '8675309' ``` _Note: Region should only be
+changed to change the default value. To change the region during testing pass
+the desired region to render(region='us-west-2')_ The default values for psedo
+variables: | Name | Default Value | | ---------------- | --------------- | |
+AccountId | "555555555555" | | NotificationARNs | [] | | **NoValue** | "" | |
+**Partition** | "aws" | | Region | "us-east-1" | | **StackId** | "" | |
+**StackName** | "" | | **URLSuffix** | "amazonaws.com" | _Note: Bold variables
+are not fully impletmented yet see the [Roadmap](#roadmap)_ A real unit testing
 example using Pytest can be seen [here](./tests/test_cf/test_examples/
-test_functional.py)\n\n\n\n## Roadmap\n\n### Project\n- Python 3.7 support\n-
-Add Logging\n- Add Logo\n- Make it easier to interact with stack resources.\n *
-Getting a resource for testing should be as easy as `stack.Resources
-(\'MyResource)` or `template.Resources(\'MyResource\')`\n- Easier to pick
-regions for testing\n\n### Unit\n- Add full functionality to pseudo
-variables.\n * Variables like `Partition`, `URLSuffix` should change if the
-region changes.\n * Variables like `StackName` and `StackId` should have a
-better default than ""\n- Handle References to resources that shouldn\'t
-exist.\n * It\'s currently possible that a `!Ref` to a Resource stays in the
-final template even if that resource is later removed because of a
-conditional.\n- Handle function order\n * Some functions are only allowed in
-[certain parts](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/
-intrinsic-function-reference-conditions.html) of the template.\n\n###
-Functional\n- Add the ability to update a stack instance to Taskcat.\n\nSee the
-[open issues](https://github.com/DontShaveTheYak/cloud-radar/issues) for a list
-of proposed features (and known issues).\n\n## Contributing\n\nContributions
-are what make the open-source community such an amazing place to learn,
-inspire, and create. Any contributions you make are **greatly
-appreciated**.\n\nThis project uses poetry to manage dependencies and pre-
-commit to run formatting, linting and tests. You will need to have both
-installed to your system as well as python 3.9.\n\n1. Fork the Project\n2.
-Setup environment (`poetry install`)\n3. Setup commit hooks (`pre-commit
-install`)\n2. Create your Feature Branch (`git checkout -b feature/
-AmazingFeature`)\n3. Commit your Changes (`git commit -m \'Add some
-AmazingFeature\'`)\n4. Push to the Branch (`git push origin feature/
-AmazingFeature`)\n5. Open a Pull Request\n\n## License\n\nDistributed under the
-Apache-2.0 License. See [LICENSE.txt](./LICENSE.txt) for more
-information.\n\n## Contact\n\nLevi - [@shady_cuz](https://twitter.com/
-shady_cuz)\n\n\n## Acknowledgements\n* [Taskcat](https://aws-
-quickstart.github.io/taskcat/)\n* [Hypermodern Python](https://
-cjolowicz.github.io/posts/hypermodern-python-01-setup/)\n* [Best-README-
-Template](https://github.com/othneildrew/Best-README-Template)\n\n\n\n[python-
-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-the-
-badge\n[version-shield]: https://img.shields.io/pypi/v/cloud-
-radar?label=latest&style=for-the-badge\n[pypi-url]: https://pypi.org/project/
-cloud-radar/\n[test-shield]: https://img.shields.io/github/workflow/status/
-DontShaveTheYak/cloud-radar/Tests?label=Tests&style=for-the-badge\n[test-url]:
-https://github.com/DontShaveTheYak/cloud-radar/
-actions?query=workflow%3ATests+branch%3Amaster\n[codecov-shield]: https://
+test_unit.py)   Functional Testing (Click to expand) Using Cloud-Radar starts
+by importing it into your test file or framework. ```python from pathlib import
+Path from cloud_radar.cf.e2e import Stack # Stack is a context manager that
+makes sure your stacks are deleted after testing. template_path = Path("tests/
+templates/log_bucket/log_bucket.yaml") params = {"BucketPrefix": "testing",
+"KeepBucket": "False"} regions = ['us-west-2'] # template_path can be a string
+or a Path object. # params can be optional if all your template params have
+default values # regions can be optional, default region is 'us-east-1' with
+Stack(template_path, params, regions) as stacks: # Stacks will be created and
+returned as a list in the stacks variable. for stack in stacks: # stack will be
+an instance of Taskcat's Stack class. # It has all the expected properties like
+parameters, outputs and resources print(f"Testing {stack.name}") bucket_name =
+"" for output in stack.outputs: if output.key == "LogsBucketName": bucket_name
+= output.value break assert "logs" in bucket_name assert stack.region.name in
+bucket_name print(f"Created bucket: {bucket_name}") # Once the test is over
+then all resources will be deleted from your AWS account. ``` You can use
+taskcat [tokens](https://aws.amazon.com/blogs/infrastructure-and-automation/a-
+deep-dive-into-testing-with-taskcat/) in your parameter values. ```python
+parameters = { "BucketPrefix": "taskcat-$[taskcat_random-string]",
+"KeepBucket": "FALSE", } ``` You can skip the context manager. Here is an
+example for `unittest` ```python import unittest from cloud-radar.cf.e2e import
+Stack class TestLogBucket(unittest.TestCase): @classmethod def setUpClass(cls):
+template_path = Path("tests/templates/log_bucket/log_bucket.yaml") cls.test =
+Stack(template_path) cls.test.create() @classmethod def tearDownClass(cls):
+cls.test.delete() def test_bucket(self): stacks = self.__class__.test.stacks
+for stack in stacks: # Test ``` All the properties and methods of a [stack
+instance](https://github.com/aws-quickstart/taskcat/blob/main/taskcat/_cfn/
+stack.py#L188). A real functional testing example using Pytest can be seen
+[here](./tests/test_cf/test_examples/test_functional.py)  ## Roadmap ###
+Project - Python 3.7 support - Add Logging - Add Logo - Make it easier to
+interact with stack resources. * Getting a resource for testing should be as
+easy as `stack.Resources('MyResource)` or `template.Resources('MyResource')` -
+Easier to pick regions for testing ### Unit - Add full functionality to pseudo
+variables. * Variables like `Partition`, `URLSuffix` should change if the
+region changes. * Variables like `StackName` and `StackId` should have a better
+default than "" - Handle References to resources that shouldn't exist. * It's
+currently possible that a `!Ref` to a Resource stays in the final template even
+if that resource is later removed because of a conditional. - Handle function
+order * Some functions are only allowed in [certain parts](https://
+docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-
+reference-conditions.html) of the template. ### Functional - Add the ability to
+update a stack instance to Taskcat. See the [open issues](https://github.com/
+DontShaveTheYak/cloud-radar/issues) for a list of proposed features (and known
+issues). ## Contributing Contributions are what make the open-source community
+such an amazing place to learn, inspire, and create. Any contributions you make
+are **greatly appreciated**. This project uses poetry to manage dependencies
+and pre-commit to run formatting, linting and tests. You will need to have both
+installed to your system as well as python 3.9. 1. Fork the Project 2. Setup
+environment (`poetry install`) 3. Setup commit hooks (`pre-commit install`) 2.
+Create your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit
+your Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch
+(`git push origin feature/AmazingFeature`) 5. Open a Pull Request ## License
+Distributed under the Apache-2.0 License. See [LICENSE.txt](./LICENSE.txt) for
+more information. ## Contact Levi - [@shady_cuz](https://twitter.com/shady_cuz)
+## Acknowledgements * [Taskcat](https://aws-quickstart.github.io/taskcat/) *
+[Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-
+setup/) * [Best-README-Template](https://github.com/othneildrew/Best-README-
+Template)   [python-shield]: https://img.shields.io/pypi/pyversions/cloud-
+radar?style=for-the-badge [version-shield]: https://img.shields.io/pypi/v/
+cloud-radar?label=latest&style=for-the-badge [pypi-url]: https://pypi.org/
+project/cloud-radar/ [test-shield]: https://img.shields.io/github/actions/
+workflow/status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-
+badge [test-url]: https://github.com/DontShaveTheYak/cloud-radar/
+actions?query=workflow%3ATests+branch%3Amaster [codecov-shield]: https://
 img.shields.io/codecov/c/gh/DontShaveTheYak/cloud-radar?color=green&style=for-
-the-badge&token=NE5C92139X\n[codecov-url]: https://codecov.io/gh/
-DontShaveTheYak/cloud-radar\n[contributors-shield]: https://img.shields.io/
-github/contributors/DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n
+the-badge&token=NE5C92139X [codecov-url]: https://codecov.io/gh/
+DontShaveTheYak/cloud-radar [contributors-shield]: https://img.shields.io/
+github/contributors/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
 [contributors-url]: https://github.com/DontShaveTheYak/cloud-radar/graphs/
-contributors\n[forks-shield]: https://img.shields.io/github/forks/
-DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n[forks-url]: https://
-github.com/DontShaveTheYak/cloud-radar/network/members\n[stars-shield]: https:/
-/img.shields.io/github/stars/DontShaveTheYak/cloud-radar.svg?style=for-the-
-badge\n[stars-url]: https://github.com/DontShaveTheYak/cloud-radar/stargazers\n
-[issues-shield]: https://img.shields.io/github/issues/DontShaveTheYak/cloud-
-radar.svg?style=for-the-badge\n[issues-url]: https://github.com/
-DontShaveTheYak/cloud-radar/issues\n[license-shield]: https://img.shields.io/
-github/license/DontShaveTheYak/cloud-radar.svg?style=for-the-badge\n[license-
-url]: https://github.com/DontShaveTheYak/cloud-radar/blob/master/LICENSE.txt\n
-[product-screenshot]: images/screenshot.png\n', 'author': 'Levi Blaney',
-'author_email': 'shadycuz@gmail.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/DontShaveTheYak/cloud-radar', 'package_dir':
-package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+contributors [forks-shield]: https://img.shields.io/github/forks/
+DontShaveTheYak/cloud-radar.svg?style=for-the-badge [forks-url]: https://
+github.com/DontShaveTheYak/cloud-radar/network/members [stars-shield]: https://
+img.shields.io/github/stars/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
+[stars-url]: https://github.com/DontShaveTheYak/cloud-radar/stargazers [issues-
+shield]: https://img.shields.io/github/issues/DontShaveTheYak/cloud-
+radar.svg?style=for-the-badge [issues-url]: https://github.com/DontShaveTheYak/
+cloud-radar/issues [license-shield]: https://img.shields.io/github/license/
+DontShaveTheYak/cloud-radar.svg?style=for-the-badge [license-url]: https://
+github.com/DontShaveTheYak/cloud-radar/blob/master/LICENSE.txt [product-
+screenshot]: images/screenshot.png
```

