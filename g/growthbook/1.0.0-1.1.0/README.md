# Comparing `tmp/growthbook-1.0.0.tar.gz` & `tmp/growthbook-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/growthbook-1.0.0.tar", last modified: Sun Apr 23 22:03:58 2023, max compression
+gzip compressed data, was "growthbook-1.1.0.tar", last modified: Fri Apr 12 02:40:54 2024, max compression
```

## Comparing `growthbook-1.0.0.tar` & `growthbook-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2023-04-23 22:03:58.537231 growthbook-1.0.0/
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)     1069 2022-02-13 16:34:23.000000 growthbook-1.0.0/LICENSE
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       91 2021-09-16 22:25:57.000000 growthbook-1.0.0/MANIFEST.in
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    17204 2023-04-23 22:03:58.537231 growthbook-1.0.0/PKG-INFO
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    13138 2023-04-23 22:03:31.000000 growthbook-1.0.0/README.md
-drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2023-04-23 22:03:58.537231 growthbook-1.0.0/growthbook.egg-info/
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    17204 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/PKG-INFO
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)      256 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)        1 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       39 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/requires.txt
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)       11 2023-04-23 22:03:58.000000 growthbook-1.0.0/growthbook.egg-info/top_level.txt
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    38706 2023-04-23 22:03:31.000000 growthbook-1.0.0/growthbook.py
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)      256 2023-04-23 22:03:58.537231 growthbook-1.0.0/setup.cfg
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)     1339 2023-04-23 22:03:31.000000 growthbook-1.0.0/setup.py
-drwxrwxr-x   0 jeremy    (1001) jeremy    (1001)        0 2023-04-23 22:03:58.537231 growthbook-1.0.0/tests/
--rw-rw-r--   0 jeremy    (1001) jeremy    (1001)    15878 2023-04-23 22:03:31.000000 growthbook-1.0.0/tests/test_growthbook.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-12 02:40:54.048325 growthbook-1.1.0/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1069 2023-08-11 12:28:52.000000 growthbook-1.1.0/LICENSE
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       91 2023-08-11 12:28:52.000000 growthbook-1.1.0/MANIFEST.in
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16202 2024-04-12 02:40:54.048325 growthbook-1.1.0/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    15250 2024-04-12 01:39:53.000000 growthbook-1.1.0/README.md
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-12 02:40:54.048325 growthbook-1.1.0/growthbook.egg-info/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16202 2024-04-12 02:40:54.000000 growthbook-1.1.0/growthbook.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      256 2024-04-12 02:40:54.000000 growthbook-1.1.0/growthbook.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-12 02:40:54.000000 growthbook-1.1.0/growthbook.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       39 2024-04-12 02:40:54.000000 growthbook-1.1.0/growthbook.egg-info/requires.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       11 2024-04-12 02:40:54.000000 growthbook-1.1.0/growthbook.egg-info/top_level.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    58402 2024-04-11 19:15:14.000000 growthbook-1.1.0/growthbook.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      256 2024-04-12 02:40:54.048325 growthbook-1.1.0/setup.cfg
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1538 2024-04-10 23:56:08.000000 growthbook-1.1.0/setup.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-12 02:40:54.048325 growthbook-1.1.0/tests/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    22935 2024-04-10 03:59:03.000000 growthbook-1.1.0/tests/test_growthbook.py
```

### Comparing `growthbook-1.0.0/LICENSE` & `growthbook-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `growthbook-1.0.0/PKG-INFO` & `growthbook-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,437 +1,491 @@
 Metadata-Version: 2.1
 Name: growthbook
-Version: 1.0.0
+Version: 1.1.0
 Summary: Powerful Feature flagging and A/B testing for Python apps
 Home-page: https://github.com/growthbook/growthbook-python
 Author: GrowthBook
 Author-email: hello@growthbook.io
 License: MIT
-Description: # GrowthBook Python SDK
-        
-        Powerful Feature flagging and A/B testing for Python apps.
-        
-        ![Build Status](https://github.com/growthbook/growthbook-python/workflows/Build/badge.svg)
-        
-        -   **Lightweight and fast**
-        -   **Local evaluation**, no network requests required
-        -   Python 3.6+
-        -   100% test coverage
-        -   Flexible **targeting**
-        -   **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
-        -   **Remote configuration** to change feature flags without deploying new code
-        
-        ## Installation
-        
-        `pip install growthbook` (recommended) or copy `growthbook.py` into your project
-        
-        ## Quick Usage
-        
-        ```python
-        from growthbook import GrowthBook
-        
-        # User attributes for targeting and experimentation
-        attributes = {
-          "id": "123",
-          "customUserAttribute": "foo"
-        }
-        
-        def on_experiment_viewed(experiment, result):
-          # Use whatever event tracking system you want
-          analytics.track(attributes["id"], "Experiment Viewed", {
-            'experimentId': experiment.key,
-            'variationId': result.variationId
-          })
-        
-        # Create a GrowthBook instance
-        gb = GrowthBook(
-          attributes = attributes,
-          on_experiment_viewed = on_experiment_viewed,
-          api_host = "https://cdn.growthbook.io",
-          client_key = "sdk-abc123"
-        )
-        
-        # Load features from the GrowthBook API with caching
-        gb.load_features()
-        
-        # Simple on/off feature gating
-        if gb.is_on("my-feature"):
-          print("My feature is on!")
-        
-        # Get the value of a feature with a fallback
-        color = gb.get_feature_value("button-color-feature", "blue")
-        ```
-        
-        ### Web Frameworks (Django, Flask, etc.)
-        
-        For web frameworks, you should create a new `GrowthBook` instance for every incoming request and call `destroy()` at the end of the request to clean up resources.
-        
-        In Django, for example, this is best done with a simple middleware:
-        
-        ```python
-        from growthbook import GrowthBook
-        
-        def growthbook_middleware(get_response):
-            def middleware(request):
-                request.gb = GrowthBook(
-                  # ...
-                )
-                request.gb.load_features()
-        
-                response = get_response(request)
-        
-                request.gb.destroy() # Cleanup
-        
-                return response
-            return middleware
-        ```
-        
-        Then, you can easily use GrowthBook in any of your views:
-        
-        ```python
-        def index(request):
-            feature_enabled = request.gb.is_on("my-feature")
-            # ...
-        ```
-        
-        ## Loading Features
-        
-        There are two ways to load feature flags into the GrowthBook SDK. You can either use the built-in fetching/caching logic or implement your own custom solution.
-        
-        ### Built-in Fetching and Caching
-        
-        To use the built-in fetching and caching logic, in the `GrowthBook` constructor, pass in your GrowthBook `api_host` and `client_key`. If you have encryption enabled for your GrowthBook endpoint, you also need to pass the `decryption_key` into the constructor.
-        
-        Then, call the `load_features()` method to initiate the HTTP request with a cache layer.
-        
-        Here's a full example:
-        
-        ```python
-        gb = GrowthBook(
-          api_host = "https://cdn.growthbook.io",
-          client_key = "sdk-abc123",
-          # How long to cache features in seconds (Optional, default 60s)
-          cache_ttl = 60,
-        )
-        gb.load_features()
-        ```
-        
-        #### Caching
-        
-        GrowthBook comes with a custom in-memory cache. If you run Python in a multi-process mode, the different processes cannot share memory, so you likely want to switch to a distributed cache system like Redis instead.
-        
-        Here is an example of using Redis:
-        
-        ```python
-        from redis import Redis
-        import json
-        from growthbook import GrowthBook, AbstractFeatureCache, feature_repo
-        
-        class RedisFeatureCache(AbstractFeatureCache):
-          def __init__(self):
-            self.r = Redis(host='localhost', port=6379)
-            self.prefix = "gb:"
-        
-          def get(self, key: str):
-            data = self.r.get(self.prefix + key)
-            # Data stored as a JSON string, parse into dict before returning
-            return None if data is None else json.loads(data)
-        
-          def set(self, key: str, value: dict, ttl: int) -> None:
-            self.r.set(self.prefix + key, json.dumps(value))
-            self.r.expire(self.prefix + key, ttl)
-        
-        # Configure GrowthBook to use your custom cache class
-        feature_repo.set_cache(RedisFeatureCache())
-        ```
-        
-        ### Custom Implementation
-        
-        If you prefer to handle the entire fetching/caching logic yourself, you can just pass in a `dict` of features from the GrowthBook API directly into the constructor:
-        
-        ```python
-        # From the GrowthBook API
-        features = {'my-feature':{'defaultValue':False}}
-        
-        gb = GrowthBook(
-          features = features
-        )
-        ```
-        
-        Note: When doing this, you do not need to specify your `api_host` or `client_key` and you don't need to call `gb.load_features()`.
-        
-        ## GrowthBook class
-        
-        The GrowthBook constructor has the following parameters:
-        
-        -   **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
-        -   **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
-        -   **url** (`str`) - The URL of the current request (if applicable)
-        -   **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
-        -   **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
-        -   **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
-        -   **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
-        -   **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
-        -   **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
-        -   **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
-        -   **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
-        
-        There are also getter and setter methods for features and attributes if you need to update them later in the request:
-        
-        ```python
-        gb.set_features(gb.get_features())
-        gb.set_attributes(gb.get_attributes())
-        ```
-        
-        ### Attributes
-        
-        You can specify attributes about the current user and request. These are used for two things:
-        
-        1.  Feature targeting (e.g. paid users get one value, free users get another)
-        2.  Assigning persistent variations in A/B tests (e.g. user id "123" always gets variation B)
-        
-        Attributes can be any JSON data type - boolean, integer, float, string, list, or dict.
-        
-        ```python
-        attributes = {
-          'id': "123",
-          'loggedIn': True,
-          'age': 21.5,
-          'tags': ["tag1", "tag2"],
-          'account': {
-            'age': 90
-          }
-        }
-        
-        # Pass into constructor
-        gb = GrowthBook(attributes = attributes)
-        
-        # Or set later
-        gb.set_attributes(attributes)
-        ```
-        
-        ### Tracking Experiments
-        
-        Any time an experiment is run to determine the value of a feature, you want to track that event in your analytics system.
-        
-        You can use the `on_experiment_viewed` option to do this:
-        
-        ```python
-        from growthbook import GrowthBook, Experiment, Result
-        
-        def on_experiment_viewed(experiment: Experiment, result: Result):
-          # Use whatever event tracking system you want
-          analytics.track(attributes["id"], "Experiment Viewed", {
-            'experimentId': experiment.key,
-            'variationId': result.variationId
-          })
-        
-        # Pass into constructor
-        gb = GrowthBook(
-          on_experiment_viewed = on_experiment_viewed
-        )
-        ```
-        
-        ## Using Features
-        
-        There are 3 main methods for interacting with features.
-        
-        -   `gb.is_on("feature-key")` returns true if the feature is on
-        -   `gb.is_off("feature-key")` returns false if the feature is on
-        -   `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
-        
-        In addition, you can use `gb.evalFeature("feature-key")` to get back a `FeatureResult` object with the following properties:
-        
-        -   **value** - The JSON-decoded value of the feature (or `None` if not defined)
-        -   **on** and **off** - The JSON-decoded value cast to booleans
-        -   **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
-        -   **experiment** - Information about the experiment (if any) which was used to assign the value to the user
-        -   **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
-        
-        ## Inline Experiments
-        
-        Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `run` method:
-        
-        ```python
-        from growthbook import Experiment
-        
-        exp = Experiment(
-          key = "my-experiment",
-          variations = ["red", "blue", "green"]
-        )
-        
-        # Either "red", "blue", or "green"
-        print(gb.run(exp).value)
-        ```
-        
-        As you can see, there are 2 required parameters for experiments, a string key, and an array of variations. Variations can be any data type, not just strings.
-        
-        There are a number of additional settings to control the experiment behavior:
-        
-        -   **key** (`str`) - The globally unique tracking key for the experiment
-        -   **variations** (`any[]`) - The different variations to choose between
-        -   **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
-        -   **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
-        -   **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
-        -   **condition** (`dict`) - Targeting conditions
-        -   **force** (`int`) - All users included in the experiment will be forced into the specified variation index
-        -   **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
-        -   **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
-        -   **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
-        
-        Here's an example that uses all of them:
-        
-        ```python
-        exp = Experiment(
-          key="my-test",
-          # Variations can be a list of any data type
-          variations=[0, 1],
-          # If this changes, it will re-randomize all users in the experiment
-          seed="abcdef123456",
-          # Run a 40/60 experiment instead of the default even split (50/50)
-          weights=[0.4, 0.6],
-          # Only include 20% of users in the experiment
-          coverage=0.2,
-          # Targeting condition using a MongoDB-like syntax
-          condition={
-            'country': 'US',
-            'browser': {
-              '$in': ['chrome', 'firefox']
-            }
-          },
-          # Use an alternate attribute for assigning variations (default is 'id')
-          hashAttribute="sessionId",
-          # Use the latest hashing algorithm
-          hashVersion=2,
-          # Includes the first 50% of users in the "pricing" namespace
-          # Another experiment with a non-overlapping range will be mutually exclusive (e.g. [0.5, 1])
-          namespace=("pricing", 0, 0.5),
-        )
-        ```
-        
-        ### Inline Experiment Return Value
-        
-        A call to `run` returns a `Result` object with a few useful properties:
-        
-        ```python
-        result = gb.run(exp)
-        
-        # If user is part of the experiment
-        print(result.inExperiment) # True or False
-        
-        # The index of the assigned variation
-        print(result.variationId) # e.g. 0 or 1
-        
-        # The value of the assigned variation
-        print(result.value) # e.g. "A" or "B"
-        
-        # If the variation was randomly assigned by hashing user attributes
-        print(result.hashUsed) # True or False
-        
-        # The user attribute used to assign a variation
-        print(result.hashAttribute) # "id"
-        
-        # The value of that attribute
-        print(result.hashValue) # e.g. "123"
-        ```
-        
-        The `inExperiment` flag will be false if the user was excluded from being part of the experiment for any reason (e.g. failed targeting conditions).
-        
-        The `hashUsed` flag will only be true if the user was randomly assigned a variation. If the user was forced into a specific variation instead, this flag will be false.
-        
-        ### Example Experiments
-        
-        3-way experiment with uneven variation weights:
-        
-        ```python
-        gb.run(Experiment(
-          key = "3-way-uneven",
-          variations = ["A","B","C"],
-          weights = [0.5, 0.25, 0.25]
-        ))
-        ```
-        
-        Slow rollout (10% of users who match the targeting condition):
-        
-        ```python
-        # User is marked as being in "qa" and "beta"
-        gb = GrowthBook(
-          attributes = {
-            "id": "123",
-            "beta": True,
-            "qa": True,
-          },
-        )
-        
-        gb.run(Experiment(
-          key = "slow-rollout",
-          variations = ["A", "B"],
-          coverage = 0.1,
-          condition = {
-            'beta': True
-          }
-        ))
-        ```
-        
-        Complex variations
-        
-        ```python
-        result = gb.run(Experiment(
-          key = "complex-variations",
-          variations = [
-            ("blue", "large"),
-            ("green", "small")
-          ],
-        ))
-        
-        # Either "blue,large" OR "green,small"
-        print(result.value[0] + "," + result.value[1])
-        ```
-        
-        Assign variations based on something other than user id
-        
-        ```python
-        gb = GrowthBook(
-          attributes = {
-            "id": "123",
-            "company": "growthbook"
-          }
-        )
-        
-        # Users in the same company will always get the same variation
-        gb.run(Experiment(
-          key = "by-company-id",
-          variations = ["A", "B"],
-          hashAttribute = "company"
-        ))
-        ```
-        
-        ## Logging
-        
-        The GrowthBook SDK uses a Python logger with the name `growthbook` and includes helpful info for debugging as well as warnings/errors if something is misconfigured.
-        
-        Here's an example of logging to the console
-        
-        ```python
-        import logging
-        
-        logger = logging.getLogger('growthbook')
-        logger.setLevel(logging.DEBUG)
-        
-        handler = logging.StreamHandler()
-        formatter = logging.Formatter('%(asctime)s %(name)s %(levelname)s %(message)s')
-        handler.setFormatter(formatter)
-        logger.addHandler(handler)
-        ```
-        
 Keywords: growthbook
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GrowthBook Python SDK
+
+Powerful Feature flagging and A/B testing for Python apps.
+
+![Build Status](https://github.com/growthbook/growthbook-python/workflows/Build/badge.svg)
+
+- **Lightweight and fast**
+- **Local evaluation**, no network requests required
+- Python 3.6+
+- 100% test coverage
+- Flexible **targeting**
+- **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
+- **Remote configuration** to change feature flags without deploying new code
+
+## Installation
+
+`pip install growthbook` (recommended) or copy `growthbook.py` into your project
+
+## Quick Usage
+
+```python
+from growthbook import GrowthBook
+
+# User attributes for targeting and experimentation
+attributes = {
+  "id": "123",
+  "customUserAttribute": "foo"
+}
+
+def on_experiment_viewed(experiment, result):
+  # Use whatever event tracking system you want
+  analytics.track(attributes["id"], "Experiment Viewed", {
+    'experimentId': experiment.key,
+    'variationId': result.variationId
+  })
+
+# Create a GrowthBook instance
+gb = GrowthBook(
+  attributes = attributes,
+  on_experiment_viewed = on_experiment_viewed,
+  api_host = "https://cdn.growthbook.io",
+  client_key = "sdk-abc123"
+)
+
+# Load features from the GrowthBook API with caching
+gb.load_features()
+
+# Simple on/off feature gating
+if gb.is_on("my-feature"):
+  print("My feature is on!")
+
+# Get the value of a feature with a fallback
+color = gb.get_feature_value("button-color-feature", "blue")
+```
+
+### Web Frameworks (Django, Flask, etc.)
+
+For web frameworks, you should create a new `GrowthBook` instance for every incoming request and call `destroy()` at the end of the request to clean up resources.
+
+In Django, for example, this is best done with a simple middleware:
+
+```python
+from growthbook import GrowthBook
+
+def growthbook_middleware(get_response):
+    def middleware(request):
+        request.gb = GrowthBook(
+          # ...
+        )
+        request.gb.load_features()
+
+        response = get_response(request)
+
+        request.gb.destroy() # Cleanup
+
+        return response
+    return middleware
+```
+
+Then, you can easily use GrowthBook in any of your views:
+
+```python
+def index(request):
+    feature_enabled = request.gb.is_on("my-feature")
+    # ...
+```
+
+## Loading Features
+
+There are two ways to load feature flags into the GrowthBook SDK. You can either use the built-in fetching/caching logic or implement your own custom solution.
+
+### Built-in Fetching and Caching
+
+To use the built-in fetching and caching logic, in the `GrowthBook` constructor, pass in your GrowthBook `api_host` and `client_key`. If you have encryption enabled for your GrowthBook endpoint, you also need to pass the `decryption_key` into the constructor.
+
+Then, call the `load_features()` method to initiate the HTTP request with a cache layer.
+
+Here's a full example:
+
+```python
+gb = GrowthBook(
+  api_host = "https://cdn.growthbook.io",
+  client_key = "sdk-abc123",
+  # How long to cache features in seconds (Optional, default 60s)
+  cache_ttl = 60,
+)
+gb.load_features()
+```
+
+#### Caching
+
+GrowthBook comes with a custom in-memory cache. If you run Python in a multi-process mode, the different processes cannot share memory, so you likely want to switch to a distributed cache system like Redis instead.
+
+Here is an example of using Redis:
+
+```python
+from redis import Redis
+import json
+from growthbook import GrowthBook, AbstractFeatureCache, feature_repo
+
+class RedisFeatureCache(AbstractFeatureCache):
+  def __init__(self):
+    self.r = Redis(host='localhost', port=6379)
+    self.prefix = "gb:"
+
+  def get(self, key: str):
+    data = self.r.get(self.prefix + key)
+    # Data stored as a JSON string, parse into dict before returning
+    return None if data is None else json.loads(data)
+
+  def set(self, key: str, value: dict, ttl: int) -> None:
+    self.r.set(self.prefix + key, json.dumps(value))
+    self.r.expire(self.prefix + key, ttl)
+
+# Configure GrowthBook to use your custom cache class
+feature_repo.set_cache(RedisFeatureCache())
+```
+
+### Custom Implementation
+
+If you prefer to handle the entire fetching/caching logic yourself, you can just pass in a `dict` of features from the GrowthBook API directly into the constructor:
+
+```python
+# From the GrowthBook API
+features = {'my-feature':{'defaultValue':False}}
+
+gb = GrowthBook(
+  features = features
+)
+```
+
+Note: When doing this, you do not need to specify your `api_host` or `client_key` and you don't need to call `gb.load_features()`.
+
+## GrowthBook class
+
+The GrowthBook constructor has the following parameters:
+
+- **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
+- **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
+- **url** (`str`) - The URL of the current request (if applicable)
+- **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
+- **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
+- **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
+- **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
+- **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
+- **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
+- **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
+- **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
+
+There are also getter and setter methods for features and attributes if you need to update them later in the request:
+
+```python
+gb.set_features(gb.get_features())
+gb.set_attributes(gb.get_attributes())
+```
+
+### Attributes
+
+You can specify attributes about the current user and request. These are used for two things:
+
+1.  Feature targeting (e.g. paid users get one value, free users get another)
+2.  Assigning persistent variations in A/B tests (e.g. user id "123" always gets variation B)
+
+Attributes can be any JSON data type - boolean, integer, float, string, list, or dict.
+
+```python
+attributes = {
+  'id': "123",
+  'loggedIn': True,
+  'age': 21.5,
+  'tags': ["tag1", "tag2"],
+  'account': {
+    'age': 90
+  }
+}
+
+# Pass into constructor
+gb = GrowthBook(attributes = attributes)
+
+# Or set later
+gb.set_attributes(attributes)
+```
+
+### Tracking Experiments
+
+Any time an experiment is run to determine the value of a feature, you want to track that event in your analytics system.
+
+You can use the `on_experiment_viewed` option to do this:
+
+```python
+from growthbook import GrowthBook, Experiment, Result
+
+def on_experiment_viewed(experiment: Experiment, result: Result):
+  # Use whatever event tracking system you want
+  analytics.track(attributes["id"], "Experiment Viewed", {
+    'experimentId': experiment.key,
+    'variationId': result.variationId
+  })
+
+# Pass into constructor
+gb = GrowthBook(
+  on_experiment_viewed = on_experiment_viewed
+)
+```
+
+## Using Features
+
+There are 3 main methods for interacting with features.
+
+- `gb.is_on("feature-key")` returns true if the feature is on
+- `gb.is_off("feature-key")` returns false if the feature is on
+- `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
+
+In addition, you can use `gb.evalFeature("feature-key")` to get back a `FeatureResult` object with the following properties:
+
+- **value** - The JSON-decoded value of the feature (or `None` if not defined)
+- **on** and **off** - The JSON-decoded value cast to booleans
+- **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
+- **experiment** - Information about the experiment (if any) which was used to assign the value to the user
+- **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
+
+## Sticky Bucketing
+
+By default GrowthBook does not persist assigned experiment variations for a user. We rely on deterministic hashing to ensure that the same user attributes always map to the same experiment variation. However, there are cases where this isn't good enough. For example, if you change targeting conditions in the middle of an experiment, users may stop being shown a variation even if they were previously bucketed into it.
+
+Sticky Bucketing is a solution to these issues. You can provide a Sticky Bucket Service to the GrowthBook instance to persist previously seen variations and ensure that the user experience remains consistent for your users.
+
+A sample `InMemoryStickyBucketService` implementation is provided for reference, but in production you will definitely want to implement your own version using a database, cookies, or similar for persistence.
+
+Sticky Bucket documents contain three fields
+
+- `attributeName` - The name of the attribute used to identify the user (e.g. `id`, `cookie_id`, etc.)
+- `attributeValue` - The value of the attribute (e.g. `123`)
+- `assignments` - A dictionary of persisted experiment assignments. For example: `{"exp1__0":"control"}`
+
+The attributeName/attributeValue combo is the primary key.
+
+Here's an example implementation using a theoretical `db` object:
+
+```python
+from growthbook import AbstractStickyBucketService, GrowthBook
+
+class MyStickyBucketService(AbstractStickyBucketService):
+    # Lookup a sticky bucket document
+    def get_assignments(self, attributeName: str, attributeValue: str) -> Optional[Dict]:
+        return db.find({
+          "attributeName": attributeName,
+          "attributeValue": attributeValue
+        })
+
+    def save_assignments(self, doc: Dict) -> None:
+        # Insert new record if not exists, otherwise update
+        db.upsert({
+            "attributeName": doc["attributeName"],
+            "attributeValue": doc["attributeValue"]
+        }, {
+          "$set": {
+            "assignments": doc["assignments"]
+          }
+        })
+
+# Pass in an instance of this service to your GrowthBook constructor
+
+gb = GrowthBook(
+  sticky_bucket_service = MyStickyBucketService()
+)
+```
+
+## Inline Experiments
+
+Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `run` method:
+
+```python
+from growthbook import Experiment
+
+exp = Experiment(
+  key = "my-experiment",
+  variations = ["red", "blue", "green"]
+)
+
+# Either "red", "blue", or "green"
+print(gb.run(exp).value)
+```
+
+As you can see, there are 2 required parameters for experiments, a string key, and an array of variations. Variations can be any data type, not just strings.
+
+There are a number of additional settings to control the experiment behavior:
+
+- **key** (`str`) - The globally unique tracking key for the experiment
+- **variations** (`any[]`) - The different variations to choose between
+- **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
+- **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
+- **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
+- **condition** (`dict`) - Targeting conditions
+- **force** (`int`) - All users included in the experiment will be forced into the specified variation index
+- **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
+- **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
+- **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
+
+Here's an example that uses all of them:
+
+```python
+exp = Experiment(
+  key="my-test",
+  # Variations can be a list of any data type
+  variations=[0, 1],
+  # If this changes, it will re-randomize all users in the experiment
+  seed="abcdef123456",
+  # Run a 40/60 experiment instead of the default even split (50/50)
+  weights=[0.4, 0.6],
+  # Only include 20% of users in the experiment
+  coverage=0.2,
+  # Targeting condition using a MongoDB-like syntax
+  condition={
+    'country': 'US',
+    'browser': {
+      '$in': ['chrome', 'firefox']
+    }
+  },
+  # Use an alternate attribute for assigning variations (default is 'id')
+  hashAttribute="sessionId",
+  # Use the latest hashing algorithm
+  hashVersion=2,
+  # Includes the first 50% of users in the "pricing" namespace
+  # Another experiment with a non-overlapping range will be mutually exclusive (e.g. [0.5, 1])
+  namespace=("pricing", 0, 0.5),
+)
+```
+
+### Inline Experiment Return Value
+
+A call to `run` returns a `Result` object with a few useful properties:
+
+```python
+result = gb.run(exp)
+
+# If user is part of the experiment
+print(result.inExperiment) # True or False
+
+# The index of the assigned variation
+print(result.variationId) # e.g. 0 or 1
+
+# The value of the assigned variation
+print(result.value) # e.g. "A" or "B"
+
+# If the variation was randomly assigned by hashing user attributes
+print(result.hashUsed) # True or False
+
+# The user attribute used to assign a variation
+print(result.hashAttribute) # "id"
+
+# The value of that attribute
+print(result.hashValue) # e.g. "123"
+```
+
+The `inExperiment` flag will be false if the user was excluded from being part of the experiment for any reason (e.g. failed targeting conditions).
+
+The `hashUsed` flag will only be true if the user was randomly assigned a variation. If the user was forced into a specific variation instead, this flag will be false.
+
+### Example Experiments
+
+3-way experiment with uneven variation weights:
+
+```python
+gb.run(Experiment(
+  key = "3-way-uneven",
+  variations = ["A","B","C"],
+  weights = [0.5, 0.25, 0.25]
+))
+```
+
+Slow rollout (10% of users who match the targeting condition):
+
+```python
+# User is marked as being in "qa" and "beta"
+gb = GrowthBook(
+  attributes = {
+    "id": "123",
+    "beta": True,
+    "qa": True,
+  },
+)
+
+gb.run(Experiment(
+  key = "slow-rollout",
+  variations = ["A", "B"],
+  coverage = 0.1,
+  condition = {
+    'beta': True
+  }
+))
+```
+
+Complex variations
+
+```python
+result = gb.run(Experiment(
+  key = "complex-variations",
+  variations = [
+    ("blue", "large"),
+    ("green", "small")
+  ],
+))
+
+# Either "blue,large" OR "green,small"
+print(result.value[0] + "," + result.value[1])
+```
+
+Assign variations based on something other than user id
+
+```python
+gb = GrowthBook(
+  attributes = {
+    "id": "123",
+    "company": "growthbook"
+  }
+)
+
+# Users in the same company will always get the same variation
+gb.run(Experiment(
+  key = "by-company-id",
+  variations = ["A", "B"],
+  hashAttribute = "company"
+))
+```
+
+## Logging
+
+The GrowthBook SDK uses a Python logger with the name `growthbook` and includes helpful info for debugging as well as warnings/errors if something is misconfigured.
+
+Here's an example of logging to the console
+
+```python
+import logging
+
+logger = logging.getLogger('growthbook')
+logger.setLevel(logging.DEBUG)
+
+handler = logging.StreamHandler()
+formatter = logging.Formatter('%(asctime)s %(name)s %(levelname)s %(message)s')
+handler.setFormatter(formatter)
+logger.addHandler(handler)
+```
+
+
```

### Comparing `growthbook-1.0.0/README.md` & `growthbook-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # GrowthBook Python SDK
 
 Powerful Feature flagging and A/B testing for Python apps.
 
 ![Build Status](https://github.com/growthbook/growthbook-python/workflows/Build/badge.svg)
 
--   **Lightweight and fast**
--   **Local evaluation**, no network requests required
--   Python 3.6+
--   100% test coverage
--   Flexible **targeting**
--   **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
--   **Remote configuration** to change feature flags without deploying new code
+- **Lightweight and fast**
+- **Local evaluation**, no network requests required
+- Python 3.6+
+- 100% test coverage
+- Flexible **targeting**
+- **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
+- **Remote configuration** to change feature flags without deploying new code
 
 ## Installation
 
 `pip install growthbook` (recommended) or copy `growthbook.py` into your project
 
 ## Quick Usage
 
@@ -151,25 +151,25 @@
 
 Note: When doing this, you do not need to specify your `api_host` or `client_key` and you don't need to call `gb.load_features()`.
 
 ## GrowthBook class
 
 The GrowthBook constructor has the following parameters:
 
--   **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
--   **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
--   **url** (`str`) - The URL of the current request (if applicable)
--   **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
--   **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
--   **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
--   **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
--   **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
--   **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
--   **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
--   **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
+- **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
+- **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
+- **url** (`str`) - The URL of the current request (if applicable)
+- **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
+- **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
+- **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
+- **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
+- **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
+- **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
+- **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
+- **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
 
 There are also getter and setter methods for features and attributes if you need to update them later in the request:
 
 ```python
 gb.set_features(gb.get_features())
 gb.set_attributes(gb.get_attributes())
 ```
@@ -223,25 +223,72 @@
 )
 ```
 
 ## Using Features
 
 There are 3 main methods for interacting with features.
 
--   `gb.is_on("feature-key")` returns true if the feature is on
--   `gb.is_off("feature-key")` returns false if the feature is on
--   `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
+- `gb.is_on("feature-key")` returns true if the feature is on
+- `gb.is_off("feature-key")` returns false if the feature is on
+- `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
 
 In addition, you can use `gb.evalFeature("feature-key")` to get back a `FeatureResult` object with the following properties:
 
--   **value** - The JSON-decoded value of the feature (or `None` if not defined)
--   **on** and **off** - The JSON-decoded value cast to booleans
--   **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
--   **experiment** - Information about the experiment (if any) which was used to assign the value to the user
--   **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
+- **value** - The JSON-decoded value of the feature (or `None` if not defined)
+- **on** and **off** - The JSON-decoded value cast to booleans
+- **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
+- **experiment** - Information about the experiment (if any) which was used to assign the value to the user
+- **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
+
+## Sticky Bucketing
+
+By default GrowthBook does not persist assigned experiment variations for a user. We rely on deterministic hashing to ensure that the same user attributes always map to the same experiment variation. However, there are cases where this isn't good enough. For example, if you change targeting conditions in the middle of an experiment, users may stop being shown a variation even if they were previously bucketed into it.
+
+Sticky Bucketing is a solution to these issues. You can provide a Sticky Bucket Service to the GrowthBook instance to persist previously seen variations and ensure that the user experience remains consistent for your users.
+
+A sample `InMemoryStickyBucketService` implementation is provided for reference, but in production you will definitely want to implement your own version using a database, cookies, or similar for persistence.
+
+Sticky Bucket documents contain three fields
+
+- `attributeName` - The name of the attribute used to identify the user (e.g. `id`, `cookie_id`, etc.)
+- `attributeValue` - The value of the attribute (e.g. `123`)
+- `assignments` - A dictionary of persisted experiment assignments. For example: `{"exp1__0":"control"}`
+
+The attributeName/attributeValue combo is the primary key.
+
+Here's an example implementation using a theoretical `db` object:
+
+```python
+from growthbook import AbstractStickyBucketService, GrowthBook
+
+class MyStickyBucketService(AbstractStickyBucketService):
+    # Lookup a sticky bucket document
+    def get_assignments(self, attributeName: str, attributeValue: str) -> Optional[Dict]:
+        return db.find({
+          "attributeName": attributeName,
+          "attributeValue": attributeValue
+        })
+
+    def save_assignments(self, doc: Dict) -> None:
+        # Insert new record if not exists, otherwise update
+        db.upsert({
+            "attributeName": doc["attributeName"],
+            "attributeValue": doc["attributeValue"]
+        }, {
+          "$set": {
+            "assignments": doc["assignments"]
+          }
+        })
+
+# Pass in an instance of this service to your GrowthBook constructor
+
+gb = GrowthBook(
+  sticky_bucket_service = MyStickyBucketService()
+)
+```
 
 ## Inline Experiments
 
 Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `run` method:
 
 ```python
 from growthbook import Experiment
@@ -255,24 +302,24 @@
 print(gb.run(exp).value)
 ```
 
 As you can see, there are 2 required parameters for experiments, a string key, and an array of variations. Variations can be any data type, not just strings.
 
 There are a number of additional settings to control the experiment behavior:
 
--   **key** (`str`) - The globally unique tracking key for the experiment
--   **variations** (`any[]`) - The different variations to choose between
--   **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
--   **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
--   **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
--   **condition** (`dict`) - Targeting conditions
--   **force** (`int`) - All users included in the experiment will be forced into the specified variation index
--   **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
--   **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
--   **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
+- **key** (`str`) - The globally unique tracking key for the experiment
+- **variations** (`any[]`) - The different variations to choose between
+- **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
+- **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
+- **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
+- **condition** (`dict`) - Targeting conditions
+- **force** (`int`) - All users included in the experiment will be forced into the specified variation index
+- **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
+- **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
+- **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
 
 Here's an example that uses all of them:
 
 ```python
 exp = Experiment(
   key="my-test",
   # Variations can be a list of any data type
```

### Comparing `growthbook-1.0.0/growthbook.egg-info/PKG-INFO` & `growthbook-1.1.0/growthbook.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,437 +1,491 @@
 Metadata-Version: 2.1
 Name: growthbook
-Version: 1.0.0
+Version: 1.1.0
 Summary: Powerful Feature flagging and A/B testing for Python apps
 Home-page: https://github.com/growthbook/growthbook-python
 Author: GrowthBook
 Author-email: hello@growthbook.io
 License: MIT
-Description: # GrowthBook Python SDK
-        
-        Powerful Feature flagging and A/B testing for Python apps.
-        
-        ![Build Status](https://github.com/growthbook/growthbook-python/workflows/Build/badge.svg)
-        
-        -   **Lightweight and fast**
-        -   **Local evaluation**, no network requests required
-        -   Python 3.6+
-        -   100% test coverage
-        -   Flexible **targeting**
-        -   **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
-        -   **Remote configuration** to change feature flags without deploying new code
-        
-        ## Installation
-        
-        `pip install growthbook` (recommended) or copy `growthbook.py` into your project
-        
-        ## Quick Usage
-        
-        ```python
-        from growthbook import GrowthBook
-        
-        # User attributes for targeting and experimentation
-        attributes = {
-          "id": "123",
-          "customUserAttribute": "foo"
-        }
-        
-        def on_experiment_viewed(experiment, result):
-          # Use whatever event tracking system you want
-          analytics.track(attributes["id"], "Experiment Viewed", {
-            'experimentId': experiment.key,
-            'variationId': result.variationId
-          })
-        
-        # Create a GrowthBook instance
-        gb = GrowthBook(
-          attributes = attributes,
-          on_experiment_viewed = on_experiment_viewed,
-          api_host = "https://cdn.growthbook.io",
-          client_key = "sdk-abc123"
-        )
-        
-        # Load features from the GrowthBook API with caching
-        gb.load_features()
-        
-        # Simple on/off feature gating
-        if gb.is_on("my-feature"):
-          print("My feature is on!")
-        
-        # Get the value of a feature with a fallback
-        color = gb.get_feature_value("button-color-feature", "blue")
-        ```
-        
-        ### Web Frameworks (Django, Flask, etc.)
-        
-        For web frameworks, you should create a new `GrowthBook` instance for every incoming request and call `destroy()` at the end of the request to clean up resources.
-        
-        In Django, for example, this is best done with a simple middleware:
-        
-        ```python
-        from growthbook import GrowthBook
-        
-        def growthbook_middleware(get_response):
-            def middleware(request):
-                request.gb = GrowthBook(
-                  # ...
-                )
-                request.gb.load_features()
-        
-                response = get_response(request)
-        
-                request.gb.destroy() # Cleanup
-        
-                return response
-            return middleware
-        ```
-        
-        Then, you can easily use GrowthBook in any of your views:
-        
-        ```python
-        def index(request):
-            feature_enabled = request.gb.is_on("my-feature")
-            # ...
-        ```
-        
-        ## Loading Features
-        
-        There are two ways to load feature flags into the GrowthBook SDK. You can either use the built-in fetching/caching logic or implement your own custom solution.
-        
-        ### Built-in Fetching and Caching
-        
-        To use the built-in fetching and caching logic, in the `GrowthBook` constructor, pass in your GrowthBook `api_host` and `client_key`. If you have encryption enabled for your GrowthBook endpoint, you also need to pass the `decryption_key` into the constructor.
-        
-        Then, call the `load_features()` method to initiate the HTTP request with a cache layer.
-        
-        Here's a full example:
-        
-        ```python
-        gb = GrowthBook(
-          api_host = "https://cdn.growthbook.io",
-          client_key = "sdk-abc123",
-          # How long to cache features in seconds (Optional, default 60s)
-          cache_ttl = 60,
-        )
-        gb.load_features()
-        ```
-        
-        #### Caching
-        
-        GrowthBook comes with a custom in-memory cache. If you run Python in a multi-process mode, the different processes cannot share memory, so you likely want to switch to a distributed cache system like Redis instead.
-        
-        Here is an example of using Redis:
-        
-        ```python
-        from redis import Redis
-        import json
-        from growthbook import GrowthBook, AbstractFeatureCache, feature_repo
-        
-        class RedisFeatureCache(AbstractFeatureCache):
-          def __init__(self):
-            self.r = Redis(host='localhost', port=6379)
-            self.prefix = "gb:"
-        
-          def get(self, key: str):
-            data = self.r.get(self.prefix + key)
-            # Data stored as a JSON string, parse into dict before returning
-            return None if data is None else json.loads(data)
-        
-          def set(self, key: str, value: dict, ttl: int) -> None:
-            self.r.set(self.prefix + key, json.dumps(value))
-            self.r.expire(self.prefix + key, ttl)
-        
-        # Configure GrowthBook to use your custom cache class
-        feature_repo.set_cache(RedisFeatureCache())
-        ```
-        
-        ### Custom Implementation
-        
-        If you prefer to handle the entire fetching/caching logic yourself, you can just pass in a `dict` of features from the GrowthBook API directly into the constructor:
-        
-        ```python
-        # From the GrowthBook API
-        features = {'my-feature':{'defaultValue':False}}
-        
-        gb = GrowthBook(
-          features = features
-        )
-        ```
-        
-        Note: When doing this, you do not need to specify your `api_host` or `client_key` and you don't need to call `gb.load_features()`.
-        
-        ## GrowthBook class
-        
-        The GrowthBook constructor has the following parameters:
-        
-        -   **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
-        -   **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
-        -   **url** (`str`) - The URL of the current request (if applicable)
-        -   **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
-        -   **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
-        -   **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
-        -   **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
-        -   **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
-        -   **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
-        -   **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
-        -   **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
-        
-        There are also getter and setter methods for features and attributes if you need to update them later in the request:
-        
-        ```python
-        gb.set_features(gb.get_features())
-        gb.set_attributes(gb.get_attributes())
-        ```
-        
-        ### Attributes
-        
-        You can specify attributes about the current user and request. These are used for two things:
-        
-        1.  Feature targeting (e.g. paid users get one value, free users get another)
-        2.  Assigning persistent variations in A/B tests (e.g. user id "123" always gets variation B)
-        
-        Attributes can be any JSON data type - boolean, integer, float, string, list, or dict.
-        
-        ```python
-        attributes = {
-          'id': "123",
-          'loggedIn': True,
-          'age': 21.5,
-          'tags': ["tag1", "tag2"],
-          'account': {
-            'age': 90
-          }
-        }
-        
-        # Pass into constructor
-        gb = GrowthBook(attributes = attributes)
-        
-        # Or set later
-        gb.set_attributes(attributes)
-        ```
-        
-        ### Tracking Experiments
-        
-        Any time an experiment is run to determine the value of a feature, you want to track that event in your analytics system.
-        
-        You can use the `on_experiment_viewed` option to do this:
-        
-        ```python
-        from growthbook import GrowthBook, Experiment, Result
-        
-        def on_experiment_viewed(experiment: Experiment, result: Result):
-          # Use whatever event tracking system you want
-          analytics.track(attributes["id"], "Experiment Viewed", {
-            'experimentId': experiment.key,
-            'variationId': result.variationId
-          })
-        
-        # Pass into constructor
-        gb = GrowthBook(
-          on_experiment_viewed = on_experiment_viewed
-        )
-        ```
-        
-        ## Using Features
-        
-        There are 3 main methods for interacting with features.
-        
-        -   `gb.is_on("feature-key")` returns true if the feature is on
-        -   `gb.is_off("feature-key")` returns false if the feature is on
-        -   `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
-        
-        In addition, you can use `gb.evalFeature("feature-key")` to get back a `FeatureResult` object with the following properties:
-        
-        -   **value** - The JSON-decoded value of the feature (or `None` if not defined)
-        -   **on** and **off** - The JSON-decoded value cast to booleans
-        -   **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
-        -   **experiment** - Information about the experiment (if any) which was used to assign the value to the user
-        -   **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
-        
-        ## Inline Experiments
-        
-        Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `run` method:
-        
-        ```python
-        from growthbook import Experiment
-        
-        exp = Experiment(
-          key = "my-experiment",
-          variations = ["red", "blue", "green"]
-        )
-        
-        # Either "red", "blue", or "green"
-        print(gb.run(exp).value)
-        ```
-        
-        As you can see, there are 2 required parameters for experiments, a string key, and an array of variations. Variations can be any data type, not just strings.
-        
-        There are a number of additional settings to control the experiment behavior:
-        
-        -   **key** (`str`) - The globally unique tracking key for the experiment
-        -   **variations** (`any[]`) - The different variations to choose between
-        -   **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
-        -   **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
-        -   **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
-        -   **condition** (`dict`) - Targeting conditions
-        -   **force** (`int`) - All users included in the experiment will be forced into the specified variation index
-        -   **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
-        -   **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
-        -   **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
-        
-        Here's an example that uses all of them:
-        
-        ```python
-        exp = Experiment(
-          key="my-test",
-          # Variations can be a list of any data type
-          variations=[0, 1],
-          # If this changes, it will re-randomize all users in the experiment
-          seed="abcdef123456",
-          # Run a 40/60 experiment instead of the default even split (50/50)
-          weights=[0.4, 0.6],
-          # Only include 20% of users in the experiment
-          coverage=0.2,
-          # Targeting condition using a MongoDB-like syntax
-          condition={
-            'country': 'US',
-            'browser': {
-              '$in': ['chrome', 'firefox']
-            }
-          },
-          # Use an alternate attribute for assigning variations (default is 'id')
-          hashAttribute="sessionId",
-          # Use the latest hashing algorithm
-          hashVersion=2,
-          # Includes the first 50% of users in the "pricing" namespace
-          # Another experiment with a non-overlapping range will be mutually exclusive (e.g. [0.5, 1])
-          namespace=("pricing", 0, 0.5),
-        )
-        ```
-        
-        ### Inline Experiment Return Value
-        
-        A call to `run` returns a `Result` object with a few useful properties:
-        
-        ```python
-        result = gb.run(exp)
-        
-        # If user is part of the experiment
-        print(result.inExperiment) # True or False
-        
-        # The index of the assigned variation
-        print(result.variationId) # e.g. 0 or 1
-        
-        # The value of the assigned variation
-        print(result.value) # e.g. "A" or "B"
-        
-        # If the variation was randomly assigned by hashing user attributes
-        print(result.hashUsed) # True or False
-        
-        # The user attribute used to assign a variation
-        print(result.hashAttribute) # "id"
-        
-        # The value of that attribute
-        print(result.hashValue) # e.g. "123"
-        ```
-        
-        The `inExperiment` flag will be false if the user was excluded from being part of the experiment for any reason (e.g. failed targeting conditions).
-        
-        The `hashUsed` flag will only be true if the user was randomly assigned a variation. If the user was forced into a specific variation instead, this flag will be false.
-        
-        ### Example Experiments
-        
-        3-way experiment with uneven variation weights:
-        
-        ```python
-        gb.run(Experiment(
-          key = "3-way-uneven",
-          variations = ["A","B","C"],
-          weights = [0.5, 0.25, 0.25]
-        ))
-        ```
-        
-        Slow rollout (10% of users who match the targeting condition):
-        
-        ```python
-        # User is marked as being in "qa" and "beta"
-        gb = GrowthBook(
-          attributes = {
-            "id": "123",
-            "beta": True,
-            "qa": True,
-          },
-        )
-        
-        gb.run(Experiment(
-          key = "slow-rollout",
-          variations = ["A", "B"],
-          coverage = 0.1,
-          condition = {
-            'beta': True
-          }
-        ))
-        ```
-        
-        Complex variations
-        
-        ```python
-        result = gb.run(Experiment(
-          key = "complex-variations",
-          variations = [
-            ("blue", "large"),
-            ("green", "small")
-          ],
-        ))
-        
-        # Either "blue,large" OR "green,small"
-        print(result.value[0] + "," + result.value[1])
-        ```
-        
-        Assign variations based on something other than user id
-        
-        ```python
-        gb = GrowthBook(
-          attributes = {
-            "id": "123",
-            "company": "growthbook"
-          }
-        )
-        
-        # Users in the same company will always get the same variation
-        gb.run(Experiment(
-          key = "by-company-id",
-          variations = ["A", "B"],
-          hashAttribute = "company"
-        ))
-        ```
-        
-        ## Logging
-        
-        The GrowthBook SDK uses a Python logger with the name `growthbook` and includes helpful info for debugging as well as warnings/errors if something is misconfigured.
-        
-        Here's an example of logging to the console
-        
-        ```python
-        import logging
-        
-        logger = logging.getLogger('growthbook')
-        logger.setLevel(logging.DEBUG)
-        
-        handler = logging.StreamHandler()
-        formatter = logging.Formatter('%(asctime)s %(name)s %(levelname)s %(message)s')
-        handler.setFormatter(formatter)
-        logger.addHandler(handler)
-        ```
-        
 Keywords: growthbook
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GrowthBook Python SDK
+
+Powerful Feature flagging and A/B testing for Python apps.
+
+![Build Status](https://github.com/growthbook/growthbook-python/workflows/Build/badge.svg)
+
+- **Lightweight and fast**
+- **Local evaluation**, no network requests required
+- Python 3.6+
+- 100% test coverage
+- Flexible **targeting**
+- **Use your existing event tracking** (GA, Segment, Mixpanel, custom)
+- **Remote configuration** to change feature flags without deploying new code
+
+## Installation
+
+`pip install growthbook` (recommended) or copy `growthbook.py` into your project
+
+## Quick Usage
+
+```python
+from growthbook import GrowthBook
+
+# User attributes for targeting and experimentation
+attributes = {
+  "id": "123",
+  "customUserAttribute": "foo"
+}
+
+def on_experiment_viewed(experiment, result):
+  # Use whatever event tracking system you want
+  analytics.track(attributes["id"], "Experiment Viewed", {
+    'experimentId': experiment.key,
+    'variationId': result.variationId
+  })
+
+# Create a GrowthBook instance
+gb = GrowthBook(
+  attributes = attributes,
+  on_experiment_viewed = on_experiment_viewed,
+  api_host = "https://cdn.growthbook.io",
+  client_key = "sdk-abc123"
+)
+
+# Load features from the GrowthBook API with caching
+gb.load_features()
+
+# Simple on/off feature gating
+if gb.is_on("my-feature"):
+  print("My feature is on!")
+
+# Get the value of a feature with a fallback
+color = gb.get_feature_value("button-color-feature", "blue")
+```
+
+### Web Frameworks (Django, Flask, etc.)
+
+For web frameworks, you should create a new `GrowthBook` instance for every incoming request and call `destroy()` at the end of the request to clean up resources.
+
+In Django, for example, this is best done with a simple middleware:
+
+```python
+from growthbook import GrowthBook
+
+def growthbook_middleware(get_response):
+    def middleware(request):
+        request.gb = GrowthBook(
+          # ...
+        )
+        request.gb.load_features()
+
+        response = get_response(request)
+
+        request.gb.destroy() # Cleanup
+
+        return response
+    return middleware
+```
+
+Then, you can easily use GrowthBook in any of your views:
+
+```python
+def index(request):
+    feature_enabled = request.gb.is_on("my-feature")
+    # ...
+```
+
+## Loading Features
+
+There are two ways to load feature flags into the GrowthBook SDK. You can either use the built-in fetching/caching logic or implement your own custom solution.
+
+### Built-in Fetching and Caching
+
+To use the built-in fetching and caching logic, in the `GrowthBook` constructor, pass in your GrowthBook `api_host` and `client_key`. If you have encryption enabled for your GrowthBook endpoint, you also need to pass the `decryption_key` into the constructor.
+
+Then, call the `load_features()` method to initiate the HTTP request with a cache layer.
+
+Here's a full example:
+
+```python
+gb = GrowthBook(
+  api_host = "https://cdn.growthbook.io",
+  client_key = "sdk-abc123",
+  # How long to cache features in seconds (Optional, default 60s)
+  cache_ttl = 60,
+)
+gb.load_features()
+```
+
+#### Caching
+
+GrowthBook comes with a custom in-memory cache. If you run Python in a multi-process mode, the different processes cannot share memory, so you likely want to switch to a distributed cache system like Redis instead.
+
+Here is an example of using Redis:
+
+```python
+from redis import Redis
+import json
+from growthbook import GrowthBook, AbstractFeatureCache, feature_repo
+
+class RedisFeatureCache(AbstractFeatureCache):
+  def __init__(self):
+    self.r = Redis(host='localhost', port=6379)
+    self.prefix = "gb:"
+
+  def get(self, key: str):
+    data = self.r.get(self.prefix + key)
+    # Data stored as a JSON string, parse into dict before returning
+    return None if data is None else json.loads(data)
+
+  def set(self, key: str, value: dict, ttl: int) -> None:
+    self.r.set(self.prefix + key, json.dumps(value))
+    self.r.expire(self.prefix + key, ttl)
+
+# Configure GrowthBook to use your custom cache class
+feature_repo.set_cache(RedisFeatureCache())
+```
+
+### Custom Implementation
+
+If you prefer to handle the entire fetching/caching logic yourself, you can just pass in a `dict` of features from the GrowthBook API directly into the constructor:
+
+```python
+# From the GrowthBook API
+features = {'my-feature':{'defaultValue':False}}
+
+gb = GrowthBook(
+  features = features
+)
+```
+
+Note: When doing this, you do not need to specify your `api_host` or `client_key` and you don't need to call `gb.load_features()`.
+
+## GrowthBook class
+
+The GrowthBook constructor has the following parameters:
+
+- **enabled** (`bool`) - Flag to globally disable all experiments. Default true.
+- **attributes** (`dict`) - Dictionary of user attributes that are used for targeting and to assign variations
+- **url** (`str`) - The URL of the current request (if applicable)
+- **qa_mode** (`boolean`) - If true, random assignment is disabled and only explicitly forced variations are used.
+- **on_experiment_viewed** (`callable`) - A function that takes `experiment` and `result` as arguments.
+- **api_host** (`str`) - The GrowthBook API host to fetch feature flags from. Defaults to `https://cdn.growthbook.io`
+- **client_key** (`str`) - The client key that will be passed to the API Host to fetch feature flags
+- **decryption_key** (`str`) - If the GrowthBook API endpoint has encryption enabled, specify the decryption key here
+- **cache_ttl** (`int`) - How long to cache features in-memory from the GrowthBook API (seconds, default `60`)
+- **features** (`dict`) - Feature definitions from the GrowthBook API (only required if `client_key` is not specified)
+- **forced_variations** (`dict`) - Dictionary of forced experiment variations (used for QA)
+
+There are also getter and setter methods for features and attributes if you need to update them later in the request:
+
+```python
+gb.set_features(gb.get_features())
+gb.set_attributes(gb.get_attributes())
+```
+
+### Attributes
+
+You can specify attributes about the current user and request. These are used for two things:
+
+1.  Feature targeting (e.g. paid users get one value, free users get another)
+2.  Assigning persistent variations in A/B tests (e.g. user id "123" always gets variation B)
+
+Attributes can be any JSON data type - boolean, integer, float, string, list, or dict.
+
+```python
+attributes = {
+  'id': "123",
+  'loggedIn': True,
+  'age': 21.5,
+  'tags': ["tag1", "tag2"],
+  'account': {
+    'age': 90
+  }
+}
+
+# Pass into constructor
+gb = GrowthBook(attributes = attributes)
+
+# Or set later
+gb.set_attributes(attributes)
+```
+
+### Tracking Experiments
+
+Any time an experiment is run to determine the value of a feature, you want to track that event in your analytics system.
+
+You can use the `on_experiment_viewed` option to do this:
+
+```python
+from growthbook import GrowthBook, Experiment, Result
+
+def on_experiment_viewed(experiment: Experiment, result: Result):
+  # Use whatever event tracking system you want
+  analytics.track(attributes["id"], "Experiment Viewed", {
+    'experimentId': experiment.key,
+    'variationId': result.variationId
+  })
+
+# Pass into constructor
+gb = GrowthBook(
+  on_experiment_viewed = on_experiment_viewed
+)
+```
+
+## Using Features
+
+There are 3 main methods for interacting with features.
+
+- `gb.is_on("feature-key")` returns true if the feature is on
+- `gb.is_off("feature-key")` returns false if the feature is on
+- `gb.get_feature_value("feature-key", "default")` returns the value of the feature with a fallback
+
+In addition, you can use `gb.evalFeature("feature-key")` to get back a `FeatureResult` object with the following properties:
+
+- **value** - The JSON-decoded value of the feature (or `None` if not defined)
+- **on** and **off** - The JSON-decoded value cast to booleans
+- **source** - Why the value was assigned to the user. One of `unknownFeature`, `defaultValue`, `force`, or `experiment`
+- **experiment** - Information about the experiment (if any) which was used to assign the value to the user
+- **experimentResult** - The result of the experiment (if any) which was used to assign the value to the user
+
+## Sticky Bucketing
+
+By default GrowthBook does not persist assigned experiment variations for a user. We rely on deterministic hashing to ensure that the same user attributes always map to the same experiment variation. However, there are cases where this isn't good enough. For example, if you change targeting conditions in the middle of an experiment, users may stop being shown a variation even if they were previously bucketed into it.
+
+Sticky Bucketing is a solution to these issues. You can provide a Sticky Bucket Service to the GrowthBook instance to persist previously seen variations and ensure that the user experience remains consistent for your users.
+
+A sample `InMemoryStickyBucketService` implementation is provided for reference, but in production you will definitely want to implement your own version using a database, cookies, or similar for persistence.
+
+Sticky Bucket documents contain three fields
+
+- `attributeName` - The name of the attribute used to identify the user (e.g. `id`, `cookie_id`, etc.)
+- `attributeValue` - The value of the attribute (e.g. `123`)
+- `assignments` - A dictionary of persisted experiment assignments. For example: `{"exp1__0":"control"}`
+
+The attributeName/attributeValue combo is the primary key.
+
+Here's an example implementation using a theoretical `db` object:
+
+```python
+from growthbook import AbstractStickyBucketService, GrowthBook
+
+class MyStickyBucketService(AbstractStickyBucketService):
+    # Lookup a sticky bucket document
+    def get_assignments(self, attributeName: str, attributeValue: str) -> Optional[Dict]:
+        return db.find({
+          "attributeName": attributeName,
+          "attributeValue": attributeValue
+        })
+
+    def save_assignments(self, doc: Dict) -> None:
+        # Insert new record if not exists, otherwise update
+        db.upsert({
+            "attributeName": doc["attributeName"],
+            "attributeValue": doc["attributeValue"]
+        }, {
+          "$set": {
+            "assignments": doc["assignments"]
+          }
+        })
+
+# Pass in an instance of this service to your GrowthBook constructor
+
+gb = GrowthBook(
+  sticky_bucket_service = MyStickyBucketService()
+)
+```
+
+## Inline Experiments
+
+Instead of declaring all features up-front and referencing them by ids in your code, you can also just run an experiment directly. This is done with the `run` method:
+
+```python
+from growthbook import Experiment
+
+exp = Experiment(
+  key = "my-experiment",
+  variations = ["red", "blue", "green"]
+)
+
+# Either "red", "blue", or "green"
+print(gb.run(exp).value)
+```
+
+As you can see, there are 2 required parameters for experiments, a string key, and an array of variations. Variations can be any data type, not just strings.
+
+There are a number of additional settings to control the experiment behavior:
+
+- **key** (`str`) - The globally unique tracking key for the experiment
+- **variations** (`any[]`) - The different variations to choose between
+- **seed** (`str`) - Added to the user id when hashing to determine a variation. Defaults to the experiment `key`
+- **weights** (`float[]`) - How to weight traffic between variations. Must add to 1.
+- **coverage** (`float`) - What percent of users should be included in the experiment (between 0 and 1, inclusive)
+- **condition** (`dict`) - Targeting conditions
+- **force** (`int`) - All users included in the experiment will be forced into the specified variation index
+- **hashAttribute** (`string`) - What user attribute should be used to assign variations (defaults to "id")
+- **hashVersion** (`int`) - What version of our hashing algorithm to use. We recommend using the latest version `2`.
+- **namespace** (`tuple[str,float,float]`) - Used to run mutually exclusive experiments.
+
+Here's an example that uses all of them:
+
+```python
+exp = Experiment(
+  key="my-test",
+  # Variations can be a list of any data type
+  variations=[0, 1],
+  # If this changes, it will re-randomize all users in the experiment
+  seed="abcdef123456",
+  # Run a 40/60 experiment instead of the default even split (50/50)
+  weights=[0.4, 0.6],
+  # Only include 20% of users in the experiment
+  coverage=0.2,
+  # Targeting condition using a MongoDB-like syntax
+  condition={
+    'country': 'US',
+    'browser': {
+      '$in': ['chrome', 'firefox']
+    }
+  },
+  # Use an alternate attribute for assigning variations (default is 'id')
+  hashAttribute="sessionId",
+  # Use the latest hashing algorithm
+  hashVersion=2,
+  # Includes the first 50% of users in the "pricing" namespace
+  # Another experiment with a non-overlapping range will be mutually exclusive (e.g. [0.5, 1])
+  namespace=("pricing", 0, 0.5),
+)
+```
+
+### Inline Experiment Return Value
+
+A call to `run` returns a `Result` object with a few useful properties:
+
+```python
+result = gb.run(exp)
+
+# If user is part of the experiment
+print(result.inExperiment) # True or False
+
+# The index of the assigned variation
+print(result.variationId) # e.g. 0 or 1
+
+# The value of the assigned variation
+print(result.value) # e.g. "A" or "B"
+
+# If the variation was randomly assigned by hashing user attributes
+print(result.hashUsed) # True or False
+
+# The user attribute used to assign a variation
+print(result.hashAttribute) # "id"
+
+# The value of that attribute
+print(result.hashValue) # e.g. "123"
+```
+
+The `inExperiment` flag will be false if the user was excluded from being part of the experiment for any reason (e.g. failed targeting conditions).
+
+The `hashUsed` flag will only be true if the user was randomly assigned a variation. If the user was forced into a specific variation instead, this flag will be false.
+
+### Example Experiments
+
+3-way experiment with uneven variation weights:
+
+```python
+gb.run(Experiment(
+  key = "3-way-uneven",
+  variations = ["A","B","C"],
+  weights = [0.5, 0.25, 0.25]
+))
+```
+
+Slow rollout (10% of users who match the targeting condition):
+
+```python
+# User is marked as being in "qa" and "beta"
+gb = GrowthBook(
+  attributes = {
+    "id": "123",
+    "beta": True,
+    "qa": True,
+  },
+)
+
+gb.run(Experiment(
+  key = "slow-rollout",
+  variations = ["A", "B"],
+  coverage = 0.1,
+  condition = {
+    'beta': True
+  }
+))
+```
+
+Complex variations
+
+```python
+result = gb.run(Experiment(
+  key = "complex-variations",
+  variations = [
+    ("blue", "large"),
+    ("green", "small")
+  ],
+))
+
+# Either "blue,large" OR "green,small"
+print(result.value[0] + "," + result.value[1])
+```
+
+Assign variations based on something other than user id
+
+```python
+gb = GrowthBook(
+  attributes = {
+    "id": "123",
+    "company": "growthbook"
+  }
+)
+
+# Users in the same company will always get the same variation
+gb.run(Experiment(
+  key = "by-company-id",
+  variations = ["A", "B"],
+  hashAttribute = "company"
+))
+```
+
+## Logging
+
+The GrowthBook SDK uses a Python logger with the name `growthbook` and includes helpful info for debugging as well as warnings/errors if something is misconfigured.
+
+Here's an example of logging to the console
+
+```python
+import logging
+
+logger = logging.getLogger('growthbook')
+logger.setLevel(logging.DEBUG)
+
+handler = logging.StreamHandler()
+formatter = logging.Formatter('%(asctime)s %(name)s %(levelname)s %(message)s')
+handler.setFormatter(formatter)
+logger.addHandler(handler)
+```
+
+
```

### Comparing `growthbook-1.0.0/growthbook.py` & `growthbook-1.1.0/growthbook.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,28 +46,28 @@
     if version == 1:
         n = fnv1a32(value + seed)
         return (n % 1000) / 1000
     return None
 
 
 def inRange(n: float, range: Tuple[float, float]) -> bool:
-    return n >= range[0] and n < range[1]
+    return range[0] <= n < range[1]
 
 
 def inNamespace(userId: str, namespace: Tuple[str, float, float]) -> bool:
     n = gbhash("__" + namespace[0], userId, 1)
     if n is None:
         return False
-    return n >= namespace[1] and n < namespace[2]
+    return namespace[1] <= n < namespace[2]
 
 
 def getEqualWeights(numVariations: int) -> List[float]:
     if numVariations < 1:
         return []
-    return [1 / numVariations for i in range(numVariations)]
+    return [1 / numVariations for _ in range(numVariations)]
 
 
 def getBucketRanges(
     numVariations: int, coverage: float = 1, weights: List[float] = None
 ) -> List[Tuple[float, float]]:
     if coverage < 0:
         coverage = 0
@@ -127,14 +127,43 @@
 
     unpadder = padding.PKCS7(128).unpadder()
     bytestring = unpadder.update(decrypted) + unpadder.finalize()
 
     return bytestring.decode("utf-8")
 
 
+def paddedVersionString(input) -> str:
+    # If input is a number, convert to a string
+    if type(input) is int or type(input) is float:
+        input = str(input)
+
+    if not input or type(input) is not str:
+        input = "0"
+
+    # Remove build info and leading `v` if any
+    input = re.sub(r"(^v|\+.*$)", "", input)
+    # Split version into parts (both core version numbers and pre-release tags)
+    # "v1.2.3-rc.1+build123" -> ["1","2","3","rc","1"]
+    parts = re.split(r"[-.]", input)
+    # If it's SemVer without a pre-release, add `~` to the end
+    # ["1","0","0"] -> ["1","0","0","~"]
+    # "~" is the largest ASCII character, so this will make "1.0.0" greater than "1.0.0-beta" for example
+    if len(parts) == 3:
+        parts.append("~")
+    # Left pad each numeric part with spaces so string comparisons will work ("9">"10", but " 9"<"10")
+    # Then, join back together into a single string
+    return "-".join([v.rjust(5, " ") if re.match(r"^[0-9]+$", v) else v for v in parts])
+
+
+def isIn(conditionValue, attributeValue) -> bool:
+    if type(attributeValue) is list:
+        return bool(set(conditionValue) & set(attributeValue))
+    return attributeValue in conditionValue
+
+
 def evalCondition(attributes: dict, condition: dict) -> bool:
     if "$or" in condition:
         return evalOr(attributes, condition["$or"])
     if "$nor" in condition:
         return not evalOr(attributes, condition["$nor"])
     if "$and" in condition:
         return evalAnd(attributes, condition["$and"])
@@ -220,37 +249,91 @@
         else:
             if evalCondition(item, condition):
                 return True
 
     return False
 
 
+def compare(val1, val2) -> int:
+    if (type(val1) is int or type(val1) is float) and not (type(val2) is int or type(val2) is float):
+        if (val2 is None):
+            val2 = 0
+        else:
+            val2 = float(val2)
+
+    if (type(val2) is int or type(val2) is float) and not (type(val1) is int or type(val1) is float):
+        if (val1 is None):
+            val1 = 0
+        else:
+            val1 = float(val1)
+
+    if val1 > val2:
+        return 1
+    if val1 < val2:
+        return -1
+    return 0
+
+
 def evalOperatorCondition(operator, attributeValue, conditionValue) -> bool:
     if operator == "$eq":
-        return attributeValue == conditionValue
+        try:
+            return compare(attributeValue, conditionValue) == 0
+        except Exception:
+            return False
     elif operator == "$ne":
-        return attributeValue != conditionValue
+        try:
+            return compare(attributeValue, conditionValue) != 0
+        except Exception:
+            return False
     elif operator == "$lt":
-        return attributeValue < conditionValue
+        try:
+            return compare(attributeValue, conditionValue) < 0
+        except Exception:
+            return False
     elif operator == "$lte":
-        return attributeValue <= conditionValue
+        try:
+            return compare(attributeValue, conditionValue) <= 0
+        except Exception:
+            return False
     elif operator == "$gt":
-        return attributeValue > conditionValue
+        try:
+            return compare(attributeValue, conditionValue) > 0
+        except Exception:
+            return False
     elif operator == "$gte":
-        return attributeValue >= conditionValue
+        try:
+            return compare(attributeValue, conditionValue) >= 0
+        except Exception:
+            return False
+    elif operator == "$veq":
+        return paddedVersionString(attributeValue) == paddedVersionString(conditionValue)
+    elif operator == "$vne":
+        return paddedVersionString(attributeValue) != paddedVersionString(conditionValue)
+    elif operator == "$vlt":
+        return paddedVersionString(attributeValue) < paddedVersionString(conditionValue)
+    elif operator == "$vlte":
+        return paddedVersionString(attributeValue) <= paddedVersionString(conditionValue)
+    elif operator == "$vgt":
+        return paddedVersionString(attributeValue) > paddedVersionString(conditionValue)
+    elif operator == "$vgte":
+        return paddedVersionString(attributeValue) >= paddedVersionString(conditionValue)
     elif operator == "$regex":
         try:
             r = re.compile(conditionValue)
             return bool(r.search(attributeValue))
         except Exception:
             return False
     elif operator == "$in":
-        return attributeValue in conditionValue
+        if not type(conditionValue) is list:
+            return False
+        return isIn(conditionValue, attributeValue)
     elif operator == "$nin":
-        return not (attributeValue in conditionValue)
+        if not type(conditionValue) is list:
+            return False
+        return not isIn(conditionValue, attributeValue)
     elif operator == "$elemMatch":
         return elemMatch(conditionValue, attributeValue)
     elif operator == "$size":
         if not (type(attributeValue) is list):
             return False
         return evalConditionValue(conditionValue, len(attributeValue))
     elif operator == "$all":
@@ -300,21 +383,26 @@
         condition: dict = None,
         namespace: Tuple[str, float, float] = None,
         url: str = "",
         include=None,
         groups: list = None,
         force: int = None,
         hashAttribute: str = "id",
+        fallbackAttribute: str = None,
         hashVersion: int = None,
         ranges: List[Tuple[float, float]] = None,
         meta: List[VariationMeta] = None,
         filters: List[Filter] = None,
         seed: str = None,
         name: str = None,
         phase: str = None,
+        disableStickyBucketing: bool = False,
+        bucketVersion: int = None,
+        minBucketVersion: int = None,
+        parentConditions: List[dict] = None,
     ) -> None:
         self.key = key
         self.variations = variations
         self.weights = weights
         self.active = active
         self.coverage = coverage
         self.condition = condition
@@ -324,14 +412,22 @@
         self.hashVersion = hashVersion or 1
         self.ranges = ranges
         self.meta = meta
         self.filters = filters
         self.seed = seed
         self.name = name
         self.phase = phase
+        self.disableStickyBucketing = disableStickyBucketing
+        self.bucketVersion = bucketVersion or 0
+        self.minBucketVersion = minBucketVersion or 0
+        self.parentConditions = parentConditions
+
+        self.fallbackAttribute = None
+        if not self.disableStickyBucketing:
+            self.fallbackAttribute = fallbackAttribute
 
         # Deprecated properties
         self.status = status
         self.url = url
         self.include = include
         self.groups = groups
 
@@ -350,14 +446,26 @@
             "ranges": self.ranges,
             "meta": self.meta,
             "filters": self.filters,
             "seed": self.seed,
             "name": self.name,
             "phase": self.phase,
         }
+
+        if self.fallbackAttribute:
+            obj["fallbackAttribute"] = self.fallbackAttribute
+        if self.disableStickyBucketing:
+            obj["disableStickyBucketing"] = True
+        if self.bucketVersion:
+            obj["bucketVersion"] = self.bucketVersion
+        if self.minBucketVersion:
+            obj["minBucketVersion"] = self.minBucketVersion
+        if self.parentConditions:
+            obj["parentConditions"] = self.parentConditions
+
         return obj
 
     def update(self, data: dict) -> None:
         weights = data.get("weights", None)
         status = data.get("status", None)
         coverage = data.get("coverage", None)
         url = data.get("url", None)
@@ -386,23 +494,25 @@
         value,
         hashUsed: bool,
         hashAttribute: str,
         hashValue: str,
         featureId: Optional[str],
         meta: VariationMeta = None,
         bucket: float = None,
+        stickyBucketUsed: bool = False,
     ) -> None:
         self.variationId = variationId
         self.inExperiment = inExperiment
         self.value = value
         self.hashUsed = hashUsed
         self.hashAttribute = hashAttribute
         self.hashValue = hashValue
         self.featureId = featureId or None
         self.bucket = bucket
