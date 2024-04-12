# Comparing `tmp/mms_client-1.0.6.tar.gz` & `tmp/mms_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.0.6.tar", max compression
+gzip compressed data, was "mms_client-1.1.0.tar", max compression
```

## Comparing `mms_client-1.0.6.tar` & `mms_client-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1211 2024-03-25 02:58:07.283830 mms_client-1.0.6/LICENSE
--rw-r--r--   0        0        0    13096 2024-03-25 02:58:07.283830 mms_client-1.0.6/README.md
--rw-r--r--   0        0        0     2300 2024-03-25 02:58:07.287830 mms_client-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/__init__.py
--rw-r--r--   0        0        0      571 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    25363 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/services/base.py
--rw-r--r--   0        0        0     4892 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/services/market.py
--rw-r--r--   0        0        0      521 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/services/omi.py
--rw-r--r--   0        0        0      571 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      537 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0     9681 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/types/base.py
--rw-r--r--   0        0        0      329 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/types/enums.py
--rw-r--r--   0        0        0     6250 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2588 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/types/market.py
--rw-r--r--   0        0        0     6300 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     4419 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     2306 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    25206 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0     9653 2024-03-25 02:58:07.287830 mms_client-1.0.6/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    13840 1970-01-01 00:00:00.000000 mms_client-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-12 02:05:07.565098 mms_client-1.1.0/LICENSE
+-rw-r--r--   0        0        0    13458 2024-04-12 02:05:07.565098 mms_client-1.1.0/README.md
+-rw-r--r--   0        0        0     2913 2024-04-12 02:05:07.569098 mms_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2149 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    25363 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     4892 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      521 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3419 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      537 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0     9701 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/base.py
+-rw-r--r--   0        0        0      464 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    12065 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2588 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     7693 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0    66466 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4407 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-04-12 02:05:07.569098 mms_client-1.1.0/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-12 02:05:07.573098 mms_client-1.1.0/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0    25438 2024-04-12 02:05:07.573098 mms_client-1.1.0/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0     9653 2024-04-12 02:05:07.573098 mms_client-1.1.0/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    14742 1970-01-01 00:00:00.000000 mms_client-1.1.0/PKG-INFO
```

### Comparing `mms_client-1.0.6/LICENSE` & `mms_client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/README.md` & `mms_client-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 The underlying API sends and receives XML documents. Each of these request or responses, which we will hereafter refer to as *outer* requests and responses, contains metadata about the request/response as well as three fields which are extremely important to successful communication with the API:
 - Attachments data, included as a list of elements with the binary data in a base-64 encoded format
 - Payload data, encoded in a base-64 encoded format
 - Payload signature, which is the SHA256 hash of the payload XML data, then signed with an RSA key, in a base-64 encoded format
 
 After the data has been converted and added to the outer request object, it is sent to the appropriate server endpoint via a Zeep client. The client certificate is also injected into the request using a PCKS12 adaptor.
 
+# Serialization
+This library relies on Pydantic 2 and the pydantic-xml library for serialization/deserialization. As such, any type in this library can be converted to not only XML, but to JSON as well. This is extremely useful if you're trying to build a pass-through API service or something similar.
+
 ## Client Types
 Clients cannot call any and all endpoints in this API, willy-nilly. Some endpoints are restricted to particular clients. At the moment, there are two clients: Balance Service Providers (BSPs) and Transmission Service Operators (TSOs). Most likely you're operating as a BSP, in which case you'll have access to all endpoints. However, it makes little sense for a TSO to be able to submit bids on their own power, so they are restricted to a read-only role in most cases.
 
 Should you request an endpoint which you are not authorized for, you will receive an `mms_client.utils.errors.AudienceError`.
 
 ## Interface Type
 The MMS has two separate endpoints, depending on whether you want to access market information (MI), or other market information (OMI). Really informative, I know. Fortunately, we have designed this API in such a way that the distinction around which interface is which is unnecessary for you to know. However, note that separate Zeep clients will be maintained for each interface. These will be created as needed, which endpoints requiring the associated interface are first called. These are both setup to cache schemas to improve performance, as well. The memory required for these clients is still light, but you may want to reduce that further based on your application.
 
 # Object Hierarchy
 The object hierarchy contained in this project is not trivial, and perhaps that reflects a bit of overengineering on our part. However, we chose the paradigm we did to reduce the number of types which had to be exposed to the user. The diagram below indicates how this hierarchy works:
 
