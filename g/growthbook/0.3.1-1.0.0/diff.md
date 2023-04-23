# Comparing `tmp/growthbook-0.3.1.tar.gz` & `tmp/growthbook-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/growthbook-0.3.1.tar", last modified: Mon Aug  1 20:08:57 2022, max compression
+gzip compressed data, was "dist/growthbook-1.0.0.tar", last modified: Sun Apr 23 22:03:58 2023, max compression
```

## Comparing `growthbook-0.3.1.tar` & `growthbook-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2022-08-01 20:08:57.742735 growthbook-0.3.1/
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)     1069 2022-02-13 16:34:23.000000 growthbook-0.3.1/LICENSE
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       91 2021-09-16 22:25:57.000000 growthbook-0.3.1/MANIFEST.in
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    13412 2022-08-01 20:08:57.742735 growthbook-0.3.1/PKG-INFO
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)     9994 2022-08-01 20:07:55.000000 growthbook-0.3.1/README.md
-drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2022-08-01 20:08:57.742735 growthbook-0.3.1/growthbook.egg-info/
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    13412 2022-08-01 20:08:57.000000 growthbook-0.3.1/growthbook.egg-info/PKG-INFO
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)      223 2022-08-01 20:08:57.000000 growthbook-0.3.1/growthbook.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)        1 2022-08-01 20:08:57.000000 growthbook-0.3.1/growthbook.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       11 2022-08-01 20:08:57.000000 growthbook-0.3.1/growthbook.egg-info/top_level.txt
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    22654 2022-08-01 20:08:36.000000 growthbook-0.3.1/growthbook.py
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)      256 2022-08-01 20:08:57.742735 growthbook-0.3.1/setup.cfg
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)     1291 2022-08-01 20:08:36.000000 growthbook-0.3.1/setup.py
-drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2022-08-01 20:08:57.742735 growthbook-0.3.1/tests/
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    12321 2022-05-24 14:28:26.000000 growthbook-0.3.1/tests/test_growthbook.py
+drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2023-04-23 22:03:58.537231 growthbook-1.0.0/
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)     1069 2022-02-13 16:34:23.000000 growthbook-1.0.0/LICENSE
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       91 2021-09-16 22:25:57.000000 growthbook-1.0.0/MANIFEST.in
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    17204 2023-04-23 22:03:58.537231 growthbook-1.0.0/PKG-INFO
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    13138 2023-04-23 22:03:31.000000 growthbook-1.0.0/README.md
+drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2023-04-23 22:03:58.537231 growthbook-1.0.0/growthbook.egg-info/
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    17204 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)      256 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)        1 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       39 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/requires.txt
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       11 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/top_level.txt
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    38706 2023-04-23 22:03:31.000000 growthbook-1.0.0/growthbook.py
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)      256 2023-04-23 22:03:58.537231 growthbook-1.0.0/setup.cfg
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)     1339 2023-04-23 22:03:31.000000 growthbook-1.0.0/setup.py
+drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2023-04-23 22:03:58.537231 growthbook-1.0.0/tests/
+-rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    15878 2023-04-23 22:03:31.000000 growthbook-1.0.0/tests/test_growthbook.py
```

### Comparing `growthbook-0.3.1/LICENSE` & `growthbook-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `growthbook-0.3.1/PKG-INFO` & `growthbook-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 Metadata-Version: 2.1
 Name: growthbook
-Version: 0.3.1
+Version: 1.0.0
 Summary: Powerful Feature flagging and A/B testing for Python apps
 Home-page: https://github.com/growthbook/growthbook-python
 Author: GrowthBook
 Author-email: hello@growthbook.io
 License: MIT
 Description: # GrowthBook Python SDK
         
         Powerful Feature flagging and A/B testing for Python apps.
         
         ![Build Status](https://github.com/growthbook/growthbook-python/workflows/Build/badge.svg)
         
-        -  **No external dependencies**
-        -  **Lightweight and fast**
-        -  **No HTTP requests** everything is defined and evaluated locally
-        -  Python 3.6+
-        -  100% test coverage
-        -  Flexible **targeting**
-        -  **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
-        -  **Remote configuration** to change feature flags without deploying new code
+        -   **Lightweight and fast**
+        -   **Local evaluation**, no network requests required
+        -   Python 3.6+
+        -   100% test coverage
+        -   Flexible **targeting**
+        -   **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
+        -   **Remote configuration** to change feature flags without deploying new code
         
         ## Installation
         
         `pip install growthbook` (recommended) or copy `growthbook.py` into your project
         
         ## Quick Usage
         
         ```python
-        import requests
         from growthbook import GrowthBook
         
-        
-        # We recommend using a db or cache layer in production
-        apiResp = requests.get("https://cdn.growthbook.io/api/features/MY_API_KEY")
-        features = apiResp.json()["features"]
-        
         # User attributes for targeting and experimentation
         attributes = {
           "id": "123",
           "customUserAttribute": "foo"
         }
         
         def on_experiment_viewed(experiment, result):
