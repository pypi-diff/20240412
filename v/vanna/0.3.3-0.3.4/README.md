# Comparing `tmp/vanna-0.3.3.tar.gz` & `tmp/vanna-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vanna-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vanna-0.3.3.tar` & `vanna-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     7922 2024-04-05 14:52:15.482886 vanna-0.3.3/README.md
--rw-r--r--   0        0        0     1247 2024-04-05 14:52:15.498886 vanna-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     8728 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_Chat.py
--rw-r--r--   0        0        0     2849 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
--rw-r--r--   0        0        0      116 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ZhipuAI/__init__.py
--rw-r--r--   0        0        0     9248 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/__init__.py
--rw-r--r--   0        0        0       43 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/anthropic/__init__.py
--rw-r--r--   0        0        0     2615 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/anthropic/anthropic_chat.py
--rw-r--r--   0        0        0       28 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/base/__init__.py
--rw-r--r--   0        0        0    54875 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/base/base.py
--rw-r--r--   0        0        0       50 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/chromadb/__init__.py
--rw-r--r--   0        0        0     8453 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/chromadb/chromadb_vector.py
--rw-r--r--   0        0        0      717 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/exceptions/__init__.py
--rw-r--r--   0        0        0    21212 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/flask/__init__.py
--rw-r--r--   0        0        0   180924 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/flask/assets.py
--rw-r--r--   0        0        0      313 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/local.py
--rw-r--r--   0        0        0       37 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/marqo/__init__.py
--rw-r--r--   0        0        0     5242 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/marqo/marqo.py
--rw-r--r--   0        0        0       29 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/mistral/__init__.py
--rw-r--r--   0        0        0     1508 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/mistral/mistral.py
--rw-r--r--   0        0        0       27 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ollama/__init__.py
--rw-r--r--   0        0        0     2418 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/ollama/ollama.py
--rw-r--r--   0        0        0       86 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/openai/__init__.py
--rw-r--r--   0        0        0     4764 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/openai/openai_chat.py
--rw-r--r--   0        0        0     1260 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/openai/openai_embeddings.py
--rw-r--r--   0        0        0    12803 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/remote.py
--rw-r--r--   0        0        0     4957 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/types/__init__.py
--rw-r--r--   0        0        0     2247 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/utils.py
--rw-r--r--   0        0        0       48 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/vannadb/__init__.py
--rw-r--r--   0        0        0     5644 2024-04-05 14:52:15.498886 vanna-0.3.3/src/vanna/vannadb/vannadb_vector.py
--rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 vanna-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     7922 2024-04-12 19:54:05.263634 vanna-0.3.4/README.md
+-rw-r--r--   0        0        0     1247 2024-04-12 19:54:05.279634 vanna-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8725 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0        0        0     2849 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0        0        0      116 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/ZhipuAI/__init__.py
+-rw-r--r--   0        0        0     9248 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/anthropic/__init__.py
+-rw-r--r--   0        0        0     2615 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/anthropic/anthropic_chat.py
+-rw-r--r--   0        0        0       28 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/base/__init__.py
+-rw-r--r--   0        0        0    58100 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/base/base.py
+-rw-r--r--   0        0        0       50 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/chromadb/__init__.py
+-rw-r--r--   0        0        0     8461 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/chromadb/chromadb_vector.py
+-rw-r--r--   0        0        0      717 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/exceptions/__init__.py
+-rw-r--r--   0        0        0    21211 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/flask/__init__.py
+-rw-r--r--   0        0        0   180924 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/flask/assets.py
+-rw-r--r--   0        0        0      313 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/local.py
+-rw-r--r--   0        0        0       37 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/marqo/__init__.py
+-rw-r--r--   0        0        0     5242 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/marqo/marqo.py
+-rw-r--r--   0        0        0       29 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/mistral/__init__.py
+-rw-r--r--   0        0        0     1508 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/mistral/mistral.py
+-rw-r--r--   0        0        0       27 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/ollama/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/ollama/ollama.py
+-rw-r--r--   0        0        0       86 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/openai/__init__.py
+-rw-r--r--   0        0        0     4764 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/openai/openai_chat.py
+-rw-r--r--   0        0        0     1260 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/openai/openai_embeddings.py
+-rw-r--r--   0        0        0     1856 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/remote.py
+-rw-r--r--   0        0        0     4957 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/types/__init__.py
+-rw-r--r--   0        0        0     2247 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/utils.py
+-rw-r--r--   0        0        0       48 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/vannadb/__init__.py
+-rw-r--r--   0        0        0     6168 2024-04-12 19:54:05.279634 vanna-0.3.4/src/vanna/vannadb/vannadb_vector.py
+-rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 vanna-0.3.4/PKG-INFO
```

### Comparing `vanna-0.3.3/README.md` & `vanna-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/pyproject.toml` & `vanna-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vanna"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_Chat.py` & `vanna-0.3.4/src/vanna/ZhipuAI/ZhipuAI_Chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return len(string) / 4
 
     @staticmethod
     def add_ddl_to_prompt(
         initial_prompt: str, ddl_list: List[str], max_tokens: int = 14000
     ) -> str:
         if len(ddl_list) > 0:
-            initial_prompt += f"\nYou may use the following DDL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
+            initial_prompt += "\nYou may use the following DDL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
 
             for ddl in ddl_list:
                 if (
                     ZhipuAI_Chat.str_to_approx_token_count(initial_prompt)
                     + ZhipuAI_Chat.str_to_approx_token_count(ddl)
                     < max_tokens
                 ):
@@ -53,15 +53,15 @@
         return initial_prompt
 
     @staticmethod
     def add_documentation_to_prompt(
         initial_prompt: str, documentation_List: List[str], max_tokens: int = 14000
     ) -> str:
         if len(documentation_List) > 0:
-            initial_prompt += f"\nYou may use the following documentation as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
+            initial_prompt += "\nYou may use the following documentation as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
 
             for documentation in documentation_List:
                 if (
                     ZhipuAI_Chat.str_to_approx_token_count(initial_prompt)
                     + ZhipuAI_Chat.str_to_approx_token_count(documentation)
                     < max_tokens
                 ):
@@ -70,15 +70,15 @@
         return initial_prompt
 
     @staticmethod
     def add_sql_to_prompt(
         initial_prompt: str, sql_List: List[str], max_tokens: int = 14000
     ) -> str:
         if len(sql_List) > 0:
-            initial_prompt += f"\nYou may use the following SQL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
+            initial_prompt += "\nYou may use the following SQL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
 
             for question in sql_List:
                 if (
                     ZhipuAI_Chat.str_to_approx_token_count(initial_prompt)
                     + ZhipuAI_Chat.str_to_approx_token_count(question["sql"])
                     < max_tokens
                 ):
```

### Comparing `vanna-0.3.3/src/vanna/ZhipuAI/ZhipuAI_embeddings.py` & `vanna-0.3.4/src/vanna/ZhipuAI/ZhipuAI_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/__init__.py` & `vanna-0.3.4/src/vanna/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/anthropic/anthropic_chat.py` & `vanna-0.3.4/src/vanna/anthropic/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/base/base.py` & `vanna-0.3.4/src/vanna/base/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,26 @@
         )
         self.log(prompt)
         llm_response = self.submit_prompt(prompt, **kwargs)
         self.log(llm_response)
         return self.extract_sql(llm_response)
 
     def extract_sql(self, llm_response: str) -> str:
+        # If the llm_response is not markdown formatted, extract sql by finding select and ; in the response
+        sql = re.search(r"SELECT.*?;", llm_response, re.DOTALL)
+        if sql:
+            self.log(f"Output from LLM: {llm_response} \nExtracted SQL: {sql.group(0)}"
+            )
+            return sql.group(0)
+
+        # If the llm_response contains a CTE (with clause), extract the sql bewteen WITH and ;
+        sql = re.search(r"WITH.*?;", llm_response, re.DOTALL)
+        if sql:
+            self.log(f"Output from LLM: {llm_response} \nExtracted SQL: {sql.group(0)}")
+            return sql.group(0)
         # If the llm_response contains a markdown code block, with or without the sql tag, extract the sql from it
         sql = re.search(r"```sql\n(.*)```", llm_response, re.DOTALL)
         if sql:
             self.log(f"Output from LLM: {llm_response} \nExtracted SQL: {sql.group(1)}")
             return sql.group(1)
 
         sql = re.search(r"```(.*)```", llm_response, re.DOTALL)
@@ -359,15 +371,15 @@
     def str_to_approx_token_count(self, string: str) -> int:
         return len(string) / 4
 
     def add_ddl_to_prompt(
         self, initial_prompt: str, ddl_list: list[str], max_tokens: int = 14000
     ) -> str:
         if len(ddl_list) > 0:
-            initial_prompt += f"\nYou may use the following DDL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
+            initial_prompt += "\nYou may use the following DDL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
 
             for ddl in ddl_list:
                 if (
                     self.str_to_approx_token_count(initial_prompt)
                     + self.str_to_approx_token_count(ddl)
                     < max_tokens
                 ):
@@ -378,15 +390,15 @@
     def add_documentation_to_prompt(
         self,
         initial_prompt: str,
         documentation_list: list[str],
         max_tokens: int = 14000,
     ) -> str:
         if len(documentation_list) > 0:
-            initial_prompt += f"\nYou may use the following documentation as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
+            initial_prompt += "\nYou may use the following documentation as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
 
             for documentation in documentation_list:
                 if (
                     self.str_to_approx_token_count(initial_prompt)
                     + self.str_to_approx_token_count(documentation)
                     < max_tokens
                 ):
@@ -394,15 +406,15 @@
 
         return initial_prompt
 
     def add_sql_to_prompt(
         self, initial_prompt: str, sql_list: list[str], max_tokens: int = 14000
     ) -> str:
         if len(sql_list) > 0:
-            initial_prompt += f"\nYou may use the following SQL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
+            initial_prompt += "\nYou may use the following SQL statements as a reference for what tables might be available. Use responses to past questions also to guide you:\n\n"
 
             for question in sql_list:
                 if (
                     self.str_to_approx_token_count(initial_prompt)
                     + self.str_to_approx_token_count(question["sql"])
                     < max_tokens
                 ):
@@ -886,14 +898,102 @@
                 except Exception as e:
                     conn.rollback()
                     raise e
 
         self.run_sql_is_set = True
         self.run_sql = run_sql_mysql
 
+    def connect_to_oracle(
+    self,
+    user: str = None,
+    password: str = None,
+    dsn: str = None,
+    ):
+
+        """
+        Connect to an Oracle db using oracledb package. This is just a helper function to set [`vn.run_sql`][vanna.base.base.VannaBase.run_sql]
+        **Example:**
+        ```python
+        vn.connect_to_oracle(
+        user="username",
+        password="password",
+        dns="host:port/sid",
+        )
+        ```
+        Args:
+            USER (str): Oracle db user name.
+            PASSWORD (str): Oracle db user password.
+            DSN (str): Oracle db host ip - host:port/sid.
+        """
+
+        try:
+            import oracledb
+        except ImportError:
+
+            raise DependencyError(
+                "You need to install required dependencies to execute this method,"
+                " run command: \npip install oracledb"
+            )
+
+        if not dsn:
+            dsn = os.getenv("DSN")
+
+        if not dsn:
+            raise ImproperlyConfigured("Please set your Oracle dsn which should include host:port/sid")
+
+        if not user:
+            user = os.getenv("USER")
+
+        if not user:
+            raise ImproperlyConfigured("Please set your Oracle db user")
+
+        if not password:
+            password = os.getenv("PASSWORD")
+
+        if not password:
+            raise ImproperlyConfigured("Please set your Oracle db password")
+
+        conn = None
+
+        try:
+            conn = oracledb.connect(
+                user=user,
+                password=password,
+                dsn=dsn,
+                )
+        except oracledb.Error as e:
+            raise ValidationError(e)
+
+        def run_sql_oracle(sql: str) -> Union[pd.DataFrame, None]:
+            if conn:
+                try:
+                    sql = sql.rstrip()
+                    if sql.endswith(';'): #fix for a known problem with Oracle db where an extra ; will cause an error.
+                        sql = sql[:-1]
+
+                    cs = conn.cursor()
+                    cs.execute(sql)
+                    results = cs.fetchall()
+
+                    # Create a pandas dataframe from the results
+                    df = pd.DataFrame(
+                        results, columns=[desc[0] for desc in cs.description]
+                    )
+                    return df
+
+                except oracledb.Error as e:
+                    conn.rollback()
+                    raise ValidationError(e)
+
+                except Exception as e:
+                    conn.rollback()
+                    raise e
+
+        self.run_sql_is_set = True
+        self.run_sql = run_sql_oracle
 
     def connect_to_bigquery(self, cred_file_path: str = None, project_id: str = None):
         """
         Connect to gcs using the bigquery connector. This is just a helper function to set [`vn.run_sql`][vanna.base.base.VannaBase.run_sql]
         **Example:**
         ```python
         vn.connect_to_bigquery(
@@ -1234,15 +1334,15 @@
             sql (str): The SQL query to train on.
             ddl (str):  The DDL statement.
             documentation (str): The documentation to train on.
             plan (TrainingPlan): The training plan to train on.
         """
 
         if question and not sql:
-            raise ValidationError(f"Please also provide a SQL query")
+            raise ValidationError("Please also provide a SQL query")
 
         if documentation:
             print("Adding documentation....")
             return self.add_documentation(documentation)
 
         if sql:
             if question is None:
```

### Comparing `vanna-0.3.3/src/vanna/chromadb/chromadb_vector.py` & `vanna-0.3.4/src/vanna/chromadb/chromadb_vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import uuid
 from typing import List
 
 import chromadb
 import pandas as pd
 from chromadb.config import Settings
 from chromadb.utils import embedding_functions
 
@@ -12,25 +11,22 @@
 
 default_ef = embedding_functions.DefaultEmbeddingFunction()
 
 
 class ChromaDB_VectorStore(VannaBase):
     def __init__(self, config=None):
         VannaBase.__init__(self, config=config)
+        if config is None:
+            config = {}
 
-        if config is not None:
-            path = config.get("path", ".")
-            self.embedding_function = config.get("embedding_function", default_ef)
-            curr_client = config.get("client", "persistent")
-            self.n_results = config.get("n_results", 10)
-        else:
-            path = "."
-            self.embedding_function = default_ef
-            curr_client = "persistent"  # defaults to persistent storage
-            self.n_results = 10  # defaults to 10 documents
+        path = config.get("path", ".")
+        self.embedding_function = config.get("embedding_function", default_ef)
+        curr_client = config.get("client", "persistent")
+        collection_metadata = config.get("collection_metadata", None)
+        self.n_results = config.get("n_results", 10)
 
         if curr_client == "persistent":
             self.chroma_client = chromadb.PersistentClient(
                 path=path, settings=Settings(anonymized_telemetry=False)
             )
         elif curr_client == "in-memory":
             self.chroma_client = chromadb.EphemeralClient(
@@ -39,21 +35,27 @@
         elif isinstance(curr_client, chromadb.api.client.Client):
             # allow providing client directly
             self.chroma_client = curr_client
         else:
             raise ValueError(f"Unsupported client was set in config: {curr_client}")
 
         self.documentation_collection = self.chroma_client.get_or_create_collection(
-            name="documentation", embedding_function=self.embedding_function
+            name="documentation",
+            embedding_function=self.embedding_function,
+            metadata=collection_metadata,
         )
         self.ddl_collection = self.chroma_client.get_or_create_collection(
-            name="ddl", embedding_function=self.embedding_function
+            name="ddl",
+            embedding_function=self.embedding_function,
+            metadata=collection_metadata,
         )
         self.sql_collection = self.chroma_client.get_or_create_collection(
-            name="sql", embedding_function=self.embedding_function
+            name="sql",
+            embedding_function=self.embedding_function,
+            metadata=collection_metadata,
         )
 
     def generate_embedding(self, data: str, **kwargs) -> List[float]:
         embedding = self.embedding_function([data])
         if len(embedding) == 1:
             return embedding[0]
         return embedding
```

### Comparing `vanna-0.3.3/src/vanna/exceptions/__init__.py` & `vanna-0.3.4/src/vanna/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/flask/__init__.py` & `vanna-0.3.4/src/vanna/flask/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
 
             # Return 404
             return "File not found", 404
 
         # Proxy the /vanna.svg file to the remote server
         @self.flask_app.route("/vanna.svg")
         def proxy_vanna_svg():
-            remote_url = f"https://vanna.ai/img/vanna.svg"
+            remote_url = "https://vanna.ai/img/vanna.svg"
             response = requests.get(remote_url, stream=True)
 
             # Check if the request to the remote URL was successful
             if response.status_code == 200:
                 excluded_headers = [
                     "content-encoding",
                     "content-length",
```

### Comparing `vanna-0.3.3/src/vanna/flask/assets.py` & `vanna-0.3.4/src/vanna/flask/assets.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/marqo/marqo.py` & `vanna-0.3.4/src/vanna/marqo/marqo.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/mistral/mistral.py` & `vanna-0.3.4/src/vanna/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/ollama/ollama.py` & `vanna-0.3.4/src/vanna/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/openai/openai_chat.py` & `vanna-0.3.4/src/vanna/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/openai/openai_embeddings.py` & `vanna-0.3.4/src/vanna/openai/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/types/__init__.py` & `vanna-0.3.4/src/vanna/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/utils.py` & `vanna-0.3.4/src/vanna/utils.py`

 * *Files identical despite different names*

### Comparing `vanna-0.3.3/src/vanna/vannadb/vannadb_vector.py` & `vanna-0.3.4/src/vanna/vannadb/vannadb_vector.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,57 +3,41 @@
 from io import StringIO
 
 import pandas as pd
 import requests
 
 from ..base import VannaBase
 from ..types import (
-    DataFrameJSON,
-    Question,
-    QuestionSQLPair,
-    Status,
-    StatusWithId,
-    StringData,
-    TrainingData,
+  DataFrameJSON,
+  NewOrganization,
+  OrganizationList,
+  Question,
+  QuestionSQLPair,
+  Status,
+  StatusWithId,
+  StringData,
+  TrainingData,
 )
+from ..utils import sanitize_model_name
 
 
 class VannaDB_VectorStore(VannaBase):
     def __init__(self, vanna_model: str, vanna_api_key: str, config=None):
         VannaBase.__init__(self, config=config)
 
         self._model = vanna_model
         self._api_key = vanna_api_key
 
         self._endpoint = (
             "https://ask.vanna.ai/rpc"
             if config is None or "endpoint" not in config
             else config["endpoint"]
         )
-        self._unauthenticated_endpoint = (
-            "https://ask.vanna.ai/unauthenticated_rpc"
-            if config is None or "unauthenticated_endpoint" not in config
-            else config["unauthenticated_endpoint"]
-        )
         self.related_training_data = {}
 
-    def _unauthenticated_rpc_call(self, method, params):
-        headers = {
-            "Content-Type": "application/json",
-        }
-        data = {
-            "method": method,
-            "params": [self._dataclass_to_dict(obj) for obj in params],
-        }
-
-        response = requests.post(
-            self._unauthenticated_endpoint, headers=headers, data=json.dumps(data)
-        )
-        return response.json()
-
     def _rpc_call(self, method, params):
         if method != "list_orgs":
             headers = {
                 "Content-Type": "application/json",
                 "Vanna-Key": self._api_key,
                 "Vanna-Org": self._model,
             }
@@ -71,14 +55,61 @@
 
         response = requests.post(self._endpoint, headers=headers, data=json.dumps(data))
         return response.json()
 
     def _dataclass_to_dict(self, obj):
         return dataclasses.asdict(obj)
 
+    def create_model(self, model: str, **kwargs) -> bool:
+        """
+        **Example:**
+        ```python
+        success = vn.create_model("my_model")
+        ```
+        Create a new model.
+
+        Args:
+            model (str): The name of the model to create.
+
+        Returns:
+            bool: True if the model was created, False otherwise.
+        """
+        model = sanitize_model_name(model)
+        params = [NewOrganization(org_name=model, db_type="")]
+
+        d = self._rpc_call(method="create_org", params=params)
+
+        if "result" not in d:
+            return False
+
+        status = Status(**d["result"])
+
+        return status.success
+
+    def get_models(self) -> list:
+        """
+        **Example:**
+        ```python
+        models = vn.get_models()
+        ```
+
+        List the models that belong to the user.
+
+        Returns:
+            List[str]: A list of model names.
+        """
+        d = self._rpc_call(method="list_my_models", params=[])
+
+        if "result" not in d:
+            return []
+
+        orgs = OrganizationList(**d["result"])
+
+        return orgs.organizations
+
     def generate_embedding(self, data: str, **kwargs) -> list[float]:
         # This is done server-side
         pass
 
     def add_question_sql(self, question: str, sql: str, **kwargs) -> str:
         if "tag" in kwargs:
             tag = kwargs["tag"]
@@ -137,15 +168,15 @@
 
     def remove_training_data(self, id: str, **kwargs) -> bool:
         params = [StringData(data=id)]
 
         d = self._rpc_call(method="remove_training_data", params=params)
 
         if "result" not in d:
-            raise Exception(f"Error removing training data")
+            raise Exception("Error removing training data")
 
         status = Status(**d["result"])
 
         if not status.success:
             raise Exception(f"Error removing training data: {status.message}")
 
         return status.success
```

### Comparing `vanna-0.3.3/PKG-INFO` & `vanna-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.3.3
+Version: 0.3.4
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

