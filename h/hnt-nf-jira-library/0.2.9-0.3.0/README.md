# Comparing `tmp/hnt_nf_jira_library-0.2.9.tar.gz` & `tmp/hnt_nf_jira_library-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_library-0.2.9.tar", last modified: Wed Apr 10 15:06:53 2024, max compression
+gzip compressed data, was "hnt_nf_jira_library-0.3.0.tar", last modified: Fri Apr 12 20:11:51 2024, max compression
```

## Comparing `hnt_nf_jira_library-0.2.9.tar` & `hnt_nf_jira_library-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 15:06:53.082695 hnt_nf_jira_library-0.2.9/
--rw-rw-rw-   0        0        0      286 2024-04-10 15:06:53.081657 hnt_nf_jira_library-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 15:06:53.079657 hnt_nf_jira_library-0.2.9/hnt_nf_jira_library.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-10 15:06:52.000000 hnt_nf_jira_library-0.2.9/hnt_nf_jira_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      860 2024-04-10 15:06:52.000000 hnt_nf_jira_library-0.2.9/hnt_nf_jira_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 15:06:52.000000 hnt_nf_jira_library-0.2.9/hnt_nf_jira_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-10 15:06:52.000000 hnt_nf_jira_library-0.2.9/hnt_nf_jira_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 15:06:52.000000 hnt_nf_jira_library-0.2.9/hnt_nf_jira_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 15:06:53.025925 hnt_nf_jira_library-0.2.9/nf_jira/
--rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.2.9/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:06:53.063816 hnt_nf_jira_library-0.2.9/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:06:53.077145 hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4750 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0     1377 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     2019 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     2941 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     2888 2024-04-10 12:12:39.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      145 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/dados_basicos.py
--rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/dados_nfe.py
--rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      140 2024-03-15 19:20:34.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0       97 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      397 2024-03-08 19:34:36.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0      379 2024-03-20 15:23:30.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.2.9/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0    16497 2024-04-10 15:05:11.000000 hnt_nf_jira_library-0.2.9/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-04-10 15:06:53.084727 hnt_nf_jira_library-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-10 15:06:46.000000 hnt_nf_jira_library-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.344657 hnt_nf_jira_library-0.3.0/
+-rw-rw-rw-   0        0        0      286 2024-04-12 20:11:51.344657 hnt_nf_jira_library-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-02-22 17:33:05.000000 hnt_nf_jira_library-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.343196 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1065 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 20:11:51.000000 hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.264292 hnt_nf_jira_library-0.3.0/nf_jira/
+-rw-rw-rw-   0        0        0       30 2024-04-04 19:57:31.000000 hnt_nf_jira_library-0.3.0/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.317672 hnt_nf_jira_library-0.3.0/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-02-22 18:39:39.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      110 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:11:51.332775 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4819 2024-04-12 19:57:34.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0     2011 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     2019 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     3049 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1695 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     2956 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      331 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      145 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0      198 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/dados_nfe.py
+-rw-rw-rw-   0        0        0       76 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      201 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0      140 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      224 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      402 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/miro copy.py
+-rw-rw-rw-   0        0        0      402 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      127 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0      379 2024-04-11 13:23:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0      169 2024-04-12 19:38:28.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-02-26 13:33:35.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-03-08 17:09:47.000000 hnt_nf_jira_library-0.3.0/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0    20872 2024-04-12 19:50:36.000000 hnt_nf_jira_library-0.3.0/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 20:11:51.344657 hnt_nf_jira_library-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      510 2024-04-12 20:11:05.000000 hnt_nf_jira_library-0.3.0/setup.py
```

### Comparing `hnt_nf_jira_library-0.2.9/hnt_nf_jira_library.egg-info/SOURCES.txt` & `hnt_nf_jira_library-0.3.0/hnt_nf_jira_library.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,28 @@
 hnt_nf_jira_library.egg-info/requires.txt
 hnt_nf_jira_library.egg-info/top_level.txt
 nf_jira/__init__.py
 nf_jira/wrapper_nf_jira.py
 nf_jira/entities/anexo.py
 nf_jira/entities/chave_acesso.py
 nf_jira/entities/constants.py
-nf_jira/entities/dados_basicos.py
+nf_jira/entities/dados_basicos_fatura.py
+nf_jira/entities/dados_basicos_miro.py
 nf_jira/entities/dados_nfe.py
 nf_jira/entities/detalhe.py