+        self.stickyBucketUsed = stickyBucketUsed
 
         self.key = str(variationId)
         self.name = ""
         self.passthrough = False
 
         if meta:
             if "name" in meta:
@@ -418,14 +528,15 @@
             "variationId": self.variationId,
             "inExperiment": self.inExperiment,
             "value": self.value,
             "hashUsed": self.hashUsed,
             "hashAttribute": self.hashAttribute,
             "hashValue": self.hashValue,
             "key": self.key,
+            "stickyBucketUsed": self.stickyBucketUsed,
         }
 
         if self.bucket is not None:
             obj["bucket"] = self.bucket
         if self.name:
             obj["name"] = self.name
         if self.passthrough:
@@ -438,62 +549,103 @@
     def __init__(self, defaultValue=None, rules: list = []) -> None:
         self.defaultValue = defaultValue
         self.rules: List[FeatureRule] = []
         for rule in rules:
             if isinstance(rule, FeatureRule):
                 self.rules.append(rule)
             else:
-                self.rules.append(FeatureRule(**rule))
+                self.rules.append(FeatureRule(
+                    id=rule.get("id", None),
+                    key=rule.get("key", ""),
+                    variations=rule.get("variations", None),
+                    weights=rule.get("weights", None),
+                    coverage=rule.get("coverage", None),
+                    condition=rule.get("condition", None),
+                    namespace=rule.get("namespace", None),
+                    force=rule.get("force", None),
+                    hashAttribute=rule.get("hashAttribute", "id"),
+                    fallbackAttribute=rule.get("fallbackAttribute", None),
+                    hashVersion=rule.get("hashVersion", None),
+                    range=rule.get("range", None),
+                    ranges=rule.get("ranges", None),
+                    meta=rule.get("meta", None),
+                    filters=rule.get("filters", None),
+                    seed=rule.get("seed", None),
+                    name=rule.get("name", None),
+                    phase=rule.get("phase", None),
+                    disableStickyBucketing=rule.get("disableStickyBucketing", False),
+                    bucketVersion=rule.get("bucketVersion", None),
+                    minBucketVersion=rule.get("minBucketVersion", None),
+                    parentConditions=rule.get("parentConditions", None),
+                ))
 
     def to_dict(self) -> dict:
         return {
             "defaultValue": self.defaultValue,
             "rules": [rule.to_dict() for rule in self.rules],
         }
 
 
 class FeatureRule(object):
     def __init__(
         self,
+        id: str = None,
         key: str = "",
         variations: list = None,
         weights: List[float] = None,
         coverage: int = None,
         condition: dict = None,
         namespace: Tuple[str, float, float] = None,
         force=None,
         hashAttribute: str = "id",
+        fallbackAttribute: str = None,
         hashVersion: int = None,
         range: Tuple[float, float] = None,
         ranges: List[Tuple[float, float]] = None,
         meta: List[VariationMeta] = None,
         filters: List[Filter] = None,
         seed: str = None,
         name: str = None,
         phase: str = None,
+        disableStickyBucketing: bool = False,
+        bucketVersion: int = None,
+        minBucketVersion: int = None,
+        parentConditions: List[dict] = None,
     ) -> None:
