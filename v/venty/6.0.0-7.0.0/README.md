# Comparing `tmp/venty-6.0.0.tar.gz` & `tmp/venty-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venty-6.0.0.tar", last modified: Fri Apr  5 14:09:02 2024, max compression
+gzip compressed data, was "venty-7.0.0.tar", last modified: Fri Apr 12 13:48:48 2024, max compression
```

## Comparing `venty-6.0.0.tar` & `venty-7.0.0.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:09:02.390830 venty-6.0.0/
--rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-6.0.0/LICENSE
--rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-6.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2120 2024-04-05 14:09:02.376830 venty-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2024-03-16 17:46:39.000000 venty-6.0.0/README.md
--rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-6.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 14:09:02.390830 venty-6.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2021 2024-04-05 09:15:17.000000 venty-6.0.0/setup.py
--rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-6.0.0/test_requirements.txt
--rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-6.0.0/tox.ini
-drwxrwxrwx   0        0        0        0 2024-04-05 14:09:02.339830 venty-6.0.0/venty/
--rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-6.0.0/venty/__init__.py
--rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-6.0.0/venty/_dummy.py
--rw-rw-rw-   0        0        0     1693 2024-03-26 00:45:31.000000 venty-6.0.0/venty/aggregate_root.py
--rw-rw-rw-   0        0        0     1304 2024-04-05 08:47:53.000000 venty-6.0.0/venty/aggregate_store.py
--rw-rw-rw-   0        0        0     2123 2024-03-27 06:14:06.000000 venty-6.0.0/venty/aggregate_store_test.py
--rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-6.0.0/venty/event_channel.py
--rw-rw-rw-   0        0        0      521 2024-03-16 16:58:05.000000 venty-6.0.0/venty/event_channel_test.py
--rw-rw-rw-   0        0        0     5036 2024-03-27 06:20:52.000000 venty-6.0.0/venty/event_logger.py
--rw-rw-rw-   0        0        0     2986 2024-04-05 04:27:52.000000 venty-6.0.0/venty/event_producer.py
--rw-rw-rw-   0        0        0     1544 2024-04-05 05:09:43.000000 venty-6.0.0/venty/event_producer_stack.py
--rw-rw-rw-   0        0        0     1435 2024-03-27 06:37:35.000000 venty-6.0.0/venty/event_producer_stack_test.py
--rw-rw-rw-   0        0        0     1419 2024-04-05 04:27:59.000000 venty-6.0.0/venty/event_producer_test.py
--rw-rw-rw-   0        0        0     6996 2024-03-16 15:40:44.000000 venty-6.0.0/venty/event_store.py
--rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-6.0.0/venty/http_event_channel.py
--rw-rw-rw-   0        0        0     1850 2024-03-16 17:18:33.000000 venty-6.0.0/venty/http_event_channel_test.py
--rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-6.0.0/venty/in_memory_event_channel.py
--rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-6.0.0/venty/in_memory_event_channel_test.py
--rw-rw-rw-   0        0        0     4492 2024-03-16 17:02:22.000000 venty-6.0.0/venty/in_memory_event_store.py
--rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-6.0.0/venty/in_memory_event_store_test.py
--rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-6.0.0/venty/py.typed
--rw-rw-rw-   0        0        0      294 2024-04-05 09:27:44.000000 venty-6.0.0/venty/settings.py
--rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-6.0.0/venty/settings_test.py
--rw-rw-rw-   0        0        0     8270 2024-04-05 09:44:12.000000 venty-6.0.0/venty/sql_event_store.py
--rw-rw-rw-   0        0        0     6821 2024-03-16 22:24:29.000000 venty-6.0.0/venty/sql_event_store_test.py
--rw-rw-rw-   0        0        0      287 2024-03-16 17:21:51.000000 venty-6.0.0/venty/strong_types.py
--rw-rw-rw-   0        0        0     1003 2024-03-15 19:20:28.000000 venty-6.0.0/venty/strong_types_test.py
--rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-6.0.0/venty/timing.py
--rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-6.0.0/venty/timing_test.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:09:02.375831 venty-6.0.0/venty.egg-info/
--rw-rw-rw-   0        0        0     2120 2024-04-05 14:09:01.000000 venty-6.0.0/venty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2024-04-05 14:09:01.000000 venty-6.0.0/venty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:09:01.000000 venty-6.0.0/venty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-05 14:09:01.000000 venty-6.0.0/venty.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-05 14:09:01.000000 venty-6.0.0/venty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 13:48:48.164651 venty-7.0.0/
+-rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-7.0.0/LICENSE
+-rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-7.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2189 2024-04-12 13:48:48.164651 venty-7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2024-04-08 17:56:19.000000 venty-7.0.0/README.md
+-rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-7.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:48:48.164651 venty-7.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2024-04-12 13:09:25.000000 venty-7.0.0/setup.py
+-rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-7.0.0/test_requirements.txt
+-rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-7.0.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-12 13:48:48.149651 venty-7.0.0/venty/
+-rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-7.0.0/venty/__init__.py
+-rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-7.0.0/venty/_dummy.py
+-rw-rw-rw-   0        0        0     1858 2024-04-08 17:52:38.000000 venty-7.0.0/venty/aggregate_root.py
+-rw-rw-rw-   0        0        0     1304 2024-04-05 08:47:53.000000 venty-7.0.0/venty/aggregate_store.py
+-rw-rw-rw-   0        0        0     2123 2024-03-27 06:14:06.000000 venty-7.0.0/venty/aggregate_store_test.py
+-rw-rw-rw-   0        0        0      999 2024-04-12 13:16:52.000000 venty-7.0.0/venty/auth_event_producer.py
+-rw-rw-rw-   0        0        0      756 2024-04-12 13:43:22.000000 venty-7.0.0/venty/classification.py
+-rw-rw-rw-   0        0        0     1277 2024-04-12 13:34:09.000000 venty-7.0.0/venty/classification_test.py
+-rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-7.0.0/venty/event_channel.py
+-rw-rw-rw-   0        0        0      521 2024-03-16 16:58:05.000000 venty-7.0.0/venty/event_channel_test.py
+-rw-rw-rw-   0        0        0     5036 2024-03-27 06:20:52.000000 venty-7.0.0/venty/event_logger.py
+-rw-rw-rw-   0        0        0     3521 2024-04-12 13:16:52.000000 venty-7.0.0/venty/event_producer.py
+-rw-rw-rw-   0        0        0     1773 2024-04-12 13:36:23.000000 venty-7.0.0/venty/event_producer_stack.py
+-rw-rw-rw-   0        0        0     1584 2024-04-12 13:07:59.000000 venty-7.0.0/venty/event_producer_stack_test.py
+-rw-rw-rw-   0        0        0     1537 2024-04-12 13:08:41.000000 venty-7.0.0/venty/event_producer_test.py
+-rw-rw-rw-   0        0        0     6996 2024-03-16 15:40:44.000000 venty-7.0.0/venty/event_store.py
+-rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-7.0.0/venty/http_event_channel.py
+-rw-rw-rw-   0        0        0     1850 2024-03-16 17:18:33.000000 venty-7.0.0/venty/http_event_channel_test.py
+-rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-7.0.0/venty/in_memory_event_channel.py
+-rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-7.0.0/venty/in_memory_event_channel_test.py
+-rw-rw-rw-   0        0        0     4492 2024-03-16 17:02:22.000000 venty-7.0.0/venty/in_memory_event_store.py
+-rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-7.0.0/venty/in_memory_event_store_test.py
+-rw-rw-rw-   0        0        0      781 2024-04-08 17:48:30.000000 venty-7.0.0/venty/object_storage.py
+-rw-rw-rw-   0        0        0      301 2024-04-08 18:03:19.000000 venty-7.0.0/venty/optional.py
+-rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-7.0.0/venty/py.typed
+-rw-rw-rw-   0        0        0      294 2024-04-05 09:27:44.000000 venty-7.0.0/venty/settings.py
+-rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-7.0.0/venty/settings_test.py
+-rw-rw-rw-   0        0        0     8270 2024-04-12 13:45:12.000000 venty-7.0.0/venty/sql_event_store.py
+-rw-rw-rw-   0        0        0     6821 2024-03-16 22:24:29.000000 venty-7.0.0/venty/sql_event_store_test.py
+-rw-rw-rw-   0        0        0      399 2024-04-12 13:16:52.000000 venty-7.0.0/venty/strong_types.py
+-rw-rw-rw-   0        0        0     1003 2024-03-15 19:20:28.000000 venty-7.0.0/venty/strong_types_test.py
+-rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-7.0.0/venty/timing.py
+-rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-7.0.0/venty/timing_test.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:48:48.163649 venty-7.0.0/venty.egg-info/
+-rw-rw-rw-   0        0        0     2189 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/top_level.txt
```

### Comparing `venty-6.0.0/LICENSE` & `venty-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/PKG-INFO` & `venty-7.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 6.0.0
+Version: 7.0.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
-Author: Alexander Tkachev
+Author: Sasha Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,16 @@
  * [Simple Event Store Interface](venty/event_store.py)
    * [In Memory Event Store Implementation](venty/in_memory_event_store.py)
    * [Simple SQL Event Store Implementation](venty/sql_event_store.py) 
    * DynamoDB Event Store Implementation (Planned)
  * [Aggregate Store Implementation](venty/aggregate_store.py)
     * Based on the event store interface.
  * [Strong Types](venty/strong_types.py) for event driven development.