@@ -48,68 +41,150 @@
             'experimentId': experiment.key,
             'variationId': result.variationId
           })
         
         # Create a GrowthBook instance
         gb = GrowthBook(
           attributes = attributes,
-          features = features,
-          trackingCallback = on_experiment_viewed
+          on_experiment_viewed = on_experiment_viewed,
+          api_host = "https://cdn.growthbook.io",
+          client_key = "sdk-abc123"
         )
         
+        # Load features from the GrowthBook API with caching
+        gb.load_features()
+        
         # Simple on/off feature gating
-        if gb.isOn("my-feature"):
+        if gb.is_on("my-feature"):
           print("My feature is on!")
         
         # Get the value of a feature with a fallback
-        color = gb.getFeatureValue("button-color-feature", "blue")
+        color = gb.get_feature_value("button-color-feature", "blue")
         ```
         
-        ## GrowthBook class
+        ### Web Frameworks (Django, Flask, etc.)
         
-        The GrowthBook constructor has the following parameters:
+        For web frameworks, you should create a new `GrowthBook` instance for every incoming request and call `destroy()` at the end of the request to clean up resources.
         
-        -  **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
-        -  **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
-        -  **url** (`str`) - The URL of the current request (if applicable)
-        -  **features** (`dict`) - Feature definitions from the GrowthBook API
-        -  **forcedVariations** (`dict`) - Dictionary of forced experiment variations (used for QA)
-        -  **qaMode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
-        -  **trackingCallback** (`callable`) - A function that takes `experiment` and `result` as arguments.
+        In Django, for example, this is best done with a simple middleware:
         
-        There are also getter and setter methods for features and attributes if you need to update them later in the request:
+        ```python
+        from growthbook import GrowthBook
+        
+        def growthbook_middleware(get_response):
+            def middleware(request):
+                request.gb = GrowthBook(
+                  # ...
+                )
+                request.gb.load_features()
+        
+                response = get_response(request)
+        
+                request.gb.destroy() # Cleanup
+        
+                return response
+            return middleware
+        ```
+        
+        Then, you can easily use GrowthBook in any of your views:
         
         ```python
-        gb.setFeatures(gb.getFeatures())
-        gb.setAttributes(gb.getAttributes())
+        def index(request):
+            feature_enabled = request.gb.is_on("my-feature")
+            # ...
         ```
         
-        ### Features
+        ## Loading Features
         
-        Defines all of the available features plus rules for how to assign values to users. Features are usually fetched from the GrowthBook API and persisted in cache or a database in production.
+        There are two ways to load feature flags into the GrowthBook SDK. You can either use the built-in fetching/caching logic or implement your own custom solution.
         
-        Feature definitions are defined in a JSON format. You can fetch them directly from the GrowthBook API:
+        ### Built-in Fetching and Caching
         
-        ```python
-        import requests
+        To use the built-in fetching and caching logic, in the `GrowthBook` constructor, pass in your GrowthBook `api_host` and `client_key`. If you have encryption enabled for your GrowthBook endpoint, you also need to pass the `decryption_key` into the constructor.
+        
+        Then, call the `load_features()` method to initiate the HTTP request with a cache layer.
+        
+        Here's a full example:
         
-        apiResp = requests.get("https://cdn.growthbook.io/api/features/MY_API_KEY")
-        features = apiResp.json()["features"]
+        ```python
+        gb = GrowthBook(
+          api_host = "https://cdn.growthbook.io",
+          client_key = "sdk-abc123",
+          # How long to cache features in seconds (Optional, default 60s)
+          cache_ttl = 60,
+        )
+        gb.load_features()
         ```
         
-        Or, you can use a copy stored in your database or cache server instead:
+        #### Caching
+        
+        GrowthBook comes with a custom in-memory cache. If you run Python in a multi-process mode, the different processes cannot share memory, so you likely want to switch to a distributed cache system like Redis instead.
+        
+        Here is an example of using Redis:
         
         ```python
+        from redis import Redis
         import json
+        from growthbook import GrowthBook, AbstractFeatureCache, feature_repo
+        
+        class RedisFeatureCache(AbstractFeatureCache):
+          def __init__(self):
+            self.r = Redis(host='localhost', port=6379)
+            self.prefix = "gb:"
+        
+          def get(self, key: str):
+            data = self.r.get(self.prefix + key)
+            # Data stored as a JSON string, parse into dict before returning
+            return None if data is None else json.loads(data)
+        
+          def set(self, key: str, value: dict, ttl: int) -> None:
+            self.r.set(self.prefix + key, json.dumps(value))
+            self.r.expire(self.prefix + key, ttl)
+        
+        # Configure GrowthBook to use your custom cache class
+        feature_repo.set_cache(RedisFeatureCache())
+        ```
+        
+        ### Custom Implementation
+        
+        If you prefer to handle the entire fetching/caching logic yourself, you can just pass in a `dict` of features from the GrowthBook API directly into the constructor:
         
