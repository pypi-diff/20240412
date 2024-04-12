# Comparing `tmp/esd_services_api_client-2.2.0.tar.gz` & `tmp/esd_services_api_client-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-2.2.0.tar", max compression
+gzip compressed data, was "esd_services_api_client-2.2.1.tar", max compression
```

## Comparing `esd_services_api_client-2.2.0.tar` & `esd_services_api_client-2.2.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0    10693 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/LICENSE
--rw-r--r--   0        0        0      111 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/README.md
--rw-r--r--   0        0        0      603 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       22 2024-03-26 11:16:29.247338 esd_services_api_client-2.2.0/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      723 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0      754 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/beast/v3/__init__.py
--rw-r--r--   0        0        0    11478 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/beast/v3/_connector.py
--rw-r--r--   0        0        0     6766 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/beast/v3/_models.py
--rw-r--r--   0        0        0     3618 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      785 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     7445 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      981 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8677 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1702 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      603 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      792 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      837 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0    12875 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4030 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0     9393 2024-03-26 11:16:15.795326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/README.md
--rw-r--r--   0        0        0      627 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/__init__.py
--rw-r--r--   0        0        0      627 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/__init__.py
--rw-r--r--   0        0        0     3338 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/algrorithm_cache.py
--rw-r--r--   0        0        0     1761 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/input_object.py
--rw-r--r--   0        0        0     2019 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/logger_factory.py
--rw-r--r--   0        0        0     2938 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/nexus_object.py
--rw-r--r--   0        0        0     1729 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/socket_provider.py
--rw-r--r--   0        0        0      903 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/__init__.py
--rw-r--r--   0        0        0     2739 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py
--rw-r--r--   0        0        0     3900 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/_remote_algorithm.py
--rw-r--r--   0        0        0     1702 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/distributed.py
--rw-r--r--   0        0        0     4310 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/forked_algorithm.py
--rw-r--r--   0        0        0     1607 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/minimalistic.py
--rw-r--r--   0        0        0     2007 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/recursive.py
--rw-r--r--   0        0        0        0 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/configurations/__init__.py
--rw-r--r--   0        0        0     1091 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/configurations/algorithm_configuration.py
--rw-r--r--   0        0        0      627 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/core/__init__.py
--rw-r--r--   0        0        0     9654 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/core/app_core.py
--rw-r--r--   0        0        0     6521 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/core/app_dependencies.py
--rw-r--r--   0        0        0      696 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/__init__.py
--rw-r--r--   0        0        0      895 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/_nexus_error.py
--rw-r--r--   0        0        0     1622 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/cache_errors.py
--rw-r--r--   0        0        0     1765 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/input_reader_error.py
--rw-r--r--   0        0        0     1991 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/startup_error.py
--rw-r--r--   0        0        0      758 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/__init__.py
--rw-r--r--   0        0        0     3132 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/input_processor.py
--rw-r--r--   0        0        0     3505 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/input_reader.py
--rw-r--r--   0        0        0     2516 2024-03-26 11:16:15.799326 esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/payload_reader.py
--rw-r--r--   0        0        0     1237 2024-03-26 11:16:29.247338 esd_services_api_client-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 esd_services_api_client-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10693 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/LICENSE
+-rw-r--r--   0        0        0      111 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/README.md
+-rw-r--r--   0        0        0      603 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-12 11:44:04.246022 esd_services_api_client-2.2.1/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      723 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0      754 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/__init__.py
+-rw-r--r--   0        0        0    11478 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_connector.py
+-rw-r--r--   0        0        0     6766 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_models.py
+-rw-r--r--   0        0        0     3618 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      785 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     7445 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      981 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8677 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1702 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      603 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      837 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0    12875 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4030 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0     9393 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/README.md
+-rw-r--r--   0        0        0      627 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/__init__.py
+-rw-r--r--   0        0        0     3338 2024-04-12 11:43:52.854042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/algrorithm_cache.py
+-rw-r--r--   0        0        0     1761 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/input_object.py
+-rw-r--r--   0        0        0     2019 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/logger_factory.py
+-rw-r--r--   0        0        0     3039 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/nexus_object.py
+-rw-r--r--   0        0        0     1729 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/socket_provider.py
+-rw-r--r--   0        0        0      903 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/__init__.py
+-rw-r--r--   0        0        0     2925 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py
+-rw-r--r--   0        0        0     3900 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_remote_algorithm.py
+-rw-r--r--   0        0        0     1702 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/distributed.py
+-rw-r--r--   0        0        0     4310 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/forked_algorithm.py
+-rw-r--r--   0        0        0     1644 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/minimalistic.py
+-rw-r--r--   0        0        0     2007 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/recursive.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/configurations/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/configurations/algorithm_configuration.py
+-rw-r--r--   0        0        0      627 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/__init__.py
+-rw-r--r--   0        0        0    10037 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_core.py
+-rw-r--r--   0        0        0     6674 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_dependencies.py
+-rw-r--r--   0        0        0      696 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/_nexus_error.py
+-rw-r--r--   0        0        0     1622 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/cache_errors.py
+-rw-r--r--   0        0        0     1765 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/input_reader_error.py
+-rw-r--r--   0        0        0     1991 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/startup_error.py
+-rw-r--r--   0        0        0      758 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/__init__.py
+-rw-r--r--   0        0        0     3132 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_processor.py
+-rw-r--r--   0        0        0     3505 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_reader.py
+-rw-r--r--   0        0        0     2516 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/payload_reader.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/telemetry/__init__.py
+-rw-r--r--   0        0        0     3220 2024-04-12 11:43:52.858042 esd_services_api_client-2.2.1/esd_services_api_client/nexus/telemetry/recorder.py
+-rw-r--r--   0        0        0     1237 2024-04-12 11:44:04.246022 esd_services_api_client-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 esd_services_api_client-2.2.1/PKG-INFO
```

### Comparing `esd_services_api_client-2.2.0/LICENSE` & `esd_services_api_client-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/beast/v3/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/beast/v3/_connector.py` & `esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/beast/v3/_models.py` & `esd_services_api_client-2.2.1/esd_services_api_client/beast/v3/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/boxer/README.md` & `esd_services_api_client-2.2.1/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/boxer/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-2.2.1/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/common/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/crystal/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/crystal/_api_versions.py` & `esd_services_api_client-2.2.1/esd_services_api_client/crystal/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-2.2.1/esd_services_api_client/crystal/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-2.2.1/esd_services_api_client/crystal/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/README.md` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/algrorithm_cache.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/algrorithm_cache.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/input_object.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/input_object.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/logger_factory.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/logger_factory.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/nexus_object.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/nexus_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 TPayload = TypeVar("TPayload")  # pylint: disable=C0103
 TResult = TypeVar(  # pylint: disable=C0103
     "TResult", pandas.DataFrame, polars.DataFrame
 )
 
 
-class NexusObject(Generic[TPayload, TResult], ABC):
+class NexusCoreObject(ABC):
     """
     Base class for all Nexus objects.
     """
 
     def __init__(
         self,
         metrics_provider: MetricsProvider,
@@ -83,14 +83,20 @@
 
     @abstractmethod
     async def _context_close(self):
         """
         Optional actions to perform on context closure.
         """
 
+
+class NexusObject(Generic[TPayload, TResult], NexusCoreObject, ABC):
+    """
+    Base class for all Nexus objects.
+    """
+
     @classmethod
     def alias(cls) -> str:
         """
         Alias to identify this reader's output
         """
         return snakecase(
             re.sub(
```

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/abstractions/socket_provider.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/abstractions/socket_provider.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
  Base algorithm
 """
-
 #  Copyright (c) 2023-2024. ECCO Sneaks & Data
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +12,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-
 from abc import abstractmethod
 from functools import partial
 
 from adapta.metrics import MetricsProvider
 from adapta.utils.decorators import run_time_metrics_async
 
 from esd_services_api_client.nexus.abstractions.algrorithm_cache import InputCache
@@ -47,14 +45,22 @@
         logger_factory: LoggerFactory,
         *input_processors: InputProcessor,
         cache: InputCache,
     ):
         super().__init__(metrics_provider, logger_factory)
         self._input_processors = input_processors
         self._cache = cache
+        self._inputs: dict = {}
+
+    @property
+    def inputs(self) -> dict:
+        """
+        Inputs generated for this algorithm run.
+        """
+        return self._inputs
 
     @abstractmethod
     async def _run(self, **kwargs) -> AlgorithmResult:
         """
         Core logic for this algorithm. Implementing this method is mandatory.
         """
 
@@ -73,16 +79,16 @@
             template_args={
                 "algorithm": self.__class__.alias().upper(),
             },
         )
         async def _measured_run(**run_args):
             return await self._run(**run_args)
 
-        results = await self._cache.resolve(*self._input_processors, **kwargs)
+        self._inputs = await self._cache.resolve(*self._input_processors, **kwargs)
 
         return await partial(
             _measured_run,
-            **results,
+            **self._inputs,
             metric_tags=self._metric_tags,
             metrics_provider=self._metrics_provider,
             logger=self._logger,
         )()
```

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/_remote_algorithm.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/_remote_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/distributed.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/distributed.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/forked_algorithm.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/forked_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/minimalistic.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/minimalistic.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,9 +41,12 @@
         self,
         metrics_provider: MetricsProvider,
         logger_factory: LoggerFactory,
         *input_processors: InputProcessor,
         cache: InputCache,
     ):
         super().__init__(
-            metrics_provider, logger_factory, *input_processors, cache=cache
+            metrics_provider,
+            logger_factory,
+            *input_processors,
+            cache=cache,
         )
```

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/algorithms/recursive.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/algorithms/recursive.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/configurations/algorithm_configuration.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/configurations/algorithm_configuration.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/core/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/core/app_core.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 )
 from esd_services_api_client.nexus.input.input_processor import InputProcessor
 from esd_services_api_client.nexus.input.input_reader import InputReader
 from esd_services_api_client.nexus.input.payload_reader import (
     AlgorithmPayloadReader,
     AlgorithmPayload,
 )
+from esd_services_api_client.nexus.telemetry.recorder import TelemetryRecorder
 
 
 def is_transient_exception(exception: Optional[BaseException]) -> Optional[bool]:
     """
     Check if the exception is retryable.
     """
     if not exception:
@@ -240,17 +241,19 @@
             case _:
                 sys.exit(1)
 
     async def activate(self):
         """
         Activates the run sequence.
         """
+
         self._injector = Injector(self._configurator.injection_binds)
 
         algorithm: BaselineAlgorithm = self._injector.get(self._algorithm_class)
+        telemetry_recorder: TelemetryRecorder = self._injector.get(TelemetryRecorder)
 
         async with algorithm as instance:
             self._algorithm_run_task = asyncio.create_task(
                 instance.run(**self._run_args.__dict__)
             )
             await self._algorithm_run_task
             ex = self._algorithm_run_task.exception()
@@ -262,14 +265,20 @@
             await self._submit_result(
                 self._algorithm_run_task.result() if not ex else None,
                 self._algorithm_run_task.exception(),
             )
             if len(on_complete_tasks) > 0:
                 await asyncio.wait(on_complete_tasks)
 
+            # record telemetry
+            async with telemetry_recorder as recorder:
+                await recorder.record(
+                    run_id=self._run_args.request_id, **algorithm.inputs
+                )
+
             # dispose of QES instance gracefully as it might hold open connections
             qes = self._injector.get(QueryEnabledStore)
             qes.close()
 
     @classmethod
     def create(cls) -> "Nexus":
         """
