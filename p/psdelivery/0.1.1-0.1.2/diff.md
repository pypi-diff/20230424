# Comparing `tmp/psdelivery-0.1.1.tar.gz` & `tmp/psdelivery-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdelivery-0.1.1.tar", max compression
+gzip compressed data, was "psdelivery-0.1.2.tar", max compression
```

## Comparing `psdelivery-0.1.1.tar` & `psdelivery-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-04-23 15:24:01.732921 psdelivery-0.1.1/LICENSE
--rw-r--r--   0        0        0     4115 2023-04-23 15:24:01.732921 psdelivery-0.1.1/README.md
--rw-r--r--   0        0        0       82 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/__init__.py
--rw-r--r--   0        0        0      115 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/__main__.py
--rw-r--r--   0        0        0     3065 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/command_line.py
--rw-r--r--   0        0        0      976 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/controller.py
--rw-r--r--   0        0        0     1847 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/core/crawler.py
--rw-r--r--   0        0        0     1408 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/core/difficulty.py
--rw-r--r--   0        0        0     1969 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/core/engine.py
--rw-r--r--   0        0        0      877 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/core/item.py
--rw-r--r--   0        0        0      520 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/core/option.py
--rw-r--r--   0        0        0      120 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/baekjoon/__init__.py
--rw-r--r--   0        0        0     2509 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/baekjoon/crawler.py
--rw-r--r--   0        0        0      244 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/baekjoon/difficulty.py
--rw-r--r--   0        0        0      236 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/baekjoon/item.py
--rw-r--r--   0        0        0       84 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/leetcode/__init__.py
--rw-r--r--   0        0        0     2085 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/leetcode/crawler.py
--rw-r--r--   0        0        0      240 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/leetcode/difficulty.py
--rw-r--r--   0        0        0      235 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/crawlers/leetcode/item.py
--rw-r--r--   0        0        0      274 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/exc.py
--rw-r--r--   0        0        0     1098 2023-04-23 15:24:01.732921 psdelivery-0.1.1/psdelivery/utils/type_checker.py
--rw-r--r--   0        0        0     1109 2023-04-23 15:24:01.732921 psdelivery-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5383 1970-01-01 00:00:00.000000 psdelivery-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 17:45:46.707196 psdelivery-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4306 2023-04-24 17:45:46.707196 psdelivery-0.1.2/README.md
+-rw-r--r--   0        0        0       82 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/__main__.py
+-rw-r--r--   0        0        0     3094 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/command_line.py
+-rw-r--r--   0        0        0     1042 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/controller.py
+-rw-r--r--   0        0        0     2611 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/core/crawler.py
+-rw-r--r--   0        0        0     1408 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/core/difficulty.py
+-rw-r--r--   0        0        0     1969 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/core/engine.py
+-rw-r--r--   0        0        0      877 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/core/item.py
+-rw-r--r--   0        0        0      511 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/core/option.py
+-rw-r--r--   0        0        0      120 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/baekjoon/__init__.py
+-rw-r--r--   0        0        0     2579 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/baekjoon/crawler.py
+-rw-r--r--   0        0        0      244 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/baekjoon/difficulty.py
+-rw-r--r--   0        0        0      236 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/baekjoon/item.py
+-rw-r--r--   0        0        0       84 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/leetcode/__init__.py
+-rw-r--r--   0        0        0     2085 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/leetcode/crawler.py
+-rw-r--r--   0        0        0      240 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/leetcode/difficulty.py
+-rw-r--r--   0        0        0      235 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/crawlers/leetcode/item.py
+-rw-r--r--   0        0        0      274 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/exc.py
+-rw-r--r--   0        0        0      312 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/utils/logger.py
+-rw-r--r--   0        0        0     1110 2023-04-24 17:45:46.707196 psdelivery-0.1.2/psdelivery/utils/type_checker.py
+-rw-r--r--   0        0        0     1109 2023-04-24 17:45:46.707196 psdelivery-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5574 1970-01-01 00:00:00.000000 psdelivery-0.1.2/PKG-INFO
```

### Comparing `psdelivery-0.1.1/LICENSE` & `psdelivery-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psdelivery-0.1.1/README.md` & `psdelivery-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # 📦 psdelivery
 
