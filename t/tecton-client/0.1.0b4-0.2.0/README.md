# Comparing `tmp/tecton_client-0.1.0b4.tar.gz` & `tmp/tecton_client-0.2.0.tar.gz`

## Comparing `tecton_client-0.1.0b4.tar` & `tecton_client-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,35 @@
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/.github/pull_request_template.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/.github/workflows/testing.yml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/__init__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/client_options.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/constants.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/data_types.py
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/exceptions.py
--rw-r--r--   0        0        0     9201 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/http_client.py
--rw-r--r--   0        0        0    22817 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/requests.py
--rw-r--r--   0        0        0    28060 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/responses.py
--rw-r--r--   0        0        0    17149 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/tecton_client.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tecton_client/utils.py
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/data_types_test.py
--rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/http_client_test.py
--rw-r--r--   0        0        0    18314 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/requests_test.py
--rw-r--r--   0        0        0    21264 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/responses_test.py
--rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/tecton_client_test.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_utils.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/sample_metadata_response.json
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/sample_metadata_response_long.json
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/batch/batch_expected_request_1.json
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/batch/batch_expected_request_2.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/batch/batch_expected_request_3.json
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/batch/batch_expected_request_4.json
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/batch/sample_batch_response.json
--rw-r--r--   0        0        0     6719 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/batch/sample_batch_response_long_slo.json
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/batch/sample_batch_response_slo.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response.json
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response_list.json
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response_long.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response_metadata.json
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response_mixed.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response_null.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response_slo.json
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/tests/test_data/single/sample_response_struct.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/.gitignore
--rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/LICENSE.md
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/README.md
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 tecton_client-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 tecton_client-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 tecton_client-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/release-docs.yml
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/quickstart.rst
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 tecton_client-0.2.0/docs/tecton_client.rst
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 tecton_client-0.2.0/examples/example_async.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tecton_client-0.2.0/examples/example_sync.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/__about__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/__init__.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/__init__.py
+-rw-r--r--   0        0        0     6626 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/async_tecton_client.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/data_types.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/tecton_client.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tecton_client/_internal/utils.py
+-rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_async_client.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_data_types.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_tecton_client.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_data/nested_sample_response.json
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tecton_client-0.2.0/tests/test_data/sample_response.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tecton_client-0.2.0/.gitignore
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 tecton_client-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 tecton_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 tecton_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 tecton_client-0.2.0/PKG-INFO
```

### Comparing `tecton_client-0.1.0b4/.github/workflows/testing.yml` & `tecton_client-0.2.0/.github/workflows/testing.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # This workflow will install Python dependencies and run tests
 
 name: pytest
 
 on:
   push:
-    branches:
-      - '**'
+    branches: [ main ]
   pull_request:
-    branches: [ "main" ]
+    branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     strategy:
@@ -28,7 +27,20 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e '.[dev]'
     - name: Test with pytest
       run: |
         python -m pytest tests/
