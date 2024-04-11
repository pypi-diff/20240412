# Comparing `tmp/airbyte_source_salesforce-2.4.4.tar.gz` & `tmp/airbyte_source_salesforce-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_salesforce-2.4.4.tar", max compression
+gzip compressed data, was "airbyte_source_salesforce-2.5.0.tar", max compression
```

## Comparing `airbyte_source_salesforce-2.4.4.tar` & `airbyte_source_salesforce-2.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4568 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/README.md
--rw-r--r--   0        0        0      826 2024-04-09 20:25:39.281002 airbyte_source_salesforce-2.4.4/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/__init__.py
--rw-r--r--   0        0        0    16870 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/api.py
--rw-r--r--   0        0        0     1667 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/availability_strategy.py
--rw-r--r--   0        0        0      808 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/exceptions.py
--rw-r--r--   0        0        0     3946 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/rate_limiting.py
--rw-r--r--   0        0        0     1619 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/run.py
--rw-r--r--   0        0        0     9747 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/schemas/Describe.json
--rw-r--r--   0        0        0    14130 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/source.py
--rw-r--r--   0        0        0     4769 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/spec.yaml
--rw-r--r--   0        0        0    41238 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/streams.py
--rw-r--r--   0        0        0     1024 2024-04-09 19:11:27.000000 airbyte_source_salesforce-2.4.4/source_salesforce/utils.py
--rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/README.md
+-rw-r--r--   0        0        0      826 2024-04-11 13:03:32.265453 airbyte_source_salesforce-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/__init__.py
+-rw-r--r--   0        0        0    16870 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/api.py
+-rw-r--r--   0        0        0     1621 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/availability_strategy.py
+-rw-r--r--   0        0        0      808 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/exceptions.py
+-rw-r--r--   0        0        0     3946 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/rate_limiting.py
+-rw-r--r--   0        0        0     1619 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/run.py
+-rw-r--r--   0        0        0     9747 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/schemas/Describe.json
+-rw-r--r--   0        0        0    15225 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/source.py
+-rw-r--r--   0        0        0     4769 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/spec.yaml
+-rw-r--r--   0        0        0    41478 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/streams.py
+-rw-r--r--   0        0        0     1024 2024-04-11 12:33:37.000000 airbyte_source_salesforce-2.5.0/source_salesforce/utils.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.5.0/PKG-INFO
```

### Comparing `airbyte_source_salesforce-2.4.4/README.md` & `airbyte_source_salesforce-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/pyproject.toml` & `airbyte_source_salesforce-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.4.4"
+version = "2.5.0"
 name = "airbyte-source-salesforce"
 description = "Source implementation for Salesforce."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/api.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/availability_strategy.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/availability_strategy.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,11 +25,11 @@
           2. There are streams that do not allow you to make a sample using Salesforce `query` or `queryAll`.
              And since we use a dynamic method of generating streams for Salesforce connector - at the stage of discover,
              we cannot filter out these streams, so we check for them before reading from the streams.
         """
         if error.response.status_code in [codes.FORBIDDEN, codes.BAD_REQUEST]:
             error_data = error.response.json()[0]
             error_code = error_data.get("errorCode", "")
-            if error_code != "REQUEST_LIMIT_EXCEEDED" or error_code == "INVALID_TYPE_FOR_OPERATION":
+            if error_code != "REQUEST_LIMIT_EXCEEDED":
                 return False, f"Cannot receive data for stream '{stream.name}', error message: '{error_data.get('message')}'"
             return True, None
         raise error
```

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/exceptions.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/rate_limiting.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/run.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/schemas/Describe.json` & `airbyte_source_salesforce-2.5.0/source_salesforce/schemas/Describe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/source.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/source.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
-from datetime import datetime
+from datetime import datetime, timedelta, timezone
 from typing import Any, Iterator, List, Mapping, MutableMapping, Optional, Tuple, Union
 
+import isodate
 import pendulum
 import requests
 from airbyte_cdk import AirbyteLogger
 from airbyte_cdk.logger import AirbyteLogFormatter
 from airbyte_cdk.models import AirbyteMessage, AirbyteStateMessage, ConfiguredAirbyteCatalog, ConfiguredAirbyteStream, Level, SyncMode
 from airbyte_cdk.sources.concurrent_source.concurrent_source import ConcurrentSource
 from airbyte_cdk.sources.concurrent_source.concurrent_source_adapter import ConcurrentSourceAdapter
@@ -25,14 +26,15 @@
 from airbyte_protocol.models import FailureType
 from dateutil.relativedelta import relativedelta
 from pendulum.parsing.exceptions import ParserError
 from requests import codes, exceptions  # type: ignore[import]
 
 from .api import PARENT_SALESFORCE_OBJECTS, UNSUPPORTED_BULK_API_SALESFORCE_OBJECTS, UNSUPPORTED_FILTERING_STREAMS, Salesforce
 from .streams import (
+    LOOKBACK_SECONDS,
     BulkIncrementalSalesforceStream,
     BulkSalesforceStream,
     BulkSalesforceSubStream,
     Describe,
     IncrementalRestSalesforceStream,
     RestSalesforceStream,
     RestSalesforceSubStream,
@@ -168,89 +170,105 @@
             stream_kwargs["replication_key"] = replication_key
             stream_kwargs["stream_slice_step"] = config.get("stream_slice_step", "P30D")
         else:
             stream_class = full_refresh
 
         return stream_class, stream_kwargs
 
-    @classmethod
     def generate_streams(
-        cls,
+        self,
         config: Mapping[str, Any],
         stream_objects: Mapping[str, Any],
         sf_object: Salesforce,
     ) -> List[Stream]:
         """Generates a list of stream by their names. It can be used for different tests too"""
         authenticator = TokenAuthenticator(sf_object.access_token)
         schemas = sf_object.generate_schemas(stream_objects)
         default_args = [sf_object, authenticator, config]
         streams = []
+        state_manager = ConnectorStateManager(stream_instance_map={s.name: s for s in streams}, state=self.state)
         for stream_name, sobject_options in stream_objects.items():
             json_schema = schemas.get(stream_name, {})
 
-            stream_class, kwargs = cls.prepare_stream(stream_name, json_schema, sobject_options, *default_args)
+            stream_class, kwargs = self.prepare_stream(stream_name, json_schema, sobject_options, *default_args)
 
             parent_name = PARENT_SALESFORCE_OBJECTS.get(stream_name, {}).get("parent_name")
             if parent_name:
                 # get minimal schema required for getting proper class name full_refresh/incremental, rest/bulk
                 parent_schema = PARENT_SALESFORCE_OBJECTS.get(stream_name, {}).get("schema_minimal")
-                parent_class, parent_kwargs = cls.prepare_stream(parent_name, parent_schema, sobject_options, *default_args)
+                parent_class, parent_kwargs = self.prepare_stream(parent_name, parent_schema, sobject_options, *default_args)
                 kwargs["parent"] = parent_class(**parent_kwargs)
 
             stream = stream_class(**kwargs)
 
-            api_type = cls._get_api_type(stream_name, json_schema, config.get("force_use_bulk_api", False))
+            api_type = self._get_api_type(stream_name, json_schema, config.get("force_use_bulk_api", False))
             if api_type == "rest" and not stream.primary_key and stream.too_many_properties:
                 logger.warning(
                     f"Can not instantiate stream {stream_name}. It is not supported by the BULK API and can not be "
                     "implemented via REST because the number of its properties exceeds the limit and it lacks a primary key."
                 )
                 continue
-            streams.append(stream)
+
+            streams.append(self._wrap_for_concurrency(config, stream, state_manager))
+        streams.append(self._wrap_for_concurrency(config, Describe(sf_api=sf_object, catalog=self.catalog), state_manager))
         return streams
 
+    def _wrap_for_concurrency(self, config, stream, state_manager):
+        stream_slicer_cursor = None
+        if stream.cursor_field:
+            stream_slicer_cursor = self._create_stream_slicer_cursor(config, state_manager, stream)
+            if hasattr(stream, "set_cursor"):
+                stream.set_cursor(stream_slicer_cursor)
+        if hasattr(stream, "parent") and hasattr(stream.parent, "set_cursor"):
+            stream_slicer_cursor = self._create_stream_slicer_cursor(config, state_manager, stream)
+            stream.parent.set_cursor(stream_slicer_cursor)
+
+        if not stream_slicer_cursor or self._get_sync_mode_from_catalog(stream) == SyncMode.full_refresh:
+            cursor = FinalStateCursor(
+                stream_name=stream.name, stream_namespace=stream.namespace, message_repository=self.message_repository
+            )
+            state = None
+        else:
+            cursor = stream_slicer_cursor
+            state = cursor.state
+        return StreamFacade.create_from_stream(stream, self, logger, state, cursor)
+
     def streams(self, config: Mapping[str, Any]) -> List[Stream]:
         if not config.get("start_date"):
             config["start_date"] = (datetime.now() - relativedelta(years=self.START_DATE_OFFSET_IN_YEARS)).strftime(self.DATETIME_FORMAT)
         sf = self._get_sf_object(config)
         stream_objects = sf.get_validated_streams(config=config, catalog=self.catalog)
         streams = self.generate_streams(config, stream_objects, sf)
-        streams.append(Describe(sf_api=sf, catalog=self.catalog))
-        state_manager = ConnectorStateManager(stream_instance_map={s.name: s for s in streams}, state=self.state)
-
-        configured_streams = []
-
-        for stream in streams:
-            sync_mode = self._get_sync_mode_from_catalog(stream)
-            if sync_mode == SyncMode.full_refresh:
-                cursor = FinalStateCursor(
-                    stream_name=stream.name, stream_namespace=stream.namespace, message_repository=self.message_repository
-                )
-                state = None
-            else:
-                cursor_field_key = stream.cursor_field or ""
-                if not isinstance(cursor_field_key, str):
-                    raise AssertionError(f"A string cursor field key is required, but got {cursor_field_key}.")
-                cursor_field = CursorField(cursor_field_key)
-                legacy_state = state_manager.get_stream_state(stream.name, stream.namespace)
-                cursor = ConcurrentCursor(
-                    stream.name,
-                    stream.namespace,
-                    legacy_state,
-                    self.message_repository,
-                    state_manager,
-                    stream.state_converter,
-                    cursor_field,
-                    self._get_slice_boundary_fields(stream, state_manager),
-                    config["start_date"],
-                )
-                state = cursor.state
+        return streams
 
-            configured_streams.append(StreamFacade.create_from_stream(stream, self, logger, state, cursor))
-        return configured_streams
+    def _create_stream_slicer_cursor(
+        self, config: Mapping[str, Any], state_manager: ConnectorStateManager, stream: Stream
+    ) -> ConcurrentCursor:
+        """
+        We have moved the generation of stream slices to the concurrent CDK cursor
+        """
+        cursor_field_key = stream.cursor_field or ""
+        if not isinstance(cursor_field_key, str):
+            raise AssertionError(f"Nested cursor field are not supported hence type str is expected but got {cursor_field_key}.")
+        cursor_field = CursorField(cursor_field_key)
+        stream_state = state_manager.get_stream_state(stream.name, stream.namespace)
+        return ConcurrentCursor(
+            stream.name,
+            stream.namespace,
+            stream_state,
+            self.message_repository,
+            state_manager,
+            stream.state_converter,
+            cursor_field,
+            self._get_slice_boundary_fields(stream, state_manager),
+            datetime.fromtimestamp(pendulum.parse(config["start_date"]).timestamp(), timezone.utc),
+            stream.state_converter.get_end_provider(),
+            timedelta(seconds=LOOKBACK_SECONDS),
+            isodate.parse_duration(config["stream_slice_step"]) if "stream_slice_step" in config else timedelta(days=30),
+        )
 
     def _get_slice_boundary_fields(self, stream: Stream, state_manager: ConnectorStateManager) -> Optional[Tuple[str, str]]:
         return ("start_date", "end_date")
 
     def _get_sync_mode_from_catalog(self, stream: Stream) -> Optional[SyncMode]:
         if self.catalog:
             for catalog_stream in self.catalog.streams:
```

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/spec.yaml` & `airbyte_source_salesforce-2.5.0/source_salesforce/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/streams.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 import math
 import os
 import time
 import urllib.parse
 import uuid
 from abc import ABC
 from contextlib import closing
-from typing import Any, Callable, Dict, Iterable, List, Mapping, MutableMapping, Optional, Tuple, Type, Union
+from datetime import timedelta
+from typing import Any, Callable, Iterable, List, Mapping, MutableMapping, Optional, Tuple, Type, Union
 
 import backoff
 import pandas as pd
 import pendulum
 import requests  # type: ignore[import]
 from airbyte_cdk.models import ConfiguredAirbyteCatalog, FailureType, SyncMode
 from airbyte_cdk.sources.streams.availability_strategy import AvailabilityStrategy
+from airbyte_cdk.sources.streams.concurrent.cursor import Cursor
 from airbyte_cdk.sources.streams.concurrent.state_converters.datetime_stream_state_converter import IsoMillisConcurrentStreamStateConverter
 from airbyte_cdk.sources.streams.core import Stream, StreamData
 from airbyte_cdk.sources.streams.http import HttpStream, HttpSubStream
 from airbyte_cdk.sources.utils.transform import TransformConfig, TypeTransformer
 from airbyte_cdk.utils import AirbyteTracedException
 from numpy import nan
 from pendulum import DateTime  # type: ignore[attr-defined]
@@ -40,15 +42,15 @@
 
 DEFAULT_ENCODING = "utf-8"
 LOOKBACK_SECONDS = 600  # based on https://trailhead.salesforce.com/trailblazer-community/feed/0D54V00007T48TASAZ
 _JOB_TRANSIENT_ERRORS_MAX_RETRY = 1
 
 
 class SalesforceStream(HttpStream, ABC):
-    state_converter = IsoMillisConcurrentStreamStateConverter()
+    state_converter = IsoMillisConcurrentStreamStateConverter(is_sequential_state=False)
     page_size = 2000
     transformer = TypeTransformer(TransformConfig.DefaultSchemaNormalization)
     encoding = DEFAULT_ENCODING
 
     def __init__(
         self,
         sf_api: Salesforce,
@@ -138,15 +140,15 @@
         self.properties = properties
         self.first_time = True
         self.record_counter = 0
         self.next_page = None
 
 
 class RestSalesforceStream(SalesforceStream):
-    state_converter = IsoMillisConcurrentStreamStateConverter()
+    state_converter = IsoMillisConcurrentStreamStateConverter(is_sequential_state=False)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         assert self.primary_key or not self.too_many_properties
 
     def path(self, next_page_token: Mapping[str, Any] = None, **kwargs: Any) -> str:
         if next_page_token:
@@ -316,15 +318,15 @@
         )
         request_kwargs = self.request_kwargs(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
         response = self._send_request(request, request_kwargs)
         return request, response
 
 
 class BatchedSubStream(HttpSubStream):
-    state_converter = IsoMillisConcurrentStreamStateConverter()
+    state_converter = IsoMillisConcurrentStreamStateConverter(is_sequential_state=False)
     SLICE_BATCH_SIZE = 200
 
     def stream_slices(
         self, sync_mode: SyncMode, cursor_field: Optional[List[str]] = None, stream_state: Optional[Mapping[str, Any]] = None
     ) -> Iterable[Optional[Mapping[str, Any]]]:
         """Instead of yielding one parent record at a time, make stream slice contain a batch of parent records.
 
