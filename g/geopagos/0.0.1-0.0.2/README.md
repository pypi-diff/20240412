# Comparing `tmp/geopagos-0.0.1.tar.gz` & `tmp/geopagos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopagos-0.0.1.tar", last modified: Thu Mar 21 22:00:01 2024, max compression
+gzip compressed data, was "geopagos-0.0.2.tar", last modified: Fri Apr 12 14:07:05 2024, max compression
```

## Comparing `geopagos-0.0.1.tar` & `geopagos-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-03-21 22:00:01.935752 geopagos-0.0.1/
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     1073 2024-03-21 21:59:16.000000 geopagos-0.0.1/LICENCE
--rw-r--r--   0 alvezgr   (1001) alvezgr   (1001)     2630 2024-03-21 22:00:01.935752 geopagos-0.0.1/PKG-INFO
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2045 2024-03-21 21:59:16.000000 geopagos-0.0.1/README.md
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)      654 2024-03-21 21:59:16.000000 geopagos-0.0.1/pyproject.toml
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       38 2024-03-21 22:00:01.935752 geopagos-0.0.1/setup.cfg
-drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-03-21 22:00:01.931753 geopagos-0.0.1/src/
-drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-03-21 22:00:01.935752 geopagos-0.0.1/src/geopagos/
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       21 2024-03-21 21:59:16.000000 geopagos-0.0.1/src/geopagos/__init__.py
-drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-03-21 22:00:01.935752 geopagos-0.0.1/src/geopagos/client/
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       27 2024-03-21 21:59:16.000000 geopagos-0.0.1/src/geopagos/client/__init__.py
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2768 2024-03-21 21:59:16.000000 geopagos-0.0.1/src/geopagos/client/client.py
-drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-03-21 22:00:01.935752 geopagos-0.0.1/src/geopagos/schemas/
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       54 2024-03-21 21:59:16.000000 geopagos-0.0.1/src/geopagos/schemas/__init__.py
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2420 2024-03-21 21:59:16.000000 geopagos-0.0.1/src/geopagos/schemas/order.py
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     4040 2024-03-21 21:59:16.000000 geopagos-0.0.1/src/geopagos/schemas/payment.py
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     1446 2024-03-21 21:59:16.000000 geopagos-0.0.1/src/geopagos/sdk.py
-drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-03-21 22:00:01.935752 geopagos-0.0.1/src/geopagos.egg-info/
--rw-r--r--   0 alvezgr   (1001) alvezgr   (1001)     2630 2024-03-21 22:00:01.000000 geopagos-0.0.1/src/geopagos.egg-info/PKG-INFO
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)      421 2024-03-21 22:00:01.000000 geopagos-0.0.1/src/geopagos.egg-info/SOURCES.txt
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)        1 2024-03-21 22:00:01.000000 geopagos-0.0.1/src/geopagos.egg-info/dependency_links.txt
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)        9 2024-03-21 22:00:01.000000 geopagos-0.0.1/src/geopagos.egg-info/top_level.txt
-drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-03-21 22:00:01.935752 geopagos-0.0.1/tests/
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2707 2024-03-21 21:59:16.000000 geopagos-0.0.1/tests/test_order.py
--rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2885 2024-03-21 21:59:16.000000 geopagos-0.0.1/tests/test_payments.py
+drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-04-12 14:07:05.875618 geopagos-0.0.2/
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     1073 2024-03-21 21:59:16.000000 geopagos-0.0.2/LICENCE
+-rw-r--r--   0 alvezgr   (1001) alvezgr   (1001)     2410 2024-04-12 14:07:05.875618 geopagos-0.0.2/PKG-INFO
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     1825 2024-04-12 14:00:59.000000 geopagos-0.0.2/README.md
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)      655 2024-04-12 14:05:14.000000 geopagos-0.0.2/pyproject.toml
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       38 2024-04-12 14:07:05.875618 geopagos-0.0.2/setup.cfg
+drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-04-12 14:07:05.871618 geopagos-0.0.2/src/
+drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-04-12 14:07:05.871618 geopagos-0.0.2/src/geopagos/
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       21 2024-03-21 21:59:16.000000 geopagos-0.0.2/src/geopagos/__init__.py
+drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-04-12 14:07:05.875618 geopagos-0.0.2/src/geopagos/client/
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       27 2024-03-21 21:59:16.000000 geopagos-0.0.2/src/geopagos/client/__init__.py
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2768 2024-03-21 21:59:16.000000 geopagos-0.0.2/src/geopagos/client/client.py
+drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-04-12 14:07:05.875618 geopagos-0.0.2/src/geopagos/schemas/
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)       54 2024-03-21 21:59:16.000000 geopagos-0.0.2/src/geopagos/schemas/__init__.py
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2420 2024-03-21 21:59:16.000000 geopagos-0.0.2/src/geopagos/schemas/order.py
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     4040 2024-03-21 21:59:16.000000 geopagos-0.0.2/src/geopagos/schemas/payment.py
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     1446 2024-03-21 21:59:16.000000 geopagos-0.0.2/src/geopagos/sdk.py
+drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-04-12 14:07:05.875618 geopagos-0.0.2/src/geopagos.egg-info/
+-rw-r--r--   0 alvezgr   (1001) alvezgr   (1001)     2410 2024-04-12 14:07:05.000000 geopagos-0.0.2/src/geopagos.egg-info/PKG-INFO
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)      421 2024-04-12 14:07:05.000000 geopagos-0.0.2/src/geopagos.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)        1 2024-04-12 14:07:05.000000 geopagos-0.0.2/src/geopagos.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)        9 2024-04-12 14:07:05.000000 geopagos-0.0.2/src/geopagos.egg-info/top_level.txt
+drwxrwxr-x   0 alvezgr   (1001) alvezgr   (1001)        0 2024-04-12 14:07:05.875618 geopagos-0.0.2/tests/
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2707 2024-03-21 21:59:16.000000 geopagos-0.0.2/tests/test_order.py
+-rw-rw-r--   0 alvezgr   (1001) alvezgr   (1001)     2885 2024-03-21 21:59:16.000000 geopagos-0.0.2/tests/test_payments.py
```

### Comparing `geopagos-0.0.1/LICENCE` & `geopagos-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `geopagos-0.0.1/PKG-INFO` & `geopagos-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopagos
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unoffial geopagos sdk to work with apps like (Viumi, Getnet, OpenPay, Taca Taca, Toque, Sipago...).
 Author-email: Alvez Gerardo <alvezpope@gmail.com>
 Project-URL: Homepage, https://github.com/alvezgr/unofficial-gp-sdk/
 Project-URL: Issues, https://github.com/Alvezgr/unofficial-gp-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,72 +13,67 @@
 License-File: LICENCE
 
 # Unofficial Geopagos APPS (Getnet, Viumi...) Python SDK 
 
 This sdk provides basic methos to integrate geopagos apps (Getnet, Viumi, OpenPay, Taca Taca, Toque, Sipago, Uala Bis) payment API for a platform to start receiving payments.
 
 ## Requirements
-
-python3
+```txt
+python3.x
 requests
