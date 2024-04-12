# Comparing `tmp/pymagento-1.9.2.tar.gz` & `tmp/pymagento-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.9.2.tar", max compression
+gzip compressed data, was "pymagento-1.9.3.tar", max compression
```

## Comparing `pymagento-1.9.2.tar` & `pymagento-1.9.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-10-06 15:39:09.066223 pymagento-1.9.2/LICENSE
--rw-r--r--   0        0        0      903 2023-10-06 15:39:09.066223 pymagento-1.9.2/README.md
--rw-r--r--   0        0        0     1550 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/__init__.py
--rw-r--r--   0        0        0     4773 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/batches.py
--rw-r--r--   0        0        0    43365 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/client.py
--rw-r--r--   0        0        0     1768 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/queries.py
--rw-r--r--   0        0        0      357 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/types.py
--rw-r--r--   0        0        0       22 2023-10-06 15:39:09.066223 pymagento-1.9.2/magento/version.py
--rw-r--r--   0        0        0     1249 2023-10-06 15:39:09.070223 pymagento-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 pymagento-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-01-08 10:57:42.302917 pymagento-1.9.3/LICENSE
+-rw-r--r--   0        0        0      903 2024-01-08 10:57:42.302917 pymagento-1.9.3/README.md
+-rw-r--r--   0        0        0     1550 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/__init__.py
+-rw-r--r--   0        0        0     4773 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/attributes.py
+-rw-r--r--   0        0        0     3925 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/batches.py
+-rw-r--r--   0        0        0    43521 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/client.py
+-rw-r--r--   0        0        0     1768 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/py.typed
+-rw-r--r--   0        0        0     3374 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/queries.py
+-rw-r--r--   0        0        0      357 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/types.py
+-rw-r--r--   0        0        0       22 2024-01-08 10:57:42.302917 pymagento-1.9.3/magento/version.py
+-rw-r--r--   0        0        0     1249 2024-01-08 10:57:42.302917 pymagento-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 pymagento-1.9.3/PKG-INFO
```

### Comparing `pymagento-1.9.2/LICENSE` & `pymagento-1.9.3/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2020-2023 – Bixoto.com
+Copyright © 2020-2024 – Bixoto.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `pymagento-1.9.2/README.md` & `pymagento-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.9.2/magento/__init__.py` & `pymagento-1.9.3/magento/__init__.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.9.2/magento/attributes.py` & `pymagento-1.9.3/magento/attributes.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.9.2/magento/batches.py` & `pymagento-1.9.3/magento/batches.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,27 +28,28 @@
         """
         self._batch.append(item_data)
         if len(self._batch) >= self.batch_size:
             self.send_batch()
 
     def send_batch(self):
         """
-        Send the current pending batch (if any).
+        Send the current pending batch (if any) and return the response from the Magento API.
         """
         if not self._batch:
-            return
+            return None
 
-        self._put_batch()
+        resp = self._put_batch()
         self._sent_items += len(self._batch)
         self._sent_batches += 1
         self._batch = []
+        return resp
 
     def _put_batch(self):  # pragma: nocover
         # Note this raises on error
-        _resp = self.client.put_api(self.path, json=self._batch, throw=True, async_bulk=True).json()
+        return self.client.put_api(self.path, json=self._batch, throw=True, async_bulk=True).json()
 
     def finalize(self):
         """
         Send the last pending batch (if any). This doesn’t need to be called when the object is used as a context
         manager.
 
         :return: a dictionary with the total number of batches and items
```

### Comparing `pymagento-1.9.2/magento/client.py` & `pymagento-1.9.3/magento/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,17 @@
         Get the status of an async/bulk operation.
         """
         return self.get_api(f"/V1/bulk/{escape_path(bulk_uuid)}/status", throw=True).json()
 
     # Carts
     # =====
 
+    def get_cart(self, *, cart_id: PathId, **kwargs) -> MagentoEntity:
+        return self.get_json_api(f"/V1/carts/{cart_id}", **kwargs)
+
     def get_carts(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all carts (generator)."""
         return self.get_paginated("/V1/carts/search", query=query, limit=limit, **kwargs)
 
     # Categories
     # ==========
 
@@ -570,15 +573,15 @@
     def get_product(self, sku: Sku) -> Optional[Product]:
         """
         Get a single product. Return ``None`` if it doesn’t exist.
 
         :param sku: SKU of the product
         :return:
         """
-        return self.get_json_api(f"/V1/products/{escape_path(sku)}")
+        return self.get_json_api(f"/V1/products/{escape_path(sku)}", none_on_404=True)
 
     def get_product_by_id(self, product_id: int) -> Optional[Product]:
         """
         Get a product given its id. Return ``None`` if the product doesn’t exist.
 
         :param product_id: ID of the product
         :return:
@@ -708,15 +711,15 @@
         return cast(bool, response.json())
 
     def async_update_products(self, product_updates: Iterable[Product]):
         """
         Update multiple products using the async bulk API.
 
         Example:
-            >>> Magento().async_update_products([{"sku": "SK123", "name": "Abc"}), {"sku": "SK4", "name": "Def"}])
+            >>> Magento().async_update_products([{"sku": "SK123", "name": "Abc"}, {"sku": "SK4", "name": "Def"}])
 
         See https://devdocs.magento.com/guides/v2.4/rest/bulk-endpoints.html
 
         :param product_updates: sequence of product data dicts. They MUST contain an `sku` key.
         :return:
         """
         payload = [{"product": product_update} for product_update in product_updates]
```

### Comparing `pymagento-1.9.2/magento/exceptions.py` & `pymagento-1.9.3/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.9.2/magento/order_helpers.py` & `pymagento-1.9.3/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.9.2/magento/queries.py` & `pymagento-1.9.3/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.9.2/pyproject.toml` & `pymagento-1.9.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.9.2"
+version = "1.9.3"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
```

### Comparing `pymagento-1.9.2/PKG-INFO` & `pymagento-1.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.9.2
+Version: 1.9.3
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=4.4.0,<5.0.0) ; extra == "docs"
 Requires-Dist: api-session (>=1.3.2,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
 Description-Content-Type: text/markdown
 
 # PyMagento
```

