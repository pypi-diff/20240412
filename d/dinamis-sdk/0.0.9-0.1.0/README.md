# Comparing `tmp/dinamis-sdk-0.0.9.tar.gz` & `tmp/dinamis-sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinamis-sdk-0.0.9.tar", last modified: Wed May 24 07:21:08 2023, max compression
+gzip compressed data, was "dinamis-sdk-0.1.0.tar", last modified: Sun Feb 18 13:54:12 2024, max compression
```

## Comparing `dinamis-sdk-0.0.9.tar` & `dinamis-sdk-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:08.001575 dinamis-sdk-0.0.9/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2023-02-22 11:50:47.000000 dinamis-sdk-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 07:21:08.001575 dinamis-sdk-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-03-28 12:19:28.000000 dinamis-sdk-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:07.993574 dinamis-sdk-0.0.9/dinamis_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.9/dinamis_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8267 2023-03-28 09:22:01.000000 dinamis-sdk-0.0.9/dinamis_sdk/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:07.997574 dinamis-sdk-0.0.9/dinamis_sdk/examples/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 13:55:36.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_ndvi_loss.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-11 10:48:18.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_toa_mosaic.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-03-30 14:16:11.000000 dinamis-sdk-0.0.9/dinamis_sdk/examples/rio_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    16374 2023-05-24 07:16:26.000000 dinamis-sdk-0.0.9/dinamis_sdk/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-03 18:03:30.000000 dinamis-sdk-0.0.9/dinamis_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:21:07.997574 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-24 07:21:07.000000 dinamis-sdk-0.0.9/dinamis_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 07:21:08.001575 dinamis-sdk-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-24 07:12:42.000000 dinamis-sdk-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      391 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.491108 dinamis-sdk-0.1.0/dinamis_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8089 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.491108 dinamis-sdk-0.1.0/dinamis_sdk/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_ndvi_loss.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_toa_mosaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/rio_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    17394 2024-02-15 14:06:09.000000 dinamis-sdk-0.1.0/dinamis_sdk/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2024-02-15 14:06:09.000000 dinamis-sdk-0.1.0/dinamis_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      391 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       80 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-02-18 13:48:22.000000 dinamis-sdk-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/tests/test_spot-6-7-drs.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/tests/test_super-s2.py
```

### Comparing `dinamis-sdk-0.0.9/LICENSE` & `dinamis-sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.9/README.md` & `dinamis-sdk-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <img src="https://gitlab.irstea.fr/dinamis/dinamis-sdk/badges/main/pipeline.svg">
 </a>
 <a href="LICENSE">
 <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
 </a>
 
 Largely inspired from *Microsoft Planetary Computer SDK*, **Dinamis-SDK** is 
-built on the STAC ecosystem and provides easy access to open-date Spot-6/7 
+built on the STAC ecosystem and provides easy access to open-data Spot-6/7 
 imagery in COG format.
 
 ```python
 import dinamis_sdk
 import pystac_client
 
 api = pystac_client.Client.open(
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # DINAMIS SDK
 _[_h_t_t_p_s_:_/_/_g_i_t_l_a_b_._i_r_s_t_e_a_._f_r_/_d_i_n_a_m_i_s_/_d_i_n_a_m_i_s_-_s_d_k_/_-_/_b_a_d_g_e_s_/_r_e_l_e_a_s_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _g_i_t_l_a_b_._i_r_s_t_e_a_._f_r_/_d_i_n_a_m_i_s_/_d_i_n_a_m_i_s_-_s_d_k_/_b_a_d_g_e_s_/_m_a_i_n_/_p_i_p_e_l_i_n_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]Largely inspired from
 *Microsoft Planetary Computer SDK*, **Dinamis-SDK** is built on the STAC
-ecosystem and provides easy access to open-date Spot-6/7 imagery in COG format.
+ecosystem and provides easy access to open-data Spot-6/7 imagery in COG format.
 ```python import dinamis_sdk import pystac_client api =
 pystac_client.Client.open( 'https://stacapi-
 dinamis.apps.okd.crocc.meso.umontpellier.fr',
 modifier=dinamis_sdk.sign_inplace, ) ``` For more information read the
 [documentation](https://dinamis.gitlab.irstea.page/dinamis-sdk).
```