+
+        if disableStickyBucketing:
+            fallbackAttribute = None
+
+        self.id = id
         self.key = key
         self.variations = variations
         self.weights = weights
         self.coverage = coverage
         self.condition = condition
         self.namespace = namespace
         self.force = force
         self.hashAttribute = hashAttribute
+        self.fallbackAttribute = fallbackAttribute
         self.hashVersion = hashVersion or 1
         self.range = range
         self.ranges = ranges
         self.meta = meta
         self.filters = filters
         self.seed = seed
         self.name = name
         self.phase = phase
+        self.disableStickyBucketing = disableStickyBucketing
+        self.bucketVersion = bucketVersion or 0
+        self.minBucketVersion = minBucketVersion or 0
+        self.parentConditions = parentConditions
 
     def to_dict(self) -> dict:
         data: Dict[str, Any] = {}
+        if self.id:
+            data["id"] = self.id
         if self.key:
             data["key"] = self.key
         if self.variations is not None:
             data["variations"] = self.variations
         if self.weights is not None:
             data["weights"] = self.weights
         if self.coverage and self.coverage != 1:
@@ -518,40 +670,54 @@
             data["filters"] = self.filters
         if self.seed is not None:
             data["seed"] = self.seed
         if self.name is not None:
             data["name"] = self.name
         if self.phase is not None:
             data["phase"] = self.phase