@@ -701,15 +703,18 @@
             authenticator=self.authenticator,
         )
         new_cls: Type[SalesforceStream] = RestSalesforceStream
         if isinstance(self, BulkIncrementalSalesforceStream):
             stream_kwargs.update({"replication_key": self.replication_key, "start_date": self.start_date})
             new_cls = IncrementalRestSalesforceStream
 
-        return new_cls(**stream_kwargs)
+        standard_instance = new_cls(**stream_kwargs)
+        if hasattr(standard_instance, "set_cursor"):
+            standard_instance.set_cursor(self._stream_slicer_cursor)
+        return standard_instance
 
 
 class BulkSalesforceSubStream(BatchedSubStream, BulkSalesforceStream):
     pass
 
 
 @BulkSalesforceStream.transformer.registerCustomTransform
@@ -728,32 +733,30 @@
     state_checkpoint_interval = 500
     _slice = None
 
     def __init__(self, replication_key: str, stream_slice_step: str = "P30D", **kwargs):
         super().__init__(**kwargs)
         self.replication_key = replication_key
         self._stream_slice_step = stream_slice_step
+        self._stream_slicer_cursor = None
+
+    def set_cursor(self, cursor: Cursor) -> None:
+        self._stream_slicer_cursor = cursor
 
     def stream_slices(
         self, *, sync_mode: SyncMode, cursor_field: List[str] = None, stream_state: Mapping[str, Any] = None
     ) -> Iterable[Optional[Mapping[str, Any]]]:
-        now = pendulum.now(tz="UTC")
-        assert LOOKBACK_SECONDS is not None and LOOKBACK_SECONDS >= 0
+        if not self._stream_slicer_cursor:
+            raise ValueError("Cursor should be set at this point")
 
-        initial_date = self.get_start_date_from_state(stream_state) - pendulum.Duration(seconds=LOOKBACK_SECONDS)
-        slice_start = initial_date
-        while slice_start < now:
-            slice_end = slice_start + self.stream_slice_step
-            self._slice = {
+        for slice_start, slice_end in self._stream_slicer_cursor.generate_slices():
+            yield {
                 "start_date": slice_start.isoformat(timespec="milliseconds"),
-                "end_date": min(slice_end, now).isoformat(timespec="milliseconds"),
+                "end_date": slice_end.isoformat(timespec="milliseconds"),
             }
-            yield self._slice
-
-            slice_start += self.stream_slice_step
 
     @property
     def stream_slice_step(self) -> pendulum.Duration:
         return pendulum.parse(self._stream_slice_step)
 
     def request_params(
         self,
@@ -825,15 +828,15 @@
 
         where_clause = f"WHERE {' AND '.join(where_conditions)}"
         query = f"SELECT {select_fields} FROM {table_name} {where_clause}"
         return {"q": query}
 
 
 class Describe(Stream):
-    state_converter = IsoMillisConcurrentStreamStateConverter()
+    state_converter = IsoMillisConcurrentStreamStateConverter(is_sequential_state=False)
     """
     Stream of sObjects' (Salesforce Objects) describe:
     https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/resources_sobject_describe.htm
     """
 
     name = "Describe"
     primary_key = "name"
```

### Comparing `airbyte_source_salesforce-2.4.4/source_salesforce/utils.py` & `airbyte_source_salesforce-2.5.0/source_salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.4/PKG-INFO` & `airbyte_source_salesforce-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesforce
-Version: 2.4.4
+Version: 2.5.0
 Summary: Source implementation for Salesforce.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

