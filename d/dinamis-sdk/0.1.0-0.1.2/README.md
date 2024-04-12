# Comparing `tmp/dinamis-sdk-0.1.0.tar.gz` & `tmp/dinamis-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinamis-sdk-0.1.0.tar", last modified: Sun Feb 18 13:54:12 2024, max compression
+gzip compressed data, was "dinamis-sdk-0.1.2.tar", last modified: Fri Apr 12 08:47:37 2024, max compression
```

## Comparing `dinamis-sdk-0.1.0.tar` & `dinamis-sdk-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      391 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.491108 dinamis-sdk-0.1.0/dinamis_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8089 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.491108 dinamis-sdk-0.1.0/dinamis_sdk/examples/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_ndvi_loss.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_toa_mosaic.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/dinamis_sdk/examples/rio_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    17394 2024-02-15 14:06:09.000000 dinamis-sdk-0.1.0/dinamis_sdk/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2024-02-15 14:06:09.000000 dinamis-sdk-0.1.0/dinamis_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      391 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       80 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-02-18 13:54:12.000000 dinamis-sdk-0.1.0/dinamis_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-02-18 13:48:22.000000 dinamis-sdk-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 13:54:12.495108 dinamis-sdk-0.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/tests/test_spot-6-7-drs.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-11-09 10:35:42.000000 dinamis-sdk-0.1.0/tests/test_super-s2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:47:37.773682 dinamis-sdk-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      391 2024-04-12 08:47:37.773682 dinamis-sdk-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:47:37.753682 dinamis-sdk-0.1.2/dinamis_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8763 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:47:37.773682 dinamis-sdk-0.1.2/dinamis_sdk/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/examples/pyotb_ndvi_loss.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/examples/pyotb_toa_mosaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/examples/rio_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    17394 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/dinamis_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:47:37.773682 dinamis-sdk-0.1.2/dinamis_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      391 2024-04-12 08:47:37.000000 dinamis-sdk-0.1.2/dinamis_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-04-12 08:47:37.000000 dinamis-sdk-0.1.2/dinamis_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 08:47:37.000000 dinamis-sdk-0.1.2/dinamis_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 08:47:37.000000 dinamis-sdk-0.1.2/dinamis_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-12 08:47:37.000000 dinamis-sdk-0.1.2/dinamis_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-12 08:47:37.000000 dinamis-sdk-0.1.2/dinamis_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 08:47:37.773682 dinamis-sdk-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:47:37.773682 dinamis-sdk-0.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/tests/test_spot-6-7-drs.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-12 08:36:53.000000 dinamis-sdk-0.1.2/tests/test_super-s2.py
```

### Comparing `dinamis-sdk-0.1.0/LICENSE` & `dinamis-sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.0/README.md` & `dinamis-sdk-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # DINAMIS SDK
 
 <br>
-<a href="https://gitlab.irstea.fr/dinamis/dinamis-sdk/-/releases">
-<img src="https://gitlab.irstea.fr/dinamis/dinamis-sdk/-/badges/release.svg">
+<a href="https://forgemia.inra.fr/cdos-pub/dinamis-sdk/-/releases">
+<img src="https://forgemia.inra.fr/cdos-pub/dinamis-sdk/-/badges/release.svg">
 </a>
-<a href="https://gitlab.irstea.fr/dinamis/dinamis-sdk/-/commits/main">
-<img src="https://gitlab.irstea.fr/dinamis/dinamis-sdk/badges/main/pipeline.svg">
+<a href="https://forgemia.inra.fr/cdos-pub/dinamis-sdk/-/commits/main">
+<img src="https://forgemia.inra.fr/cdos-pub/dinamis-sdk/badges/main/pipeline.svg">
 </a>
 <a href="LICENSE">
 <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
 </a>
 
 Largely inspired from *Microsoft Planetary Computer SDK*, **Dinamis-SDK** is 
