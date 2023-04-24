# Comparing `tmp/pytest-playwright-0.3.2.tar.gz` & `tmp/pytest-playwright-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-playwright-0.3.2.tar", last modified: Fri Mar 10 08:52:06 2023, max compression
+gzip compressed data, was "pytest-playwright-0.3.3.tar", last modified: Mon Apr 24 19:29:19 2023, max compression
```

## Comparing `pytest-playwright-0.3.2.tar` & `pytest-playwright-0.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.852846 pytest-playwright-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.848846 pytest-playwright-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.848846 pytest-playwright-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-10 08:52:06.852846 pytest-playwright-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/local-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.848846 pytest-playwright-0.3.2/pytest_playwright/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/pytest_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-10 08:52:06.000000 pytest-playwright-0.3.2/pytest_playwright/_repo_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/pytest_playwright/pytest_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.852846 pytest-playwright-0.3.2/pytest_playwright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-10 08:52:06.000000 pytest-playwright-0.3.2/pytest_playwright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-10 08:52:06.000000 pytest-playwright-0.3.2/pytest_playwright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 08:52:06.000000 pytest-playwright-0.3.2/pytest_playwright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-10 08:52:06.000000 pytest-playwright-0.3.2/pytest_playwright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-10 08:52:06.000000 pytest-playwright-0.3.2/pytest_playwright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-10 08:52:06.000000 pytest-playwright-0.3.2/pytest_playwright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-10 08:52:06.852846 pytest-playwright-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.852846 pytest-playwright-0.3.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.848846 pytest-playwright-0.3.2/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:52:06.852846 pytest-playwright-0.3.2/tests/assets/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/tests/assets/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/tests/assets/django/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/tests/assets/django/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-03-10 08:51:48.000000 pytest-playwright-0.3.2/tests/test_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/local-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/pytest_playwright/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/pytest_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright/_repo_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12394 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/pytest_playwright/pytest_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/pytest_playwright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 19:29:19.000000 pytest-playwright-0.3.3/pytest_playwright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:29:19.218269 pytest-playwright-0.3.3/tests/assets/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/assets/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/assets/django/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/assets/django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-04-24 19:28:55.000000 pytest-playwright-0.3.3/tests/test_playwright.py
```

### Comparing `pytest-playwright-0.3.2/.github/workflows/ci.yml` & `pytest-playwright-0.3.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/.github/workflows/python-publish.yml` & `pytest-playwright-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/.gitignore` & `pytest-playwright-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/.pre-commit-config.yaml` & `pytest-playwright-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/CONTRIBUTING.md` & `pytest-playwright-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/LICENSE` & `pytest-playwright-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/PKG-INFO` & `pytest-playwright-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.3.2
+Version: 0.3.3
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-playwright-0.3.2/README.md` & `pytest-playwright-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/SECURITY.md` & `pytest-playwright-0.3.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/pytest_playwright/pytest_playwright.py` & `pytest-playwright-0.3.3/pytest_playwright/pytest_playwright.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import hashlib
 import shutil
 import os
 import sys
 import warnings
 from typing import Any, Callable, Dict, Generator, List, Optional
 
 import pytest
@@ -147,15 +148,25 @@
     return debugger.is_attached()
 
 
 def _build_artifact_test_folder(
     pytestconfig: Any, request: pytest.FixtureRequest, folder_or_file_name: str
 ) -> str:
     output_dir = pytestconfig.getoption("--output")