-![MMS Client Object Hierarchy](https://github.com/ElectroRoute-Japan/mms-client/blob/main/docs/mmsclient_hierarchy.drawio.png)
+![MMS Client Object Hierarchy](https://github.com/ElectroRoute-Japan/mms-client/raw/main/docs/mmsclient_hierarchy.drawio.png)
 
 Note that there are some types here that are shared between the request and response: mainly, anything inheriting from `mms_client.types.base.Envelop` or `mms_client.types.base.Payload`. For users of the client, only the Payload types need ever be used. Everything else has been obfuscated away, so it is unecessary for the user to have access to these. However, we will explain our reasoning here to provide additional context.
 
 ## Requests
 The primary request DTO is the `mms_client.types.transport.MmsRequest` object. The majority of the fields here are metadata specifying how the client should communicate with the MMS server. However, `requestData`, `requestSignature` and `attachmentData` do bear considering as these represent the actual request, a signature used to verify that the request was received, and any attachments to the request, respectively. As mentioned before, `requestData` and `attachementData` can each represent more complex objects, which should be serialized and then encoded as base-64 strings.
 
 ## Responses
@@ -159,14 +162,16 @@
 The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
+- RegistrationSubmit_Resource
+- RegistrationQuery_Resource
 
 We can add support for additional endpoints as time goes on, and independent contribution is, of course, welcome. However, support for attachments is currently limited because none of the endpoints we support currently require them. We have implemented attachment support up to the client level, but we haven't developed an architecture for submitting them through an endpoint yet.
 
 # Installation
 We have a package on PyPI so installation is as easy as doing:
 
 ```
```

### Comparing `mms_client-1.0.6/pyproject.toml` & `mms_client-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.0.6"
+version = "v1.1.0"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
+homepage = "https://github.com/ElectroRoute-Japan/mms-client"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Framework :: Pydantic :: 2",
+    "Framework :: Pytest",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: The Unlicense (Unlicense)",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Typing :: Typed",
+]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
 zeep = "^4.2.1"
 requests-pkcs12 = "^1.24"
 pydantic = "^2.6.3"
@@ -95,10 +109,13 @@
 
 [tool.coverage.run]
 omit = ["*/__init__.py"]
 
 [tool.coverage.report]
 fail_under = 100
 
+[tool.coverage.html]
+directory = "coverage_html_report"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mms_client-1.0.6/src/mms_client/client.py` & `mms_client-1.1.0/src/mms_client/client.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.1.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.1.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.1.0/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.1.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.1.0/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.1.0/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.1.0/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/security/certs.py` & `mms_client-1.1.0/src/mms_client/security/certs.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/security/crypto.py` & `mms_client-1.1.0/src/mms_client/security/crypto.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/services/base.py` & `mms_client-1.1.0/src/mms_client/services/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/services/market.py` & `mms_client-1.1.0/src/mms_client/services/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/services/omi.py` & `mms_client-1.1.0/src/mms_client/services/omi.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/services/registration.py` & `mms_client-1.1.0/src/mms_client/services/report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Contains the client layer for making registration requests to the MMS server."""
+"""Contains the client layer for making report requests to the MMS server."""
 
 from mms_client.services.base import ServiceConfiguration
 from mms_client.utils.serialization import SchemaType
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import Interface
 
 
-class RegistrationClientMixin:  # pylint: disable=unused-argument
-    """Registration client for the MMS server."""
+class ReportClientMixin:  # pylint: disable=unused-argument
+    """Report client for the MMS server."""
 
-    # The configuration for the registration service
-    config = ServiceConfiguration(Interface.MI, Serializer(SchemaType.REGISTRATION, "RegistrationData"))
+    # The configuration for the report service
+    config = ServiceConfiguration(Interface.MI, Serializer(SchemaType.REPORT, "MarketReport"))
```

### Comparing `mms_client-1.0.6/src/mms_client/types/base.py` & `mms_client-1.1.0/src/mms_client/types/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from pydantic import PrivateAttr
 from pydantic_extra_types.pendulum_dt import DateTime
 from pydantic_xml import BaseXmlModel
 from pydantic_xml import attr
 from pydantic_xml import element
 
+from mms_client.types.fields import transaction_id
+
 
 class ValidationStatus(Enum):
     """Represents the status of the validation check done on an element."""
 
     PASSED = "PASSED"  # The validation check for all data within the element has succeeded.
     WARNING = "WARNING"  # There are data within the element that have triggered warnings during the validation check.
     PASSED_PARTIAL = "PASSED_PARTIAL"  # Some data within the element has failed the validation check.
@@ -63,15 +65,15 @@
     # The number of objects that were unsuccessfully processed
     unsuccessful: Optional[int] = attr(default=None, name="Unsuccessful")
 
     # The amount of time it took to process the request in milliseconds
     time_ms: Optional[int] = attr(default=None, name="ProcessingTimeMs")
 
     # The transaction ID of the request
-    transaction_id: Optional[str] = attr(default=None, name="TransactionID", min_length=8, max_length=10)
+    transaction_id: Optional[str] = transaction_id("TransactionId", True)
 
     # When the request was received, in the format "DDD MMM DD HH:MM:SS TZ YYYY"
     timestamp: str = attr(default="", name="TimeStamp")
 
     # When the request was received, in the format "YYYY-MM-DD HH:MM:SSZ"
     timestamp_xml: Optional[DateTime] = attr(default=None, name="XmlTimeStamp")
```

### Comparing `mms_client-1.0.6/src/mms_client/types/fields.py` & `mms_client-1.1.0/src/mms_client/types/fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Contains the definitions for various fields used in the MMS API."""
 
 from pydantic_core import PydanticUndefined
 from pydantic_xml import attr
 
 # Describes the regular expression required by the MMS API for Japanese text
-JAPANESE_TEXT = r"^[\u3000-\u30FF\uFF00-\uFF60\uFFA0-\uFFEF\u4E00-\u9FEA]*$"
+JAPANESE_TEXT = r"[\u3000-\u30FF\uFF00-\uFF60\uFFA0-\uFFEF\u4E00-\u9FEA]*"
+
+# Describes the regular expression required by the MMS API for ASCII text
+ASCII_TEXT = r"[a-zA-Z0-9 ~!@#$*()_+}{:?>`='/.,%;\^\|\-\]\[\\&lt;&amp;&quot;]*"
+
+# Describes the regular expression required by the MMS API for Japanese or ASCII text
+JAPANESE_ASCII_TEXT = f"{JAPANESE_TEXT}|{ASCII_TEXT}"
 
 
 def participant(alias: str, optional: bool = False):
     """Create a field for a participant ID.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
@@ -39,14 +45,49 @@
     Returns:    A Pydantic Field object for the operator code.
     """
     return attr(
         default=None if optional else PydanticUndefined, name=alias, min_length=4, max_length=4, pattern=r"^[A-Z0-9]*$"
     )
 
 
+def transaction_id(alias: str, optional: bool = False):
+    """Create a field for a transaction ID.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the transaction ID.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined,
+        name=alias,
+        min_length=8,
+        max_length=10,
+        pattern=r"^[a-zA-Z0-9]{8,10}$",
+    )
+
+
+def capacity(alias: str, minimum: int, optional: bool = False):
+    """Create a field for a capacity value.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    minimum (int):      The minimum value for the capacity field.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the capacity value.
+    """
+    return attr(default=None if optional else PydanticUndefined, name=alias, ge=minimum, le=10000000)
+
+
 def power_positive(alias: str, optional: bool = False):
     """Create a field for a positive power value.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
     optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
@@ -64,15 +105,29 @@
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
     optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
                         required, with no default.
 
     Returns:    A Pydantic Field object for the price value.
     """
-    return attr(default=None if optional else PydanticUndefined, name=alias, ge=0.00, le=10000.00, decimal_places=2)
+    return attr(default=None if optional else PydanticUndefined, name=alias, ge=0.00, lt=10000.00, decimal_places=2)
+
+
+def percentage(alias: str, optional: bool = False):
+    """Create a field for a percentage value.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the percentage value.
+    """
+    return attr(default=None if optional else PydanticUndefined, name=alias, ge=0.0, le=100.0, decimal_places=1)
 
 
 def dr_patter_number(alias: str, optional: bool = False):
     """Create a field for a DR pattern number.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
@@ -81,14 +136,30 @@
                         required, with no default.
 
     Returns:    A Pydantic Field object for the DR pattern number.
     """
     return attr(default=None if optional else PydanticUndefined, name=alias, ge=1, le=20)
 
 
+def pattern_name(alias: str, optional: bool = False):
+    """Create a field for a pattern name.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the pattern name.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined, name=alias, min_length=1, max_length=20, pattern=JAPANESE_TEXT
+    )
+
+
 def company_short_name(alias: str, optional: bool = False):
     """Create a field for a company short name.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
     optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
@@ -97,14 +168,52 @@
     Returns:    A Pydantic Field object for the company short name.
     """
     return attr(
         default=None if optional else PydanticUndefined, name=alias, min_length=1, max_length=10, pattern=JAPANESE_TEXT
     )
 
 
