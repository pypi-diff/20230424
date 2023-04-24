# Comparing `tmp/aws_hexagonal_adapters-0.0.7.tar.gz` & `tmp/aws_hexagonal_adapters-1.0.0.tar.gz`

## Comparing `aws_hexagonal_adapters-0.0.7.tar` & `aws_hexagonal_adapters-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,42 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/.DS_Store
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/dynamo_db_service.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/event_bridge_service.py
--rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/s3_service.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/ses_service.py
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/sqs_service.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/ssm_service.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/LICENSE
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/README.md
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.DS_Store
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/ruff.toml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/168cc38b04774c1d
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/618c6b6cc269398a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/81d6bea09b3bfddc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/8f6d8158c77dd870
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/a5ccc3b3108d4277
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/c285b1f3993c3cc4
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/c5082269dd966539
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/c82b673ec67750f8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/df318c36e6722395
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/fc051c84047f8578
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.ruff_cache/content/fff176ebb881786c
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/dynamo_db_service.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/event_bridge_service.py
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/s3_service.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ses_service.py
+-rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/sqs_service.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ssm_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/nonexistent.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/test.txt
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/test_s3_service.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/LICENSE
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/README.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 aws_hexagonal_adapters-1.0.0/PKG-INFO
```

### Comparing `aws_hexagonal_adapters-0.0.7/.DS_Store` & `aws_hexagonal_adapters-1.0.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/dynamo_db_service.py` & `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/dynamo_db_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/event_bridge_service.py` & `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/event_bridge_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/ses_service.py` & `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ses_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/sqs_service.py` & `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/sqs_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-0.0.7/aws_hexagonal_adapters/ssm_service.py` & `aws_hexagonal_adapters-1.0.0/aws_hexagonal_adapters/ssm_service.py`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-0.0.7/LICENSE` & `aws_hexagonal_adapters-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_hexagonal_adapters-0.0.7/pyproject.toml` & `aws_hexagonal_adapters-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aws_hexagonal_adapters"
 description = "Adapters following hexagonal architecture to connect various AWS services."
-version = "0.0.7"
+version = "1.0.0"
 authors = [{name = "Tomasz Szuster", email = "tomasz.szuster@gmail.com"}]
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
         "boto3>=1.26.71,<2.0.0",
         "botocore>=1.29.71,<2.0.0",
-        "aws_lambda_powertools>=2.8.0,<3.0.0",
+        "aws_lambda_powertools>=2.8.0,<4.0.0",
 ]
 [project.urls]
 Home = "https://github.com/airmonitor/aws-hexagonal-adapters"
 Bug_Tracker = "https://github.com/airmonitor/aws-hexagonal-adapters/issues"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
```

### Comparing `aws_hexagonal_adapters-0.0.7/PKG-INFO` & `aws_hexagonal_adapters-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_hexagonal_adapters
-Version: 0.0.7
+Version: 1.0.0
 Summary: Adapters following hexagonal architecture to connect various AWS services.
 Project-URL: Home, https://github.com/airmonitor/aws-hexagonal-adapters
 Project-URL: Bug_Tracker, https://github.com/airmonitor/aws-hexagonal-adapters/issues
 Author-email: Tomasz Szuster <tomasz.szuster@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Szuster
@@ -24,17 +24,18 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
-Requires-Dist: aws-lambda-powertools<3.0.0,>=2.8.0
+Requires-Python: >=3.10
+Requires-Dist: aws-lambda-powertools<4.0.0,>=2.8.0
 Requires-Dist: boto3<2.0.0,>=1.26.71
 Requires-Dist: botocore<2.0.0,>=1.29.71
 Description-Content-Type: text/markdown
 
 [![auto-merge](https://github.com/airmonitor/aws-hexagonal-adapters/actions/workflows/auto_merge.yml/badge.svg)](https://github.com/airmonitor/aws-hexagonal-adapters/actions/workflows/auto_merge.yml)
+[![tests](https://github.com/airmonitor/aws-hexagonal-adapters/actions/workflows/tests.yml/badge.svg)](https://github.com/airmonitor/aws-hexagonal-adapters/actions/workflows/tests.yml)
 
 # aws-hexagonal-adapters
 Adapters following hexagonal architecture to connect various AWS services
```