-built on the STAC ecosystem and provides easy access to open-data Spot-6/7 
-imagery in COG format.
+built on the STAC ecosystem to provide an easy access to remote sensing imagery
+and thematic products of the **THEIA/DINAMIS data center of Montpellier**.
 
 ```python
 import dinamis_sdk
 import pystac_client
 
 api = pystac_client.Client.open(
-   'https://stacapi-dinamis.apps.okd.crocc.meso.umontpellier.fr',
+   'https://stacapi-cdos.apps.okd.crocc.meso.umontpellier.fr',
    modifier=dinamis_sdk.sign_inplace,
 )
 ```
 
 For more information read the 
-[documentation](https://dinamis.gitlab.irstea.page/dinamis-sdk).
+[documentation](https://cdos-pub.pages.mia.inra.fr/dinamis-sdk).
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # DINAMIS SDK
-_[_h_t_t_p_s_:_/_/_g_i_t_l_a_b_._i_r_s_t_e_a_._f_r_/_d_i_n_a_m_i_s_/_d_i_n_a_m_i_s_-_s_d_k_/_-_/_b_a_d_g_e_s_/_r_e_l_e_a_s_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
-_g_i_t_l_a_b_._i_r_s_t_e_a_._f_r_/_d_i_n_a_m_i_s_/_d_i_n_a_m_i_s_-_s_d_k_/_b_a_d_g_e_s_/_m_a_i_n_/_p_i_p_e_l_i_n_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
+_[_h_t_t_p_s_:_/_/_f_o_r_g_e_m_i_a_._i_n_r_a_._f_r_/_c_d_o_s_-_p_u_b_/_d_i_n_a_m_i_s_-_s_d_k_/_-_/_b_a_d_g_e_s_/_r_e_l_e_a_s_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
+_f_o_r_g_e_m_i_a_._i_n_r_a_._f_r_/_c_d_o_s_-_p_u_b_/_d_i_n_a_m_i_s_-_s_d_k_/_b_a_d_g_e_s_/_m_a_i_n_/_p_i_p_e_l_i_n_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]Largely inspired from
 *Microsoft Planetary Computer SDK*, **Dinamis-SDK** is built on the STAC
-ecosystem and provides easy access to open-data Spot-6/7 imagery in COG format.
-```python import dinamis_sdk import pystac_client api =
-pystac_client.Client.open( 'https://stacapi-
-dinamis.apps.okd.crocc.meso.umontpellier.fr',
+ecosystem to provide an easy access to remote sensing imagery and thematic
+products of the **THEIA/DINAMIS data center of Montpellier**. ```python import
+dinamis_sdk import pystac_client api = pystac_client.Client.open( 'https://
+stacapi-cdos.apps.okd.crocc.meso.umontpellier.fr',
 modifier=dinamis_sdk.sign_inplace, ) ``` For more information read the
-[documentation](https://dinamis.gitlab.irstea.page/dinamis-sdk).
+[documentation](https://cdos-pub.pages.mia.inra.fr/dinamis-sdk).
```

### Comparing `dinamis-sdk-0.1.0/dinamis_sdk/auth.py` & `dinamis-sdk-0.1.2/dinamis_sdk/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import time
 from abc import abstractmethod
 from typing import Dict
 import requests
 from pydantic import BaseModel, Field  # pylint: disable = no-name-in-module
 import qrcode
-from .utils import log, JWT_FILE, TOKEN_ENDPOINT, AUTH_BASE_URL
+from .utils import log, JWT_FILE, TOKEN_ENDPOINT, AUTH_BASE_URL, TOKEN_SERVER
 
 
 class JWT(BaseModel):  # pylint: disable = R0903
     """JWT model."""
 
     access_token: str = Field(alias="access_token")
     expires_in: int = Field(alias="expires_in")
@@ -244,15 +244,33 @@
                 self.save_token(datetime.datetime.now())
 
         self.refresh_if_needed()
 
         return self.jwt.access_token
 
 
-session = OAuth2Session()
+class TokenServer:
+    def __init__(endpoint: str):
+        session = requests.Session()
+        retry = urllib3.util.retry.Retry(
+            total=total_retry,
+            backoff_factor=backoff_factor,
+            status_forcelist=[404, 429, 500, 502, 503, 504],
+        )
+        adapter = requests.adapters.HTTPAdapter(max_retries=retry)
+        session.mount("https://", adapter)
+        session.mount("http://", adapter)
+        self.endpoint = endpoint
+        log.info("Using Token Server: %s", endpoint)
+
+    def get_access_token() -> str:
+        return session.get(self.endpoint, timeout=10).json()
+
+
+session = TokenServer(TOKEN_SERVER) if TOKEN_SERVER else OAuth2Session()
 
 
 def _get_access_token():
     return session.get_access_token()
 
 
 get_access_token = _get_access_token
```

### Comparing `dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_ndvi_loss.py` & `dinamis-sdk-0.1.2/dinamis_sdk/examples/pyotb_ndvi_loss.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.0/dinamis_sdk/examples/pyotb_toa_mosaic.py` & `dinamis-sdk-0.1.2/dinamis_sdk/examples/pyotb_toa_mosaic.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.0/dinamis_sdk/examples/rio_metadata.py` & `dinamis-sdk-0.1.2/dinamis_sdk/examples/rio_metadata.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.0/dinamis_sdk/s3.py` & `dinamis-sdk-0.1.2/dinamis_sdk/s3.py`

 * *Files identical despite different names*

### Comparing `dinamis-sdk-0.1.0/dinamis_sdk/utils.py` & `dinamis-sdk-0.1.2/dinamis_sdk/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,26 @@
     val = os.environ.get(env_var_name)
     if val:
         if val.isdigit():
             return int(val)
     return None
 
 # Signed TTL margin default to 1800 seconds (30 minutes), or env. var.
-ttl_margin_from_env = _get_seconds("DINAMIS_SDK_TTL_MARGIN")
-log.info(
-    "Setting TTL margin from environment variable to %s seconds",
-    ttl_margin_from_env
-)
+if (ttl_margin_from_env := _get_seconds("DINAMIS_SDK_TTL_MARGIN")):
+    log.info(
+        "Setting TTL margin from environment variable to %s seconds",
+        ttl_margin_from_env
+    )
 SIGNED_URL_TTL_MARGIN = ttl_margin_from_env or 1800
 
-SIGNED_URL_DURATION_SECONDS = _get_seconds("DINAMIS_SDK_DURATION_SECONDS")
-log.info(
-    "Setting duration seconds from environment variable to %s seconds",
-    SIGNED_URL_DURATION_SECONDS
-)
+if (SIGNED_URL_DURATION_SECONDS := _get_seconds("DINAMIS_SDK_DURATION_SECONDS")):
+    log.info(
+        "Setting duration seconds from environment variable to %s seconds",
+        SIGNED_URL_DURATION_SECONDS
+    )
 
 MAX_URLS = 64
 S3_STORAGE_DOMAIN = "meso.umontpellier.fr"
 S3_SIGNING_ENDPOINT = \
     "https://s3-signing-cdos.apps.okd.crocc.meso.umontpellier.fr/"
 
 CFG_PTH = appdirs.user_config_dir(appname='dinamis_sdk_auth')
@@ -85,7 +85,10 @@
 
 # Token endpoint is typically something like: https://keycloak-dinamis.apps.okd
 # .crocc.meso.umontpellier.fr/auth/realms/dinamis/protocol/openid-connect/token
 TOKEN_ENDPOINT = retrieve_token_endpoint()
 # Auth base URL is typically something like: https://keycloak-dinamis.apps.okd.
 # crocc.meso.umontpellier.fr/auth/realms/dinamis/protocol/openid-connect
 AUTH_BASE_URL = TOKEN_ENDPOINT.rsplit('/', 1)[0]
+
+# Token server (optional)
+TOKEN_SERVER = os.environ.get("DINAMIS_SDK_TOKEN_SERVER")
```

### Comparing `dinamis-sdk-0.1.0/dinamis_sdk.egg-info/SOURCES.txt` & `dinamis-sdk-0.1.2/dinamis_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