+```
 
 
 ## Installation 
 
 Run ```git clone git@github.com:Alvezgr/unofficial-gp-sdk.git```
 
 ## Getting Started
 Before you begin, you must request the API credential from your supplier (Getnet, Viumi, OpenPay, Taca Taca, Toque, Sipago, Uala Bis)
 
 Request the your `Access Token` to the [geopagos auth](https://auth.geopagos.com/oauth/token) and API url
 
 ### Simple usage
   
 ```python
-import gp
+import geopagos
 
-sdk = gp.SDK("ACCESS_TOKEN", "https://api.url.com")
+sdk = geopagos.SDK("ACCESS_TOKEN", "https://api.url.com")
 
-order_data = {
-  "data": {
-    "attributes": {
-      "redirect_urls": {
-        "success": "https://www.mitienda.com/success",
-        "failed": "https://www.mitienda.com/failed"
-      },
-      "shipping": {
-        "name": "Correo Argentino",
-        "price": {
-          "currency": "032",
-          "amount": 450
-        }
-      },
-      "items": [
-        {
-          "name": "Lomo con papas",
-          "unitPrice": {
-            "currency": "032",
-            "amount": 10050
-          },
-          "quantity": 2
-        },
-        {
-          "unitPrice": {
-            "currency": "032",
-            "amount": 1
-          },
-          "quantity": 1
-        }
-      ],
-      "externalData": "{\"NroLegajo\": 25993}"
-    }
-  }
+urls = {
+    "success": "https://www.mitienda.com/success",
+    "failed": "https://www.mitienda.com/failed"
 }
 
-result = sdk.order().create(order_data)
+shipping =  {
+    "name": "Correo Argentino",
+    "price": {
+        "currency": "032",
+        "amount": 450
+  }
+}
+items =  [
+  {
+      "name": "Lomo con papas",
+      "unitPrice": {
+          "currency": "032",
+          "amount": 10050
+      },
+      "quantity": 2
+  },
+]
+
+external_data = "25993"
+
+result = sdk.order().create(
+      items,
+      urls=urls,
+      shipping=shipping,
+      external_data=external_data
+)
 payment = result["response"]
 
 print(payment)
 ```
 ## Documentation 
 
 Visit apps site for docs:
```

### Comparing `geopagos-0.0.1/README.md` & `geopagos-0.0.2/src/geopagos.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,79 @@
+Metadata-Version: 2.1
+Name: geopagos
+Version: 0.0.2
+Summary: Unoffial geopagos sdk to work with apps like (Viumi, Getnet, OpenPay, Taca Taca, Toque, Sipago...).
+Author-email: Alvez Gerardo <alvezpope@gmail.com>
+Project-URL: Homepage, https://github.com/alvezgr/unofficial-gp-sdk/
+Project-URL: Issues, https://github.com/Alvezgr/unofficial-gp-sdk/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # Unofficial Geopagos APPS (Getnet, Viumi...) Python SDK 
 
 This sdk provides basic methos to integrate geopagos apps (Getnet, Viumi, OpenPay, Taca Taca, Toque, Sipago, Uala Bis) payment API for a platform to start receiving payments.
 
 ## Requirements
-
-python3
+```txt
+python3.x
 requests
+```
 
 
 ## Installation 
 
 Run ```git clone git@github.com:Alvezgr/unofficial-gp-sdk.git```
 
 ## Getting Started
 Before you begin, you must request the API credential from your supplier (Getnet, Viumi, OpenPay, Taca Taca, Toque, Sipago, Uala Bis)
 
 Request the your `Access Token` to the [geopagos auth](https://auth.geopagos.com/oauth/token) and API url
 
 ### Simple usage
   
 ```python
-import gp
+import geopagos
 
-sdk = gp.SDK("ACCESS_TOKEN", "https://api.url.com")
+sdk = geopagos.SDK("ACCESS_TOKEN", "https://api.url.com")
 
-order_data = {
-  "data": {
-    "attributes": {
-      "redirect_urls": {
-        "success": "https://www.mitienda.com/success",
-        "failed": "https://www.mitienda.com/failed"
-      },
-      "shipping": {
-        "name": "Correo Argentino",
-        "price": {
-          "currency": "032",
-          "amount": 450
-        }
-      },
-      "items": [
-        {
-          "name": "Lomo con papas",
-          "unitPrice": {
-            "currency": "032",
-            "amount": 10050
-          },
-          "quantity": 2
-        },
-        {
-          "unitPrice": {
-            "currency": "032",
-            "amount": 1
-          },
-          "quantity": 1
-        }
-      ],
-      "externalData": "{\"NroLegajo\": 25993}"
-    }
-  }
+urls = {
+    "success": "https://www.mitienda.com/success",
+    "failed": "https://www.mitienda.com/failed"
 }
 
-result = sdk.order().create(order_data)
+shipping =  {
+    "name": "Correo Argentino",
+    "price": {
+        "currency": "032",
+        "amount": 450
+  }
+}
+items =  [
+  {
+      "name": "Lomo con papas",
+      "unitPrice": {
+          "currency": "032",
+          "amount": 10050
+      },
+      "quantity": 2
+  },
+]
+
+external_data = "25993"
+
+result = sdk.order().create(
+      items,
+      urls=urls,
+      shipping=shipping,
+      external_data=external_data
+)
 payment = result["response"]
 
 print(payment)
 ```
 ## Documentation 
 
 Visit apps site for docs:
```

### Comparing `geopagos-0.0.1/pyproject.toml` & `geopagos-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geopagos"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Alvez Gerardo", email="alvezpope@gmail.com" },
 ]
 description = "Unoffial geopagos sdk to work with apps like (Viumi, Getnet, OpenPay, Taca Taca, Toque, Sipago...)."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/alvezgr/unofficial-gp-sdk/"
-Issues = "https://github.com/Alvezgr/unofficial-gp-sdk/issues"
+Issues = "https://github.com/Alvezgr/unofficial-gp-sdk/issues"
```

### Comparing `geopagos-0.0.1/src/geopagos/client/client.py` & `geopagos-0.0.2/src/geopagos/client/client.py`

 * *Files identical despite different names*

### Comparing `geopagos-0.0.1/src/geopagos/schemas/order.py` & `geopagos-0.0.2/src/geopagos/schemas/order.py`

 * *Files identical despite different names*

### Comparing `geopagos-0.0.1/src/geopagos/schemas/payment.py` & `geopagos-0.0.2/src/geopagos/schemas/payment.py`

 * *Files identical despite different names*

### Comparing `geopagos-0.0.1/src/geopagos/sdk.py` & `geopagos-0.0.2/src/geopagos/sdk.py`

 * *Files identical despite different names*

### Comparing `geopagos-0.0.1/tests/test_order.py` & `geopagos-0.0.2/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `geopagos-0.0.1/tests/test_payments.py` & `geopagos-0.0.2/tests/test_payments.py`

 * *Files identical despite different names*