+        if self.fallbackAttribute:
+            data["fallbackAttribute"] = self.fallbackAttribute
+        if self.disableStickyBucketing:
+            data["disableStickyBucketing"] = True
+        if self.bucketVersion:
+            data["bucketVersion"] = self.bucketVersion
+        if self.minBucketVersion:
+            data["minBucketVersion"] = self.minBucketVersion
+        if self.parentConditions:
+            data["parentConditions"] = self.parentConditions
 
         return data
 
 
 class FeatureResult(object):
     def __init__(
         self,
         value,
         source: str,
         experiment: Experiment = None,
         experimentResult: Result = None,
+        ruleId: str = None,
     ) -> None:
         self.value = value
         self.source = source
+        self.ruleId = ruleId
         self.experiment = experiment
         self.experimentResult = experimentResult
         self.on = bool(value)
         self.off = not bool(value)
 
     def to_dict(self) -> dict:
         data = {
             "value": self.value,
             "source": self.source,
             "on": self.on,
             "off": self.off,
         }
+        if self.ruleId:
+            data["ruleId"] = self.ruleId
         if self.experiment:
             data["experiment"] = self.experiment.to_dict()
         if self.experimentResult:
             data["experimentResult"] = self.experimentResult.to_dict()
 
         return data
 
@@ -596,14 +762,51 @@
             self.cache[key].update(value)
         self.cache[key] = CacheEntry(value, ttl)
 
     def clear(self) -> None:
         self.cache.clear()
 
 