+
+  build-docs:
+    name: verify-docs-build
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v3
+      - name: Install dependencies
+        run: |
+          pip install -e ".[docs]"
+      - name: Sphinx build
+        run: |
+          sphinx-build docs docs/build
```

### Comparing `tecton_client-0.1.0b4/tests/test_data/single/sample_response_list.json` & `tecton_client-0.2.0/tests/test_data/sample_response.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'metadata'": "{'features': {insert: [(3, OrderedDict([('name', 'average_rain.fake_example'), "*

 * *               "('dataType', OrderedDict([('type', 'array'), ('elementType', OrderedDict([('type', "*

 * *               "'int64')]))]))]))]}}",*

 * * "'result'": "{'features': {insert: [(3, ['0', '1', None, '3', '4', None])]}}"}*

```diff
@@ -23,14 +23,23 @@
                 "dataType": {
                     "elementType": {
                         "type": "float64"
                     },
                     "type": "array"
                 },
                 "name": "average_rain.average_temperate_6hrs"
+            },
+            {
+                "dataType": {
+                    "elementType": {
+                        "type": "int64"
+                    },
+                    "type": "array"
+                },
+                "name": "average_rain.fake_example"
             }
         ]
     },
     "result": {
         "features": [
             [
                 "0"
@@ -39,11 +48,19 @@
             [
                 55.5,
                 57.88,
                 58.96,
                 57.66,
                 null,
                 55.98
+            ],
+            [
+                "0",
+                "1",
+                null,
+                "3",
+                "4",
+                null
             ]
         ]
     }
 }
```

### Comparing `tecton_client-0.1.0b4/tests/test_data/single/sample_response_mixed.json` & `tecton_client-0.2.0/tests/test_data/nested_sample_response.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8050440228174603%*

 * *Differences: {"'metadata'": "{'features': {0: {'name': 'schema.map', 'dataType': {'type': 'map', 'keyType': "*

 * *               "OrderedDict([('type', 'string')]), 'valueType': OrderedDict([('type', 'int64')]), "*

 * *               "delete: ['fields']}}, 1: {'name': 'schema.two_dimensional_array', 'dataType': "*

 * *               "{'elementType': {'type': 'array', 'elementType': OrderedDict([('type', "*

 * *               "'int64')])}}}, 2: {'name': 'schema.simple_struct', 'dataType': {'type': 'struct', "*

 * *               "'fields': [Ord […]*

```diff
@@ -1,92 +1,83 @@
 {
     "metadata": {
         "features": [
             {
                 "dataType": {
-                    "fields": [
-                        {
-                            "dataType": {
-                                "type": "string"
-                            },
-                            "name": "string_field"
+                    "keyType": {
+                        "type": "string"
+                    },
+                    "type": "map",
+                    "valueType": {
+                        "type": "int64"
+                    }
+                },
+                "name": "schema.map"
+            },
+            {
+                "dataType": {
+                    "elementType": {
+                        "elementType": {
+                            "type": "int64"
                         },
-                        {
-                            "dataType": {
-                                "type": "float64"
-                            },
-                            "name": "float64_field"
-                        }
-                    ],
-                    "type": "struct"
+                        "type": "array"
+                    },
+                    "type": "array"
                 },
-                "name": "test.output_struct1"
+                "name": "schema.two_dimensional_array"
             },
             {
                 "dataType": {
                     "fields": [
                         {
                             "dataType": {
                                 "type": "string"
                             },
                             "name": "string_field"
                         },
                         {
                             "dataType": {
+                                "type": "int64"
+                            },
+                            "name": "int64_field"
+                        },
+                        {
+                            "dataType": {
                                 "type": "float64"
                             },
                             "name": "float64_field"
                         }
                     ],
                     "type": "struct"
                 },
-                "name": "test.output_struct2"
-            },
-            {
-                "dataType": {
-                    "elementType": {
-                        "type": "int64"
-                    },
-                    "type": "array"
-                },
-                "name": "test.output_array"
-            },
-            {
-                "dataType": {
-                    "type": "string"
-                },
-                "name": "test.output_string"
-            },
-            {
-                "dataType": {
-                    "type": "int64"
-                },
-                "name": "test.output_int1"
+                "name": "schema.simple_struct"
             },
             {
                 "dataType": {
                     "type": "int64"
                 },
-                "name": "test.output_int2"
+                "name": "schema.dist_km"
             }
         ]
     },
     "result": {
         "features": [
-            null,
+            {
+                "this": "123"
+            },
             [
-                "2.46",
-                2.46
+                [
+                    "123",
+                    null
+                ],
+                null,
+                []
             ],
             [
-                1,
-                2,
-                3,
-                null,
-                5
+                "fake-string",
+                "12",
+                123
             ],
-            "test",
-            24,
-            691
+            "100"
         ]
     }
 }
```

### Comparing `tecton_client-0.1.0b4/LICENSE.md` & `tecton_client-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tecton_client-0.1.0b4/README.md` & `tecton_client-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 # Python Client Library for Tecton Online Feature Store
 
 A simple Python client for the Feature Server HTTP API that helps customers integrate with Tecton easily.
 
 
 ## Documentation
 
+* [Tecton Python Client API Reference](https://tecton-ai.github.io/tecton-http-client-python/html/index.html)
 
-* [Fetching Online Features](https://docs.tecton.ai/latest/examples/fetch-real-time-features.html)
+* [Tecton Python Client Example Code](/examples)
 
 * [FeatureServer API Reference](https://docs.tecton.ai/rest-swagger/docs.html)
 
-* [Tecton Python Client API Reference](https://tecton-ai.github.io/tecton-http-client-python/html/index.html)
-
-* [Tecton Python Client Example Code](https://github.com/tecton-ai/tecton-http-client-python-demo/)
+* [Fetching Online Features](https://docs.tecton.ai/latest/examples/fetch-real-time-features.html)
 
 
 ## Troubleshooting
 
 
-If you have any questions or need help, please [open an Issue](https://github.com/tecton-ai/tecton-http-client-python)
-or reach out to us on Slack!
+If you have any questions or need help, please contact us using the instructions in the
+[Tecton Docs](https://docs.tecton.ai/creating-a-tecton-support-ticket).
 
 ## Installing the client
 
 The client can be installed using `pip`.
 
 ```bash
 pip install tecton-client
 ```
 
 The client can then be used as below:
 
 
 ```python
-tecton_client = TectonClient(url, api_key)
-
-get_features_request_data = GetFeaturesRequestData(
-    join_key_map={"user_id": "123", "merchant": "xyz"},
-    request_context_map={"amt": 500.00},
-)
+from tecton_client import TectonClient
 
-get_features_request = GetFeaturesRequest(
-    workspace_name="<Your-workspace>",
-    feature_service_name="fraud_detection_feature_service",
-    request_data=get_features_request_data,
+url = "https://explore.tecton.ai/"
+workspace = "prod"
+api_key = "my-secret-key"
+
+client = TectonClient(url=url, default_workspace_name=workspace, api_key=api_key)
+
+resp = client.get_features(
+    feature_service_name="fraud_detection_feature_service:v2",
+    join_key_map={"user_id": "user_4407104885"},
+    request_context_map={"amount": 500.00},
 )
 
-get_features_response = tecton_client.get_features(get_features_request)
-
-print(
-    [feature.feature_value for feature in get_features_response.feature_values.values()]
-)
+print(resp.get_features_dict())
 ```
 
 For more information, please refer to Tecton documentation on the Python Client Library.
 
+## Filing Issues and Feature Requests
+
+### Python Client Issues
+If you encounter a problem specifically related to the Python client, please file a but using the instructions in the
+[Tecton Docs](https://docs.tecton.ai/creating-a-tecton-support-ticket). Please include the following information:
+
+   - Description of the problem.
+   - Steps to reproduce the issue.
+   - Any relevant error messages or stack traces.
+   - Versions of Python and the Python client you are using.
+
+Please provide as much detail as possible when filing a support ticket to help us understand and resolve the issue efficiently.
+
+Thank you for helping us improve our platform!
+
+## Contributing
+
+If you would like to contribute to the client, see [CONTRIBUTING.md](CONTRIBUTING.md)
+
 ## License
 
 The project is licensed
 under [Apache License 2.0](https://github.com/tecton-ai/tecton-http-client-python/blob/main/LICENSE.md)
```

