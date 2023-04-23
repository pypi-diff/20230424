# Comparing `tmp/ripio_client-0.0.2.tar.gz` & `tmp/ripio_client-0.0.3.tar.gz`

## Comparing `ripio_client-0.0.2.tar` & `ripio_client-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ripio_client-0.0.2/ripio/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ripio_client-0.0.2/ripio/trade/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ripio_client-0.0.2/ripio/trade/client.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ripio_client-0.0.2/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 ripio_client-0.0.2/LICENSE
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 ripio_client-0.0.2/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ripio_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ripio_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ripio_client-0.0.3/.flake8
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ripio_client-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ripio_client-0.0.3/sample.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ripio_client-0.0.3/test_client.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ripio_client-0.0.3/ripio/__init__.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ripio_client-0.0.3/ripio/core.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ripio_client-0.0.3/ripio/exceptions/auth.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ripio_client-0.0.3/ripio/exceptions/request.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ripio_client-0.0.3/ripio/exceptions/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ripio_client-0.0.3/ripio/trade/__init__.py
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 ripio_client-0.0.3/ripio/trade/client.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ripio_client-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 ripio_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 ripio_client-0.0.3/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 ripio_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ripio_client-0.0.3/PKG-INFO
```

### Comparing `ripio_client-0.0.2/LICENSE` & `ripio_client-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `ripio_client-0.0.2/pyproject.toml` & `ripio_client-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ripio-client"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Sebastian Serrano", email="sebastian@ripio.com" },
 ]
 description = "Ripio Client for Python"
 readme = "README.md"
 requires-python = ">=3.7"
+dependencies = [
+  'requests >= 2.28.0',
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ripio/ripio-client-python"
 "Bug Tracker" = "https://github.com/ripio/ripio-client-python/issues"
 
 [tool.hatch.build.targets.wheel]
 only-include = ["ripio"]
+
+[tool.black]
+line-length = 79
+target-version = ['py310']
```

### Comparing `ripio_client-0.0.2/PKG-INFO` & `ripio_client-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 Metadata-Version: 2.1
 Name: ripio-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ripio Client for Python
 Project-URL: Homepage, https://github.com/ripio/ripio-client-python
 Project-URL: Bug Tracker, https://github.com/ripio/ripio-client-python/issues
 Author-email: Sebastian Serrano <sebastian@ripio.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: requests>=2.28.0
 Description-Content-Type: text/markdown
 
 # Ripio Client for Python
 ###  ALPHA SOFTWARE
-  
+
 
 This is a lightweight library that works as a client to [Ripio](https://www.ripio.com) Services
 
 ## Installation
 ```bash
 pip install ripio-client
 ```
 
 ## Usage example
 ```python
-from ripio.trade import Client
+from ripio.trade.client import Client
 
 # API key is required for user data endpoints
 client = Client(api_key='<api_key>')
 
 # Get balance information
 print(client.balance())
 
-# Post a new order
+# Create a market order
 params = {
 	'pair': 'BTC_USDC',
 	'side': 'buy',
 	'amount': 0.01,
 	'type': 'market'
 }
 response = client.create_order(**params)
 print(response)
+
+# Create a limit buy order
+params = {
+	'pair': 'BTC_USDC',
+	'side': 'buy',
+	'amount': 0.0002,
+	'type': 'limit',
+	'price': 27471.65
+}
+response = client.create_order(**params)
+print(response)
+
+# Create a limit sell order
+params = {
+	'pair': 'BTC_USDC',
+	'side': 'sell',
+	'amount': 0.0002,
+	'type': 'limit',
+	'price': 27470
+}
+response = client.create_order(**params)
+print(response)
+
 ```
```