-        json_string = '{"feature-1":{...},"feature-2":{...},...}'
-        features = json.loads(json_string)
+        ```python
+        # From the GrowthBook API
+        features = {'my-feature':{'defaultValue':False}}
+        
+        gb = GrowthBook(
+          features = features
+        )
         ```
         
-        We recommend using the db/cache approach for production.
+        Note: When doing this, you do not need to specify your `api_host` or `client_key` and you don't need to call `gb.load_features()`.
+        
+        ## GrowthBook class
+        
+        The GrowthBook constructor has the following parameters:
+        
+        -   **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
+        -   **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
+        -   **url** (`str`) - The URL of the current request (if applicable)
+        -   **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
+        -   **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
+        -   **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
+        -   **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
+        -   **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
+        -   **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
+        -   **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
+        -   **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
+        
+        There are also getter and setter methods for features and attributes if you need to update them later in the request:
+        
+        ```python
+        gb.set_features(gb.get_features())
+        gb.set_attributes(gb.get_attributes())
+        ```
         
         ### Attributes
         
         You can specify attributes about the current user and request. These are used for two things:
         
         1.  Feature targeting (e.g. paid users get one value, free users get another)
         2.  Assigning persistent variations in A/B tests (e.g. user id "123" always gets variation B)
@@ -120,106 +195,117 @@
         attributes = {
           'id': "123",
           'loggedIn': True,
           'age': 21.5,
           'tags': ["tag1", "tag2"],
           'account': {
             'age': 90
-          ]
+          }
         }
+        
+        # Pass into constructor
+        gb = GrowthBook(attributes = attributes)
+        
+        # Or set later
+        gb.set_attributes(attributes)
         ```
         
         ### Tracking Experiments
         
         Any time an experiment is run to determine the value of a feature, you want to track that event in your analytics system.
         
-        You can use the `trackingCallback` option to do this:
+        You can use the `on_experiment_viewed` option to do this:
         
         ```python
         from growthbook import GrowthBook, Experiment, Result
         
         def on_experiment_viewed(experiment: Experiment, result: Result):
           # Use whatever event tracking system you want
           analytics.track(attributes["id"], "Experiment Viewed", {
             'experimentId': experiment.key,
             'variationId': result.variationId
           })
         
+        # Pass into constructor
         gb = GrowthBook(
-          trackingCallback = on_experiment_viewed
+          on_experiment_viewed = on_experiment_viewed
         )
         ```
         
         ## Using Features
         
         There are 3 main methods for interacting with features.
         
-        - `gb.isOn("feature-key")` returns true if the feature is on
-        - `gb.isOff("feature-key")` returns false if the feature is on
-        - `gb.getFeatureValue("feature-key", "default")` returns the value of the feature with a fallback
-        
+        -   `gb.is_on("feature-key")` returns true if the feature is on
+        -   `gb.is_off("feature-key")` returns false if the feature is on
+        -   `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
         
         In addition, you can use `gb.evalFeature("feature-key")` to get back a `FeatureResult` object with the following properties:
         
-        - **value** - The JSON-decoded value of the feature (or `null` if not defined)
-        - **on** and **off** - The JSON-decoded value cast to booleans
-        - **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
-        - **experiment** - Information about the experiment (if any) which was used to assign the value to the user
-        - **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
-        
+        -   **value** - The JSON-decoded value of the feature (or `None` if not defined)
+        -   **on** and **off** - The JSON-decoded value cast to booleans
+        -   **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
+        -   **experiment** - Information about the experiment (if any) which was used to assign the value to the user
+        -   **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
         
         ## Inline Experiments
         
-        Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `gb->run` method:
+        Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `run` method:
         
         ```python
         from growthbook import Experiment
         
         exp = Experiment(
-          key = "my-experiment", 
+          key = "my-experiment",
           variations = ["red", "blue", "green"]
         )
         
         # Either "red", "blue", or "green"
         print(gb.run(exp).value)
         ```
         
-        As you can see, there are 2 required parameters for experiments, a string key, and an array of variations.  Variations can be any data type, not just strings.
+        As you can see, there are 2 required parameters for experiments, a string key, and an array of variations. Variations can be any data type, not just strings.
         
         There are a number of additional settings to control the experiment behavior:
         
-        -  **key** (`str`) - The globally unique tracking key for the experiment
-        -  **variations** (`any[]`) - The different variations to choose between
-        -  **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
-        -  **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
-        - **condition** (`dict`) - Targeting conditions
-        -  **force** (`int`) - All users included in the experiment will be forced into the specified variation index
-        -  **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
-        -  **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
+        -   **key** (`str`) - The globally unique tracking key for the experiment
+        -   **variations** (`any[]`) - The different variations to choose between
+        -   **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
+        -   **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
+        -   **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
+        -   **condition** (`dict`) - Targeting conditions
+        -   **force** (`int`) - All users included in the experiment will be forced into the specified variation index
+        -   **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
+        -   **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
+        -   **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
         
         Here's an example that uses all of them:
         
         ```python
         exp = Experiment(
           key="my-test",
           # Variations can be a list of any data type
           variations=[0, 1],
+          # If this changes, it will re-randomize all users in the experiment
+          seed="abcdef123456",
           # Run a 40/60 experiment instead of the default even split (50/50)
           weights=[0.4, 0.6],
           # Only include 20% of users in the experiment
           coverage=0.2,
           # Targeting condition using a MongoDB-like syntax
           condition={
             'country': 'US',
             'browser': {
               '$in': ['chrome', 'firefox']
             }
           },
           # Use an alternate attribute for assigning variations (default is 'id')
           hashAttribute="sessionId",
+          # Use the latest hashing algorithm
+          hashVersion=2,
           # Includes the first 50% of users in the "pricing" namespace
           # Another experiment with a non-overlapping range will be mutually exclusive (e.g. [0.5, 1])
           namespace=("pricing", 0, 0.5),
         )
         ```
         
         ### Inline Experiment Return Value