+nf_jira/entities/fatura.py
 nf_jira/entities/item.py
+nf_jira/entities/itens_fatura.py
 nf_jira/entities/jira_info.py
+nf_jira/entities/miro copy.py
 nf_jira/entities/miro.py
 nf_jira/entities/nfe_sefaz.py
 nf_jira/entities/nota_pedido.py
+nf_jira/entities/pagamento.py
 nf_jira/entities/referencia_pedido.py
 nf_jira/entities/sintese_itens.py
 nf_jira/entities/sintese_miro.py
 nf_jira/entities/classes/form_jira.py
 nf_jira/entities/classes/helper.py
 nf_jira/entities/classes/issue_fields.py
-nf_jira/entities/classes/issue_jira.py
+nf_jira/entities/classes/issue_jira.py
+nf_jira/entities/classes/n8n_domain.py
```

### Comparing `hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/form_jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,16 @@
         fields_values = data.get('state')['answers']
         fields_root = data.get('design')['questions']
         
         for root in fields_root:
 
             field_name = fields_root[root].get('questionKey')
             if fields_values.get(root) is not None:
-                field_index = list(fields_values.get(root).keys())[0] if "choices" not in list(fields_values.get(root).keys()) else list(fields_values.get(root).keys())[1]
+                # field_index = list(fields_values.get(root).keys())[0]
+                field_index = list(fields_values.get(root).keys())[1] if "choices" in list(fields_values.get(root).keys()) else list(fields_values.get(root).keys())[0]
                 field_value = fields_values.get(root)[field_index]
             else: 
                 field_value = None
 
             fields_json[field_name] = field_value
 
         return fields_json
```

### Comparing `hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_library-0.2.9/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_library-0.3.0/nf_jira/entities/classes/issue_jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,22 @@
         
 class AttachmentJira:
 
     def get_attachment(self, issue):
 
         self._check_issue_attachment(issue)
         attachments_ids = self._get_attachment_id(issue)
+        attachment = {}
         for attachment_key in attachments_ids:
             attachments_from_issue = self._get_attachments_from_issue(attachment_key)
+            if attachments_from_issue:
+                attachment = attachments_from_issue
+
         
-        return attachments_from_issue
+        return attachment
         
     def _check_issue_attachment(self, issue):
         if issue.get("fields")["attachment"] is None:
             raise Exception("Could not find attachment")
         
     def _get_attachments_from_issue(self, attachment_key):
         try:
```

### Comparing `hnt_nf_jira_library-0.2.9/nf_jira/entities/constants.py` & `hnt_nf_jira_library-0.3.0/nf_jira/entities/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 
 #Constant N8N
 N8N_AUTH = (os.getenv("N8N_USERNAME"), os.getenv("N8N_PASSWORD"))
 API_DOMAIN_N8N_URL = os.getenv("DOMAIN_URL")
+FORNECEDOR_N8N_DOMAIN = "fornecedor"
+CENTRO_N8N_DOMAIN = "centro"
 
 # Constantes dos ID's de Formulario
 FORM_TEMPLATE_AUTOMACAO = "910a886b-701a-490d-8b02-708b6c2d9881"
 FORM_TEMPLATE_COMPLEMENTO = "720b4c69-9d84-4f08-930e-1d6c22805f71"
 
 # Constants Jira
 JIRA_AUTH = (os.getenv("USER"), os.getenv("ACCESS_TOKEN"))
@@ -23,15 +25,15 @@
                          }
 API_ATLASSIAN_HEADERS = {
                             "Accept": "application/json",
                             "X-ExperimentalApi": "opt-in",
                         }
 
 #Test Constants
-ISSUE_KEY = "GHN-404"
+ISSUE_KEY = "GHN-487"
 TRASITION_PEDIDO_CRIADO = '241'
 TRASITION_REVISAR_ERRO  = '231'
 FORM_COMPLEMENTO_ID = "f1671ecd-fc44-418f-b6e3-88d774a4b0d4"
 FORM_AUTOMACAO_ID = "e6214bb3-eafc-4de8-ad5a-c8b387346c3e"
 STATUS_LIBERADO = "2"
 STATUS_BLOQUEADO = "1"