+class AbstractStickyBucketService(ABC):
+    @abstractmethod
+    def get_assignments(self, attributeName: str, attributeValue: str) -> Optional[Dict]:
+        pass
+
+    @abstractmethod
+    def save_assignments(self, doc: Dict) -> None:
+        pass
+
+    def get_key(self, attributeName: str, attributeValue: str) -> str:
+        return f"{attributeName}||{attributeValue}"
+
+    # By default, just loop through all attributes and call get_assignments
+    # Override this method in subclasses to perform a multi-query instead
+    def get_all_assignments(self, attributes: Dict[str, str]) -> Dict[str, Dict]:
+        docs = {}
+        for attributeName, attributeValue in attributes.items():
+            doc = self.get_assignments(attributeName, attributeValue)
+            if doc:
+                docs[self.get_key(attributeName, attributeValue)] = doc
+        return docs
+
+
+class InMemoryStickyBucketService(AbstractStickyBucketService):
+    def __init__(self) -> None:
+        self.docs: Dict[str, Dict] = {}
+
+    def get_assignments(self, attributeName: str, attributeValue: str) -> Optional[Dict]:
+        return self.docs.get(self.get_key(attributeName, attributeValue), None)
+
+    def save_assignments(self, doc: Dict) -> None:
+        self.docs[self.get_key(doc["attributeName"], doc["attributeValue"])] = doc
+
+    def destroy(self) -> None:
+        self.docs.clear()
+
+
 class FeatureRepository(object):
     def __init__(self) -> None:
         self.cache: AbstractFeatureCache = InMemoryFeatureCache()
         self.http: Optional[PoolManager] = None
 
     def set_cache(self, cache: AbstractFeatureCache) -> None:
         self.cache = cache
