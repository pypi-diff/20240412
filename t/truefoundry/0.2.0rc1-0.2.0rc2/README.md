# Comparing `tmp/truefoundry-0.2.0rc1.tar.gz` & `tmp/truefoundry-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.0rc1.tar", max compression
+gzip compressed data, was "truefoundry-0.2.0rc2.tar", max compression
```

## Comparing `truefoundry-0.2.0rc1.tar` & `truefoundry-0.2.0rc2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      871 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/README.md
--rw-r--r--   0        0        0     1487 2024-04-12 05:58:10.178581 truefoundry-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6321 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4428 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2289 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    10660 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0      435 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0       54 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      787 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5823 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     5059 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     1751 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0     5358 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0        0 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0     1585 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       29 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0       39 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      151 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/README.md
+-rw-r--r--   0        0        0     1147 2024-04-12 07:12:28.672483 truefoundry-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4428 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2348 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    10660 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0      435 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0       54 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5890 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5076 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     1751 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0     5358 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0     1585 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc2/PKG-INFO
```

### Comparing `truefoundry-0.2.0rc1/README.md` & `truefoundry-0.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/pyproject.toml` & `truefoundry-0.2.0rc2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.0rc1"
+version = "0.2.0rc2"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
 servicefoundry = "0.10.6"
 mlfoundry = { version = "0.10.9", optional = true }
-openai = {version = "^1.16.2", optional = true}
-docker = {version = "^7.0.0", optional = true}
-pydantic = {version = "^2.6.4", optional = true}
-rich = {version = "^13.7.1", optional = true}
-requests = {version = "^2.31.0", optional = true}
-python-dotenv = {version = "^1.0.1", optional = true}
-gitignorefile = {version = "^1.1.2", optional = true}
-gitpython = {version = "^3.1.43", optional = true}
+openai = "^1.16.2"
+docker = "^7.0.0"
+pydantic = ">=1.10.0,<3"
+rich = "^13.7.1"
+requests = "^2.31.0"
+python-dotenv = "^1.0.1"
+gitignorefile = "^1.1.2"
+gitpython = "^3.1.43"
 
 [tool.poetry.extras]
 ml = ["mlfoundry"]
