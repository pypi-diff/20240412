# Comparing `tmp/moby_distribution-0.8.1.tar.gz` & `tmp/moby_distribution-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moby_distribution-0.8.1.tar", max compression
+gzip compressed data, was "moby_distribution-0.8.2.tar", max compression
```

## Comparing `moby_distribution-0.8.1.tar` & `moby_distribution-0.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/LICENSE
--rw-r--r--   0        0        0     7006 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/README.md
--rw-r--r--   0        0        0      954 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/moby_distribution/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/moby_distribution/registry/__init__.py
--rw-r--r--   0        0        0     5910 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/moby_distribution/registry/auth.py
--rw-r--r--   0        0        0     7598 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/moby_distribution/registry/client.py
--rw-r--r--   0        0        0      917 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/moby_distribution/registry/exceptions.py
--rw-r--r--   0        0        0      752 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/moby_distribution/registry/resources/__init__.py
--rw-r--r--   0        0        0    11137 2024-04-08 02:20:35.859545 moby_distribution-0.8.1/moby_distribution/registry/resources/blobs.py
--rw-r--r--   0        0        0    16004 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/registry/resources/image.py
--rw-r--r--   0        0        0     4875 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/registry/resources/manifests.py
--rw-r--r--   0        0        0     1033 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/registry/resources/tags.py
--rw-r--r--   0        0        0     3972 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/registry/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/spec/__init__.py
--rw-r--r--   0        0        0     1140 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/spec/auth.py
--rw-r--r--   0        0        0     1077 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/spec/base.py
--rw-r--r--   0        0        0     4204 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/spec/endpoint.py
--rw-r--r--   0        0        0     3985 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/spec/image_json.py
--rw-r--r--   0        0        0     4615 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/moby_distribution/spec/manifest.py
--rw-r--r--   0        0        0      914 2024-04-08 02:20:35.863545 moby_distribution-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     7957 1970-01-01 00:00:00.000000 moby_distribution-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/LICENSE
+-rw-r--r--   0        0        0     7006 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/README.md
+-rw-r--r--   0        0        0      954 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/registry/__init__.py
+-rw-r--r--   0        0        0     5910 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/registry/auth.py
+-rw-r--r--   0        0        0     7598 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/registry/client.py
+-rw-r--r--   0        0        0      917 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/registry/exceptions.py
+-rw-r--r--   0        0        0      752 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/registry/resources/__init__.py
+-rw-r--r--   0        0        0    11137 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/registry/resources/blobs.py
+-rw-r--r--   0        0        0    16004 2024-04-12 04:17:24.889344 moby_distribution-0.8.2/moby_distribution/registry/resources/image.py
+-rw-r--r--   0        0        0     5243 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/registry/resources/manifests.py
+-rw-r--r--   0        0        0     1033 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/registry/resources/tags.py
+-rw-r--r--   0        0        0     3972 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/registry/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/spec/__init__.py
+-rw-r--r--   0        0        0     1140 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/spec/auth.py
+-rw-r--r--   0        0        0     1077 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/spec/base.py
+-rw-r--r--   0        0        0     4204 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/spec/endpoint.py
+-rw-r--r--   0        0        0     3985 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/spec/image_json.py
+-rw-r--r--   0        0        0     4615 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/moby_distribution/spec/manifest.py
+-rw-r--r--   0        0        0      914 2024-04-12 04:17:24.893344 moby_distribution-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     7957 1970-01-01 00:00:00.000000 moby_distribution-0.8.2/PKG-INFO
```

### Comparing `moby_distribution-0.8.1/LICENSE` & `moby_distribution-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/README.md` & `moby_distribution-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/__init__.py` & `moby_distribution-0.8.2/moby_distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from moby_distribution.spec.image_json import ImageJSON
 from moby_distribution.spec.manifest import (
     ManifestSchema1,
     ManifestSchema2,
     OCIManifestSchema1,
 )
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 __all__ = [
     "DockerRegistryV2Client",
     "Blob",
     "ManifestRef",
     "Tags",
     "APIEndpoint",
     "OFFICIAL_ENDPOINT",
```

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/auth.py` & `moby_distribution-0.8.2/moby_distribution/registry/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/client.py` & `moby_distribution-0.8.2/moby_distribution/registry/client.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/exceptions.py` & `moby_distribution-0.8.2/moby_distribution/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/resources/__init__.py` & `moby_distribution-0.8.2/moby_distribution/registry/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/resources/blobs.py` & `moby_distribution-0.8.2/moby_distribution/registry/resources/blobs.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/resources/image.py` & `moby_distribution-0.8.2/moby_distribution/registry/resources/image.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/resources/manifests.py` & `moby_distribution-0.8.2/moby_distribution/registry/resources/manifests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 from typing import Optional, Union
 
 import libtrust
 
-from moby_distribution.registry.client import DockerRegistryV2Client, URLBuilder, default_client
+from moby_distribution.registry.client import (
+    DockerRegistryV2Client,
+    URLBuilder,
+    default_client,
+)
 from moby_distribution.registry.exceptions import ResourceNotFound, UnSupportMediaType
 from moby_distribution.registry.resources import RepositoryResource
-from moby_distribution.registry.utils import TypeTimeout, client_default_timeout, get_private_key
-from moby_distribution.spec.manifest import ManifestDescriptor, ManifestSchema1, ManifestSchema2, OCIManifestSchema1
+from moby_distribution.registry.utils import (
+    TypeTimeout,
+    client_default_timeout,
+    get_private_key,
+)
+from moby_distribution.spec.manifest import (
+    ManifestDescriptor,
+    ManifestSchema1,
+    ManifestSchema2,
+    OCIManifestSchema1,
+)
 
 
 class ManifestRef(RepositoryResource):
     TYPES = {
         ManifestSchema1.content_type(): ManifestSchema1,
         ManifestSchema2.content_type(): ManifestSchema2,
         OCIManifestSchema1.content_type(): OCIManifestSchema1,
@@ -29,26 +42,32 @@
 
     def get(self, media_type: str = ManifestSchema2.content_type()):
         """retrieve image manifest as the provided media_type"""
         if media_type not in self.TYPES:
             raise UnSupportMediaType(media_type)
 
         type_ = self.TYPES[media_type]
-        url = URLBuilder.build_manifests_url(self.client.api_base_url, self.repo, self.reference)
+        url = URLBuilder.build_manifests_url(
+            self.client.api_base_url, self.repo, self.reference
+        )
         headers = {"Accept": media_type}
         data = self.client.get(url=url, headers=headers, timeout=self.timeout).json()
         return type_(**data)
 
-    def get_metadata(self, media_type: str = ManifestSchema2.content_type()) -> Optional[ManifestDescriptor]:
+    def get_metadata(
+        self, media_type: str = ManifestSchema2.content_type()
+    ) -> Optional[ManifestDescriptor]:
         """return ManifestDescriptor if the manifest exists."""
         if media_type not in self.TYPES:
             raise UnSupportMediaType(media_type)
 
         headers = {"Accept": media_type}
-        url = URLBuilder.build_manifests_url(self.client.api_base_url, self.repo, self.reference)
+        url = URLBuilder.build_manifests_url(
+            self.client.api_base_url, self.repo, self.reference
+        )
         try:
             resp = self.client.head(url=url, headers=headers, timeout=self.timeout)
         except ResourceNotFound:
             return None
 
         media_type = resp.headers.get("Content-Type")
         digest = resp.headers.get("Docker-Content-Digest")
@@ -65,53 +84,70 @@
         """
         descriptor = self.get_metadata()
         if not descriptor:
             if raise_not_found:
                 raise ResourceNotFound
             return False
 
-        url = URLBuilder.build_manifests_url(self.client.api_base_url, self.repo, descriptor.digest)
+        url = URLBuilder.build_manifests_url(
+            self.client.api_base_url, self.repo, descriptor.digest
+        )
         try:
             resp = self.client.delete(url=url, timeout=self.timeout)
         except ResourceNotFound:
             if raise_not_found:
                 raise
             return False
 
         return resp.ok
 
-    def put(self, manifest: Union[ManifestSchema1, ManifestSchema2, OCIManifestSchema1]) -> bool:
+    def put(
+        self, manifest: Union[ManifestSchema1, ManifestSchema2, OCIManifestSchema1]
+    ) -> bool:
         """creates or updates the given manifest."""
         if isinstance(manifest, ManifestSchema1):
             resp = self._put_legacy_manifest(manifest)
         else:
             resp = self._put_new_manifest(manifest)
 
         return resp.ok
 
     def _put_legacy_manifest(self, manifest: ManifestSchema1):
         """put the docker schema 1 manifest with signed signature to the repository"""
-        url = URLBuilder.build_manifests_url(self.client.api_base_url, self.repo, self.reference)
+        url = URLBuilder.build_manifests_url(
+            self.client.api_base_url, self.repo, self.reference
+        )
         private_key = get_private_key()
         data = manifest.json(
             include={
                 "name",
                 "tag",
                 "architecture",
                 "fsLayers",
                 "history",
                 "schemaVersion",
-            }
+            },
         )
         js = libtrust.JSONSignature.new(data)
         js.sign(private_key)
 
         headers = {"Content-Type": manifest.content_type()}
         data = js.to_pretty_signature("signatures")
-        return self.client.put(url=url, data=data, headers=headers, timeout=self.timeout)
+        return self.client.put(
+            url=url, data=data, headers=headers, timeout=self.timeout
+        )
 
     def _put_new_manifest(self, manifest: Union[ManifestSchema2, OCIManifestSchema1]):
         """put the docker schema 2 manifest or OCI manifest to the repository"""
-        url = URLBuilder.build_manifests_url(self.client.api_base_url, self.repo, self.reference)
+        url = URLBuilder.build_manifests_url(
+            self.client.api_base_url, self.repo, self.reference
+        )
         headers = {"Content-Type": manifest.content_type()}
-        data = manifest.json()
-        return self.client.put(url=url, data=data, headers=headers, timeout=self.timeout)
+        data = manifest.json(
+            exclude={
+                "config": {"urls"},
+                "layers": {"__all__": {"urls"}},
+            }
+        )
+        return self.client.put(
+            url=url, data=data, headers=headers, timeout=self.timeout
+        )
```

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/resources/tags.py` & `moby_distribution-0.8.2/moby_distribution/registry/resources/tags.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/registry/utils.py` & `moby_distribution-0.8.2/moby_distribution/registry/utils.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/spec/auth.py` & `moby_distribution-0.8.2/moby_distribution/spec/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/spec/base.py` & `moby_distribution-0.8.2/moby_distribution/spec/base.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/spec/endpoint.py` & `moby_distribution-0.8.2/moby_distribution/spec/endpoint.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/spec/image_json.py` & `moby_distribution-0.8.2/moby_distribution/spec/image_json.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/moby_distribution/spec/manifest.py` & `moby_distribution-0.8.2/moby_distribution/spec/manifest.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.8.1/pyproject.toml` & `moby_distribution-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moby-distribution"
-version = "0.8.1"
+version = "0.8.2"
 description = "Yet another moby(docker) distribution implement by python."
 authors = ["shabbywu <shabbywu@qq.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/distribution"
 homepage = "https://github.com/shabbywu/distribution"
```

### Comparing `moby_distribution-0.8.1/PKG-INFO` & `moby_distribution-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moby-distribution
-Version: 0.8.1
+Version: 0.8.2
 Summary: Yet another moby(docker) distribution implement by python.
 Home-page: https://github.com/shabbywu/distribution
 License: Apache-2.0
 Author: shabbywu
 Author-email: shabbywu@qq.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