+def address(alias: str, optional: bool = False):
+    """Create a field for an address.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the address.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined, name=alias, min_length=1, max_length=50, pattern=JAPANESE_TEXT
+    )
+
+
+def phone(alias: str, first_part: bool, optional: bool = False):
+    """Create a field for a phone number.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    first_part (bool):  If True, the field will be the first part of the phone number. If False, the field will be the
+                        second part of the phone number.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the phone number.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined,
+        name=alias,
+        min_length=1,
+        max_length=5 if first_part else 4,
+        pattern=r"^[0-9]*$",
+    )
+
+
 def resource_name(alias: str, optional: bool = False):
     """Create a field for a resource name.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
     optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
@@ -147,7 +256,46 @@
                         required, with no default.
 
     Returns:    A Pydantic Field object for the system code.
     """
     return attr(
         default=None if optional else PydanticUndefined, name=alias, min_length=5, max_length=5, pattern=r"^[A-Z0-9]*$"
     )
+
+
+def minute(alias: str, optional: bool = False):
+    """Create a field for a minute value.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the minute value.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined,
+        name=alias,
+        ge=0,
+        le=99,
+    )
+
+
+def hour(alias: str, optional: bool = False):
+    """Create a field for an hour value.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the hour value.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined,
+        name=alias,
+        ge=0.0,
+        lt=100.0,
+        decimal_places=1,
+    )
```

### Comparing `mms_client-1.0.6/src/mms_client/types/market.py` & `mms_client-1.1.0/src/mms_client/types/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/types/offer.py` & `mms_client-1.1.0/src/mms_client/types/offer.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,21 +57,32 @@
 
     Notes:
         For the Day-ahead Market, the tertiary 2 sell bidding volume is mandatory.
         For the Week-ahead Market, one of primary, secondary 1, secondary 2, or tertiary 1 sell bidding volumes are
         mandatory.
     """
 
-    # A number used to identify this PQ pair within the offer
+    # A number used to identify this PQ pair within the offer. Ensure that there are no duplicates of the combination
+    # of the same resource, pattern number, start date and time, and bid management number in the submitted data. In
+    # case of multiple bids in the same time slot and for the same resource, each bid must have a unique number. Enter
+    # '1' for a single bid.
     number: int = attr(name="StackNumber", ge=1, le=20)
 
-    # The minimum quantity that must be provided before the offer can be awarded
+    # The minimum quantity that must be provided before the offer can be awarded. For resources with dedicated line
+    # control or monitoring methods, must be 5000kW or higher. For resources with simple command (online) control
+    # or monitoring methods, must be 1000kW or higher.
     minimum_quantity_kw: int = power_positive("MinimumQuantityInKw")
 
-    # The primary bid quantity in kW
+    # The primary bid quantity in kW. Must be equal to or greater than minimum_quantity_kw. For non-VPP resources, the
+    # total bid volume of all records with the same resource and start date and time must be below the maximum supply
+    # capacity for the corresponding product category of the power source. However, in the case of tertiary adjustment
+    # power 2, it must be the value obtained by subtracting the total agreed capacity of effective tertiary adjustment
+    # power 1. For VPP power sources, the total bid volume of all records with the same power source code and start
+    # date and time must be below the maximum supply capacity registered for the corresponding product category in the
+    # pattern number.
     primary_qty_kw: Optional[int] = power_positive("PrimaryOfferQuantityInKw", True)
 
     # The first secondary bid quantity in kW
     secondary_1_qty_kw: Optional[int] = power_positive("Secondary1OfferQuantityInKw", True)
 
     # The second secondary bid quantity in kW
     secondary_2_qty_kw: Optional[int] = power_positive("Secondary2OfferQuantityInKw", True)
@@ -103,15 +114,16 @@
 
     # Date and time of the ending block associated with the offer
     end: DateTime = attr(name="EndTime")
 
     # The direction of the offer (buy, sell)
     direction: Direction = attr(name="Direction")
 
-    # The type of market for which the offer is being submitted
+    # The type of market for which the offer is being submitted. Must be a valid pattern number for the submission date
+    # Required for VPP resources. Ensure there are no duplicate pattern numbers for the same resource and start time.
     pattern_number: Optional[int] = dr_patter_number("DrPatternNumber", True)
 
     # The name of the BSP participant submitting the offer
     bsp_participant: Optional[str] = participant("BspParticipantName", True)
 
     # The abbreviated name of the counterparty
     company_short_name: Optional[str] = company_short_name("CompanyShortName", True)
```

### Comparing `mms_client-1.0.6/src/mms_client/types/transport.py` & `mms_client-1.1.0/src/mms_client/types/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Note that the first four items are valid for the Market Initiator (MI) interface, while the last item is valid for
     the Other Market Initiator (OMI) interface.
     """
 
     INFO = "mp.info"
     MARKET = "mp.market"