@@ -666,15 +869,16 @@
                 return None
         elif "features" in decoded:
             return decoded["features"]
         else:
             logger.warning("GrowthBook API response missing features")
             return None
 
-    def _get_features_url(self, api_host: str, client_key: str) -> str:
+    @staticmethod
+    def _get_features_url(api_host: str, client_key: str) -> str:
         api_host = (api_host or "https://cdn.growthbook.io").rstrip("/")
         return api_host + "/api/features/" + client_key
 
 
 # Singleton instance
 feature_repo = FeatureRepository()
 
@@ -689,14 +893,16 @@
         qa_mode: bool = False,
         on_experiment_viewed=None,
         api_host: str = "",
         client_key: str = "",
         decryption_key: str = "",
         cache_ttl: int = 60,
         forced_variations: dict = {},
+        sticky_bucket_service: AbstractStickyBucketService = None,
+        sticky_bucket_identifier_attributes: List[str] = None,
         # Deprecated args
         trackingCallback=None,
         qaMode: bool = False,
         user: dict = {},
         groups: dict = {},
         overrides: dict = {},
         forcedVariations: dict = {},
@@ -705,31 +911,36 @@
         self._attributes = attributes
         self._url = url
         self._features: Dict[str, Feature] = {}
         self._api_host = api_host
         self._client_key = client_key
         self._decryption_key = decryption_key
         self._cache_ttl = cache_ttl
