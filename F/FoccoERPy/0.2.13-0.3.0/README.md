# Comparing `tmp/FoccoERPy-0.2.13.tar.gz` & `tmp/FoccoERPy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoccoERPy-0.2.13.tar", last modified: Tue Apr 25 13:25:18 2023, max compression
+gzip compressed data, was "FoccoERPy-0.3.0.tar", last modified: Fri Apr 12 14:00:46 2024, max compression
```

## Comparing `FoccoERPy-0.2.13.tar` & `FoccoERPy-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.310290 FoccoERPy-0.2.13/
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.303623 FoccoERPy-0.2.13/FoccoERPy/
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.306957 FoccoERPy-0.2.13/FoccoERPy/Focco/
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)     7640 2023-04-25 13:24:24.000000 FoccoERPy-0.2.13/FoccoERPy/Focco/__init__.py
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.306957 FoccoERPy-0.2.13/FoccoERPy/FoccoSession/
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)      854 2023-03-08 21:36:03.000000 FoccoERPy-0.2.13/FoccoERPy/FoccoSession/__init__.py
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)       85 2023-01-09 17:18:22.000000 FoccoERPy-0.2.13/FoccoERPy/__init__.py
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.306957 FoccoERPy-0.2.13/FoccoERPy/core/
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)     3788 2023-04-05 02:29:52.000000 FoccoERPy-0.2.13/FoccoERPy/core/__init__.py
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.306957 FoccoERPy-0.2.13/FoccoERPy/exceptions/
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)     1613 2023-03-09 20:37:03.000000 FoccoERPy-0.2.13/FoccoERPy/exceptions/__init__.py
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.306957 FoccoERPy-0.2.13/FoccoERPy/handlers/
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)     2691 2023-01-09 17:18:22.000000 FoccoERPy-0.2.13/FoccoERPy/handlers/__init__.py
-drwxr-xr-x   0 ganiziolek  (1000) ganiziolek  (1001)        0 2023-04-25 13:25:18.306957 FoccoERPy-0.2.13/FoccoERPy.egg-info/
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)      635 2023-04-25 13:25:18.000000 FoccoERPy-0.2.13/FoccoERPy.egg-info/PKG-INFO
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)      372 2023-04-25 13:25:18.000000 FoccoERPy-0.2.13/FoccoERPy.egg-info/SOURCES.txt
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)        1 2023-04-25 13:25:18.000000 FoccoERPy-0.2.13/FoccoERPy.egg-info/dependency_links.txt
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)       49 2023-04-25 13:25:18.000000 FoccoERPy-0.2.13/FoccoERPy.egg-info/requires.txt
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)       10 2023-04-25 13:25:18.000000 FoccoERPy-0.2.13/FoccoERPy.egg-info/top_level.txt
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)     1073 2023-01-09 17:18:22.000000 FoccoERPy-0.2.13/LICENSE
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)      635 2023-04-25 13:25:18.306957 FoccoERPy-0.2.13/PKG-INFO
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)       80 2023-01-09 17:18:22.000000 FoccoERPy-0.2.13/README.md
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)      716 2023-04-25 13:24:24.000000 FoccoERPy-0.2.13/pyproject.toml
--rw-r--r--   0 ganiziolek  (1000) ganiziolek  (1001)       38 2023-04-25 13:25:18.310290 FoccoERPy-0.2.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/Focco/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/Focco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/FoccoSession/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/FoccoSession/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/setup.cfg
```

### Comparing `FoccoERPy-0.2.13/FoccoERPy/Focco/__init__.py` & `FoccoERPy-0.3.0/FoccoERPy/Focco/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.2.13/FoccoERPy/FoccoSession/__init__.py` & `FoccoERPy-0.3.0/FoccoERPy/FoccoSession/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.2.13/FoccoERPy/core/__init__.py` & `FoccoERPy-0.3.0/FoccoERPy/core/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from FoccoERPy.handlers import handle_json
 from datetime import datetime
 from requests.exceptions import HTTPError
 from FoccoERPy.exceptions import ErroFocco
 from FoccoERPy.exceptions import OrdemNaoEncontrada
 from FoccoERPy.FoccoSession import FoccoSession
 
@@ -10,89 +11,99 @@
 
     try:
         response = session.request('GET', PATH)
 
         resposta_focco = handle_json(response.json())
 
         return resposta_focco
