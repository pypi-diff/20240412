# Comparing `tmp/pyEscoAPI-0.0.4.tar.gz` & `tmp/pyescoapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEscoAPI-0.0.4.tar", last modified: Wed Apr 10 15:30:17 2024, max compression
+gzip compressed data, was "pyescoapi-0.0.7.tar", last modified: Fri Apr 12 18:02:26 2024, max compression
```

## Comparing `pyEscoAPI-0.0.4.tar` & `pyescoapi-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 15:30:17.618946 pyEscoAPI-0.0.4/
--rw-rw-rw-   0        0        0      514 2024-04-10 15:30:17.617945 pyEscoAPI-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       41 2024-04-10 15:22:40.000000 pyEscoAPI-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 15:30:17.605359 pyEscoAPI-0.0.4/pyEscoAPI/
--rw-rw-rw-   0        0        0      115 2024-04-10 15:22:40.000000 pyEscoAPI-0.0.4/pyEscoAPI/__init__.py
--rw-rw-rw-   0        0        0    23188 2024-04-10 15:22:40.000000 pyEscoAPI-0.0.4/pyEscoAPI/esco_api.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:30:17.617945 pyEscoAPI-0.0.4/pyEscoAPI.egg-info/
--rw-rw-rw-   0        0        0      514 2024-04-10 15:30:17.000000 pyEscoAPI-0.0.4/pyEscoAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-04-10 15:30:17.000000 pyEscoAPI-0.0.4/pyEscoAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 15:30:17.000000 pyEscoAPI-0.0.4/pyEscoAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 15:30:17.000000 pyEscoAPI-0.0.4/pyEscoAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-10 15:30:17.000000 pyEscoAPI-0.0.4/pyEscoAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2024-04-10 15:22:40.000000 pyEscoAPI-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 15:30:17.618946 pyEscoAPI-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 15:30:17.616945 pyEscoAPI-0.0.4/tests/
--rw-rw-rw-   0        0        0     4400 2024-04-10 15:22:40.000000 pyEscoAPI-0.0.4/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:02:26.009519 pyescoapi-0.0.7/
+-rw-rw-rw-   0        0        0      514 2024-04-12 18:02:26.008518 pyescoapi-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2024-04-10 15:22:40.000000 pyescoapi-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 18:02:25.964505 pyescoapi-0.0.7/pyEscoAPI/
+-rw-rw-rw-   0        0        0      115 2024-04-10 15:22:40.000000 pyescoapi-0.0.7/pyEscoAPI/__init__.py
+-rw-rw-rw-   0        0        0     5849 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/pyEscoAPI/dataclasses.py
+-rw-rw-rw-   0        0        0    78222 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/pyEscoAPI/esco_api.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:02:26.006511 pyescoapi-0.0.7/pyEscoAPI.egg-info/
+-rw-rw-rw-   0        0        0      514 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 18:02:25.000000 pyescoapi-0.0.7/pyEscoAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 18:02:26.009519 pyescoapi-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 18:02:26.005006 pyescoapi-0.0.7/tests/
+-rw-rw-rw-   0        0        0     6346 2024-04-12 18:00:25.000000 pyescoapi-0.0.7/tests/test_client.py
```

### Comparing `pyEscoAPI-0.0.4/PKG-INFO` & `pyescoapi-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEscoAPI
-Version: 0.0.4
+Version: 0.0.7
 Summary: Python client for Esco API (Esco bolsa)
 Author-email: Codetria <hola@codetria.com>
 License: MIT License
 Keywords: Esco,API,bolsa,client,market,provider
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyEscoAPI-0.0.4/pyEscoAPI.egg-info/PKG-INFO` & `pyescoapi-0.0.7/pyEscoAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEscoAPI
-Version: 0.0.4
+Version: 0.0.7
 Summary: Python client for Esco API (Esco bolsa)
 Author-email: Codetria <hola@codetria.com>
 License: MIT License
 Keywords: Esco,API,bolsa,client,market,provider
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyEscoAPI-0.0.4/pyproject.toml` & `pyescoapi-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyEscoAPI'
-version = "0.0.4"
+version = "0.0.7"
 license = {text = "MIT License"}
 authors = [
   { name="Codetria", email="hola@codetria.com" },
 ]
 dependencies = [
     "requests==2.31.0"
 ]
```

### Comparing `pyEscoAPI-0.0.4/tests/test_client.py` & `pyescoapi-0.0.7/tests/test_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,21 @@
 def test_get_disponible_mon(api_client):
     cuenta = "351008539"
     result = api_client.get_disponible_mon(cuenta=cuenta)
     assert result[0]["orden"] == 0
     assert result[0]["simbolo"] == "ARS"
 
 
+def test_get_disponible_mon_list(api_client):
+    cuenta = "172885"
+    result = api_client.get_disponible_mon_list(cuentas=cuenta)
+    assert result[0]["orden"] == 0
+    assert result[0]["simbolo"] == "$"
+
+
 def test_get_tenencia_val(api_client):
     cuenta = "351008539"
     result = api_client.get_tenencia_val(cuenta=cuenta)
     assert result[0]["grupo"] == "MON"
     assert result[0]["abreviatura"] == "ARS"
 
 
@@ -149,7 +156,77 @@
     assert len(result) > 0
 
 
 def test_get_persona(api_client):
     dni = 7638787
     result = api_client.get_persona(num_doc=dni)
     assert int(result["numDoc"]) == dni
+
+
+def test_insert_orden_compra(api_client):
+    cuenta = "351011960"
+    result = api_client.insert_orden_compra(
+        instrumento_abreviatura="COME",
+        cuenta=cuenta,
+        cantidad=1
+    )
+    assert "codOperacion" in result
+
+
+def test_insert_orden_venta(api_client):
+    cuenta = "351011960"
+    result = api_client.insert_orden_compra(
+        instrumento_abreviatura="GNCXO",
+        cuenta=cuenta,
+        cantidad=1
+    )
+    assert "codOperacion" in result
+
+
+def test_insert_suscripcion_fci(api_client):
+    cuenta = "351011960"
+    result = api_client.insert_solicitud_suscripcion_fci(
+        fondo="COGRLMF AR",
+        cuenta=cuenta,
+        importe=1000
+    )
+    assert "codSolicitudFdo" in result
+
+
+def test_get_boletos(api_client):
+    result = api_client.get_boletos()
+    assert len(result) > 0
+    assert "idBoleto" in result[0]
+
+
+def test_get_estado_orden(api_client):
+    result = api_client.get_estado_orden(47089)
+    assert result[0]["indice"] == 0
+
+
+def test_get_ordenes(api_client):
+    result = api_client.get_ordenes()
+    assert "codOrden" in result[0]
+
+
+def test_get_liquidaciones(api_client):
+    result = api_client.get_liquidaciones_fondos()
+    assert len(result) > 0
+    assert "numSolicitud" in result[0]
+
+
+def test_get_solicitudes_fci(api_client):
+    result = api_client.get_solicitudes_fondos()
+    assert len(result) > 0
+    assert "numSolicitud" in result["data"][0]
+
+
+def test_preview_orden_compra(api_client):
+    cuenta = "351011960"
+    result = api_client.previsualizar_orden_compra(
+        instrumento_abreviatura="COME",
+        cuenta=cuenta,
+        cantidad=1
+    )
+    assert "precio" in result
+
+
```