-
-        if features:
-            self.setFeatures(features)
+        self.sticky_bucket_identifier_attributes = sticky_bucket_identifier_attributes
+        self.sticky_bucket_service = sticky_bucket_service
+        self._sticky_bucket_assignment_docs: dict = {}
+        self._using_derived_sticky_bucket_attributes = not sticky_bucket_identifier_attributes
+        self._sticky_bucket_attributes: Optional[dict] = None
 
         self._qaMode = qa_mode or qaMode
         self._trackingCallback = on_experiment_viewed or trackingCallback
 
         # Deprecated args
         self._user = user
         self._groups = groups
         self._overrides = overrides
         self._forcedVariations = forced_variations or forcedVariations
 
         self._tracked: Dict[str, Any] = {}
         self._assigned: Dict[str, Any] = {}
         self._subscriptions: Set[Any] = set()
 
+        if features:
+            self.setFeatures(features)
+
     def load_features(self) -> None:
         if not self._client_key:
             raise ValueError("Must specify `client_key` to refresh features")
 
         features = feature_repo.load_features(
             self._api_host, self._client_key, self._decryption_key, self._cache_ttl
         )
@@ -742,29 +953,34 @@
 
     def set_features(self, features: dict) -> None:
         self._features = {}
         for key, feature in features.items():
             if isinstance(feature, Feature):
                 self._features[key] = feature
             else:
-                self._features[key] = Feature(**feature)
+                self._features[key] = Feature(
+                    rules=feature.get("rules", []),
+                    defaultValue=feature.get("defaultValue", None),
+                )
+        self.refresh_sticky_buckets()
 
     # @deprecated, use get_features
     def getFeatures(self) -> Dict[str, Feature]:
         return self.get_features()
 
     def get_features(self) -> Dict[str, Feature]:
         return self._features
 
     # @deprecated, use set_attributes
     def setAttributes(self, attributes: dict) -> None:
         return self.set_attributes(attributes)
 
     def set_attributes(self, attributes: dict) -> None:
         self._attributes = attributes
+        self.refresh_sticky_buckets()
 
     # @deprecated, use get_attributes
     def getAttributes(self) -> dict:
         return self.get_attributes()
 
     def get_attributes(self) -> dict:
         return self._attributes
@@ -802,22 +1018,56 @@
         res = self.evalFeature(key)
         return res.value if res.value is not None else fallback
 
     # @deprecated, use eval_feature
     def evalFeature(self, key: str) -> FeatureResult:
         return self.eval_feature(key)
 
+    def eval_prereqs(self, parentConditions: List[dict], stack: Set[str]) -> str:
+        for parentCondition in parentConditions:
+            parentRes = self._eval_feature(parentCondition.get("id", None), stack)
+
+            if parentRes.source == "cyclicPrerequisite":
+                return "cyclic"
+
+            if not evalCondition({'value': parentRes.value}, parentCondition.get("condition", None)):
+                if parentCondition.get("gate", False):
+                    return "gate"
+                return "fail"
+        return "pass"
+
     def eval_feature(self, key: str) -> FeatureResult:
+        return self._eval_feature(key, set())
+
+    def _eval_feature(self, key: str, stack: Set[str]) -> FeatureResult:
         logger.debug("Evaluating feature %s", key)
         if key not in self._features:
             logger.warning("Unknown feature %s", key)
             return FeatureResult(None, "unknownFeature")
 
+        if key in stack:
+            logger.warning("Cyclic prerequisite detected, stack: %s", stack)
+            return FeatureResult(None, "cyclicPrerequisite")
+        stack.add(key)
+
         feature = self._features[key]
         for rule in feature.rules:
+            logger.debug("Evaluating feature %s, rule %s", key, rule.to_dict())
+            if (rule.parentConditions):
+                prereq_res = self.eval_prereqs(rule.parentConditions, stack)
+                if prereq_res == "gate":
+                    logger.debug("Top-level prerequisite failed, return None, feature %s", key)
+                    return FeatureResult(None, "prerequisite")
+                if prereq_res == "cyclic":
+                    # Warning already logged in this case
+                    return FeatureResult(None, "cyclicPrerequisite")
+                if prereq_res == "fail":
+                    logger.debug("Skip rule because of failing prerequisite, feature %s", key)
+                    continue
+
             if rule.condition:
                 if not evalCondition(self._attributes, rule.condition):
                     logger.debug(
                         "Skip rule because of failed condition, feature %s", key
                     )
                     continue
             if rule.filters:
@@ -826,94 +1076,119 @@
                         "Skip rule because of filters/namespaces, feature %s", key
                     )
                     continue
             if rule.force is not None:
                 if not self._isIncludedInRollout(
                     rule.seed or key,
                     rule.hashAttribute,
+                    rule.fallbackAttribute,
                     rule.range,
                     rule.coverage,
                     rule.hashVersion,
                 ):
                     logger.debug(
                         "Skip rule because user not included in percentage rollout, feature %s",
                         key,
                     )
                     continue
 
                 logger.debug("Force value from rule, feature %s", key)
-                return FeatureResult(rule.force, "force")
+                return FeatureResult(rule.force, "force", ruleId=rule.id)
 
             if rule.variations is None:
                 logger.warning("Skip invalid rule, feature %s", key)
                 continue
 
             exp = Experiment(
                 key=rule.key or key,
                 variations=rule.variations,
                 coverage=rule.coverage,
                 weights=rule.weights,
                 hashAttribute=rule.hashAttribute,
+                fallbackAttribute=rule.fallbackAttribute,
                 namespace=rule.namespace,
                 hashVersion=rule.hashVersion,
                 meta=rule.meta,
                 ranges=rule.ranges,
                 name=rule.name,
                 phase=rule.phase,
                 seed=rule.seed,
                 filters=rule.filters,
+                condition=rule.condition,
+                disableStickyBucketing=rule.disableStickyBucketing,
+                bucketVersion=rule.bucketVersion,
+                minBucketVersion=rule.minBucketVersion,
             )
 
             result = self._run(exp, key)
             self._fireSubscriptions(exp, result)
 
             if not result.inExperiment:
-                logger.debug("Skip rule because user not included in experiment", key)
+                logger.debug(
+                    "Skip rule because user not included in experiment, feature %s", key
+                )
                 continue
 
             if result.passthrough:
                 logger.debug("Continue to next rule, feature %s", key)
                 continue
 
             logger.debug("Assign value from experiment, feature %s", key)
-            return FeatureResult(result.value, "experiment", exp, result)
+            return FeatureResult(
+                result.value, "experiment", exp, result, ruleId=rule.id
+            )
 
         logger.debug("Use default value for feature %s", key)
         return FeatureResult(feature.defaultValue, "defaultValue")
 
     # @deprecated, use get_all_results
     def getAllResults(self):
         return self.get_all_results()
 
     def get_all_results(self):
         return self._assigned.copy()
 
-    def _getOrigHashValue(self, attr: str = None):
+    def _getOrigHashValue(self, attr: str = None, fallbackAttr: str = None) -> Tuple[str, str]:
+
         attr = attr or "id"
+        val = ""
         if attr in self._attributes:
-            return self._attributes[attr] or ""
-        if attr in self._user:
-            return self._user[attr] or ""
-        return ""
-
-    def _getHashValue(self, attr: str = None) -> str:
-        return str(self._getOrigHashValue(attr))
+            val = self._attributes[attr] or ""
+        elif attr in self._user:
+            val = self._user[attr] or ""
+
+        # If no match, try fallback
+        if (not val or val == "") and fallbackAttr and self.sticky_bucket_service:
+            if fallbackAttr in self._attributes:
+                val = self._attributes[fallbackAttr] or ""
+            elif fallbackAttr in self._user:
+                val = self._user[fallbackAttr] or ""
+
+            if not val or val != "":
+                attr = fallbackAttr
+
+        return (attr, val)
+
+    def _getHashValue(self, attr: str = None, fallbackAttr: str = None) -> Tuple[str, str]:
+        (attr, val) = self._getOrigHashValue(attr, fallbackAttr)
+        return (attr, str(val))
 
     def _isIncludedInRollout(
         self,
         seed: str,
         hashAttribute: str = None,
+        fallbackAttribute: str = None,
         range: Tuple[float, float] = None,
         coverage: float = None,
         hashVersion: int = None,
     ) -> bool:
         if coverage is None and range is None:
             return True
 
-        hash_value = self._getHashValue(hashAttribute or "id")
+        (_, hash_value) = self._getHashValue(hashAttribute, fallbackAttribute)
         if hash_value == "":
             return False
 
         n = gbhash(seed, hash_value, hashVersion or 1)
         if n is None:
             return False
 
@@ -922,15 +1197,15 @@
         elif coverage is not None:
             return n <= coverage
 
         return True
 
     def _isFilteredOut(self, filters: List[Filter]) -> bool:
         for filter in filters:
-            hash_value = self._getHashValue(filter.get("attribute", "id"))
+            (_, hash_value) = self._getHashValue(filter.get("attribute", "id"))
             if hash_value == "":
                 return False
 
             n = gbhash(filter.get("seed", ""), hash_value, filter.get("hashVersion", 2))
             if n is None:
                 return False
 
@@ -1006,96 +1281,138 @@
             return self._getExperimentResult(
                 experiment, self._forcedVariations[experiment.key], featureId=featureId
             )
         # 5. If experiment is a draft or not active, return immediately
         if experiment.status == "draft" or not experiment.active:
             logger.debug("Experiment %s is not active, skip", experiment.key)
             return self._getExperimentResult(experiment, featureId=featureId)
+
         # 6. Get the user hash attribute and value
-        hashAttribute = experiment.hashAttribute or "id"
-        hashValue = self._getHashValue(hashAttribute)
+        (hashAttribute, hashValue) = self._getHashValue(experiment.hashAttribute, experiment.fallbackAttribute)
         if not hashValue:
             logger.debug(
                 "Skip experiment %s because user's hashAttribute value is empty",
                 experiment.key,
             )
             return self._getExperimentResult(experiment, featureId=featureId)
 
-        # 7. Filtered out / not in namespace
-        if experiment.filters:
-            if self._isFilteredOut(experiment.filters):
-                logger.debug(
-                    "Skip experiment %s because of filters/namespaces", experiment.key
-                )
-                return self._getExperimentResult(experiment, featureId=featureId)
-        elif experiment.namespace and not inNamespace(hashValue, experiment.namespace):
-            logger.debug("Skip experiment %s because of namespace", experiment.key)
-            return self._getExperimentResult(experiment, featureId=featureId)
+        assigned = -1
 
