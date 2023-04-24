# Comparing `tmp/cdk_proxy_api_client-0.2.2.tar.gz` & `tmp/cdk_proxy_api_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_proxy_api_client-0.2.2.tar", max compression
+gzip compressed data, was "cdk_proxy_api_client-0.2.3.tar", max compression
```

## Comparing `cdk_proxy_api_client-0.2.2.tar` & `cdk_proxy_api_client-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.2.2/LICENSE
--rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.2.2/README.md
--rw-r--r--   0        0        0      181 2023-04-16 08:58:42.448296 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/__init__.py
--rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/admin_auth/__init__.py
--rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/admin_auth/exceptions.py
--rw-r--r--   0        0        0     4849 2023-04-16 08:51:39.880237 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/cli/__init__.py
--rw-r--r--   0        0        0     4473 2023-04-16 08:53:07.712280 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/cli/main_parser.py
--rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/client_wrapper.py
--rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/__init__.py
--rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/logging.py
--rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/errors.py
--rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/models/__init__.py
--rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/models/v1b1.py
--rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/proxy_api.py
--rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/specs/__init__.py
--rw-r--r--   0        0        0     3825 2023-04-16 08:57:33.887474 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/specs/tenant_mappings-input.json
--rw-r--r--   0        0        0     2936 2023-04-16 08:53:27.770521 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tenant_mappings/__init__.py
--rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tenant_mappings/exceptions.py
--rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/__init__.py
--rw-r--r--   0        0        0    10915 2023-04-16 08:57:33.593470 cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/import_tenants_mappings.py
--rw-r--r--   0        0        0     2430 2023-04-16 08:58:42.448296 cdk_proxy_api_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.2/setup.py
--rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-03-08 09:09:19.917488 cdk_proxy_api_client-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4404 2023-03-26 16:28:29.410881 cdk_proxy_api_client-0.2.3/README.md
+-rw-r--r--   0        0        0      181 2023-04-24 16:25:30.071770 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/__init__.py
+-rw-r--r--   0        0        0     1163 2023-03-26 16:47:51.442956 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/admin_auth/__init__.py
+-rw-r--r--   0        0        0      133 2023-03-10 11:53:55.066691 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/admin_auth/exceptions.py
+-rw-r--r--   0        0        0     6668 2023-04-24 16:24:30.444038 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/cli/__init__.py
+-rw-r--r--   0        0        0     6297 2023-04-24 16:24:30.445038 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/cli/main_parser.py
+-rw-r--r--   0        0        0     5728 2023-03-14 12:38:20.148498 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/client_wrapper.py
+-rw-r--r--   0        0        0      601 2023-03-08 21:22:30.578973 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/common/__init__.py
+-rw-r--r--   0        0        0     1174 2023-03-26 16:44:44.959697 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/common/logging.py
+-rw-r--r--   0        0        0     2269 2023-04-24 16:24:30.445038 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/concentration/__init__.py
+-rw-r--r--   0        0        0     3012 2023-03-10 11:34:33.523871 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/errors.py
+-rw-r--r--   0        0        0       93 2023-03-08 21:22:30.582973 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1467 2023-03-08 10:34:32.551495 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/models/v1b1.py
+-rw-r--r--   0        0        0     1400 2023-03-26 16:47:51.434956 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/proxy_api.py
+-rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/specs/__init__.py
+-rw-r--r--   0        0        0     3825 2023-04-24 16:09:11.319693 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/specs/tenant_mappings-input.json
+-rw-r--r--   0        0        0     2973 2023-04-24 16:24:30.445038 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/tenant_mappings/__init__.py
+-rw-r--r--   0        0        0      414 2023-03-10 12:11:17.799028 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/tenant_mappings/exceptions.py
+-rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/tools/__init__.py
+-rw-r--r--   0        0        0    10915 2023-04-19 10:54:30.871690 cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/tools/import_tenants_mappings.py
+-rw-r--r--   0        0        0     2430 2023-04-24 16:25:30.071770 cdk_proxy_api_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5941 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.3/setup.py
+-rw-r--r--   0        0        0     6035 1970-01-01 00:00:00.000000 cdk_proxy_api_client-0.2.3/PKG-INFO
```

### Comparing `cdk_proxy_api_client-0.2.2/LICENSE` & `cdk_proxy_api_client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/README.md` & `cdk_proxy_api_client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/admin_auth/__init__.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/admin_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/cli/main_parser.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/cli/main_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -92,14 +92,59 @@
         "--logical-topic-name",
         dest="logicalTopicName",
         required=True,
         help="Topic name as seen in the tenant.",
     )
 
 