-    REGISTRATION = "mp.registration"
+    REGISTRATION = "mpr"
     REPORT = "mp.report"
     OMI = "mp.omi"
 
 
 class RequestDataType(Enum):
     """Represents the type of data to be sent to the MMS server.
```

### Comparing `mms_client-1.0.6/src/mms_client/utils/errors.py` & `mms_client-1.1.0/src/mms_client/utils/errors.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/src/mms_client/utils/serialization.py` & `mms_client-1.1.0/src/mms_client/utils/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
         # Next, attempt to extract the envelope and data from within the response
         resp.envelope, resp.envelope_validation, envelope_node = self._from_tree_envelope(raw, envelope_type)
 
         # Now, verify that the response doesn't contain an unexpected data type and then retrieve the payload data
         # from within the envelope
         self._verify_tree_data_tag(envelope_node, data_type)
-        resp.payload = self._from_tree_data(envelope_node.find(data_type.__name__), data_type)
+        resp.payload = self._from_tree_data(envelope_node.find(get_tag(data_type)), data_type)
 
         # Finally, attempt to extract the messages from within the payload
         resp.messages = self._from_tree_messages(raw, envelope_type, data_type, self._payload_key, False)
 
         # Return the response
         return resp
 
@@ -163,15 +163,15 @@
         resp.envelope, resp.envelope_validation, env_node = self._from_tree_envelope(raw, envelope_type)
 
         # Now, verify that the response doesn't contain an unexpected data type and then retrieve the payload data
         # from within the envelope
         # Note: apparently, mypy doesn't know about setter-getter properties either...
         self._verify_tree_data_tag(env_node, data_type)
         resp.payload = [
-            self._from_tree_data(item, data_type) for item in env_node.findall(data_type.__name__)  # type: ignore[misc]
+            self._from_tree_data(item, data_type) for item in env_node.findall(get_tag(data_type))  # type: ignore[misc]
         ]
 
         # Finally, attempt to extract the messages from within the payload
         resp.messages = self._from_tree_messages(raw, envelope_type, data_type, self._payload_key, True)
 
         # Return the response
         return resp
@@ -212,15 +212,15 @@
         raw (Element):              The raw data to be converted.
         data_type (Type[Payload]):  The type of data to be constructed.
 
         Raises:
         ValueError:    If the expected data type is not found in the response.
         """
         data_tags = set(node.tag for node in raw)