@@ -251,23 +337,25 @@
         The `inExperiment` flag will be false if the user was excluded from being part of the experiment for any reason (e.g. failed targeting conditions).
         
         The `hashUsed` flag will only be true if the user was randomly assigned a variation. If the user was forced into a specific variation instead, this flag will be false.
         
         ### Example Experiments
         
         3-way experiment with uneven variation weights:
+        
         ```python
         gb.run(Experiment(
           key = "3-way-uneven",
           variations = ["A","B","C"],
           weights = [0.5, 0.25, 0.25]
         ))
         ```
         
         Slow rollout (10% of users who match the targeting condition):
+        
         ```python
         # User is marked as being in "qa" and "beta"
         gb = GrowthBook(
           attributes = {
             "id": "123",
             "beta": True,
             "qa": True,
@@ -281,28 +369,30 @@
           condition = {
             'beta': True
           }
         ))
         ```
         
         Complex variations
+        
         ```python
         result = gb.run(Experiment(
           key = "complex-variations",
           variations = [
             ("blue", "large"),
             ("green", "small")
           ],
         ))
         
         # Either "blue,large" OR "green,small"
         print(result.value[0] + "," + result.value[1])
         ```
         
         Assign variations based on something other than user id
+        
         ```python
         gb = GrowthBook(
           attributes = {
             "id": "123",
             "company": "growthbook"
           }
         )
@@ -311,41 +401,32 @@
         gb.run(Experiment(
           key = "by-company-id",
           variations = ["A", "B"],
           hashAttribute = "company"
         ))
         ```
         
-        ### Django
+        ## Logging
         
-        For Django (and other web frameworks), we recommend adding a simple middleware where you instantiate the GrowthBook object
+        The GrowthBook SDK uses a Python logger with the name `growthbook` and includes helpful info for debugging as well as warnings/errors if something is misconfigured.
         
-        ```python
-        from growthbook import GrowthBook
+        Here's an example of logging to the console
         
-        def growthbook_middleware(get_response):
-            def middleware(request):
-                request.gb = GrowthBook(
-                  # ...
-                )
-                response = get_response(request)
+        ```python
+        import logging
         
-                request.gb.destroy() # Cleanup
+        logger = logging.getLogger('growthbook')
+        logger.setLevel(logging.DEBUG)
         
-                return response
-            return middleware
+        handler = logging.StreamHandler()
+        formatter = logging.Formatter('%(asctime)s %(name)s %(levelname)s %(message)s')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
         ```
         
-        Then, you can easily evaluate a feature (or run an inline experiment) in any of your views:
-        
-        ```python
-        def index(request):
-            featureEnabled = request.gb.isOn("my-feature")
-            # ...
-        ```
 Keywords: growthbook
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `growthbook-0.3.1/growthbook.egg-info/PKG-INFO` & `growthbook-1.0.0/growthbook.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 Metadata-Version: 2.1
 Name: growthbook