+def set_tenant_concentration_mappings_subparsers(
+    concentration_mappings_parser: ArgumentParser,
+):
+    mappings_subparser = concentration_mappings_parser.add_subparsers(
+        dest="action", help="Concentrated mappings management"
+    )
+    create_parser = mappings_subparser.add_parser(
+        name="create",
+        help="Create a new tenant concentrated mapping",
+        parents=[TENANT_PARSER],
+    )
+    create_parser.add_argument(
+        "--physical-topic-name", type=str, required=True, dest="physicalTopicName"
+    )
+    create_parser.add_argument(
+        "--topics-regex",
+        type=str,
+        required=True,
+        help="Regex of topics to match",
+        dest="topicRegex",
+    )
+    list_parser = mappings_subparser.add_parser(
+        name="list", help="List topping mappings", parents=[TENANT_PARSER]
+    )
+
+
+def set_tenant_topics_subparsers(
+    concentration_mappings_parser: ArgumentParser,
+):
+    mappings_subparser = concentration_mappings_parser.add_subparsers(
+        dest="action", help="Concentrated mappings management"
+    )
+    list_parser = mappings_subparser.add_parser(
+        name="list", help="List topping mappings", parents=[TENANT_PARSER]
+    )
+    get_topic_parser = mappings_subparser.add_parser(
+        name="get-topic",
+        help="Get topic configuration for tenant",
+        parents=[TENANT_PARSER],
+    )
+    get_topic_parser.add_argument(
+        "--logical-topic-name", required=True, dest="logicalTopicName"
+    )
+
+
 def set_parser():
     main_parser = ArgumentParser("CDK Proxy CLI", add_help=True)
     main_parser.add_argument(
         "--format",
         "--output-format",
         dest="output_format",
         help="output format",
@@ -117,15 +162,21 @@
         help="Manages proxy tenant token",
     )
     set_admin_auth_parser(auth_admin_parser)
 
     mappings_parser = cmd_parser.add_parser(
         name="tenant-topic-mappings", help="Manages tenant mappings"
     )
+    concentration_parser = cmd_parser.add_parser(
+        name="tenant-concentrated-mappings", help="Manages concentration mappings"
+    )
+    tenant_topics_subparser = cmd_parser.add_parser(name="tenant-topics")
+    set_tenant_topics_subparsers(tenant_topics_subparser)
     set_tenant_mappings_subparsers(mappings_parser)
+    set_tenant_concentration_mappings_subparsers(concentration_parser)
 
     tenants_parser = cmd_parser.add_parser(name="tenants", help="Manage tenants")
     tenants_subparser = tenants_parser.add_subparsers(
         dest="action", help="Manage tenants"
     )
     tenants_subparser.add_parser(name="list", help="List tenants", parents=[])
     return main_parser
```

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/client_wrapper.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/__init__.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/common/logging.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/common/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/errors.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/models/v1b1.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/models/v1b1.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/proxy_api.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/proxy_api.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/specs/tenant_mappings-input.json` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/specs/tenant_mappings-input.json`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tenant_mappings/__init__.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/tenant_mappings/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #   SPDX-License-Identifier: Apache-2.0
 #   Copyright 2023 John Mille <john@ews-network.net>
 
 
 from __future__ import annotations
 
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
-from requests import Response
+if TYPE_CHECKING:
+    from requests import Response
 
 from cdk_proxy_api_client.common.logging import LOG
 from cdk_proxy_api_client.errors import GenericNotFound
 from cdk_proxy_api_client.proxy_api import ApiApplication, Multitenancy
 from cdk_proxy_api_client.tenant_mappings.exceptions import (
     TenantNotFound,
     TopicOrTenantNotFound,
```

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/__init__.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/cdk_proxy_api_client/tools/import_tenants_mappings.py` & `cdk_proxy_api_client-0.2.3/cdk_proxy_api_client/tools/import_tenants_mappings.py`

 * *Files identical despite different names*

### Comparing `cdk_proxy_api_client-0.2.2/pyproject.toml` & `cdk_proxy_api_client-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cdk-proxy-api-client"
 description = "Conduktor Proxy API Client"
-version = "0.2.2"
+version = "0.2.3"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{include = "cdk_proxy_api_client"}]
 keywords = ["compose-x", "conduktor", "kafka", "proxy"]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
@@ -55,15 +55,15 @@
 cdk-cli = "cdk_proxy_api_client.cli:main"
 
 
 [tool.tbump]
 github_url = "https://codeberg.org/JohnPreston/cdk-proxy-api-client"
 
 [tool.tbump.version]