-        if not data_tags.issubset([data_type.__name__, "Messages"]):
+        if not data_tags.issubset([data_type.__name__, data_type.__xml_tag__, "Messages"]):
             raise ValueError(f"Expected data type '{data_type.__name__}' not found in response")
 
     def _from_tree_data(self, raw: Optional[Element], data_type: Type[P]) -> Optional[ResponseData[P]]:
         """Attempt to extract the data from within the payload.
 
         Arguments:
         raw (Element):                  The raw data to be converted.
@@ -287,16 +287,15 @@
             )
         elif root.endswith(envelope_type.__name__):
             messages.update(
                 self._from_tree_messages_inner(raw, envelope_type, current_type, root, current_type.__name__, multi)
             )
         else:
             # Iterate over each field on the current type...
-            for name, field in current_type.model_fields.items():
-                print(f"Checking field {name} with type {field.annotation}...")
+            for field in current_type.model_fields.values():
 
                 # First, get the arguments and origin of the field's annotation
                 args = get_args(field.annotation)
                 origin = get_origin(field.annotation)
                 has_args = len(args) > 0
 
                 # Next, check if the annotation is a subclass of Payload or else if it's a collection of Payload. If
@@ -416,27 +415,27 @@
         """Wrapper for the response payload type that will be used for serialization."""
 
     # Finally, return the payload type so we can instantiate it
     return RSPayload
 
 
 @lru_cache(maxsize=None)
-def _create_response_common_type(tag_type: Type) -> Type[ResponseCommon]:
+def _create_response_common_type(tag_type: Type[Union[E, P]]) -> Type[ResponseCommon]:
     """Create a new wrapper for the ResponseCommon type with the given tag.
 
     This method is intended to save us the overhead of writing a new class for each tag type. Instead, we can
     create a new class at runtime that contains the ResponseCommon type, and use that for deserialization.
 
     Arguments:
     tag_type (Type):    The type of tag to use for the wrapper.
 
     Returns:    The wrapper type that will be used for deserialization.
     """  # fmt: skip
     # First, create a new wrapper type that contains the ResponseCommon type with the appropriate XML tag
-    class Wrapper(ResponseCommon, tag=tag_type.__name__):  # type: ignore[call-arg]
+    class Wrapper(ResponseCommon, tag=get_tag(tag_type)):  # type: ignore[call-arg]
         """Wrapper for the validation object with the proper XML tag."""
 
     # Finally, return the wrapper type so we can instantiate it
     return Wrapper
 
 
 @lru_cache(maxsize=None)
@@ -458,15 +457,15 @@
     Returns:    A new payload type that can be used for serialization.
     """  # fmt: skip
     # First, create a wrapper for our data type that will be used to store the data in the payload
     class Envelope(envelope_type):  # type: ignore[valid-type, misc]
         """Wrapper for the data type that will be used to store the data in the payload."""
 
         # The data to be stored in the payload
