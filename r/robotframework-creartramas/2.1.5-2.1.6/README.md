# Comparing `tmp/robotframework_creartramas-2.1.5.tar.gz` & `tmp/robotframework_creartramas-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_creartramas-2.1.5.tar", max compression
+gzip compressed data, was "robotframework_creartramas-2.1.6.tar", max compression
```

## Comparing `robotframework_creartramas-2.1.5.tar` & `robotframework_creartramas-2.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2048 2024-03-20 10:52:17.764687 robotframework_creartramas-2.1.5/docs/README.md
--rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.5/LICENSE
--rw-r--r--   0        0        0      670 2024-04-11 07:27:06.795620 robotframework_creartramas-2.1.5/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.5/TRAMAS/__init__.py
--rw-r--r--   0        0        0     2480 2024-04-11 07:28:33.011479 robotframework_creartramas-2.1.5/TRAMAS/creartramas.py
--rw-r--r--   0        0        0     2803 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1946 2024-04-12 07:24:28.683559 robotframework_creartramas-2.1.6/docs/README.md
+-rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.6/LICENSE
+-rw-r--r--   0        0        0      670 2024-04-12 07:06:49.031668 robotframework_creartramas-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.6/TRAMAS/__init__.py
+-rw-r--r--   0        0        0     2757 2024-04-12 07:23:55.514784 robotframework_creartramas-2.1.6/TRAMAS/creartramas.py
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.6/PKG-INFO
```

### Comparing `robotframework_creartramas-2.1.5/docs/README.md` & `robotframework_creartramas-2.1.6/docs/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,54 +7,54 @@
 Antes de usar esta librería, asegurate de tener instalado lo siguuiente:
 - Python > 3.8
 - Robot Framework
 - pip (para instalar libreria)
 
 ## Instalación
 Puedes instalar esta librería a través de pip:
-* ` pip install --upgrade robotframework-creartramas`
+* ` pip install robotframework-creartramas`
 
 ## Uso 
 
 ``` RobotFramework
 
  Aquí tienes un ejemplo de cómo crear una trama utilizando esta librería:
 
 *** Settings ***
-Library    mi_libreria_de_tramas.TRAMAS
+Library    TRAMAS
 
 *** Test Cases ***
 Crear y enviar trama
-    ${direccion_origen}=    Set Variable    0x01
-    ${direccion_destino}=    Set Variable    0x02
-    ${numero_bits}=    Set Variable    0x08
-    ${comando}=    Set Variable    0xFE
-    ${datos}=    Create List    0x41    0x5A    0x4B
+    ${direccion_origen}=    01
+    ${direccion_destino}=   02
+    ${numero_bytes}=         08
+    ${comando}=             FE
+    @{datos}=               0x41    0x5A    0x4B
     ¡¡DATOS ES UNA LISTA!!
 
     ${trama}=    Crear Trama    ${direccion_origen}    ${direccion_destino}    ${numero_bits}    ${comando}    ${datos}
     Log    Trama creada: ${trama}
 ```
 
 ## Funciones Disponibles
 
 `calcular_checksum(trama)`
 
 Esta función calcula el checksum de una trama en hexadecimal.
 
-- `trama`: La trama en hexadecimal para la cual se calculará el checksum.
+- `trama`: La trama en bytearray para la cual se calculará el checksum.
 
 
-`crear_trama(direccion_origen, direccion_destino, numero_bits, comando, datos)`
+`crear_trama(direccion_origen,numero_bytes, direccion_destino, comando, datos)`
 
 Esta función construye una trama según la estructura proporcionada.
-TODO EN FORMATO HEXADECIMAL: 0XAB   
+TODO EN FORMATO STRING: AB   
 
 - `direccion_origen`: La dirección de origen de la trama.
 - `direccion_destino`: La dirección de destino de la trama.
