# Comparing `tmp/langchain_google_vertexai-0.1.3.tar.gz` & `tmp/langchain_google_vertexai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_vertexai-0.1.3.tar", max compression
+gzip compressed data, was "langchain_google_vertexai-1.0.1.tar", max compression
```

## Comparing `langchain_google_vertexai-0.1.3.tar` & `langchain_google_vertexai-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/LICENSE
--rw-r--r--   0        0        0     2594 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/README.md
--rw-r--r--   0        0        0     1853 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/__init__.py
--rw-r--r--   0        0        0     3255 2024-04-11 16:50:49.936082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_anthropic_utils.py
--rw-r--r--   0        0        0    11390 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_base.py
--rw-r--r--   0        0        0      151 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_enums.py
--rw-r--r--   0        0        0     8169 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_image_utils.py
--rw-r--r--   0        0        0     6591 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/_utils.py
--rw-r--r--   0        0        0     2511 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/callbacks.py
--rw-r--r--   0        0        0     5471 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/chains.py
--rw-r--r--   0        0        0    37792 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/chat_models.py
--rw-r--r--   0        0        0    16400 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/embeddings.py
--rw-r--r--   0        0        0     6304 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/functions_utils.py
--rw-r--r--   0        0        0    12748 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/gemma.py
--rw-r--r--   0        0        0    11414 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/llms.py
--rw-r--r--   0        0        0     8224 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/model_garden.py
--rw-r--r--   0        0        0        0 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/py.typed
--rw-r--r--   0        0        0      471 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/__init__.py
--rw-r--r--   0        0        0     4679 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_sdk_manager.py
--rw-r--r--   0        0        0     6103 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_searcher.py
--rw-r--r--   0        0        0     5436 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_utils.py
--rw-r--r--   0        0        0     8050 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/document_storage.py
--rw-r--r--   0        0        0    15958 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/vectorstores.py
--rw-r--r--   0        0        0    18548 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/langchain_google_vertexai/vision_models.py
--rw-r--r--   0        0        0     3366 2024-04-11 16:50:49.940082 langchain_google_vertexai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2594 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/README.md
+-rw-r--r--   0        0        0     1853 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/__init__.py
+-rw-r--r--   0        0        0     3255 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_anthropic_utils.py
+-rw-r--r--   0        0        0    11390 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_base.py
+-rw-r--r--   0        0        0      151 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_enums.py
+-rw-r--r--   0        0        0     8169 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_image_utils.py
+-rw-r--r--   0        0        0     6591 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/_utils.py
+-rw-r--r--   0        0        0     2511 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/callbacks.py
+-rw-r--r--   0        0        0     6062 2024-04-12 17:49:34.407009 langchain_google_vertexai-1.0.1/langchain_google_vertexai/chains.py
+-rw-r--r--   0        0        0    39128 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/chat_models.py
+-rw-r--r--   0        0        0    16400 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/embeddings.py
+-rw-r--r--   0        0        0     6491 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/functions_utils.py
+-rw-r--r--   0        0        0    12748 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/gemma.py
+-rw-r--r--   0        0        0    11722 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/llms.py
+-rw-r--r--   0        0        0     8224 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/model_garden.py
+-rw-r--r--   0        0        0        0 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/py.typed
+-rw-r--r--   0        0        0      471 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     4679 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_sdk_manager.py
+-rw-r--r--   0        0        0     6103 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_searcher.py
+-rw-r--r--   0        0        0     5436 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_utils.py
+-rw-r--r--   0        0        0     8050 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/document_storage.py
+-rw-r--r--   0        0        0    15958 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/vectorstores.py
+-rw-r--r--   0        0        0    18548 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/langchain_google_vertexai/vision_models.py
+-rw-r--r--   0        0        0     3366 2024-04-12 17:49:34.411010 langchain_google_vertexai-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 langchain_google_vertexai-1.0.1/PKG-INFO
```

### Comparing `langchain_google_vertexai-0.1.3/LICENSE` & `langchain_google_vertexai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/README.md` & `langchain_google_vertexai-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/__init__.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/_anthropic_utils.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/_base.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_base.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/_image_utils.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_image_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/_utils.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/callbacks.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/chains.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/chains.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     BaseGenerationOutputParser,
     BaseOutputParser,
     StrOutputParser,
 )
 from langchain_core.prompts import BasePromptTemplate, ChatPromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable
+from vertexai.generative_models._generative_models import (  # type: ignore
+    ToolConfig,
+)
 
 from langchain_google_vertexai.functions_utils import PydanticFunctionsOutputParser
 
 
 def get_output_parser(
     functions: Sequence[Type[BaseModel]],
 ) -> Union[BaseOutputParser, BaseGenerationOutputParser]:
@@ -46,15 +49,29 @@
 
 def _create_structured_runnable_extra_step(
     functions: Sequence[Type[BaseModel]],
     llm: Runnable,
     *,
     prompt: Optional[BasePromptTemplate] = None,
 ) -> Runnable:
-    llm_with_functions = llm.bind(functions=functions)
+    names = [schema.schema()["title"] for schema in functions]
+    if hasattr(llm, "is_gemini_advanced") and llm._is_gemini_advanced:  # type: ignore
+        llm_with_functions = llm.bind(
+            functions=functions,
+            tool_config={
+                "function_calling_config": {
+                    "mode": ToolConfig.FunctionCallingConfig.Mode.ANY,
+                    "allowed_function_names": names,
+                }
+            },
+        )
+    else:
+        llm_with_functions = llm.bind(
+            functions=functions,
+        )
     parsing_prompt = ChatPromptTemplate.from_template(
         "You are a world class algorithm for recording entities.\nMake calls "
         "to the relevant function to record the entities in the following "
         "input:\n{output}\nTip: Make sure to answer in the correct format."
     )
     output_parser = get_output_parser(functions)
     if prompt:
```

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/chat_models.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/chat_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from vertexai.generative_models import (  # type: ignore
     Candidate,
     Content,
     GenerativeModel,
     Part,
 )
+from vertexai.generative_models._generative_models import (  # type: ignore
+    ToolConfig,
+)
 from vertexai.language_models import (  # type: ignore
     ChatMessage,
     ChatModel,
     ChatSession,
     CodeChatModel,
     CodeChatSession,
     InputOutputTextPair,
@@ -85,14 +88,15 @@
 from langchain_google_vertexai._utils import (
     get_generation_info,
     is_codey_model,
     is_gemini_model,
 )
 from langchain_google_vertexai.functions_utils import (
     _format_tool_config,
+    _format_tool_to_vertex_function,
     _format_tools_to_vertex_tool,
 )
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -157,15 +161,15 @@
 
     def _convert_to_parts(message: BaseMessage) -> List[Part]:
         raw_content = message.content
         if isinstance(raw_content, str):
             raw_content = [raw_content]
         return [_convert_to_prompt(part) for part in raw_content]
 
-    vertex_messages = []
+    vertex_messages: List[Content] = []
     convert_system_message_to_human_content = None
     system_instruction = None
     for i, message in enumerate(history):
         if isinstance(message, SystemMessage):
             if system_instruction is not None:
                 raise ValueError(
                     "Detected more than one SystemMessage in the list of messages."
@@ -380,14 +384,18 @@
 
 class ChatVertexAI(_VertexAICommon, BaseChatModel):
     """`Vertex AI` Chat large language models API."""
 
     model_name: str = "chat-bison"
     "Underlying model name."
     examples: Optional[List[BaseMessage]] = None
+    tuned_model_name: Optional[str] = None
+    """The name of a tuned model. If tuned_model_name is passed
+    model_name will be used to determine the model family
+    """
     convert_system_message_to_human: bool = False
     """[Deprecated] Since new Gemini models support setting a System Message,
     setting this parameter to True is discouraged.
     """
 
     @classmethod
     def is_lc_serializable(self) -> bool:
@@ -399,39 +407,59 @@
         return ["langchain", "chat_models", "vertexai"]
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that the python package exists in environment."""
         is_gemini = is_gemini_model(values["model_name"])
         safety_settings = values["safety_settings"]
+        tuned_model_name = values.get("tuned_model_name")
 
         if safety_settings and not is_gemini:
             raise ValueError("Safety settings are only supported for Gemini models")
 
         cls._init_vertexai(values)
+
+        if tuned_model_name:
+            generative_model_name = values["tuned_model_name"]
+        else:
+            generative_model_name = values["model_name"]
+
         if is_gemini:
             values["client"] = GenerativeModel(
-                model_name=values["model_name"], safety_settings=safety_settings
+                model_name=generative_model_name,
+                safety_settings=safety_settings,
             )
             values["client_preview"] = GenerativeModel(
-                model_name=values["model_name"], safety_settings=safety_settings
+                model_name=generative_model_name,
+                safety_settings=safety_settings,
             )
         else:
             if is_codey_model(values["model_name"]):
                 model_cls = CodeChatModel
                 model_cls_preview = PreviewCodeChatModel
             else:
                 model_cls = ChatModel
                 model_cls_preview = PreviewChatModel
-            values["client"] = model_cls.from_pretrained(values["model_name"])
+            values["client"] = model_cls.from_pretrained(generative_model_name)
             values["client_preview"] = model_cls_preview.from_pretrained(
-                values["model_name"]
+                generative_model_name
             )
         return values
 
+    @property
+    def _is_gemini_advanced(self) -> bool:
+        try:
+            if float(self.model_name.split("-")[1]) > 1.0:
+                return True
+        except ValueError:
+            pass
+        except IndexError:
+            pass
+        return False
+
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         stream: Optional[bool] = None,
         **kwargs: Any,
@@ -715,15 +743,14 @@
         params = self._prepare_params(stop=stop, stream=True, **kwargs)
         safety_settings = params.pop("safety_settings", None)
         system_instruction, history_gemini = _parse_chat_history_gemini(
             messages,
             project=self.project,
             convert_system_message_to_human=self.convert_system_message_to_human,
         )
-        message = history_gemini.pop()
         self.client = _get_client_with_sys_instruction(
             client=self.client,
             system_instruction=system_instruction,
             model_name=self.model_name,
         )
         raw_tools = params.pop("functions") if "functions" in params else None
         tools = _format_tools_to_vertex_tool(raw_tools) if raw_tools else None
@@ -858,29 +885,44 @@
             raise ValueError(f"Received unsupported arguments {kwargs}")
         if isinstance(schema, type) and issubclass(schema, BaseModel):
             parser: OutputParserLike = PydanticOutputFunctionsParser(
                 pydantic_schema=schema
             )
         else:
             parser = JsonOutputFunctionsParser()
-        llm = self.bind(functions=[schema])
+
+        name = _format_tool_to_vertex_function(schema)["name"]
+
+        if self._is_gemini_advanced:
+            llm = self.bind(
+                functions=[schema],
+                tool_config={
+                    "function_calling_config": {
+                        "mode": ToolConfig.FunctionCallingConfig.Mode.ANY,
+                        "allowed_function_names": [name],
+                    }
+                },
+            )
+        else:
+            llm = self.bind(functions=[schema])
         if include_raw:
             parser_with_fallback = RunnablePassthrough.assign(
                 parsed=itemgetter("raw") | parser, parsing_error=lambda _: None
             ).with_fallbacks(
                 [RunnablePassthrough.assign(parsed=lambda _: None)],
                 exception_key="parsing_error",
             )
             return {"raw": llm} | parser_with_fallback
         else:
             return llm | parser
 
     def bind_tools(
         self,
         tools: Sequence[Union[Type[BaseModel], Callable, BaseTool]],
+        tool_config: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         """Bind tool-like objects to this chat model.
 
         Assumes model is compatible with Vertex tool-calling API.
 
         Args:
@@ -899,15 +941,15 @@
                 formatted_tools.append(schema)
             elif callable(schema):
                 formatted_tools.append(tool_from_callable(schema))  # type: ignore
             else:
                 raise ValueError(
                     "Tool must be a BaseTool, Pydantic model, or callable."
                 )
-        return super().bind(functions=formatted_tools, **kwargs)
+        return self.bind(functions=formatted_tools, tool_config=tool_config, **kwargs)
 
     def _start_chat(
         self, history: _ChatHistory, **kwargs: Any
     ) -> Union[ChatSession, CodeChatSession]:
         if not self.is_codey_model:
             return self.client.start_chat(
                 context=history.context, message_history=history.history, **kwargs
```

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/embeddings.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/functions_utils.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/functions_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     return {
         "name": schema["title"],
         "description": schema.get("description", ""),
         "parameters": _get_parameters_from_schema(schema=schema),
     }
 
 