### Comparing `dinamis-sdk-0.0.9/dinamis_sdk/auth.py` & `dinamis-sdk-0.1.0/dinamis_sdk/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import time
 from abc import abstractmethod
 from typing import Dict
 import requests
 from pydantic import BaseModel, Field  # pylint: disable = no-name-in-module
 import qrcode
-from .utils import log, JWT_FILE
+from .utils import log, JWT_FILE, TOKEN_ENDPOINT, AUTH_BASE_URL
 
 
 class JWT(BaseModel):  # pylint: disable = R0903
     """JWT model."""
 
     access_token: str = Field(alias="access_token")
     expires_in: int = Field(alias="expires_in")
@@ -33,20 +33,17 @@
 
 class GrantMethodBase:
     """Base class for grant methods."""
 
     headers: Dict[str, str] = {
         "Content-Type": "application/x-www-form-urlencoded"
     }
-    keycloak_server_url = "https://keycloak-dinamis.apps.okd.crocc.meso." \
-                          "umontpellier.fr/auth"
+    token_endpoint = TOKEN_ENDPOINT
+    base_url = AUTH_BASE_URL
     keycloak_realm = "dinamis"
-    base_url = f"{keycloak_server_url}/realms/{keycloak_realm}/" \
-               "protocol/openid-connect"
-    token_endpoint = f"{base_url}/token"
     client_id: str
 
     @abstractmethod
     def get_first_token(self) -> JWT:
         """
         Provide the first used token.
```

### Comparing `dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_ndvi_loss.py` & `dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_ndvi_loss.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.9/dinamis_sdk/examples/pyotb_toa_mosaic.py` & `dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_toa_mosaic.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.9/dinamis_sdk/examples/rio_metadata.py` & `dinamis-sdk-0.1.0/dinamis_sdk/examples/rio_metadata.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.0.9/dinamis_sdk/s3.py` & `dinamis-sdk-0.1.0/dinamis_sdk/s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 import re
 import time
 from copy import deepcopy
 from datetime import datetime, timezone
 from functools import singledispatch
 from typing import Any, Dict, Mapping, TypeVar, cast, List
 from urllib.parse import urlparse, parse_qs
+import math
 import urllib3.util.retry
 import requests
 import requests.adapters
 from pydantic import BaseModel, Field  # pylint: disable = no-name-in-module
 from pystac import Asset, Item, ItemCollection, STACObjectType, Collection
 from pystac.serialization.identify import identify_stac_object_type
 from pystac.utils import datetime_to_str
 import pystac_client
 from pystac_client import ItemSearch
+import packaging.version
+import pydantic
 
-from .utils import log, SIGNED_URL_TTL_MARGIN, CREDENTIALS
+from .utils import log, SIGNED_URL_TTL_MARGIN, CREDENTIALS, MAX_URLS, \
+    S3_SIGNING_ENDPOINT, S3_STORAGE_DOMAIN, SIGNED_URL_DURATION_SECONDS
 
-S3_STORAGE_DOMAIN = "minio-api-dinamis.apps.okd.crocc.meso.umontpellier.fr"
-S3_SIGNING_ENDPOINT = \
-    "https://s3-signing-dinamis.apps.okd.crocc.meso.umontpellier.fr/"
+_PYDANTIC_2_0 = packaging.version.parse(
+    pydantic.__version__
+) >= packaging.version.parse("2.0.0")
 
 AssetLike = TypeVar("AssetLike", Asset, Dict[str, Any])
 
 asset_xpr = re.compile(
     r"https://(?P<account>[A-z0-9]+?)"
     r"\.minio-dinamis\.apps\.okd\.crocc\.meso\.umontpellier\.fr/"
     r"(?P<container>.+?)"
@@ -43,16 +47,19 @@
     """Base model for responses."""
 
     expiry: datetime = Field(alias="expiry")
 
     class Config:  # pylint: disable = R0903
         """Config for URLBase model."""
 
-        json_encoders = {datetime: datetime_to_str}
-        allow_population_by_field_name = True
+        if _PYDANTIC_2_0:
+            populate_by_name = True
+        else:
+            allow_population_by_field_name = True
+            json_encoders = {datetime: datetime_to_str}
 
 
 class SignedURL(URLBase):  # pylint: disable = R0903
     """Signed URL response."""
 
     href: str = Field(alias="href")
 
@@ -467,36 +474,53 @@
             backoff_factor=retry_backoff_factor,
             status_forcelist=[404, 429, 500, 502, 503, 504],
             allowed_methods=False,
         )
         adapter = requests.adapters.HTTPAdapter(max_retries=retry)
         session.mount("http://", adapter)
         session.mount("https://", adapter)
-        response = session.post(
-            f"{S3_SIGNING_ENDPOINT}sign_urls",
-            params={"urls": not_signed_urls},
-            headers=headers
-        )
-        response.raise_for_status()
-
-        signed_url_batch = SignedURLBatch(**response.json())
-        if not signed_url_batch:
-            raise ValueError(
-                f"No signed url batch found in response: {response.json()}"
+        n_urls = len(not_signed_urls)
+        log.debug("Number of URLs to sign: %s", n_urls)
+        n_chunks = math.ceil(n_urls / MAX_URLS)
+        log.debug("Number of chunks of URLs to sign: %s", n_chunks)
+        for i_chunk in range(n_chunks):
+            log.debug("Processing chunk %s/%s", i_chunk + 1, n_chunks)
+            chunk_start = i_chunk * MAX_URLS
+            chunk_end = min(chunk_start + MAX_URLS, n_urls)
+            not_signed_urls_chunk = not_signed_urls[chunk_start:chunk_end]
+            params={"urls": not_signed_urls_chunk}
+            if SIGNED_URL_DURATION_SECONDS:
+                params.update({"duration_seconds": SIGNED_URL_DURATION_SECONDS})
+            response = session.post(
+                f"{S3_SIGNING_ENDPOINT}sign_urls",
+                params=params,
+                headers=headers,
+                timeout=10
             )
-        if not all(key in signed_url_batch.hrefs
-                   for key in not_signed_urls):
-            raise ValueError(
-                f"URLs to sign are {not_signed_urls} but returned signed URLs"
-                f"are for {signed_url_batch.hrefs.keys()}"
-            )
-        for url, href in signed_url_batch.hrefs.items():
-            signed_url = SignedURL(expiry=signed_url_batch.expiry, href=href)
-            CACHE[url] = signed_url
-            signed_urls[url] = signed_url
+            response.raise_for_status()
+
+            signed_url_batch = SignedURLBatch(**response.json())
+            if not signed_url_batch:
+                raise ValueError(
+                    f"No signed url batch found in response: {response.json()}"
+                )
+            if not all(key in signed_url_batch.hrefs
+                       for key in not_signed_urls_chunk):
+                raise ValueError(
+                    f"URLs to sign are {not_signed_urls_chunk} but returned "
+                    f"signed URLs"
+                    f"are for {signed_url_batch.hrefs.keys()}"
+                )
+            for url, href in signed_url_batch.hrefs.items():
+                signed_url = SignedURL(
+                    expiry=signed_url_batch.expiry,
+                    href=href
+                )
+                CACHE[url] = signed_url
+                signed_urls[url] = signed_url
         log.debug(
             "Got signed urls %s in %s seconds",
             signed_urls,
             f"{time.time() - start_time:.2f}"
         )
 
     return signed_urls
```