-        data: data_type = element(tag=data_type.__name__)  # type: ignore[valid-type]
+        data: data_type = element(tag=get_tag(data_type))  # type: ignore[valid-type]
 
         def __init__(self, envelope: envelope_type, data: data_type):  # type: ignore[valid-type]
             """Create a new envelope to store payload data.
 
             Arguments:
             envelope (Envelope):    The payload to be stored in the data.
             data (Payload):         The data to be stored in the payload.
@@ -507,7 +506,18 @@
 
     Raises:     ValueError if the tag isn't found in the node.
     """
     found = node.find(tag)
     if found is None:
         raise ValueError(f"Expected tag '{tag}' not found in node")  # pragma: no cover
     return found
+
+
+def get_tag(data_type: Type[P]) -> str:
+    """Get the tag for the given data type.
+
+    Arguments:
+    data_type (Type[Payload]):  The data type to get the tag for.
+
+    Returns:    The tag for the given data type.
+    """
+    return data_type.__xml_tag__ or data_type.__name__
```

### Comparing `mms_client-1.0.6/src/mms_client/utils/web.py` & `mms_client-1.1.0/src/mms_client/utils/web.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.0.6/PKG-INFO` & `mms_client-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.0.6
+Version: 1.1.0
 Summary: API client for accessing the MMS
+Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Pydantic :: 2
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: pendulum (>=3.0.0,<4.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-xml (>=2.9.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -28,26 +39,29 @@
 The underlying API sends and receives XML documents. Each of these request or responses, which we will hereafter refer to as *outer* requests and responses, contains metadata about the request/response as well as three fields which are extremely important to successful communication with the API:
 - Attachments data, included as a list of elements with the binary data in a base-64 encoded format
 - Payload data, encoded in a base-64 encoded format
 - Payload signature, which is the SHA256 hash of the payload XML data, then signed with an RSA key, in a base-64 encoded format
 
 After the data has been converted and added to the outer request object, it is sent to the appropriate server endpoint via a Zeep client. The client certificate is also injected into the request using a PCKS12 adaptor.
 
+# Serialization
+This library relies on Pydantic 2 and the pydantic-xml library for serialization/deserialization. As such, any type in this library can be converted to not only XML, but to JSON as well. This is extremely useful if you're trying to build a pass-through API service or something similar.
+
 ## Client Types
 Clients cannot call any and all endpoints in this API, willy-nilly. Some endpoints are restricted to particular clients. At the moment, there are two clients: Balance Service Providers (BSPs) and Transmission Service Operators (TSOs). Most likely you're operating as a BSP, in which case you'll have access to all endpoints. However, it makes little sense for a TSO to be able to submit bids on their own power, so they are restricted to a read-only role in most cases.
 
 Should you request an endpoint which you are not authorized for, you will receive an `mms_client.utils.errors.AudienceError`.
 
 ## Interface Type
 The MMS has two separate endpoints, depending on whether you want to access market information (MI), or other market information (OMI). Really informative, I know. Fortunately, we have designed this API in such a way that the distinction around which interface is which is unnecessary for you to know. However, note that separate Zeep clients will be maintained for each interface. These will be created as needed, which endpoints requiring the associated interface are first called. These are both setup to cache schemas to improve performance, as well. The memory required for these clients is still light, but you may want to reduce that further based on your application.
 
 # Object Hierarchy
 The object hierarchy contained in this project is not trivial, and perhaps that reflects a bit of overengineering on our part. However, we chose the paradigm we did to reduce the number of types which had to be exposed to the user. The diagram below indicates how this hierarchy works:
 
-![MMS Client Object Hierarchy](https://github.com/ElectroRoute-Japan/mms-client/blob/main/docs/mmsclient_hierarchy.drawio.png)
+![MMS Client Object Hierarchy](https://github.com/ElectroRoute-Japan/mms-client/raw/main/docs/mmsclient_hierarchy.drawio.png)
 
 Note that there are some types here that are shared between the request and response: mainly, anything inheriting from `mms_client.types.base.Envelop` or `mms_client.types.base.Payload`. For users of the client, only the Payload types need ever be used. Everything else has been obfuscated away, so it is unecessary for the user to have access to these. However, we will explain our reasoning here to provide additional context.
 
 ## Requests
 The primary request DTO is the `mms_client.types.transport.MmsRequest` object. The majority of the fields here are metadata specifying how the client should communicate with the MMS server. However, `requestData`, `requestSignature` and `attachmentData` do bear considering as these represent the actual request, a signature used to verify that the request was received, and any attachments to the request, respectively. As mentioned before, `requestData` and `attachementData` can each represent more complex objects, which should be serialized and then encoded as base-64 strings.
 
 ## Responses
@@ -180,14 +194,16 @@
 The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
+- RegistrationSubmit_Resource
+- RegistrationQuery_Resource
 
 We can add support for additional endpoints as time goes on, and independent contribution is, of course, welcome. However, support for attachments is currently limited because none of the endpoints we support currently require them. We have implemented attachment support up to the client level, but we haven't developed an architecture for submitting them through an endpoint yet.
 
 # Installation
 We have a package on PyPI so installation is as easy as doing:
 
 ```
```