-- `numero_bits`: El número de datos enviados.
+- `numero_bytes`: El número de datos enviados.
 - `comando`: El comando a enviar.
 - `datos`: Los datos a enviar, proporcionados COMO UNA LISTA
 
 
 ## Licencia
 Este proyecto esta licenciado bajo la licencia Apache-2.0
```

### Comparing `robotframework_creartramas-2.1.5/LICENSE` & `robotframework_creartramas-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.5/pyproject.toml` & `robotframework_creartramas-2.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robotframework-creartramas"
-version = "2.1.5"
+version = "2.1.6"
 description = "Creacion de tramas en hexadecimal"
 license = "Apache-2.0"
 authors = ["Anthony Arevalo"]
 maintainers = ["Anthony Arevalo"]
 readme = "./docs/README.md"
 homepage = "https://pypi.org/project/robotframework-creartramas"
 packages = [
```

### Comparing `robotframework_creartramas-2.1.5/TRAMAS/creartramas.py` & `robotframework_creartramas-2.1.6/TRAMAS/creartramas.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,51 +3,59 @@
     Dicha Librería implementa diferentes funciones que permiten calcular el checksum
     de una trama y crear una nueva trama, que posteriormente se podrá enviar.
     """
     def __init__(self) -> None:
         pass
     def calcular_checksum(self,trama):
         """
-        Esta función toma una trama en hexadecimal como entrada y calcula 
-        el checksum para esa trama. Devuelve el valor del checksum.
+        Esta función toma una trama(bytearray) como entrada y calcula 
+        el checksum para esa trama. Devuelve el valor entero del checksum.
         """
         # Suma todos los valores ASCII de los caracteres en la trama 
         check = sum(trama)
-        # Devuelve el checksum módulo 256, comprobando que si check > 256 , el cheksum es 256 menos la diferencia que hay entre ambos
+        # Devuelve el checksum módulo 256, comprobando que: si check > 256 , el cheksum es 256 menos la diferencia que hay entre ambos
         if check >= 256:
             checksum = 256 - (abs(256-check))
         else:
             checksum = abs(256-check)
         return checksum # valor absoluto por si cheksum es mayor que 256
         
-    def crear_trama(self,direccion_destino, numero_bits, direccion_origen, comando, datos):
+    def crear_trama(self,direccion_destino, numero_bytes, direccion_origen, comando, datos):
         """
         Esta función construye una trama de acuerdo con la estructura proporcionada.Tiene 5 argumentos
-        Hay que tener en cuenta que los datos que se introducen deben estar en formate hexadecimal 0XAB.
-        También a la hora de introducir datos, estso deben estar en forma de lista datos=[0x00,0x00,..]
+        Hay que tener en cuenta que los datos que se introducen deben estar en formato string 
+        Python variable='XX'
+        Robotframework  ${variable}=    XX
+        También a la hora de introducir datos, estso deben estar en forma de lista datos 
+        Python -->datos=['XX','ZZ',..]
+        Robotframework--> @{datos}= XX ZZ ...
         Finalmente, se devuelve la trama creada.
         """
-        # Convertir cadenas de texto a bytes en formato hexadecimal
+        # Convertir cadenas de texto a bytes 
         direccion_destino_bytes = bytes.fromhex(direccion_destino)
-        numero_bits_bytes = bytes.fromhex(numero_bits)
+        numero_bytes_bytes = bytes.fromhex(numero_bytes)
         direccion_origen_bytes = bytes.fromhex(direccion_origen)
         comando_bytes = bytes.fromhex(comando)
-        datos_bytes = [bytes.fromhex(dato) for dato in datos]
+        # La funcion puede no recibir datos, por eso comprueba longitud de datos
+        # para ver si tiene que convertir los datos o dejarlo vacio
+        if len(datos)>0:
+            datos_bytes = [bytes.fromhex(dato) for dato in datos.split()]
     
         # Construir la trama en forma de bytearray (valores en código ASCII)
         trama = bytearray()
-        trama.append(int.from_bytes(direccion_destino_bytes, 'big'))
-        trama.append(int.from_bytes(numero_bits_bytes, 'big'))
-        trama.append(int.from_bytes(direccion_origen_bytes, 'big'))
-        trama.append(int.from_bytes(comando_bytes, 'big'))
-        
-        # Agregar los datos a la trama
-        for dato in datos_bytes:
-            trama.append(int.from_bytes(dato, 'big'))
+        trama.extend(direccion_destino_bytes)
+        trama.extend(numero_bytes_bytes)
+        trama.extend(direccion_origen_bytes)
+        trama.extend(comando_bytes)
+            
+        # Agregar los datos a la trama, si estos tienen longitud mayor de 0
+        if len(datos)>0:
+            for dato in datos_bytes:
+                trama.extend(dato)
         
         # Calcular el checksum
-        checksum = calcular_checksum(trama)
+        checksum = self.calcular_checksum(trama)
         
         # Añadir el checksum a la trama
         trama.append(checksum)
         
         return trama
```

### Comparing `robotframework_creartramas-2.1.5/PKG-INFO` & `robotframework_creartramas-2.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-creartramas
-Version: 2.1.5
+Version: 2.1.6
 Summary: Creacion de tramas en hexadecimal
 Home-page: https://pypi.org/project/robotframework-creartramas
 License: Apache-2.0
 Author: Anthony Arevalo
 Maintainer: Anthony Arevalo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -28,54 +28,54 @@
 Antes de usar esta librería, asegurate de tener instalado lo siguuiente:
 - Python > 3.8
 - Robot Framework
 - pip (para instalar libreria)
 
 ## Instalación
 Puedes instalar esta librería a través de pip:
-* ` pip install --upgrade robotframework-creartramas`
+* ` pip install robotframework-creartramas`
 
 ## Uso 
 
 ``` RobotFramework
 
  Aquí tienes un ejemplo de cómo crear una trama utilizando esta librería:
 
 *** Settings ***
-Library    mi_libreria_de_tramas.TRAMAS
+Library    TRAMAS
 
 *** Test Cases ***
 Crear y enviar trama
-    ${direccion_origen}=    Set Variable    0x01
-    ${direccion_destino}=    Set Variable    0x02
-    ${numero_bits}=    Set Variable    0x08
-    ${comando}=    Set Variable    0xFE
-    ${datos}=    Create List    0x41    0x5A    0x4B
+    ${direccion_origen}=    01
+    ${direccion_destino}=   02
+    ${numero_bytes}=         08
+    ${comando}=             FE
+    @{datos}=               0x41    0x5A    0x4B
     ¡¡DATOS ES UNA LISTA!!
 
     ${trama}=    Crear Trama    ${direccion_origen}    ${direccion_destino}    ${numero_bits}    ${comando}    ${datos}
     Log    Trama creada: ${trama}
 ```
 
 ## Funciones Disponibles
 
 `calcular_checksum(trama)`
 
 Esta función calcula el checksum de una trama en hexadecimal.
 
-- `trama`: La trama en hexadecimal para la cual se calculará el checksum.
+- `trama`: La trama en bytearray para la cual se calculará el checksum.
 
 
-`crear_trama(direccion_origen, direccion_destino, numero_bits, comando, datos)`
+`crear_trama(direccion_origen,numero_bytes, direccion_destino, comando, datos)`
 
 Esta función construye una trama según la estructura proporcionada.
-TODO EN FORMATO HEXADECIMAL: 0XAB   
+TODO EN FORMATO STRING: AB   
 
 - `direccion_origen`: La dirección de origen de la trama.
 - `direccion_destino`: La dirección de destino de la trama.
-- `numero_bits`: El número de datos enviados.
+- `numero_bytes`: El número de datos enviados.
 - `comando`: El comando a enviar.
 - `datos`: Los datos a enviar, proporcionados COMO UNA LISTA
 
 
 ## Licencia
 Este proyecto esta licenciado bajo la licencia Apache-2.0
```