-        
+
     except HTTPError as e:
         if e.response.status_code == 404:
             raise OrdemNaoEncontrada(id_ordem)
         else:
             raise e
-    
+
     except Exception as e:
         raise ErroFocco(f"Não teve sucesso na busca da ordem: {str(e)}")
-    
+
 def consulta_operacoes_ordem(session: FoccoSession, id_roteiro: int) -> list:
-    
+
     PATH = 'api/Commands/Manufatura.Producao.Apontamento.GetApontamentosByOrdemRoteiroCommand'
 
     BODY = {
         'take': None,
         'skip': None,
         'ordemRoteiroID': id_roteiro
     }
 
     response = session.request('POST', PATH, json=BODY)
 
     try:
         response.raise_for_status()
     except Exception as e:
-        raise ErroFocco(f"Não teve sucesso na busca de operações: {resposta_focco.get('ErrorMessage')}")
+        raise ErroFocco("Não teve sucesso na busca de operações")
 
     resposta_focco = handle_json(response.json()).get('$values')
 
     if not resposta_focco:
         return None
-    
+
     return resposta_focco
 
-def apontamento_tempo_padrao(session: FoccoSession, id_ordem_roteiro: int, quantidade: float, 
-                             id_recurso: int, data: datetime, finalizar: bool):
+def apontamento_tempo_padrao(
+        session: FoccoSession,
+        id_ordem_roteiro: int,
+        quantidade: float,
+        data: datetime = datetime.now(),
+        finalizar: bool = False,
+        id_tipo_apontamento: str = 'TP',
+        origem_apontamento: str = 'API',
+        usuario: str = 'Apontamento API GTRP',
+        id_funcionario: Optional[int] = None,
+        id_recurso: Optional[int] = None,
+    ):
     """
         Apontamento por tempo padrão
     """
-    ID_TIPO_APONTAMENTO = 'TP'
-    ID_FUNCIONARIO = 0
-    ORIGEM_APONTAMENTO = 'API'
-    USUARIO = 'Apontamento API GTRP'
 
     PATH = 'api/Entities/Manufatura.Producao.Apontamento.ApontamentoProducao'
 
     BODY = {
         'OrdemRoteiro': {
             'ID': id_ordem_roteiro
         },
         'Quantidade': quantidade,
         'DataApontamento': data.isoformat(),
         'TipoApontamento': {
-            'ID': ID_TIPO_APONTAMENTO
-        },
-        'Funcionario': {
-            'ID': ID_FUNCIONARIO
+            'ID': id_tipo_apontamento
         },
         'Final': finalizar,
-        'Usuario': USUARIO,
-        'OrigemApontamento': ORIGEM_APONTAMENTO,
-        'ApontamentoMaquina': {
+        'Usuario': usuario,
+        'OrigemApontamento': origem_apontamento,
+    }
+
+    if id_funcionario is not None:
+        BODY['Funcionario'] = {
+            'ID': id_funcionario
+        }
+
+    if id_recurso is not None:
+        BODY['ApontamentoMaquina'] = {
             'Maquina': {
                 'ID': id_recurso
             }
         }
-    }
 
     response = session.request('POST', PATH, json=BODY)
 
     resposta_focco = handle_json(response.json())
 
     if not resposta_focco.get('Succeeded'):
         raise ErroFocco(f"Não teve sucesso no apontamento: {resposta_focco.get('ErrorMessage')}")
-    
+
     return resposta_focco
 
 def impressao_etiqueta(session: FoccoSession, 
         bearer: str,
         modelo_etiqueta: str,
         id_empresa: int,
         id_apontamento: int,
```

### Comparing `FoccoERPy-0.2.13/FoccoERPy/exceptions/__init__.py` & `FoccoERPy-0.3.0/FoccoERPy/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.2.13/FoccoERPy/handlers/__init__.py` & `FoccoERPy-0.3.0/FoccoERPy/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.2.13/LICENSE` & `FoccoERPy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.2.13/pyproject.toml` & `FoccoERPy-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FoccoERPy"
-version = "0.2.13"
+version = "0.3.0"
 authors = [
   { name="Gabriel Niziolek", email="ganiziolek@gmail.com" },
 ]
 description = "Biblioteca de funções que permitem se conectar à API do FoccoERP "
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