-def _format_tool_to_vertex_function(tool: BaseTool) -> FunctionDescription:
+def _format_base_tool_to_vertex_function(tool: BaseTool) -> FunctionDescription:
     "Format tool into the Vertex function API."
     if tool.args_schema:
         schema = tool.args_schema.schema()
 
         return {
             "name": tool.name or schema["title"],
             "description": tool.description or schema["description"],
@@ -53,32 +53,39 @@
                 },
                 "required": ["__arg1"],
                 "type": "object",
             },
         }
 
 
+def _format_tool_to_vertex_function(
+    tool: Union[BaseTool, Type[BaseModel], dict],
+) -> FunctionDescription:
+    "Format tool into the Vertex function declaration."
+    if isinstance(tool, BaseTool):
+        return _format_base_tool_to_vertex_function(tool)
+    elif isinstance(tool, type) and issubclass(tool, BaseModel):
+        return _format_pydantic_to_vertex_function(tool)
+    elif isinstance(tool, dict):
+        return {
+            "name": tool["name"],
+            "description": tool["description"],
+            "parameters": _get_parameters_from_schema(tool["parameters"]),
+        }
+    else:
+        raise ValueError(f"Unsupported tool call type {tool}")
+
+
 def _format_tools_to_vertex_tool(
     tools: List[Union[BaseTool, Type[BaseModel], dict]],
 ) -> List[VertexTool]:
-    "Format tool into the Vertex Tool instance."
+    "Format tools into the Vertex Tool instance."
     function_declarations = []
     for tool in tools:
-        if isinstance(tool, BaseTool):
-            func = _format_tool_to_vertex_function(tool)
-        elif isinstance(tool, type) and issubclass(tool, BaseModel):
-            func = _format_pydantic_to_vertex_function(tool)
-        elif isinstance(tool, dict):
-            func = {
-                "name": tool["name"],
-                "description": tool["description"],
-                "parameters": _get_parameters_from_schema(tool["parameters"]),
-            }
-        else:
-            raise ValueError(f"Unsupported tool call type {tool}")
+        func = _format_tool_to_vertex_function(tool)
         function_declarations.append(FunctionDeclaration(**func))
 
     return [VertexTool(function_declarations=function_declarations)]
 
 
 def _format_tool_config(tool_config: Dict[str, Any]) -> Union[ToolConfig, None]:
     if "function_calling_config" not in tool_config:
```

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/gemma.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/gemma.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/llms.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/llms.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,17 @@
 
 class VertexAI(_VertexAICommon, BaseLLM):
     """Google Vertex AI large language models."""
 
     model_name: str = "text-bison"
     "The name of the Vertex AI large language model."
     tuned_model_name: Optional[str] = None
-    "The name of a tuned model. If provided, model_name is ignored."
+    """The name of a tuned model. If tuned_model_name is passed
+    model_name will be used to determine the model family
+    """
 
     @classmethod
     def is_lc_serializable(self) -> bool:
         return True
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
@@ -143,30 +145,36 @@
             model_cls = GenerativeModel
             preview_model_cls = GenerativeModel
         else:
             model_cls = TextGenerationModel
             preview_model_cls = PreviewTextGenerationModel
 
         if tuned_model_name:
-            values["client"] = model_cls.get_tuned_model(tuned_model_name)
-            values["client_preview"] = preview_model_cls.get_tuned_model(
-                tuned_model_name
+            generative_model_name = values["tuned_model_name"]
+        else:
+            generative_model_name = values["model_name"]
+
+        if is_gemini:
+            values["client"] = model_cls(
+                model_name=generative_model_name, safety_settings=safety_settings
+            )
+            values["client_preview"] = preview_model_cls(
+                model_name=generative_model_name, safety_settings=safety_settings
             )
         else:
-            if is_gemini:
-                values["client"] = model_cls(
-                    model_name=model_name, safety_settings=safety_settings
-                )
-                values["client_preview"] = preview_model_cls(
-                    model_name=model_name, safety_settings=safety_settings
+            if tuned_model_name:
+                values["client"] = model_cls.get_tuned_model(generative_model_name)
+                values["client_preview"] = preview_model_cls.get_tuned_model(
+                    generative_model_name
                 )
             else:
-                values["client"] = model_cls.from_pretrained(model_name)
-                values["client_preview"] = preview_model_cls.from_pretrained(model_name)
-
+                values["client"] = model_cls.from_pretrained(generative_model_name)
+                values["client_preview"] = preview_model_cls.from_pretrained(
+                    generative_model_name
+                )
         if values["streaming"] and values["n"] > 1:
             raise ValueError("Only one candidate can be generated with streaming!")
         return values
 
     def _candidate_to_generation(
         self,
         response: Union[Candidate, TextGenerationResponse],
```

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/model_garden.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/model_garden.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_sdk_manager.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_sdk_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_searcher.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_searcher.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/_utils.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/document_storage.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/document_storage.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vectorstores/vectorstores.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vectorstores/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/langchain_google_vertexai/vision_models.py` & `langchain_google_vertexai-1.0.1/langchain_google_vertexai/vision_models.py`

 * *Files identical despite different names*

### Comparing `langchain_google_vertexai-0.1.3/pyproject.toml` & `langchain_google_vertexai-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "langchain-google-vertexai"
 
-version = "0.1.3"
+version = "1.0.1"
 description = "An integration package connecting Google VertexAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_google_vertexai-0.1.3/PKG-INFO` & `langchain_google_vertexai-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-vertexai
-Version: 0.1.3
+Version: 1.0.1
 Summary: An integration package connecting Google VertexAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