-Version: 0.3.1
+Version: 1.0.0
 Summary: Powerful Feature flagging and A/B testing for Python apps
 Home-page: https://github.com/growthbook/growthbook-python
 Author: GrowthBook
 Author-email: hello@growthbook.io
 License: MIT
 Description: # GrowthBook Python SDK
         
         Powerful Feature flagging and A/B testing for Python apps.
         
         ![Build Status](https://github.com/growthbook/growthbook-python/workflows/Build/badge.svg)
         
-        -  **No external dependencies**
-        -  **Lightweight and fast**
-        -  **No HTTP requests** everything is defined and evaluated locally
-        -  Python 3.6+
-        -  100% test coverage
-        -  Flexible **targeting**
-        -  **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
-        -  **Remote configuration** to change feature flags without deploying new code
+        -   **Lightweight and fast**
+        -   **Local evaluation**, no network requests required
+        -   Python 3.6+
+        -   100% test coverage
+        -   Flexible **targeting**
+        -   **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
+        -   **Remote configuration** to change feature flags without deploying new code
         
         ## Installation
         
         `pip install growthbook` (recommended) or copy `growthbook.py` into your project
         
         ## Quick Usage
         
         ```python
-        import requests
         from growthbook import GrowthBook
         
-        
-        # We recommend using a db or cache layer in production
-        apiResp = requests.get("https://cdn.growthbook.io/api/features/MY_API_KEY")
-        features = apiResp.json()["features"]
-        
         # User attributes for targeting and experimentation
         attributes = {
           "id": "123",
           "customUserAttribute": "foo"
         }
         
         def on_experiment_viewed(experiment, result):
@@ -48,68 +41,150 @@
             'experimentId': experiment.key,
             'variationId': result.variationId
           })
         
         # Create a GrowthBook instance
         gb = GrowthBook(
           attributes = attributes,
-          features = features,
-          trackingCallback = on_experiment_viewed
+          on_experiment_viewed = on_experiment_viewed,
+          api_host = "https://cdn.growthbook.io",
+          client_key = "sdk-abc123"
         )
         
+        # Load features from the GrowthBook API with caching
+        gb.load_features()
+        
         # Simple on/off feature gating
-        if gb.isOn("my-feature"):
+        if gb.is_on("my-feature"):
           print("My feature is on!")
         
         # Get the value of a feature with a fallback
-        color = gb.getFeatureValue("button-color-feature", "blue")
+        color = gb.get_feature_value("button-color-feature", "blue")
         ```
         
-        ## GrowthBook class
+        ### Web Frameworks (Django, Flask, etc.)
         
-        The GrowthBook constructor has the following parameters:
+        For web frameworks, you should create a new `GrowthBook` instance for every incoming request and call `destroy()` at the end of the request to clean up resources.
         
-        -  **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
-        -  **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
-        -  **url** (`str`) - The URL of the current request (if applicable)
-        -  **features** (`dict`) - Feature definitions from the GrowthBook API
-        -  **forcedVariations** (`dict`) - Dictionary of forced experiment variations (used for QA)
-        -  **qaMode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
-        -  **trackingCallback** (`callable`) - A function that takes `experiment` and `result` as arguments.
+        In Django, for example, this is best done with a simple middleware:
         
-        There are also getter and setter methods for features and attributes if you need to update them later in the request:
+        ```python
+        from growthbook import GrowthBook
+        
+        def growthbook_middleware(get_response):
+            def middleware(request):
+                request.gb = GrowthBook(
+                  # ...
+                )
+                request.gb.load_features()
+        
+                response = get_response(request)
+        
+                request.gb.destroy() # Cleanup
+        
+                return response
+            return middleware
+        ```
+        
+        Then, you can easily use GrowthBook in any of your views:
         
         ```python
-        gb.setFeatures(gb.getFeatures())
-        gb.setAttributes(gb.getAttributes())
+        def index(request):
+            feature_enabled = request.gb.is_on("my-feature")
+            # ...
         ```
         
-        ### Features
+        ## Loading Features
         
-        Defines all of the available features plus rules for how to assign values to users. Features are usually fetched from the GrowthBook API and persisted in cache or a database in production.
+        There are two ways to load feature flags into the GrowthBook SDK. You can either use the built-in fetching/caching logic or implement your own custom solution.
         
-        Feature definitions are defined in a JSON format. You can fetch them directly from the GrowthBook API:
+        ### Built-in Fetching and Caching
         
-        ```python
-        import requests
+        To use the built-in fetching and caching logic, in the `GrowthBook` constructor, pass in your GrowthBook `api_host` and `client_key`. If you have encryption enabled for your GrowthBook endpoint, you also need to pass the `decryption_key` into the constructor.
+        
+        Then, call the `load_features()` method to initiate the HTTP request with a cache layer.
+        
+        Here's a full example:
         
-        apiResp = requests.get("https://cdn.growthbook.io/api/features/MY_API_KEY")
-        features = apiResp.json()["features"]
+        ```python
+        gb = GrowthBook(
+          api_host = "https://cdn.growthbook.io",
+          client_key = "sdk-abc123",
+          # How long to cache features in seconds (Optional, default 60s)
+          cache_ttl = 60,
+        )
+        gb.load_features()
         ```
         
-        Or, you can use a copy stored in your database or cache server instead:
+        #### Caching
+        
+        GrowthBook comes with a custom in-memory cache. If you run Python in a multi-process mode, the different processes cannot share memory, so you likely want to switch to a distributed cache system like Redis instead.
+        
+        Here is an example of using Redis:
         
         ```python
+        from redis import Redis
         import json
+        from growthbook import GrowthBook, AbstractFeatureCache, feature_repo
+        
+        class RedisFeatureCache(AbstractFeatureCache):
+          def __init__(self):
+            self.r = Redis(host='localhost', port=6379)
+            self.prefix = "gb:"
+        
+          def get(self, key: str):
+            data = self.r.get(self.prefix + key)
+            # Data stored as a JSON string, parse into dict before returning
+            return None if data is None else json.loads(data)
+        
+          def set(self, key: str, value: dict, ttl: int) -> None:
+            self.r.set(self.prefix + key, json.dumps(value))
+            self.r.expire(self.prefix + key, ttl)
+        
+        # Configure GrowthBook to use your custom cache class
+        feature_repo.set_cache(RedisFeatureCache())
+        ```
+        
+        ### Custom Implementation
+        
+        If you prefer to handle the entire fetching/caching logic yourself, you can just pass in a `dict` of features from the GrowthBook API directly into the constructor:
         
-        json_string = '{"feature-1":{...},"feature-2":{...},...}'
-        features = json.loads(json_string)
+        ```python
+        # From the GrowthBook API
+        features = {'my-feature':{'defaultValue':False}}
+        
+        gb = GrowthBook(
+          features = features
+        )
         ```
         
-        We recommend using the db/cache approach for production.
+        Note: When doing this, you do not need to specify your `api_host` or `client_key` and you don't need to call `gb.load_features()`.
+        
+        ## GrowthBook class
+        
+        The GrowthBook constructor has the following parameters:
+        
+        -   **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
+        -   **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
+        -   **url** (`str`) - The URL of the current request (if applicable)
+        -   **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
+        -   **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
+        -   **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
+        -   **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
+        -   **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
+        -   **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
+        -   **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
+        -   **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
+        
+        There are also getter and setter methods for features and attributes if you need to update them later in the request:
+        
+        ```python
+        gb.set_features(gb.get_features())
+        gb.set_attributes(gb.get_attributes())
+        ```
         
         ### Attributes
         
         You can specify attributes about the current user and request. These are used for two things:
         
         1.  Feature targeting (e.g. paid users get one value, free users get another)
         2.  Assigning persistent variations in A/B tests (e.g. user id "123" always gets variation B)
@@ -120,106 +195,117 @@
         attributes = {
           'id': "123",
           'loggedIn': True,
           'age': 21.5,
           'tags': ["tag1", "tag2"],
           'account': {
             'age': 90
-          ]
+          }
         }
+        
+        # Pass into constructor
+        gb = GrowthBook(attributes = attributes)
+        
+        # Or set later
+        gb.set_attributes(attributes)
         ```
         
         ### Tracking Experiments
         
         Any time an experiment is run to determine the value of a feature, you want to track that event in your analytics system.
         
-        You can use the `trackingCallback` option to do this:
+        You can use the `on_experiment_viewed` option to do this:
         
         ```python
         from growthbook import GrowthBook, Experiment, Result
         
         def on_experiment_viewed(experiment: Experiment, result: Result):
           # Use whatever event tracking system you want
           analytics.track(attributes["id"], "Experiment Viewed", {
             'experimentId': experiment.key,
             'variationId': result.variationId
           })
         
+        # Pass into constructor
         gb = GrowthBook(
-          trackingCallback = on_experiment_viewed
+          on_experiment_viewed = on_experiment_viewed
         )
         ```
         
         ## Using Features
         
         There are 3 main methods for interacting with features.
         
-        - `gb.isOn("feature-key")` returns true if the feature is on
-        - `gb.isOff("feature-key")` returns false if the feature is on
-        - `gb.getFeatureValue("feature-key", "default")` returns the value of the feature with a fallback
-        
+        -   `gb.is_on("feature-key")` returns true if the feature is on
+        -   `gb.is_off("feature-key")` returns false if the feature is on
+        -   `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
         
         In addition, you can use `gb.evalFeature("feature-key")` to get back a `FeatureResult` object with the following properties:
         
-        - **value** - The JSON-decoded value of the feature (or `null` if not defined)
-        - **on** and **off** - The JSON-decoded value cast to booleans
-        - **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
-        - **experiment** - Information about the experiment (if any) which was used to assign the value to the user
-        - **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
-        
+        -   **value** - The JSON-decoded value of the feature (or `None` if not defined)
+        -   **on** and **off** - The JSON-decoded value cast to booleans
+        -   **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
+        -   **experiment** - Information about the experiment (if any) which was used to assign the value to the user
+        -   **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
         
         ## Inline Experiments
         
-        Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `gb->run` method:
+        Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `run` method:
         
         ```python
         from growthbook import Experiment
         
         exp = Experiment(
-          key = "my-experiment", 
+          key = "my-experiment",
           variations = ["red", "blue", "green"]
         )
         
         # Either "red", "blue", or "green"
         print(gb.run(exp).value)
         ```
         
-        As you can see, there are 2 required parameters for experiments, a string key, and an array of variations.  Variations can be any data type, not just strings.
+        As you can see, there are 2 required parameters for experiments, a string key, and an array of variations. Variations can be any data type, not just strings.
         
         There are a number of additional settings to control the experiment behavior:
         
-        -  **key** (`str`) - The globally unique tracking key for the experiment
-        -  **variations** (`any[]`) - The different variations to choose between
-        -  **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
-        -  **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
-        - **condition** (`dict`) - Targeting conditions
-        -  **force** (`int`) - All users included in the experiment will be forced into the specified variation index
-        -  **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
-        -  **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
+        -   **key** (`str`) - The globally unique tracking key for the experiment
+        -   **variations** (`any[]`) - The different variations to choose between
+        -   **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
+        -   **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
+        -   **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
+        -   **condition** (`dict`) - Targeting conditions
+        -   **force** (`int`) - All users included in the experiment will be forced into the specified variation index
+        -   **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
+        -   **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
+        -   **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
         
         Here's an example that uses all of them:
         
         ```python
         exp = Experiment(
           key="my-test",
           # Variations can be a list of any data type
           variations=[0, 1],
+          # If this changes, it will re-randomize all users in the experiment
+          seed="abcdef123456",
           # Run a 40/60 experiment instead of the default even split (50/50)
           weights=[0.4, 0.6],
           # Only include 20% of users in the experiment
           coverage=0.2,
           # Targeting condition using a MongoDB-like syntax
           condition={
             'country': 'US',
             'browser': {
               '$in': ['chrome', 'firefox']
             }
           },
           # Use an alternate attribute for assigning variations (default is 'id')
           hashAttribute="sessionId",
+          # Use the latest hashing algorithm
+          hashVersion=2,
           # Includes the first 50% of users in the "pricing" namespace
           # Another experiment with a non-overlapping range will be mutually exclusive (e.g. [0.5, 1])
           namespace=("pricing", 0, 0.5),
         )
         ```
         
         ### Inline Experiment Return Value
@@ -251,23 +337,25 @@
         The `inExperiment` flag will be false if the user was excluded from being part of the experiment for any reason (e.g. failed targeting conditions).
         
         The `hashUsed` flag will only be true if the user was randomly assigned a variation. If the user was forced into a specific variation instead, this flag will be false.
         
         ### Example Experiments
         
         3-way experiment with uneven variation weights:
+        
         ```python
         gb.run(Experiment(
           key = "3-way-uneven",
           variations = ["A","B","C"],
           weights = [0.5, 0.25, 0.25]
         ))
         ```
         
         Slow rollout (10% of users who match the targeting condition):
+        
         ```python
         # User is marked as being in "qa" and "beta"
         gb = GrowthBook(
           attributes = {
             "id": "123",
             "beta": True,
             "qa": True,
@@ -281,28 +369,30 @@
           condition = {
             'beta': True
           }
         ))
         ```
         
         Complex variations
+        
         ```python
         result = gb.run(Experiment(
           key = "complex-variations",
           variations = [
             ("blue", "large"),
             ("green", "small")
           ],
         ))
         
         # Either "blue,large" OR "green,small"
         print(result.value[0] + "," + result.value[1])
         ```
         
         Assign variations based on something other than user id
+        
         ```python
         gb = GrowthBook(
           attributes = {
             "id": "123",
             "company": "growthbook"
           }
         )
@@ -311,41 +401,32 @@
         gb.run(Experiment(
           key = "by-company-id",
           variations = ["A", "B"],
           hashAttribute = "company"
         ))
         ```
         
-        ### Django
+        ## Logging
         
-        For Django (and other web frameworks), we recommend adding a simple middleware where you instantiate the GrowthBook object
+        The GrowthBook SDK uses a Python logger with the name `growthbook` and includes helpful info for debugging as well as warnings/errors if something is misconfigured.
         
-        ```python
-        from growthbook import GrowthBook
+        Here's an example of logging to the console
         
-        def growthbook_middleware(get_response):
-            def middleware(request):
-                request.gb = GrowthBook(
-                  # ...
-                )
-                response = get_response(request)
+        ```python
+        import logging
         
-                request.gb.destroy() # Cleanup
+        logger = logging.getLogger('growthbook')
+        logger.setLevel(logging.DEBUG)
         
-                return response
-            return middleware
+        handler = logging.StreamHandler()
+        formatter = logging.Formatter('%(asctime)s %(name)s %(levelname)s %(message)s')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
         ```
         
-        Then, you can easily evaluate a feature (or run an inline experiment) in any of your views:
-        
-        ```python
-        def index(request):
-            featureEnabled = request.gb.isOn("my-feature")
-            # ...
-        ```
 Keywords: growthbook
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `growthbook-0.3.1/setup.py` & `growthbook-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from setuptools import setup
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-requirements = []
+requirements = ['cryptography', 'typing_extensions', 'urllib3', ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     name='growthbook',
-    version='0.3.1',
+    version='1.0.0',
     author="GrowthBook",
     author_email='hello@growthbook.io',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

### Comparing `growthbook-0.3.1/tests/test_growthbook.py` & `growthbook-1.0.0/tests/test_growthbook.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,19 @@
     getBucketRanges,
     gbhash,
     chooseVariation,
     getQueryStringOverride,
     inNamespace,
     getEqualWeights,
     evalCondition,
+    decrypt,
+    feature_repo,
 )