-autodeploy = ["openai", "docker", "pydantic", "rich", "requests", "python-dotenv", "gitignorefile", "gitpython"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.5"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 from openai.types.shared_params.function_definition import FunctionDefinition
 from pydantic import BaseModel, ValidationError
 
 from truefoundry.autodeploy.constants import AUTODEPLOY_MODEL_NAME
 from truefoundry.autodeploy.logger import logger
 from truefoundry.autodeploy.tools import Event, RequestEvent, Tool
+from truefoundry.autodeploy.utils.pydantic_compat import model_dump, model_json_schema
 
 
 def llm(
     openai_client: OpenAI,
     messages: List[ChatCompletionMessageParam],
     tools: List[ChatCompletionToolParam],
     model: str,
@@ -46,15 +47,15 @@
 
 
 def format_tool_response(
     response: BaseModel, tool_call_id: str
 ) -> ChatCompletionToolMessageParam:
     return ChatCompletionToolMessageParam(
         role="tool",
-        content=json.dumps(response.model_dump(), indent=1),
+        content=json.dumps(model_dump(response), indent=1),
         tool_call_id=tool_call_id,
     )
 
 
 def format_user_response(response: str) -> ChatCompletionUserMessageParam:
     return ChatCompletionUserMessageParam(
         role="user",
@@ -68,25 +69,25 @@
     descriptions = []
     for tool in tools:
         tool = ChatCompletionToolParam(
             type="function",
             function=FunctionDefinition(
                 name=tool.__class__.__name__,
                 description=tool.description.strip(),
-                parameters=tool.Request.model_json_schema(),
+                parameters=model_json_schema(tool.Request),
             ),
         )
         descriptions.append(tool)
 
     if response:
         tool = ChatCompletionToolParam(
             type="function",
             function=FunctionDefinition(
                 name="Response",
-                parameters=response.model_json_schema(),
+                parameters=model_json_schema(response),
             ),
         )
         descriptions.append(tool)
 
     return descriptions
```

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/tester.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict
+from typing import Dict, Optional
 
 import docker
 from openai import OpenAI
 from pydantic import Field
 from rich.console import Console
 
 from truefoundry.autodeploy.agents.base import Agent
@@ -35,14 +35,15 @@
     """
     max_iter = 30
 
     class Request(RequestEvent):
         project_identity: ProjectIdentifier.Response
         image_tag: str
         command: str
+        port_to_be_exposed: Optional[int] = None
 
     class Response(ResponseEvent):
         successful: bool = Field(..., description="is everything fine?")
         justification: str = Field(
             ...,
             description="""
 Why was the testing a failure or successful?
```

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/ask.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Iterable
 
 from rich.console import Console
 
 from truefoundry.autodeploy.tools.base import Event, RequestEvent, ResponseEvent, Tool
+from truefoundry.autodeploy.utils.pydantic_compat import model_dump
 
 
 class AskQuestion(Event):
     question: str
 
     def render(self, console: Console) -> str:
         console.print(f"[bold magenta]TFY-Agent:[/] {self.question}")
@@ -24,9 +25,9 @@
     class Request(RequestEvent):
         question: str
 
     class Response(ResponseEvent):
         response: str
 
     def run(self, request: Ask.Request) -> Iterable[Event]:
-        response = yield AskQuestion(**request.model_dump())
+        response = yield AskQuestion(**model_dump(request))
         return Ask.Response(response=response)
```

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Event,
     Message,
     RequestEvent,
     ResponseEvent,
     Tool,
 )
 from truefoundry.autodeploy.utils.diff import LLMDiff
+from truefoundry.autodeploy.utils.pydantic_compat import model_dump
 
 
 class CommitConfirmation(Event):
     patch: str
     commit_message: str
 
     def render(self, console: Console) -> Optional["Commit.Response"]:
@@ -112,15 +113,15 @@
 
     def run(
         self,
         request: Commit.Request,
     ) -> Generator[Event, Any, ResponseEvent]:
         fp = tempfile.NamedTemporaryFile(mode="w", delete=False)
         try:
-            interaction_response = yield CommitConfirmation(**request.model_dump())
+            interaction_response = yield CommitConfirmation(**model_dump(request))
             if isinstance(interaction_response, Commit.Response):
                 return interaction_response
             fp.write(request.patch)
             fp.close()
             self.repo.git.apply(["--recount", "--unidiff-zero", fp.name], index=True)
             self.repo.index.commit(message=request.commit_message)
             yield Message(
```

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 """
 
     class Request(RequestEvent):
         image_tag: str
         ports: Optional[Dict[str, int]] = Field(
             None,
             description="""
+Ports to expose.
 The keys of the dictionary are the ports to bind inside the container in 'port'.
 The values are the ports to open on the host""",
         )
         command: str
 
         def render(self, console: Console):
             console.print(
```

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/list_files.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/send_request.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.0rc2/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/truefoundry/cli/__main__.py` & `truefoundry-0.2.0rc2/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc1/PKG-INFO` & `truefoundry-0.2.0rc2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: autodeploy
 Provides-Extra: ml
-Requires-Dist: docker (>=7.0.0,<8.0.0) ; extra == "autodeploy"
-Requires-Dist: gitignorefile (>=1.1.2,<2.0.0) ; extra == "autodeploy"
-Requires-Dist: gitpython (>=3.1.43,<4.0.0) ; extra == "autodeploy"
+Requires-Dist: docker (>=7.0.0,<8.0.0)
+Requires-Dist: gitignorefile (>=1.1.2,<2.0.0)
+Requires-Dist: gitpython (>=3.1.43,<4.0.0)
 Requires-Dist: mlfoundry (==0.10.9) ; extra == "ml"
-Requires-Dist: openai (>=1.16.2,<2.0.0) ; extra == "autodeploy"
-Requires-Dist: pydantic (>=2.6.4,<3.0.0) ; extra == "autodeploy"
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) ; extra == "autodeploy"
-Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "autodeploy"
-Requires-Dist: rich (>=13.7.1,<14.0.0) ; extra == "autodeploy"
+Requires-Dist: openai (>=1.16.2,<2.0.0)
+Requires-Dist: pydantic (>=1.10.0,<3)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: servicefoundry (==0.10.6)
 Description-Content-Type: text/markdown
 
 # Truefoundry
 
 TrueFoundry library to help you interact with the platform programmatically by
```