-        # 7.5. If experiment has an include property
-        if experiment.include:
-            try:
-                if not experiment.include():
+        found_sticky_bucket = False
+        sticky_bucket_version_is_blocked = False
+        if self.sticky_bucket_service and not experiment.disableStickyBucketing:
+            sticky_bucket = self._get_sticky_bucket_variation(
+                experiment.key,
+                experiment.bucketVersion,
+                experiment.minBucketVersion,
+                experiment.meta,
+                hash_attribute=experiment.hashAttribute,
+                fallback_attribute=experiment.fallbackAttribute,
+            )
+            found_sticky_bucket = sticky_bucket.get('variation', 0) >= 0
+            assigned = sticky_bucket.get('variation', 0)
+            sticky_bucket_version_is_blocked = sticky_bucket.get('versionIsBlocked', False)
+
+        if found_sticky_bucket:
+            logger.debug("Found sticky bucket for experiment %s, assigning sticky variation %s", experiment.key, assigned)
+
+        # Some checks are not needed if we already have a sticky bucket
+        if not found_sticky_bucket:
+            # 7. Filtered out / not in namespace
+            if experiment.filters:
+                if self._isFilteredOut(experiment.filters):
                     logger.debug(
-                        "Skip experiment %s because include() returned false",
-                        experiment.key,
+                        "Skip experiment %s because of filters/namespaces", experiment.key
                     )
                     return self._getExperimentResult(experiment, featureId=featureId)
-            except Exception:
-                logger.warning(
-                    "Skip experiment %s because include() raised an Exception",
-                    experiment.key,
-                )
+            elif experiment.namespace and not inNamespace(hashValue, experiment.namespace):
+                logger.debug("Skip experiment %s because of namespace", experiment.key)
                 return self._getExperimentResult(experiment, featureId=featureId)
 
-        # 8. Exclude if condition is false
-        if experiment.condition and not evalCondition(
-            self._attributes, experiment.condition
-        ):
-            logger.debug(
-                "Skip experiment %s because user failed the condition", experiment.key
-            )
-            return self._getExperimentResult(experiment, featureId=featureId)
+            # 7.5. If experiment has an include property
+            if experiment.include:
+                try:
+                    if not experiment.include():
+                        logger.debug(
+                            "Skip experiment %s because include() returned false",
+                            experiment.key,
+                        )
+                        return self._getExperimentResult(experiment, featureId=featureId)
+                except Exception:
+                    logger.warning(
+                        "Skip experiment %s because include() raised an Exception",
+                        experiment.key,
+                    )
+                    return self._getExperimentResult(experiment, featureId=featureId)
 
-        # 8.1. Make sure user is in a matching group
-        if experiment.groups and len(experiment.groups):
-            expGroups = self._groups or {}
-            matched = False
-            for group in experiment.groups:
-                if expGroups[group]:
-                    matched = True
-            if not matched:
+            # 8. Exclude if condition is false
+            if experiment.condition and not evalCondition(
+                self._attributes, experiment.condition
+            ):
                 logger.debug(
-                    "Skip experiment %s because user not in required group",
-                    experiment.key,
+                    "Skip experiment %s because user failed the condition", experiment.key
                 )
                 return self._getExperimentResult(experiment, featureId=featureId)
+
+            # 8.05 Exclude if parent conditions are not met
+            if (experiment.parentConditions):
+                prereq_res = self.eval_prereqs(experiment.parentConditions, set())
+                if prereq_res == "gate" or prereq_res == "fail":
+                    logger.debug("Skip experiment %s because of failing prerequisite", experiment.key)
+                    return self._getExperimentResult(experiment, featureId=featureId)
+                if prereq_res == "cyclic":
+                    logger.debug("Skip experiment %s because of cyclic prerequisite", experiment.key)
+                    return self._getExperimentResult(experiment, featureId=featureId)
+
+            # 8.1. Make sure user is in a matching group
+            if experiment.groups and len(experiment.groups):
+                expGroups = self._groups or {}
+                matched = False
+                for group in experiment.groups:
+                    if expGroups[group]:
+                        matched = True
+                if not matched:
+                    logger.debug(
+                        "Skip experiment %s because user not in required group",
+                        experiment.key,
+                    )
+                    return self._getExperimentResult(experiment, featureId=featureId)
+
+        # The following apply even when in a sticky bucket
+
         # 8.2. If experiment.url is set, see if it's valid
         if experiment.url:
             if not self._urlIsValid(experiment.url):
                 logger.debug(
                     "Skip experiment %s because current URL is not targeted",
                     experiment.key,
                 )
                 return self._getExperimentResult(experiment, featureId=featureId)
 
         # 9. Get bucket ranges and choose variation
-        c = experiment.coverage
-        ranges = experiment.ranges or getBucketRanges(
-            len(experiment.variations), c if c is not None else 1, experiment.weights
-        )
         n = gbhash(
             experiment.seed or experiment.key, hashValue, experiment.hashVersion or 1
         )
         if n is None:
             logger.warning(
                 "Skip experiment %s because of invalid hashVersion", experiment.key
             )
             return self._getExperimentResult(experiment, featureId=featureId)
-        assigned = chooseVariation(n, ranges)
+
+        if not found_sticky_bucket:
+            c = experiment.coverage
+            ranges = experiment.ranges or getBucketRanges(
+                len(experiment.variations), c if c is not None else 1, experiment.weights
+            )
+            assigned = chooseVariation(n, ranges)
+
+        # Unenroll if any prior sticky buckets are blocked by version
+        if sticky_bucket_version_is_blocked:
+            logger.debug("Skip experiment %s because sticky bucket version is blocked", experiment.key)
+            return self._getExperimentResult(experiment, featureId=featureId, stickyBucketUsed=True)
 
         # 10. Return if not in experiment
         if assigned < 0:
             logger.debug(
                 "Skip experiment %s because user is not included in the rollout",
                 experiment.key,
             )
@@ -1118,24 +1435,42 @@
         # 12.5. If experiment is stopped, return immediately
         if experiment.status == "stopped":
             logger.debug("Skip experiment %s because it is stopped", experiment.key)
             return self._getExperimentResult(experiment, featureId=featureId)
 
         # 13. Build the result object
         result = self._getExperimentResult(
-            experiment, assigned, True, featureId=featureId, bucket=n
+            experiment, assigned, True, featureId=featureId, bucket=n, stickyBucketUsed=found_sticky_bucket
         )
 
+        # 13.5 Persist sticky bucket
+        if self.sticky_bucket_service and not experiment.disableStickyBucketing:
+            assignment = {}
+            assignment[self._get_sticky_bucket_experiment_key(
+                experiment.key,
+                experiment.bucketVersion
+            )] = result.key
+
+            data = self._generate_sticky_bucket_assignment_doc(
+                hashAttribute,
+                hashValue,
+                assignment
+            )
+            doc = data.get("doc", None)
+            if doc and data.get('changed', False):
+                if not self._sticky_bucket_assignment_docs:
+                    self._sticky_bucket_assignment_docs = {}
+                self._sticky_bucket_assignment_docs[data.get('key')] = doc
+                self.sticky_bucket_service.save_assignments(doc)
+
         # 14. Fire the tracking callback if set
         self._track(experiment, result)
 
         # 15. Return the result
-        logger.debug(
-            "Assigned variation %d in experiment %s", assigned, experiment.key
-        )
+        logger.debug("Assigned variation %d in experiment %s", assigned, experiment.key)
         return result
 
     def _track(self, experiment: Experiment, result: Result) -> None:
         if not self._trackingCallback:
             return None
         key = (
             result.hashAttribute
@@ -1169,30 +1504,161 @@
     def _getExperimentResult(
         self,
         experiment: Experiment,
         variationId: int = -1,
         hashUsed: bool = False,
         featureId: str = None,
         bucket: float = None,
+        stickyBucketUsed: bool = False
     ) -> Result:
-        hashAttribute = experiment.hashAttribute or "id"
-
         inExperiment = True
         if variationId < 0 or variationId > len(experiment.variations) - 1:
             variationId = 0
             inExperiment = False
 
         meta = None
         if experiment.meta:
             meta = experiment.meta[variationId]
 
+        (hashAttribute, hashValue) = self._getOrigHashValue(experiment.hashAttribute, experiment.fallbackAttribute)
+
         return Result(
             featureId=featureId,
             inExperiment=inExperiment,
             variationId=variationId,
             value=experiment.variations[variationId],
             hashUsed=hashUsed,
             hashAttribute=hashAttribute,
-            hashValue=self._getOrigHashValue(hashAttribute),
+            hashValue=hashValue,
             meta=meta,
             bucket=bucket,
+            stickyBucketUsed=stickyBucketUsed
         )
+
+    def _derive_sticky_bucket_identifier_attributes(self) -> List[str]:
+        attributes = set()
+        for key, feature in self._features.items():
+            for rule in feature.rules:
+                if rule.variations:
+                    attributes.add(rule.hashAttribute or "id")
+                    if rule.fallbackAttribute:
+                        attributes.add(rule.fallbackAttribute)
+        return list(attributes)
+
+    def _get_sticky_bucket_attributes(self) -> dict:
+        attributes: Dict[str, str] = {}
+        if self._using_derived_sticky_bucket_attributes:
+            self.sticky_bucket_identifier_attributes = self._derive_sticky_bucket_identifier_attributes()
+
+        if not self.sticky_bucket_identifier_attributes:
+            return attributes
+
+        for attr in self.sticky_bucket_identifier_attributes:
+            _, hash_value = self._getHashValue(attr)
+            if hash_value:
+                attributes[attr] = hash_value
+        return attributes
+
+    def _get_sticky_bucket_assignments(self, attr: str = None, fallback: str = None) -> Dict[str, str]:
+        merged: Dict[str, str] = {}
+
+        _, hashValue = self._getHashValue(attr)
+        key = f"{attr}||{hashValue}"
+        if key in self._sticky_bucket_assignment_docs:
+            merged = self._sticky_bucket_assignment_docs[key].get("assignments", {})
+
+        if fallback:
+            _, hashValue = self._getHashValue(fallback)
+            key = f"{fallback}||{hashValue}"
+            if key in self._sticky_bucket_assignment_docs:
+                # Merge the fallback assignments, but don't overwrite existing ones
+                for k, v in self._sticky_bucket_assignment_docs[key].get("assignments", {}).items():
+                    if k not in merged:
+                        merged[k] = v
+
+        return merged
+
+    def _is_blocked(
+        self,
+        assignments: Dict[str, str],
+        experiment_key: str,
+        min_bucket_version: int
+    ) -> bool:
+        if min_bucket_version > 0:
+            for i in range(min_bucket_version):
+                blocked_key = self._get_sticky_bucket_experiment_key(experiment_key, i)
+                if blocked_key in assignments:
+                    return True
+        return False
+
+    def _get_sticky_bucket_variation(
+        self,
+        experiment_key: str,
+        bucket_version: int = None,
+        min_bucket_version: int = None,
+        meta: List[VariationMeta] = None,
+        hash_attribute: str = None,
+        fallback_attribute: str = None
+    ) -> dict:
+        bucket_version = bucket_version or 0
+        min_bucket_version = min_bucket_version or 0
+        meta = meta or []
+
+        id = self._get_sticky_bucket_experiment_key(experiment_key, bucket_version)
+
+        assignments = self._get_sticky_bucket_assignments(hash_attribute, fallback_attribute)
+        if self._is_blocked(assignments, experiment_key, min_bucket_version):
+            return {
+                'variation': -1,
+                'versionIsBlocked': True
+            }
+
+        variation_key = assignments.get(id, None)
+        if not variation_key:
+            return {
+                'variation': -1
+            }
+
+        # Find the key in meta
+        variation = next((i for i, v in enumerate(meta) if v.get("key") == variation_key), -1)
+        if variation < 0:
+            return {
+                'variation': -1
+            }
+
+        return {'variation': variation}
+
+    def _get_sticky_bucket_experiment_key(self, experiment_key: str, bucket_version: int = 0) -> str:
+        return experiment_key + "__" + str(bucket_version)
+
+    def refresh_sticky_buckets(self, force: bool = False) -> None:
+        if not self.sticky_bucket_service:
+            return
+
+        attributes = self._get_sticky_bucket_attributes()
+        if not force and attributes == self._sticky_bucket_attributes:
+            logger.debug("Skipping refresh of sticky bucket assignments, no changes")
+            return
+
+        self._sticky_bucket_attributes = attributes
+        self._sticky_bucket_assignment_docs = self.sticky_bucket_service.get_all_assignments(attributes)
+
+    def _generate_sticky_bucket_assignment_doc(self, attribute_name: str, attribute_value: str, assignments: dict):
+        key = attribute_name + "||" + attribute_value
+        existing_assignments = self._sticky_bucket_assignment_docs.get(key, {}).get("assignments", {})
+
+        new_assignments = {**existing_assignments, **assignments}
+
+        # Compare JSON strings to see if they have changed
+        existing_json = json.dumps(existing_assignments, sort_keys=True)
+        new_json = json.dumps(new_assignments, sort_keys=True)
+        changed = existing_json != new_json
+
+        return {
+            'key': key,
+            'doc': {
+                'attributeName': attribute_name,
+                'attributeValue': attribute_value,
+                'assignments': new_assignments
+            },
+            'changed': changed
+        }
```

### Comparing `growthbook-1.0.0/setup.py` & `growthbook-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,27 +9,31 @@
 
 requirements = ['cryptography', 'typing_extensions', 'urllib3', ]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     name='growthbook',
-    version='1.0.0',
+    version='1.1.0',
     author="GrowthBook",
     author_email='hello@growthbook.io',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     description="Powerful Feature flagging and A/B testing for Python apps",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=requirements,
     license="MIT",
     include_package_data=True,
```