+from time import time
+import pytest
 
 
 def pytest_generate_tests(metafunc):
     folder = os.path.abspath(os.path.dirname(__file__))
     jsonfile = os.path.join(folder, "cases.json")
     with open(jsonfile) as file:
         data = json.load(file)
@@ -26,16 +30,16 @@
     for func, cases in data.items():
         key = func + "_data"
         if key in metafunc.fixturenames:
             metafunc.parametrize(key, cases)
 
 
 def test_hash(hash_data):
-    hashValue, expected = hash_data
-    assert gbhash(hashValue) == expected
+    seed, value, version, expected = hash_data
+    assert gbhash(seed, value, version) == expected
 
 
 def round_list(item):
     is_tuple = type(item) is tuple
 
     if is_tuple:
         item = list(item)
@@ -83,14 +87,22 @@
 
 
 def test_conditions(evalCondition_data):
     _, condition, attributes, expected = evalCondition_data
     assert evalCondition(attributes, condition) == expected
 
 
+def test_decrypt(decrypt_data):
+    _, encrypted, key, expected = decrypt_data
+    try:
+        assert (decrypt(encrypted, key)) == expected
+    except(Exception):
+        assert (expected) is None
+
+
 def test_feature(feature_data):
     _, ctx, key, expected = feature_data
     gb = GrowthBook(**ctx)
     res = gb.evalFeature(key)
 
     if "experiment" in expected:
         expected["experiment"] = Experiment(**expected["experiment"]).to_dict()