-    return os.path.join(output_dir, slugify(request.node.nodeid), folder_or_file_name)
+    return os.path.join(
+        output_dir,
+        truncate_file_name(slugify(request.node.nodeid)),
+        truncate_file_name(folder_or_file_name),
+    )
+
+
+def truncate_file_name(file_name: str) -> str:
+    if len(file_name) < 256:
+        return file_name
+    return f"{file_name[:100]}-{hashlib.sha256(file_name.encode()).hexdigest()[:7]}-{file_name[-100:]}"
 
 
 @pytest.fixture(scope="session")
 def browser_context_args(
     pytestconfig: Any,
     playwright: Playwright,
     device: Optional[str],
@@ -219,15 +230,15 @@
     context = browser.new_context(**browser_context_args)
     context.on("page", lambda page: pages.append(page))
 
     tracing_option = pytestconfig.getoption("--tracing")
     capture_trace = tracing_option in ["on", "retain-on-failure"]
     if capture_trace:
         context.tracing.start(
-            name=slugify(request.node.nodeid),
+            title=slugify(request.node.nodeid),
             screenshots=True,
             snapshots=True,
             sources=True,
         )
 
     yield context
```

### Comparing `pytest-playwright-0.3.2/pytest_playwright.egg-info/PKG-INFO` & `pytest-playwright-0.3.3/pytest_playwright.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-playwright
-Version: 0.3.2
+Version: 0.3.3
 Summary: A pytest wrapper with fixtures for Playwright to automate web browsers
 Home-page: https://github.com/microsoft/playwright-pytest
 Author: Microsoft
 Author-email: 
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-playwright-0.3.2/pytest_playwright.egg-info/SOURCES.txt` & `pytest-playwright-0.3.3/pytest_playwright.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/setup.py` & `pytest-playwright-0.3.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     url="https://github.com/microsoft/playwright-pytest",
     packages=["pytest_playwright"],
     include_package_data=True,
     install_requires=[
         "playwright>=1.18",
         "pytest>=6.2.4,<8.0.0",
         "pytest-base-url>=1.0.0,<3.0.0",
-        "python-slugify>=6.0.0,<7.0.0",
+        "python-slugify>=6.0.0,<9.0.0",
     ],
     entry_points={"pytest11": ["playwright = pytest_playwright.pytest_playwright"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `pytest-playwright-0.3.2/tests/assets/django/settings.py` & `pytest-playwright-0.3.3/tests/assets/django/settings.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/tests/conftest.py` & `pytest-playwright-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-playwright-0.3.2/tests/test_playwright.py` & `pytest-playwright-0.3.3/tests/test_playwright.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,16 +215,16 @@
 def test_goto(testdir: pytest.Testdir) -> None:
     testdir.makepyfile(
         """
         def test_base_url(page, base_url):
             assert base_url == "https://example.com"
             page.goto("/foobar")
             assert page.url == "https://example.com/foobar"
-            page.goto("http://whatsmyuseragent.org")
-            assert page.url == "http://whatsmyuseragent.org/"
+            page.goto("https://example.org")
+            assert page.url == "https://example.org/"
     """
     )
     result = testdir.runpytest("--base-url", "https://example.com")
     result.assert_outcomes(passed=1)
 
 
 def test_base_url_via_fixture(testdir: pytest.Testdir) -> None:
@@ -649,14 +649,40 @@
                 },
             ],
         }
     ]
     _assert_folder_tree(test_results_dir, expected)
 
 
+def test_should_work_with_test_names_which_exceeds_256_characters(
+    testdir: pytest.Testdir,
+) -> None:
+    long_test_name = "abcdefghijklmnopqrstuvwxyz" * 100
+    testdir.makepyfile(
+        f"""
+        def test_{long_test_name}(page):
+            pass
+    """
+    )
+    result = testdir.runpytest("--tracing", "on")
+    result.assert_outcomes(passed=1, failed=0)
+    test_results_dir = os.path.join(testdir.tmpdir, "test-results")
+    expected = [
+        {
+            "name": "test-should-work-with-test-names-which-exceeds-256-characters-py-test-abcdefghijklmnopqrstuvwxyzabcd-23f2441-nopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyzabcdefghijklmnopqrstuvwxyz-chromium/",
+            "children": [
+                {
+                    "name": "trace.zip",
+                },
+            ],
+        },
+    ]
+    _assert_folder_tree(test_results_dir, expected)
+
+
 def _assert_folder_tree(root: str, expected_tree: List[Any]) -> None:
     assert len(os.listdir(root)) == len(expected_tree)
     for file in expected_tree:
         if isinstance(file["name"], str):
             if "children" in file:
                 assert os.path.isdir(os.path.join(root, file["name"]))
             else:
```