```

### Comparing `hnt_nf_jira_library-0.2.9/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_library-0.3.0/nf_jira/wrapper_nf_jira.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,43 +3,102 @@
 import os
 from os import getcwd, path
 from datetime import datetime
 from pydantic import ValidationError
 
 from .entities.nota_pedido import NotaPedido
 from .entities.miro import Miro
+from .entities.fatura import Fatura
 from .entities.constants import *
-from .entities.classes.form_jira import FormJira
-from .entities.classes.issue_jira import IssueJira
-from .entities.classes.issue_jira import AttachmentJira
-from .entities.classes.issue_fields import IssueFields
-from .entities.classes.helper import JiraFieldsHelper, JsonHelper
-
-from nf_consumo.consumo_service import ConsumoService
-
 
+from .entities.classes.form_jira    import FormJira
+from .entities.classes.issue_jira   import IssueJira
+from .entities.classes.issue_jira   import AttachmentJira
+from .entities.classes.issue_fields import IssueFields
+from .entities.classes.helper       import JiraFieldsHelper, JsonHelper, GuiandoHelper
+from .entities.classes.n8n_domain   import N8NDomain
 class wrapper_jira:
 
     def __init__(self, debug=False):
         self._test_mode = debug
-        self._set_request()
         self.FormJira         = FormJira()
         self.IssueJira        = IssueJira()
         self.AttachmentJira   = AttachmentJira()
         self.JiraFieldsHelper = JiraFieldsHelper()
+        self.GuiandoHelper    = GuiandoHelper()
         self.JsonHelper       = JsonHelper()
         self.IssueFields      = IssueFields()
-        self.ConsumoService   = ConsumoService()
+        self.N8NDomain        = N8NDomain()
+        self._miro_is_active  = False
+
+    def get_document_by_issue(self, issue_key):
+
+        issue_sap_json = {}
+
+        issue = self._get_issue_by_key(issue_key)
+        issue_transition = issue['domain_data']['fornecedor']['transacao']
+
+        if issue_transition == 'ME21N':
+            nota_pedido_factory = self._issue_factory(issue)
+            nota_pedido_model   = NotaPedido(**nota_pedido_factory).model_dump()
+            issue_sap_json["nota_pedido"] = nota_pedido_model
+
+            if self._miro_is_active:
+                miro_factory = self._miro_factory(issue)
+                miro_model = Miro(**miro_factory).model_dump()
+                issue_sap_json["miro"] = miro_model
+
+        elif issue_transition == 'FV60':
+            fatura_factory = self._fatura_factory(issue)
+            fatura_model   = Fatura(**fatura_factory).model_dump()
+            issue_sap_json["fatura"] = fatura_model
+
+        if self._test_mode:
+            for json in issue_sap_json:
+                self.JsonHelper.save_json(f'{json}_{issue_key}', issue_sap_json[json])
+            
+        return issue_sap_json
 
-    def _set_request(self):
-        self._api_headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/json",
+    def _get_issue_by_key(self, issue_key):
+
+        issue_json = self._get_nf_jira(issue_key)
+
+        issue_attachment = issue_json["attachment"]
+        jira_info = issue_json["jira_info"]
+
+        fornecedor_domain = self.N8NDomain.get_nf_domain(FORNECEDOR_N8N_DOMAIN, issue_attachment[CNPJ_DO_FORNECEDOR])
+        centro_domain = self.N8NDomain.get_nf_domain(CENTRO_N8N_DOMAIN, issue_attachment[CNPJ_DO_CLIENTE])
+
+        domain = {
+            "fornecedor"    : fornecedor_domain,
+            "centro" : centro_domain
+        }
+
+        allocation = self.N8NDomain.get_allocation(
+            issue_attachment[CNPJ_DO_FORNECEDOR],
+            issue_attachment[CNPJ_DO_CLIENTE],
+            issue_attachment[NÚMERO_DO_CONTRATO]
+        )
+
+        pdf_data = self.GuiandoHelper.download_pdf_nexinvoice(issue_attachment)
+
+        issue = {
+            "issue_data": issue_json["issue_data"],
+            "json_data": issue_attachment,
+            "domain_data": domain,
+            "allocation_data": allocation,
+            "pdf_data": pdf_data,
+            "jira_info": jira_info,
         }
 