@@ -572,7 +584,104 @@
     assert gb.getFeatureValue("featureOff", 10) == 0
 
     assert gb.isOn("featureNone") is False
     assert gb.isOff("featureNone") is True
     assert gb.getFeatureValue("featureNone", 10) == 10
 
     gb.destroy()
+
+
+class MockHttpResp:
+    def __init__(self, status: int, data: str) -> None:
+        self.status = status
+        self.data = data.encode("utf-8")
+
+
+def test_feature_repository(mocker):
+    m = mocker.patch.object(feature_repo, "_get")
+    expected = {"feature": {"defaultValue": 5}}
+    m.return_value = MockHttpResp(200, json.dumps({"features": expected}))
+    features = feature_repo.load_features("https://cdn.growthbook.io", "sdk-abc123")
+
+    m.assert_called_once_with("https://cdn.growthbook.io/api/features/sdk-abc123")
+    assert features == expected
+
+    # Uses in-memory cache for the 2nd call
+    features = feature_repo.load_features("https://cdn.growthbook.io", "sdk-abc123")
+    assert m.call_count == 1
+    assert features == expected
+
+    # Does a new request if cache entry is expired
+    feature_repo.cache.cache["https://cdn.growthbook.io::sdk-abc123"].expires = (
+        time() - 10
+    )
+    features = feature_repo.load_features("https://cdn.growthbook.io", "sdk-abc123")
+    assert m.call_count == 2
+    assert features == expected
+
+    feature_repo.clear_cache()
+
+
+def test_feature_repository_error(mocker):
+    m = mocker.patch.object(feature_repo, "_get")
+    m.return_value = MockHttpResp(400, "400 Error")
+    features = feature_repo.load_features("https://cdn.growthbook.io", "sdk-abc123")
+
+    m.assert_called_once_with("https://cdn.growthbook.io/api/features/sdk-abc123")
+    assert features is None
+
+    # Does not cache errors
+    features = feature_repo.load_features("https://cdn.growthbook.io", "sdk-abc123")
+    assert m.call_count == 2
+    assert features is None
+
+    # Handles broken JSON response
+    m.return_value = MockHttpResp(200, "{'corrupted':6('4")
+    features = feature_repo.load_features("https://cdn.growthbook.io", "sdk-abc123")
+    assert m.call_count == 3
+    assert features is None
+
+    feature_repo.clear_cache()
+
+
+def test_feature_repository_encrypted(mocker):
+    m = mocker.patch.object(feature_repo, "_get")
+    m.return_value = MockHttpResp(
+        200,
+        json.dumps(
+            {
+                "features": {},
+                "encryptedFeatures": "m5ylFM6ndyOJA2OPadubkw==.Uu7ViqgKEt/dWvCyhI46q088PkAEJbnXKf3KPZjf9IEQQ+A8fojNoxw4wIbPX3aj",
+            }
+        ),
+    )
+    features = feature_repo.load_features(
+        "https://cdn.growthbook.io", "sdk-abc123", "Zvwv/+uhpFDznZ6SX28Yjg=="
+    )
+
+    m.assert_called_once_with("https://cdn.growthbook.io/api/features/sdk-abc123")
+    assert features == {"feature": {"defaultValue": True}}
+
+    feature_repo.clear_cache()
+
+    # Raises exception if missing decryption key
+    with pytest.raises(Exception):
+        feature_repo.load_features("https://cdn.growthbook.io", "sdk-abc123")
+
+
+def test_load_features(mocker):
+    m = mocker.patch.object(feature_repo, "_get")
+    m.return_value = MockHttpResp(
+        200, json.dumps({"features": {"feature": {"defaultValue": 5}}})
+    )
+
+    gb = GrowthBook(api_host="https://cdn.growthbook.io", client_key="sdk-abc123")
+
+    assert m.call_count == 0
+
+    gb.load_features()
+    m.assert_called_once_with("https://cdn.growthbook.io/api/features/sdk-abc123")
+
+    assert gb.get_features()["feature"].to_dict() == {"defaultValue": 5, "rules": []}
+
+    feature_repo.clear_cache()
+    gb.destroy()
```