-[![Test](https://github.com/team-angeline/psdelivery/actions/workflows/dev-test.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/dev-test.yml)
+[![Ubuntu](https://github.com/team-angeline/psdelivery/actions/workflows/test-ubuntu.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/test-ubuntu.yml)
+[![Windows](https://github.com/team-angeline/psdelivery/actions/workflows/test-windows.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/test-windows.yml)
 [![CI](https://github.com/team-angeline/psdelivery/actions/workflows/ci.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/ci.yml)
 ![GitHub](https://img.shields.io/github/license/team-angeline/psdelivery)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psdelivery?logo=python&logoColor=white)
 [![PyPI](https://img.shields.io/pypi/v/psdelivery?label=pypi%20package&logo=pypi&logoColor=white)](https://pypi.org/project/psdelivery)
 [![codecov](https://codecov.io/gh/team-angeline/psdelivery/branch/main/graph/badge.svg?token=LFC7Z4PGCT)](https://codecov.io/gh/team-angeline/psdelivery)
 
 ```shell
```

### Comparing `psdelivery-0.1.1/psdelivery/command_line.py` & `psdelivery-0.1.2/psdelivery/command_line.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     @staticmethod
     def get_problem_list(topic: str, single_page: int | None, output: str):
         data: str | None = None
 
         if single_page is not None:
             data = json.dumps(
                 PsDelivery(topic).get_list_by_single_page(
-                    single_page, True),
+                    page=single_page, serialize=True, logging=True),
                 ensure_ascii=False,
                 sort_keys=True,
                 indent=4)
 
         if data is not None:
             with open(output, 'wt') as f:
                 f.write(data)
```

### Comparing `psdelivery-0.1.1/psdelivery/controller.py` & `psdelivery-0.1.2/psdelivery/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,12 +18,14 @@
         crawler: Type[ProblemCrawler] | None = CRAWLER_MAP.get(topic.lower())
         if not crawler:
             raise ValueError(f'{topic} crawler is not exists.')
         self.crawler = crawler()
 
     def get_list_by_single_page(
             self, page: int,
-            serialize: bool = False) -> List[ProblemItem] | List[Dict[str, Any]]:
-        res: List[ProblemItem] = self.crawler.get_list(page=page)
+            serialize: bool = False,
+            logging: bool = False) -> List[ProblemItem] | List[Dict[str, Any]]:
+        res: List[ProblemItem] = \
+            self.crawler.get_list(page=page, logging=logging)
         if serialize:
             return [r.__dict__ for r in res]
         return res
```

### Comparing `psdelivery-0.1.1/psdelivery/core/crawler.py` & `psdelivery-0.1.2/psdelivery/core/engine.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,71 @@
-import time
-from typing import List, Any, final
+from typing import Any, final
 from abc import ABCMeta, abstractmethod
+import time
 
-from selenium.common.exceptions import NoSuchElementException
+import requests
+from requests import Response
+from bs4 import BeautifulSoup
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
+from webdriver_manager.chrome import ChromeDriverManager
+
+from psdelivery.core.option import CrawlerOption, DefaultSeleniumCrawlerOption
+from psdelivery.exc import RequestTimeout, RequestFailed, WebdriverIsNotLoaded
 
-from psdelivery.utils.type_checker import must_be_type
-from psdelivery.core.engine import CrawlingEngine
-from psdelivery.core.item import ProblemItem
 
+class CrawlingEngine(metaclass=ABCMeta):
+    engine: Any | None = None
+    
+    @abstractmethod
+    def open(self) -> None: ...
 
-class ProblemCrawler(metaclass=ABCMeta):
-    base_url: str
-    engine: CrawlingEngine
+    @abstractmethod
+    def close(self) -> None: ...
 
-    @final
-    def open(self) -> None:
-        self.engine.open()
+    @abstractmethod
+    def open_web(self, url: str) -> None: ...
 
     @final
-    def close(self) -> None:
-        self.engine.close()
+    def __call__(self) -> Any | None:
+        return self.engine
 
-    @final
-    def __del__(self) -> None:
-        self.close()
 
-    @final
-    def open_web(self, url: str = None):
-        if not url:
-            url = self.base_url
-        self.engine.open_web(url)
+@final
+class BeautifulSoupEngine(CrawlingEngine):
+    engine: BeautifulSoup | None = None
 
-    @abstractmethod
-    def generate_url_by_page_index(self, page: int = 1) -> str: ...
+    def open(self) -> None: ...
+    def close(self) -> None: ...
 
-    @abstractmethod
-    def access_to_problem_list(self, page: int = 1) -> None: ...
+    def open_web(self, url: str) -> None:
+        try:
+            response: Response = requests.get(url, timeout=30)
+        except TimeoutError:
+            raise RequestTimeout('Request timeout.')
 
-    @abstractmethod
-    def get_problem_elements(self) -> List[Any]: ...
+        if response.status_code == 200:
+            self.engine = BeautifulSoup(response.text, 'html.parser')
+        else:
+            raise RequestFailed('Request failed to web.')
 
-    @abstractmethod
-    def parse_problem_from_problem_element(self, item: Any) -> ProblemItem | None: ...
 
-    @final
-    @must_be_type('page', int)
-    def get_list(self, page: int = 1) -> List[ProblemItem]:
-        self.target_url: str = self.generate_url_by_page_index(page)
-        if page < 0:
-            raise ValueError('page is must not be under 0.')
-
-        self.open()
-        self.open_web(self.target_url)
-        self.access_to_problem_list()
-        items = self.get_problem_elements(page)
-        problems: List[ProblemItem] = []
-        for item in items:
-            try:
-                problem = self.parse_problem_from_problem_element(item)
-            except NoSuchElementException:
-                continue
-            else:
-                if problem:
-                    problems.append(problem)
-        self.close()
-        return problems
+@final
+class SeleniumEngine(CrawlingEngine):
+    engine: webdriver.Chrome
+    option_generator: CrawlerOption = DefaultSeleniumCrawlerOption()
+
+    def open(self) -> None:
+        self.engine = webdriver.Chrome(
+            service=Service(ChromeDriverManager().install()),
+            options=self.option_generator.generate())
+        
+    def close(self) -> None:
+        if self.engine:
+            self.engine.quit()
+
+    def open_web(self, url: str) -> None:
+        if self.engine:
+            self.engine.get(url)
+            time.sleep(2)
+        else:
+            raise WebdriverIsNotLoaded('Selenium webdriver is not loaded.')
```

### Comparing `psdelivery-0.1.1/psdelivery/core/difficulty.py` & `psdelivery-0.1.2/psdelivery/core/difficulty.py`

 * *Files identical despite different names*

### Comparing `psdelivery-0.1.1/psdelivery/core/item.py` & `psdelivery-0.1.2/psdelivery/core/item.py`

 * *Files identical despite different names*

### Comparing `psdelivery-0.1.1/psdelivery/crawlers/baekjoon/crawler.py` & `psdelivery-0.1.2/psdelivery/crawlers/baekjoon/crawler.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,17 @@
     @property
     def seq(self) -> str:
         return self.item.find_element(By.CLASS_NAME, 'css-1raije9')  \
                         .find_element(By.TAG_NAME, 'span').text
 
     @property
     def web_difficulty(self) -> str:
-        return self.item.find_element(By.CLASS_NAME, 'css-1raije9') \
-                        .find_element(By.TAG_NAME, 'span').text
+        img_url = self.item.find_element(By.CLASS_NAME, 'css-1raije9') \
+                        .find_element(By.TAG_NAME, 'img').get_attribute('src')
+        return img_url.split('/')[-1].split('.')[0]
 
     @property
     def title(self) -> str:
         return self.item.find_element(By.CLASS_NAME, 'css-d6mf5j') \
                         .find_element(By.CLASS_NAME, '__Latex__').text
 
     @property
```

### Comparing `psdelivery-0.1.1/psdelivery/crawlers/leetcode/crawler.py` & `psdelivery-0.1.2/psdelivery/crawlers/leetcode/crawler.py`

 * *Files identical despite different names*

### Comparing `psdelivery-0.1.1/psdelivery/utils/type_checker.py` & `psdelivery-0.1.2/psdelivery/utils/type_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def _decorator(func: Callable):
         def _wrapper(*args, **kwargs):
             valid_types: List[Type] = []
             if isinstance(arg_type, Type):
                 valid_types = [arg_type]
             elif isinstance(arg_type, UnionType):
                 valid_types = list(arg_type.__args__)
-
+            
             if arg_name not in kwargs:
                 raise ValueError(f'Argment {arg_name} is not exists.')
             arg_val: Any = kwargs[arg_name]
 
             is_valid = any([isinstance(arg_val, vt) for vt in valid_types])
             if not is_valid:
                 raise ValueError('This type of argument is not valid')
```

### Comparing `psdelivery-0.1.1/pyproject.toml` & `psdelivery-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psdelivery"
-version = "0.1.1"
+version = "0.1.2"
 description = "The simple crawler about algorithm problem service website"
 authors = ["recoma <seokbong60@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 repository = "https://github.com/team-angeline/psdelivery"
 keywords = ["crwaler", "problem-solving"]
 classifiers = [
```

### Comparing `psdelivery-0.1.1/PKG-INFO` & `psdelivery-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdelivery
-Version: 0.1.1
+Version: 0.1.2
 Summary: The simple crawler about algorithm problem service website
 Home-page: https://github.com/team-angeline/psdelivery
 License: GPL-3.0-only
 Keywords: crwaler,problem-solving
 Author: recoma
 Author-email: seokbong60@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -25,15 +25,16 @@
 Requires-Dist: selenium (>=4.9.0,<5.0.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Project-URL: Repository, https://github.com/team-angeline/psdelivery
 Description-Content-Type: text/markdown
 
 # 📦 psdelivery
 
-[![Test](https://github.com/team-angeline/psdelivery/actions/workflows/dev-test.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/dev-test.yml)
+[![Ubuntu](https://github.com/team-angeline/psdelivery/actions/workflows/test-ubuntu.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/test-ubuntu.yml)
+[![Windows](https://github.com/team-angeline/psdelivery/actions/workflows/test-windows.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/test-windows.yml)
 [![CI](https://github.com/team-angeline/psdelivery/actions/workflows/ci.yml/badge.svg)](https://github.com/team-angeline/psdelivery/actions/workflows/ci.yml)
 ![GitHub](https://img.shields.io/github/license/team-angeline/psdelivery)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psdelivery?logo=python&logoColor=white)
 [![PyPI](https://img.shields.io/pypi/v/psdelivery?label=pypi%20package&logo=pypi&logoColor=white)](https://pypi.org/project/psdelivery)
 [![codecov](https://codecov.io/gh/team-angeline/psdelivery/branch/main/graph/badge.svg?token=LFC7Z4PGCT)](https://codecov.io/gh/team-angeline/psdelivery)
 
 ```shell
```