-current = "0.2.2"
+current = "0.2.3"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `cdk_proxy_api_client-0.2.2/setup.py` & `cdk_proxy_api_client-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from setuptools import setup
 
 packages = \
 ['cdk_proxy_api_client',
  'cdk_proxy_api_client.admin_auth',
  'cdk_proxy_api_client.cli',
  'cdk_proxy_api_client.common',
+ 'cdk_proxy_api_client.concentration',
  'cdk_proxy_api_client.models',
  'cdk_proxy_api_client.specs',
  'cdk_proxy_api_client.tenant_mappings',
  'cdk_proxy_api_client.tools']
 
 package_data = \
 {'': ['*']}
@@ -26,15 +27,15 @@
            'importlib-resources>=5.12.0,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['cdk-cli = cdk_proxy_api_client.cli:main']}
 
 setup_kwargs = {
     'name': 'cdk-proxy-api-client',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Conduktor Proxy API Client',
     'long_description': '# cdk-proxy-api-client\n\nAPI Client library to interact with Conduktor Proxy\n\nCurrent version: v1beta1\n\n\n## Getting started\n\nFirst, create a Proxy Client\n\n```python\nfrom cdk_proxy_api_client.proxy_api import ApiClient, ProxyClient\n\napi = ApiClient("localhost", port=8888, username="superUser", password="superUser")\nproxy_client = ProxyClient(api)\n```\n\n### Features\n\nNote: we assume you are re-using the ``proxy_client`` as shown above.\n\n* Create new Token for a tenant\n\n```python\nfrom cdk_proxy_api_client.admin_auth import AdminAuth\n\nadmin = AdminAuth(proxy_client)\nadmin.create_tenant_credentials("a_tenant_name")\n```\n\n* List all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.proxy_api import Multitenancy\n\ntenants_mgmt = Multitenancy(proxy_client)\ntenants = tenants_mgmt.list_tenants(as_list=True)\n```\n\n* Create a new mapping for a tenant\n* Delete a tenant - topic mapping\n* Delete all topic mappings for a tenant\n\n```python\nfrom cdk_proxy_api_client.tenant_mappings import TenantTopicMappings\n\ntenant_mappings_mgmt = TenantTopicMappings(proxy_client)\ntenant_mappings_mgmt.create_tenant_topic_mapping(\n    "tenant_name", "logical_name", "real_name"\n)\ntenant_mappings_mgmt.delete_tenant_topic_mapping("tenant_name", "logical_name")\n```\n\n## Testing\nThe testing is for now very manual. See ``e2e_testing.py``\n\nPytest will be added later on\n\n\n## Tools & CLI\n\nTo simplify the usage of the client, you can use some CLI commands\n\n```shell\nusage: CDK Proxy CLI [-h] [--format OUTPUT_FORMAT] --username USERNAME --password PASSWORD --url URL {auth,tenant-topic-mappings,tenants} ...\n\npositional arguments:\n  {auth,tenant-topic-mappings,tenants}\n                        Resources to manage\n    auth                Manages proxy tenant token\n    tenant-topic-mappings\n                        Manages tenant mappings\n    tenants             Manage tenants\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --format OUTPUT_FORMAT, --output-format OUTPUT_FORMAT\n                        output format\n  --username USERNAME\n  --password PASSWORD\n  --url URL\n\n```\n\n### cdk-cli tenant-topic-mappings\n\n```shell\nusage: CDK Proxy CLI tenant-topic-mappings [-h] {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping} ...\n\npositional arguments:\n  {list,create,import-from-tenants-config,import-from-tenant,delete-all-mappings,delete-topic-mapping}\n                        Mappings management\n    list                List tenant mappings\n    create              Create a new tenant mapping\n    import-from-tenants-config\n                        Create topic mappings from existing tenants\n    import-from-tenant  Import all topics from a existing tenant\n    delete-all-mappings\n                        Delete all topics mappings for a given tenant\n    delete-topic-mapping\n                        Delete a topic mapping for a given tenant\n\noptional arguments:\n  -h, --help            show this help message and exit\n```\n\n#### import-from-tenants-config\n\nThis command uses a configuration file that will be used to propagate mappings from one/multiple existing tenants to another.\n\nexample file:\n\n```yaml\n---\n# example.config.yaml\n\ntenant_name: application-01\nignore_duplicates_conflict: true\nmappings:\n  - logicalTopicName: data.stock\n    physicalTopicName: data.stock\n    readOnly: true\n```\n\n```shell\ncdk-cli --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        tenant-topic-mappings import-from-tenants-config -f example.config.yaml\n```\n\n### cdk-cli auth\n\n```shell\ncdk-cli auth --help\nusage: CDK Proxy CLI auth [-h] {create} ...\n\npositional arguments:\n  {create}    Token actions to execute\n    create    Create a new tenant proxy JWT Token\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n\n#### cdk-cli-create-tenant-token\n\nCreate a new user tenant token\n\n```shell\ncdk-cli \\\n        --username ${PROXY_USERNAME} \\\n        --password ${PROXY_PASSWORD} \\\n        --url ${PROXY_URL} \\\n        auth create \\\n        --lifetime-in-seconds 3600  \\\n        --tenant-name js-fin-panther-stg\n```\n\n### cdk-cli tenants\n\nManage tenants\n\n```shell\ncdk-cli tenants --help\nusage: CDK Proxy CLI tenants [-h] {list} ...\n\npositional arguments:\n  {list}      Manage tenants\n    list      List tenants\n\noptional arguments:\n  -h, --help  show this help message and exit\n```\n',
     'author': 'John "Preston" Mille',
     'author_email': 'john@ews-network.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cdk_proxy_api_client-0.2.2/PKG-INFO` & `cdk_proxy_api_client-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-proxy-api-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Conduktor Proxy API Client
 License: LICENSE
 Keywords: compose-x,conduktor,kafka,proxy
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

