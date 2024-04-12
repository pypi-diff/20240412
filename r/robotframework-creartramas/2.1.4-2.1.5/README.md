# Comparing `tmp/robotframework_creartramas-2.1.4.tar.gz` & `tmp/robotframework_creartramas-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_creartramas-2.1.4.tar", max compression
+gzip compressed data, was "robotframework_creartramas-2.1.5.tar", max compression
```

## Comparing `robotframework_creartramas-2.1.4.tar` & `robotframework_creartramas-2.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.4/docs/README.md
--rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.4/LICENSE
--rw-r--r--   0        0        0      670 2024-04-10 09:36:30.016780 robotframework_creartramas-2.1.4/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.4/TRAMAS/__init__.py
--rw-r--r--   0        0        0     2033 2024-04-10 09:36:34.055496 robotframework_creartramas-2.1.4/TRAMAS/creartramas.py
--rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.5/docs/README.md
+-rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.5/LICENSE
+-rw-r--r--   0        0        0      670 2024-04-11 07:27:06.795620 robotframework_creartramas-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.5/TRAMAS/__init__.py
+-rw-r--r--   0        0        0     2480 2024-04-11 07:28:33.011479 robotframework_creartramas-2.1.5/TRAMAS/creartramas.py
+-rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.5/PKG-INFO
```

### Comparing `robotframework_creartramas-2.1.4/docs/README.md` & `robotframework_creartramas-2.1.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.4/LICENSE` & `robotframework_creartramas-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.4/pyproject.toml` & `robotframework_creartramas-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robotframework-creartramas"
-version = "2.1.4"
+version = "2.1.5"
 description = "Creacion de tramas en hexadecimal"
 license = "Apache-2.0"
 authors = ["Anthony Arevalo"]
 maintainers = ["Anthony Arevalo"]
 readme = "./docs/README.md"
 homepage = "https://pypi.org/project/robotframework-creartramas"
 packages = [
```

### Comparing `robotframework_creartramas-2.1.4/TRAMAS/creartramas.py` & `robotframework_creartramas-2.1.5/TRAMAS/creartramas.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,21 +22,32 @@
     def crear_trama(self,direccion_destino, numero_bits, direccion_origen, comando, datos):
         """
         Esta función construye una trama de acuerdo con la estructura proporcionada.Tiene 5 argumentos
         Hay que tener en cuenta que los datos que se introducen deben estar en formate hexadecimal 0XAB.
         También a la hora de introducir datos, estso deben estar en forma de lista datos=[0x00,0x00,..]
         Finalmente, se devuelve la trama creada.
         """
-        # Construir la trama en forma de bytearray (valores en codigo ASCII)
+        # Convertir cadenas de texto a bytes en formato hexadecimal
+        direccion_destino_bytes = bytes.fromhex(direccion_destino)
+        numero_bits_bytes = bytes.fromhex(numero_bits)
+        direccion_origen_bytes = bytes.fromhex(direccion_origen)
+        comando_bytes = bytes.fromhex(comando)
+        datos_bytes = [bytes.fromhex(dato) for dato in datos]
+    
+        # Construir la trama en forma de bytearray (valores en código ASCII)
         trama = bytearray()
-        trama.append(int.from_bytes(direccion_destino, 'big'))
-        trama.append(int.from_bytes(numero_bits, 'big'))
-        trama.append(int.from_bytes(direccion_origen, 'big'))
-        trama.append(int.from_bytes(comando, 'big'))
+        trama.append(int.from_bytes(direccion_destino_bytes, 'big'))
+        trama.append(int.from_bytes(numero_bits_bytes, 'big'))
+        trama.append(int.from_bytes(direccion_origen_bytes, 'big'))
+        trama.append(int.from_bytes(comando_bytes, 'big'))
+        
         # Agregar los datos a la trama
-        for dato in datos:
+        for dato in datos_bytes:
             trama.append(int.from_bytes(dato, 'big'))
+        
         # Calcular el checksum
         checksum = calcular_checksum(trama)
+        
         # Añadir el checksum a la trama
         trama.append(checksum)
+        
         return trama
```

### Comparing `robotframework_creartramas-2.1.4/PKG-INFO` & `robotframework_creartramas-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-creartramas
-Version: 2.1.4
+Version: 2.1.5
 Summary: Creacion de tramas en hexadecimal
 Home-page: https://pypi.org/project/robotframework-creartramas
 License: Apache-2.0
 Author: Anthony Arevalo
 Maintainer: Anthony Arevalo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