+        if self._test_mode:
+            self.JsonHelper.save_json(f'Issue_data_{issue_key}', issue)
+
+        return issue
+
     def _issue_factory(self, issue: dict):
 
         sintese_itens = []
         validTotalPercents = 0.0
 
         if not issue["allocation_data"]:
 
@@ -117,65 +176,65 @@
             .upper()
         )
 
         if issue[COMPLEMENTO_DE_ÁGUA] is not None:
             leitura_anterior = (
                 datetime.strptime(
                     issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAnterior"],
-                    "%Y-%m-%dT%H:%M:%S",
+                    "%Y-%m-%d",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
-                    issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_ÁGUA]["DataLeituraAtual"], "%Y-%m-%d"
                 )
                 .strftime("%b/%y")
                 .upper()
             )
         elif issue[COMPLEMENTO_DE_ENERGIA] is not None:
             leitura_anterior = (
                 datetime.strptime(
                     issue[COMPLEMENTO_DE_ENERGIA]["DataLeituraAnterior"],
-                    "%Y-%m-%dT%H:%M:%S",
+                    "%Y-%m-%d",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
                     issue[COMPLEMENTO_DE_ENERGIA]["DataLeituraAtual"],
-                    "%Y-%m-%dT%H:%M:%S",
+                    "%Y-%m-%d",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
         elif issue[COMPLEMENTO_DE_GÁS] is not None:
             leitura_anterior = (
                 datetime.strptime(
                     issue[COMPLEMENTO_DE_GÁS]["DataLeituraAnterior"],
-                    "%Y-%m-%dT%H:%M:%S",
+                    "%Y-%m-%d",
                 )
                 .strftime("%b/%y")
                 .upper()
             )
             leitura_atual = (
                 datetime.strptime(
-                    issue[COMPLEMENTO_DE_GÁS]["DataLeituraAtual"], "%Y-%m-%dT%H:%M:%S"
+                    issue[COMPLEMENTO_DE_GÁS]["DataLeituraAtual"], "%Y-%m-%d"
                 )
                 .strftime("%b/%y")
                 .upper()
             )
 
         texto = f"REF: {data_ref} PERIODO: {leitura_anterior} A {leitura_atual}"
 
         dados_basicos = {
             "data_da_fatura": datetime.strptime(
-                issue[DATA_DE_EMISSÃO], "%Y-%m-%dT%H:%M:%S"
+                issue[DATA_DE_EMISSÃO], "%Y-%m-%d"
             ).strftime("%d%m%Y"),
             "referencia": f"{issue['ChaveAcessoNotaFiscal'][25:34]}-{issue['ChaveAcessoNotaFiscal'][22:25]}",
             "montante": str(issue[VALOR_TOTAL_DA_FATURA]),
             "texto": texto,
         }
 
         referencia_pedido = {"numero_pedido": issue["cod_sap"]}
@@ -202,16 +261,53 @@
             "referencia_pedido": referencia_pedido,
             "detalhe": detalhe,
             "sintese": sintese,
             "dados_nfe": dados_nfe,
         }
 
         return miro_model
+    
+    def _fatura_factory(self, issue): 
+
+        texto = self._prepare_ref(issue)
+
+        item = {
+            "Cta_razao": issue['domain_data']['fornecedor']['razao'], #Conta Contabil SAP
+            "Montante":  str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
+            "loc_negocios": issue['domain_data']['centro']['centro'],
+            "atribuicao": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%Y%m%d"),
+            "texto": texto,
+            "centro_custo":  f"{issue['domain_data']['centro']['centro']}210"
+        }
+
+        itens = [item]
+
+        dados_basicos = {
+            "cod_fornecedor": issue['domain_data']['fornecedor']['codigo_sap'], #ID_EXTERNO_SAP
+            "data_fatura": datetime.strptime(issue['json_data'][DATA_DE_EMISSÃO], "%Y-%m-%d").strftime("%d.%m.%Y"),
+            "referencia": issue['json_data'][NÚMERO_DA_FATURA_DO_FORNECEDOR],
+            "montante": str(issue['json_data'][VALOR_TOTAL_DA_FATURA]),
+            "bus_pl_sec_cd": itens[0]["loc_negocios"],
+            "texto": texto,
+            "itens": itens
+        }
 
-    def get_nf_issue_context(self, issue_id: str):
+        pagamento = {
+            "data_basica": datetime.now().strftime("%d.%m.%Y"),
+            "cond_pgto": "0000" #CONSTANTE 
+        }
+
+        fatura_model = {
+            "dados_basicos": dados_basicos,
+            "pagamento":pagamento
+        }
+
+        return fatura_model
+
+    def _get_nf_issue_context(self, issue_id: str):
         try:
 
             issue_json = self._get_nf_jira(issue_id)
 
             attachment = issue_json["attachment"]
             jira_info = issue_json["jira_info"]
 
@@ -233,41 +329,33 @@
             allocation = self._get_allocation(
                 attachment[CNPJ_DO_FORNECEDOR],
                 attachment[CNPJ_DO_CLIENTE],
                 attachment[NÚMERO_DO_CONTRATO],
             )
 
             ##### FORMAT JSON #####
-            issue = {
-                "issue_data": issue_json["issue_data"],
-                "json_data": attachment,
-                "domain_data": domain,
-                "allocation_data": allocation,
-                "pdf_data": pdf_data,
-                "jira_info": jira_info,
-            }
+
 
             ##### PARSE JSON #####
-            issue_model = self._issue_factory(issue)
+            # issue_model = self._issue_factory(issue)
 
             ##### CREATE MODEL #####
-            nota_pedido = NotaPedido(**issue_model).model_dump()
+            # nota_pedido = NotaPedido(**issue_model).model_dump()
 
             #### SAVE JSON ####
-            if self._test_mode:
-                self.JsonHelper.save_json(f'Nota_Pedido_{issue_id}', nota_pedido)
 
-            return nota_pedido
+
+            # return nota_pedido
         except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
         except Exception as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
-    def get_nf_miro_context(self, issue_id: str, cod_sap: str):
+    def _get_nf_miro_context(self, issue_id: str, cod_sap: str):
         try:
 
             issue_data = self._get_nf_jira(issue_id)
 
             clean_fields = self._remove_null_fields(
                 issue_data["issue_data"].get("fields")
             )
@@ -298,15 +386,57 @@
 
         except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
         except Exception as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
-    def _get_nf_jira(self, issue_id: str):
+    def _get_nf_fatura_context(self, issue_id):
+        try:
+
+            issue_data = self._get_nf_jira(issue_id)
+
+            attachment = issue_data['attachment']
+
+            # não esta vindo no json guiando, não há como validar sem isso no momento
+            # if not attachment['invoiceNumber']:
+            #     return {}
+
+            cnpj_fornecedor = attachment.get(CNPJ_DO_FORNECEDOR)
+            fornecedor = self._get_nf_domain('fornecedor', cnpj_fornecedor)
+
+            cnpj_centro = attachment.get(CNPJ_DO_CLIENTE)
+            centro = self._get_nf_domain('centro', cnpj_centro)
+
+            domain_data = {
+                "fornecedor": fornecedor,
+                "centro": centro
+            }
+
+            issue = {
+                'json_data': attachment,
+                'domain_data': domain_data
+            }
+
+            fatura_model = self._fatura_factory(issue)
+
+            fatura = Fatura(**fatura_model).model_dump()
+
+            if self._test_mode:
+                self.JsonHelper.save_json(f'Fatura_{issue_id}', fatura)
+
+            return fatura
+    
+        except requests.exceptions.HTTPError as e:
+            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
+
+        except Exception as e:
+            raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
+        
+    def _get_nf_jira(self, issue_id):
         try:
 
             issue_data = self.IssueJira.get_issue(issue_id)
             complement_form = self._get_issue_fields_by_keys( issue_id, FORM_TEMPLATE_COMPLEMENTO )
 
             issue_data["fields"] = self.JiraFieldsHelper.remove_null_fields(issue_data.get("fields"))
             attachment = self.AttachmentJira.get_attachment(issue_data)
@@ -342,18 +472,17 @@
             attachment[DATA_DE_REFERÊNCIA] = complement_form['periodo_referencia']
             attachment["numero_log"] = complement_form['protocolo_autorizacao']
             attachment["data_procmto"] = complement_form['data_autorizacao']
             attachment["hora_procmto"] = complement_form['hora_autorizacao']
             attachment[nf_type]["DataLeituraAnterior"] = complement_form['data_leitura_anterior']
             attachment[nf_type]["DataLeituraAtual"] = complement_form['data_leitura_atual']
             attachment["grupo_compradores"] = complement_form['grupo_compradores']
-            attachment["grupo_compradores"] = complement_form['grupo_compradores']
 
             #Validação de Valor Liquido da Fatura
-            if complement_form['valor_liquido'] != None:
+            if complement_form['valor_liquido'] != "":
                 attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_liquido']
             elif complement_form['valor_nota'] != None:
                 attachment[VALOR_TOTAL_DA_FATURA] = complement_form['valor_nota']
             else:
                 attachment[VALOR_TOTAL_DA_FATURA] = attachment.get(
                     VALOR_TOTAL_DA_FATURA
                 )
@@ -372,56 +501,29 @@
 
         except requests.exceptions.HTTPError as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
         except Exception as e:
             raise Exception(f"Erro ao receber a Nota Fiscal:\n{e}")
 
-    def _get_nf_domain(self, type: str, cnpj: str):
-
-        try:
-            domain_request = requests.get(
-                f"{API_DOMAIN_N8N_URL}/{'fornecedores' if type == 'fornecedor' else 'centros'}?cnpj={cnpj}",
-                auth=N8N_AUTH,
-            )
-            domain_request.raise_for_status()
-            domain_data = domain_request.json()
-
-            if not domain_data:
-                raise Exception("Could not find domain")
+    def _prepare_ref(self, issue):
 
-        except Exception as e:
-            raise Exception(f"Erro ao receber {type}:\n{e}")
-
-        return domain_data
-
-    def _get_allocation(
-        self, cnpj_fornecedor: str, cnpj_cliente: str, numero_contrato: str
-    ):
-
-        try:
-            allocation_request = requests.get(
-                f"{API_DOMAIN_N8N_URL}/rateio?cnpj_fornecedor={cnpj_fornecedor}&cnpj_hortifruti={cnpj_cliente}&numero_contrato={numero_contrato}",
-                auth=N8N_AUTH,
-            )
-            allocation_request.raise_for_status()
-            if allocation_request.text.strip() != "":
-                allocation_data = allocation_request.json()
-            else:
-                allocation_data = None
-        except Exception as e:
-            raise Exception(f"Erro ao receber rateio:\n{e}")
+        data_ref = datetime.strptime(issue['json_data'][DATA_DE_REFERÊNCIA], "%m/%Y").strftime("%b/%y").upper()
 
-        return allocation_data
+        if issue['json_data'][COMPLEMENTO_DE_ÁGUA] is not None:
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper()
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ÁGUA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()
+        elif issue['json_data'][COMPLEMENTO_DE_ENERGIA] is not None:
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper()
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_ENERGIA]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()
+        elif issue['json_data'][COMPLEMENTO_DE_GÁS] is not None:
+            leitura_anterior = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAnterior'], "%Y-%m-%d").strftime("%b/%y").upper()
+            leitura_atual = datetime.strptime(issue['json_data'][COMPLEMENTO_DE_GÁS]['DataLeituraAtual'], "%Y-%m-%d").strftime("%b/%y").upper()
 
-    def _download_pdf(self, pdf_path):
-        path_dir = path.join(getcwd(), "output/pdf")
-        pdf_file = self.ConsumoService.download_pdf(pdf_path, path_dir)
-
-        return pdf_file
+        return f"REF: {data_ref} PERIODO: {leitura_anterior} A {leitura_atual}"
 
     def post_transition(self, transition_id, issue_id):
         payload = json.dumps(
             {
                 "transition": {"id": transition_id},
                 "update": {"comment": []},
             }
@@ -437,8 +539,10 @@
     def _get_issue_fields_by_keys(self, issue_key, form_template):
 
         form_jira_keys = self.FormJira.get_form_jira_keys(issue_key, form_template)
         form_fields    = self.FormJira.get_form_fields(issue_key, form_template)
         jira_fields    = self.IssueJira.get_issue_fields_data(issue_key)
         fields_by_jira_and_form = self.IssueFields.get_fields_by_form_and_jira(form_jira_keys, form_fields, jira_fields)
 
-        return fields_by_jira_and_form
+        return fields_by_jira_and_form
+    
+
```