- * Log Formatter as CloudEvents (Planned)
+ * [Log Formatter as CloudEvents](venty/event_logger.py)
  * Correlation-ID and Causation-ID augmentation (Planned) 
  * Claim Check (Planned)
+ * [Object Storage abstraction](venty/object_storage.py)
  
  
  ## Configuration
  You can configure the venty package via [the package settings](venty/settings.md)
```

### Comparing `venty-6.0.0/README.md` & `venty-7.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
  * [Simple Event Store Interface](venty/event_store.py)
    * [In Memory Event Store Implementation](venty/in_memory_event_store.py)
    * [Simple SQL Event Store Implementation](venty/sql_event_store.py) 
    * DynamoDB Event Store Implementation (Planned)
  * [Aggregate Store Implementation](venty/aggregate_store.py)
     * Based on the event store interface.
  * [Strong Types](venty/strong_types.py) for event driven development.
- * Log Formatter as CloudEvents (Planned)
+ * [Log Formatter as CloudEvents](venty/event_logger.py)
  * Correlation-ID and Causation-ID augmentation (Planned) 
  * Claim Check (Planned)
+ * [Object Storage abstraction](venty/object_storage.py)
  
  
  ## Configuration
  You can configure the venty package via [the package settings](venty/settings.md)
```

### Comparing `venty-6.0.0/setup.py` & `venty-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 here = Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setuptools.setup(
         name="venty",
-        version="6.0.0",
-        author="Alexander Tkachev",
+        version="7.0.0",
+        author="Sasha Tkachev",
         author_email="sasha64sasha@gmail.com",
         description="Venty",
         long_description_content_type="text/markdown",
         long_description=long_description,
         home_page="https://github.com/sasha-tkachev/venty",
         url="https://github.com/sasha-tkachev/venty",
         keywords=[
```

### Comparing `venty-6.0.0/tox.ini` & `venty-7.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/aggregate_root.py` & `venty-7.0.0/venty/aggregate_root.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from dataclasses import field
 from typing import List, NewType, Iterable, TypeVar
 from uuid import UUID
 
 from cloudevents.abstract import CloudEvent
 from pydantic import BaseModel, PrivateAttr
 
 from venty.strong_types import StreamVersion, NO_EVENT_VERSION
@@ -47,7 +46,13 @@
     def load_from_history(self, events: Iterable[CloudEvent]) -> None:
         for event in events:
             self.when(event)
             self._aggregate_version = StreamVersion(self.aggregate_version() + 1)
 
 
 AggregateRootT = TypeVar("AggregateRootT", bound=AggregateRoot)
+
+
+def subject_aggregate(event: CloudEvent) -> AggregateUUID:
+    if subject := event.get("subject"):
+        return AggregateUUID(UUID(subject))
+    raise ValueError("venty.MissingSubject")
```

### Comparing `venty-6.0.0/venty/aggregate_store.py` & `venty-7.0.0/venty/aggregate_store.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/aggregate_store_test.py` & `venty-7.0.0/venty/aggregate_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/event_channel.py` & `venty-7.0.0/venty/event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/event_channel_test.py` & `venty-7.0.0/venty/event_channel_test.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/event_logger.py` & `venty-7.0.0/venty/event_logger.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/event_producer.py` & `venty-7.0.0/venty/event_producer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import sys
 from datetime import datetime, timezone
-from typing import Any, Dict, Optional, Callable, TypeVar
-from uuid import uuid4, UUID, uuid5
+from typing import Any, Callable, Dict, Optional, TypeVar, Type, Union
+from uuid import UUID, uuid4, uuid5
 
-from cloudevents.pydantic import CloudEvent
 from cloudevents.sdk.event.attribute import (
     default_id_selection_algorithm,
     default_time_selection_algorithm,
 )
 
-from venty.strong_types import EventSource
+from venty.strong_types import EventSource, CloudEventT
 
 
 def _ignore_invalid_attributes(attributes: Dict[str, Any]) -> Dict[str, Any]:
     return {
         k: v for k, v in attributes.items() if k not in {"data", "id", "source", "time"}
     }
 
 
 IdSelection = Callable[[], str]
 TimeSelection = Callable[[], datetime]
 
+AttributeValue = Union[str, int, UUID, bool]
+
 
 class EventProducer:
     def produce_event(
-        self, attributes: Dict[str, Any], data: Optional[Any]
-    ) -> CloudEvent:
+        self,
+        type_: Type[CloudEventT],
+        data: Optional[Any],
+        *,
+        attributes: Optional[Dict[str, AttributeValue]] = None,
+    ) -> CloudEventT:
         raise NotImplementedError()
 
 
 EventProducerT = TypeVar("EventProducerT", bound=EventProducer)
 
 
 def deterministic_id_factory(seed: int = 0) -> Callable[[], str]:
@@ -46,14 +51,23 @@
 
     def _next() -> datetime:
         return datetime.fromtimestamp(next(i), tz=timezone.utc)
 
     return _next
 
 
+def _normalize_attributes(
+    attributes: Dict[str, AttributeValue]
+) -> Dict[str, Union[str, int, bool]]:
+    return {
+        k: v if isinstance(v, (str, int, bool)) else str(v)
+        for k, v in attributes.items()
+    }
+
+
 class SimpleEventProducer(EventProducer):
     def __init__(
         self,
         *,
         source: Optional[EventSource] = None,
         default_attributes: Optional[Dict[str, Any]] = None,
         id_selection_algorithm: IdSelection = default_id_selection_algorithm,
@@ -65,22 +79,28 @@
         if default_attributes is None:
             default_attributes = {}
         self._default_attributes = _ignore_invalid_attributes(default_attributes)
         self._id_selection_algorithm = id_selection_algorithm
         self._time_selection_algorithm = time_selection_algorithm
 
     def produce_event(
-        self, attributes: Dict[str, Any], data: Optional[Any]
-    ) -> CloudEvent:
+        self,
+        type_: Type[CloudEventT],
+        data: Optional[Any],
+        *,
+        attributes: Optional[Dict[str, AttributeValue]] = None,
+    ) -> CloudEventT:
+        if attributes is None:
+            attributes = {}
         actual_attributes = self._default_attributes.copy()
         actual_attributes.update(attributes)
         actual_attributes["source"] = self._source
         actual_attributes["id"] = self._id_selection_algorithm()
         actual_attributes["time"] = self._time_selection_algorithm()
-        return CloudEvent.create(actual_attributes, data)
+        return type_.create(_normalize_attributes(actual_attributes), data)
 
 
 def testing_event_producer(
     *,
     source: Optional[EventSource] = EventSource("fake-source"),
     default_attributes: Optional[Dict[str, Any]] = None,
     seed: int = 0,
```

### Comparing `venty-6.0.0/venty/event_producer_stack_test.py` & `venty-7.0.0/venty/event_producer_stack_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,46 @@
+from typing import Literal
+
 import pytest
+from cloudevents.pydantic import CloudEvent
 
 from venty.event_producer import SimpleEventProducer
 from venty.event_producer_stack import EventProducerStack
 from venty.strong_types import EventSource
 
 
+class MyType(CloudEvent):
+    type: Literal["my-type"] = "my-type"
+
+
+class YourType(CloudEvent):
+    type: Literal["your-type"] = "your-type"
+
+
 def test_event_producer_stack():
     my_producer = SimpleEventProducer(source=EventSource("my-source"))
     your_producer = SimpleEventProducer(source=EventSource("your-source"))
     stack = EventProducerStack(my_producer)
 
-    a = stack.produce_event({"type": "my-type"}, None)
+    a = stack.produce_event(MyType, None)
     assert a.source == "my-source"
     with stack.scoped_event_producer(your_producer):
-        b = stack.produce_event({"type": "your-type"}, None)
+        b = stack.produce_event(YourType, None)
         assert b.source == "your-source"
-    c = stack.produce_event({"type": "my-type"}, None)
+    c = stack.produce_event(MyType, None)
     assert c.source == "my-source"
 
 
 def test_event_producer_stack_should_pop_on_exception():
     my_producer = SimpleEventProducer(source=EventSource("my-source"))
     your_producer = SimpleEventProducer(source=EventSource("your-source"))
     stack = EventProducerStack(my_producer)
 
-    a = stack.produce_event({"type": "my-type"}, None)
+    a = stack.produce_event(MyType, None)
     assert a.source == "my-source"
     with pytest.raises(ValueError):
         with stack.scoped_event_producer(your_producer):
-            b = stack.produce_event({"type": "your-type"}, None)
+            b = stack.produce_event(YourType, None)
             assert b.source == "your-source"
             raise ValueError("boom")
-    c = stack.produce_event({"type": "my-type"}, None)
+    c = stack.produce_event(MyType, None)
     assert c.source == "my-source"
```

### Comparing `venty-6.0.0/venty/event_producer_test.py` & `venty-7.0.0/venty/http_event_channel_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,60 @@
-from datetime import datetime
+from cloudevents.pydantic import CloudEvent
+from mock import Mock
 
-from cloudevents.conversion import to_dict
+from venty.event_channel import publish_event
+from venty.http_event_channel import HttpEventChannel, HttpChannelMode
 
 
-from venty.event_producer import SimpleEventProducer, testing_event_producer
-from venty.strong_types import EventSource
-
-
-def test_event_producer_sanity():
-    producer = SimpleEventProducer(
-        source=EventSource("my-source"),
-        id_selection_algorithm=lambda: "1",
-        time_selection_algorithm=lambda: datetime(year=2024, month=1, day=1),
-        default_attributes={"subject": "hello"},
-    )
-    result = producer.produce_event({"type": "my-type"}, None)
-    assert to_dict(result) == {
-        "data": None,
-        "datacontenttype": None,
-        "dataschema": None,
-        "id": "1",
-        "source": "my-source",
-        "specversion": "1.0",
-        "subject": "hello",
-        "time": "2024-01-01T00:00:00",
-        "type": "my-type",
-    }
+def test_http_channel_with_binary_mode_must_put_all_ce_attributes_in_header():
+    session = Mock()
+    channel = HttpEventChannel(
+        "https://localhost:1337", session, HttpChannelMode.BINARY
+    )
+    publish_event(
+        CloudEvent(
+            {
+                "type": "my-type",
+                "source": "my-source",
+                "id": "my-id",
+                "time": "2024-01-01",
+            },
+            {"hello": "world"},
+        ),
+        channel,
+    )
+    session.post.assert_called_once_with(
+        "https://localhost:1337",
+        b'{"hello": "world"}',
+        headers={
+            "ce-specversion": "1.0",
+            "ce-id": "my-id",
+            "ce-source": "my-source",
+            "ce-type": "my-type",
+            "ce-time": "2024-01-01T00:00:00",
+        },
+    )
 
 
-def test_fake_event_producer():
-    producer = testing_event_producer(
-        default_attributes={"subject": "hello"},
-    )
-    result = producer.produce_event({"type": "my-type"}, None)
-    assert to_dict(result) == {
-        "data": None,
-        "datacontenttype": None,
-        "dataschema": None,
-        "id": "b6c54489-38a0-5f50-a60a-fd8d76219cae",
-        "source": "fake-source",
-        "specversion": "1.0",
-        "subject": "hello",
-        "time": "1970-01-01T00:00:00+00:00",
-        "type": "my-type",
-    }
+def test_http_channel_with_structured_mode_must_put_event_as_json_in_body():
+    session = Mock()
+    channel = HttpEventChannel(
+        "https://localhost:1337", session, HttpChannelMode.STRUCTURED
+    )
+    publish_event(
+        CloudEvent(
+            {
+                "type": "my-type",
+                "source": "my-source",
+                "id": "my-id",
+                "time": "2024-01-01",
+            },
+            {"hello": "world"},
+        ),
+        channel,
+    )
+    session.post.assert_called_once_with(
+        "https://localhost:1337",
+        b'{"specversion": "1.0", "id": "my-id", "source": "my-source", "type": '
+        b'"my-type", "time": "2024-01-01T00:00:00", "data": {"hello": "world"}}',
+        headers={"content-type": "application/cloudevents+json"},
+    )
```

### Comparing `venty-6.0.0/venty/event_store.py` & `venty-7.0.0/venty/event_store.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/http_event_channel.py` & `venty-7.0.0/venty/http_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/in_memory_event_channel.py` & `venty-7.0.0/venty/in_memory_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/in_memory_event_store.py` & `venty-7.0.0/venty/in_memory_event_store.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/in_memory_event_store_test.py` & `venty-7.0.0/venty/in_memory_event_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/settings_test.py` & `venty-7.0.0/venty/settings_test.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/sql_event_store.py` & `venty-7.0.0/venty/sql_event_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         )
         for i, event in enumerate(events)
     ]
 
 
 def _row_to_recorded_event(
     event_row: RecordedEventRow,
-    stream_name_map: dict[bytes, StreamName],
+    stream_name_map: Dict[bytes, StreamName],
     event_type: Type[AnyCloudEvent],
 ) -> RecordedEvent:
     return RecordedEvent(
         commit_position=CommitPosition(
             event_row.id,
         ),
         stream_position=StreamVersion(
```

### Comparing `venty-6.0.0/venty/sql_event_store_test.py` & `venty-7.0.0/venty/sql_event_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/strong_types_test.py` & `venty-7.0.0/venty/strong_types_test.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/timing.py` & `venty-7.0.0/venty/timing.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty/timing_test.py` & `venty-7.0.0/venty/timing_test.py`

 * *Files identical despite different names*

### Comparing `venty-6.0.0/venty.egg-info/PKG-INFO` & `venty-7.0.0/venty.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 6.0.0
+Version: 7.0.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
-Author: Alexander Tkachev
+Author: Sasha Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
@@ -40,15 +40,16 @@
  * [Simple Event Store Interface](venty/event_store.py)
    * [In Memory Event Store Implementation](venty/in_memory_event_store.py)
    * [Simple SQL Event Store Implementation](venty/sql_event_store.py) 
    * DynamoDB Event Store Implementation (Planned)
  * [Aggregate Store Implementation](venty/aggregate_store.py)
     * Based on the event store interface.
  * [Strong Types](venty/strong_types.py) for event driven development.
- * Log Formatter as CloudEvents (Planned)
+ * [Log Formatter as CloudEvents](venty/event_logger.py)
  * Correlation-ID and Causation-ID augmentation (Planned) 
  * Claim Check (Planned)
+ * [Object Storage abstraction](venty/object_storage.py)
  
  
  ## Configuration
  You can configure the venty package via [the package settings](venty/settings.md)
```

### Comparing `venty-6.0.0/venty.egg-info/SOURCES.txt` & `venty-7.0.0/venty.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,33 @@
 test_requirements.txt
 tox.ini
 venty/__init__.py
 venty/_dummy.py
 venty/aggregate_root.py
 venty/aggregate_store.py
 venty/aggregate_store_test.py
+venty/auth_event_producer.py
+venty/classification.py
+venty/classification_test.py
 venty/event_channel.py
 venty/event_channel_test.py
 venty/event_logger.py
 venty/event_producer.py
 venty/event_producer_stack.py
 venty/event_producer_stack_test.py
 venty/event_producer_test.py
 venty/event_store.py
 venty/http_event_channel.py
 venty/http_event_channel_test.py
 venty/in_memory_event_channel.py
 venty/in_memory_event_channel_test.py
 venty/in_memory_event_store.py
 venty/in_memory_event_store_test.py
+venty/object_storage.py
+venty/optional.py
 venty/py.typed
 venty/settings.py
 venty/settings_test.py
 venty/sql_event_store.py
 venty/sql_event_store_test.py
 venty/strong_types.py
 venty/strong_types_test.py
```