```

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/core/app_dependencies.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/core/app_dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     FatalStartupConfigurationError,
 )
 from esd_services_api_client.nexus.input.input_processor import InputProcessor
 from esd_services_api_client.nexus.input.input_reader import InputReader
 from esd_services_api_client.nexus.input.payload_reader import (
     AlgorithmPayload,
 )
+from esd_services_api_client.nexus.telemetry.recorder import TelemetryRecorder
 
 
 @final
 class MetricsModule(Module):
     """
     Metrics provider module.
     """
@@ -191,14 +192,15 @@
         self._injection_binds = [
             MetricsModule(),
             CrystalReceiverClientModule(),
             QueryEnabledStoreModule(),
             StorageClientModule(),
             ExternalSocketsModule(),
             CacheModule(),
+            type(f"{TelemetryRecorder.__name__}Module", (Module,), {})(),
         ]
 
     @property
     def injection_binds(self) -> list:
         """
         Currently configured injection bindings
         """
```

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/_nexus_error.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/_nexus_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/cache_errors.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/cache_errors.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/input_reader_error.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/input_reader_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/exceptions/startup_error.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/exceptions/startup_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/__init__.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/input_processor.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_processor.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/input_reader.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/input_reader.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/esd_services_api_client/nexus/input/payload_reader.py` & `esd_services_api_client-2.2.1/esd_services_api_client/nexus/input/payload_reader.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.0/pyproject.toml` & `esd_services_api_client-2.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "2.2.0"
+version = "2.2.1"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
```

### Comparing `esd_services_api_client-2.2.0/PKG-INFO` & `esd_services_api_client-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

