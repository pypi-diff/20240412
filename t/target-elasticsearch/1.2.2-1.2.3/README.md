# Comparing `tmp/target_elasticsearch-1.2.2.tar.gz` & `tmp/target_elasticsearch-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_elasticsearch-1.2.2.tar", max compression
+gzip compressed data, was "target_elasticsearch-1.2.3.tar", max compression
```

## Comparing `target_elasticsearch-1.2.2.tar` & `target_elasticsearch-1.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-02-09 20:36:32.090518 target_elasticsearch-1.2.2/LICENSE
--rw-r--r--   0        0        0     1124 2024-02-09 20:36:50.402517 target_elasticsearch-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-09 20:36:32.090518 target_elasticsearch-1.2.2/target_elasticsearch/__init__.py
--rw-r--r--   0        0        0      780 2024-02-09 20:36:32.094518 target_elasticsearch-1.2.2/target_elasticsearch/common.py
--rw-r--r--   0        0        0     8536 2024-02-09 20:36:32.094518 target_elasticsearch-1.2.2/target_elasticsearch/sinks.py
--rw-r--r--   0        0        0     4574 2024-02-09 20:36:32.094518 target_elasticsearch-1.2.2/target_elasticsearch/target.py
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 target_elasticsearch-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-11 23:55:49.505906 target_elasticsearch-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1124 2024-04-11 23:56:08.361920 target_elasticsearch-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 23:55:49.509906 target_elasticsearch-1.2.3/target_elasticsearch/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-11 23:55:49.509906 target_elasticsearch-1.2.3/target_elasticsearch/common.py
+-rw-r--r--   0        0        0     8808 2024-04-11 23:55:49.509906 target_elasticsearch-1.2.3/target_elasticsearch/sinks.py
+-rw-r--r--   0        0        0     4959 2024-04-11 23:55:49.509906 target_elasticsearch-1.2.3/target_elasticsearch/target.py
+-rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 target_elasticsearch-1.2.3/PKG-INFO
```

### Comparing `target_elasticsearch-1.2.2/LICENSE` & `target_elasticsearch-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `target_elasticsearch-1.2.2/pyproject.toml` & `target_elasticsearch-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-elasticsearch"
-version = "1.2.2"
+version = "1.2.3"
 description = "`target-elasticsearch` is a singer target using the meltano SDK for targets"
 authors = ["DT Mirizzi <dtmirizzi@gmail.com>"]
 keywords = [
     "elasticsearch",
     "ELT",
     "target",
     "meltano",
```

### Comparing `target_elasticsearch-1.2.2/target_elasticsearch/common.py` & `target_elasticsearch-1.2.3/target_elasticsearch/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 API_KEY = "api_key"
 ENCODED_API_KEY = "encoded_api_key"
 SSL_CA_FILE = "ssl_ca_file"
 INDEX_FORMAT = "index_format"
 INDEX_TEMPLATE_FIELDS = "index_schema_fields"
 METADATA_FIELDS = "metadata_fields"
 NAME = "target-elasticsearch"
+REQUEST_TIMEOUT = "request_timeout"
+RETRY_ON_TIMEOUT = "retry_on_timeout"
+
+DEFAULT_REQUEST_TIMEOUT = 10
+DEFAULT_RETRY_ON_TIMEOUT = True
 
 
 def to_daily(date) -> str:
     return parse(date).date().strftime(ELASTIC_DAILY_FORMAT)
 
 
 def to_monthly(date) -> str:
```

### Comparing `target_elasticsearch-1.2.2/target_elasticsearch/sinks.py` & `target_elasticsearch-1.2.3/target_elasticsearch/sinks.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     SSL_CA_FILE,
     INDEX_TEMPLATE_FIELDS,
     ELASTIC_YEARLY_FORMAT,
     ELASTIC_MONTHLY_FORMAT,
     ELASTIC_DAILY_FORMAT,
     METADATA_FIELDS,
     NAME,
+    REQUEST_TIMEOUT,
+    RETRY_ON_TIMEOUT,
     to_daily,
     to_monthly,
     to_yearly,
 )
 
 
 def template_index(stream_name: str, index_format: str, schemas: Dict) -> str:
@@ -183,14 +185,20 @@
         scheme = self.config[SCHEME]
         if SSL_CA_FILE in self.config:
             scheme = "https"
             config["ca_certs"] = self.config[SSL_CA_FILE]
 
         config["hosts"] = [f"{scheme}://{self.config[HOST]}:{self.config[PORT]}"]
 
+        if REQUEST_TIMEOUT in self.config:
+            config["request_timeout"] = self.config[REQUEST_TIMEOUT]
+
+        if RETRY_ON_TIMEOUT in self.config:
+            config["retry_on_timeout"] = self.config[RETRY_ON_TIMEOUT]
+
         if USERNAME in self.config and PASSWORD in self.config:
             config["basic_auth"] = (self.config[USERNAME], self.config[PASSWORD])
         elif API_KEY in self.config and API_KEY_ID in self.config:
             config["api_key"] = (self.config[API_KEY_ID], self.config[API_KEY])
         elif ENCODED_API_KEY in self.config:
             config["api_key"] = self.config[ENCODED_API_KEY]
         elif BEARER_TOKEN in self.config:
```

### Comparing `target_elasticsearch-1.2.2/target_elasticsearch/target.py` & `target_elasticsearch-1.2.3/target_elasticsearch/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     BEARER_TOKEN,
     API_KEY_ID,
     API_KEY,
     ENCODED_API_KEY,
     SSL_CA_FILE,
     INDEX_TEMPLATE_FIELDS,
     METADATA_FIELDS,
+    REQUEST_TIMEOUT,
+    RETRY_ON_TIMEOUT,
 )
 
 
 class TargetElasticsearch(Target):
     """Sample target for parquet."""
 
     name = "target-elasticsearch"
@@ -125,13 +127,25 @@
             description="""Metadata Fields can be used to pull out specific fields via jsonpath to be
     used on for [ecs metadata patters](https://www.elastic.co/guide/en/elasticsearch/reference/current/mapping-fields.html)
     This would best be used for data that has a primary key.
     ie. `{"guid": 102, "foo": "bar"}`
     then create a mapping of `_id: guid""",
             default=None,
         ),
+        th.Property(
+            REQUEST_TIMEOUT,
+            th.NumberType,
+            description="request timeout in seconds",
+            default=10,
+        ),
+        th.Property(
+            RETRY_ON_TIMEOUT,
+            th.BooleanType,
+            description="retry failed requests on timeout",
+            default=True,
+        ),
     ).to_dict()
     default_sink_class = sinks.ElasticSink
 
     @property
     def state(self) -> Dict:
         return {}
```

### Comparing `target_elasticsearch-1.2.2/PKG-INFO` & `target_elasticsearch-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-elasticsearch
-Version: 1.2.2
+Version: 1.2.3
 Summary: `target-elasticsearch` is a singer target using the meltano SDK for targets
 License: GNU v3
 Keywords: elasticsearch,ELT,target,meltano,singer
 Author: DT Mirizzi
 Author-email: dtmirizzi@gmail.com
 Requires-Python: >=3.9.1,<3.12
 Classifier: License :: Other/Proprietary License
```

