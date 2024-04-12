# Comparing `tmp/llmfunctionclient-0.1.3.tar.gz` & `tmp/llmfunctionclient-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfunctionclient-0.1.3.tar", max compression
+gzip compressed data, was "llmfunctionclient-0.1.5.tar", max compression
```

## Comparing `llmfunctionclient-0.1.3.tar` & `llmfunctionclient-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-11 00:02:39.575768 llmfunctionclient-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     4328 2024-04-11 00:02:39.575768 llmfunctionclient-0.1.3/README.md
--rw-r--r--   0        0        0       19 2024-04-11 00:02:39.575768 llmfunctionclient-0.1.3/llmfunctionclient/__init__.py
--rw-r--r--   0        0        0     6952 2024-04-11 00:02:39.575768 llmfunctionclient-0.1.3/llmfunctionclient/main.py
--rw-r--r--   0        0        0      321 2024-04-11 00:02:39.575768 llmfunctionclient-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 llmfunctionclient-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-12 01:48:14.938003 llmfunctionclient-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     4332 2024-04-12 01:48:14.938003 llmfunctionclient-0.1.5/README.md
+-rw-r--r--   0        0        0       19 2024-04-12 01:48:14.938003 llmfunctionclient-0.1.5/llmfunctionclient/__init__.py
+-rw-r--r--   0        0        0     7021 2024-04-12 01:48:14.938003 llmfunctionclient-0.1.5/llmfunctionclient/main.py
+-rw-r--r--   0        0        0      321 2024-04-12 01:48:14.938003 llmfunctionclient-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5030 1970-01-01 00:00:00.000000 llmfunctionclient-0.1.5/PKG-INFO
```

### Comparing `llmfunctionclient-0.1.3/LICENSE.md` & `llmfunctionclient-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmfunctionclient-0.1.3/README.md` & `llmfunctionclient-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   Gets the weather
 
   location: where to get the forecast for
   """
   return f"The weather in {location} is 75 degrees"
 ```
 
-This function will have "Gets the weather" as the function description and the location parameter will have the description "where to get the forecase for"
+This function will have "Gets the weather" as the function description and the location parameter will have the description "where to get the forecast for"
 
 ## FunctionClient
 
 The `FunctionClient` class is made to abstract away the logic of passing along tool calls by taking in a list of functions that are allowed to be called by the LLM client, running any tool calls required by LLM client responses until it is left with just text to respond with.
 
 ```python
 from llmfunctionclient import FunctionClient
@@ -47,16 +47,16 @@
 client = FunctionClient(OpenAI(), "gpt-3.5-turbo", [get_weather])
 client.add_message("You are a helpful weather assistant.", "system")
 response = client.send_message("What's the weather in LA?", "user")
 print(response) # "The current weather in Los Angeles is 75 degrees"
 ```
 
 When this is run, the following happens under the hood:  
-1. The two message specified here will be submitted to the LLM Client
-2. The LLM Client responds with a tool call for "get_weather"
+1. The two messages specified here will be submitted to the LLM Client
+2. The LLM Client responds with a tool called for "get_weather"
 3. The get_weather function is called and the result is appended as a message
 4. The LLM Client is called again with the function result.
 5. The LLM Client Responds with an informed answer.
 6. This response text is passed back.
 
 You can pass functions into the constructor of the client to create the default set of tools for every message as well as pass in the `functions` kwarg to `send_message` to specify a specific set of functions for that portion of the conversation.
 
@@ -95,8 +95,8 @@
 messages = [{"role": "user", "content": "What's the weather like in Boston today?"}]
 completion = client.chat.completions.create(
   model="gpt-3.5-turbo",
   messages=messages,
   tools=[to_tool(get_weather)],
   tool_choice="auto"
 )
-```
+```
```

### Comparing `llmfunctionclient-0.1.3/llmfunctionclient/main.py` & `llmfunctionclient-0.1.5/llmfunctionclient/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         result = tools_map[tool_call.function.name](**args)
         self.messages.append({"role": "function", "tool_call_id": tool_call.id, "name": tool_call.function.name, "content": result})
       return False
     else:
       self.messages.append({"role": "assistant", "content": message.content})
       return True
 
-  def send_message(self, content: Optional[str]=None, role: Optional[str]=None, model: Optional[str]=None, functions: Optional[list[Callable]]=None, force_function: Optional[str | Callable]=None) -> str:
+  def send_message(self, content: Optional[str]=None, role: Optional[str]=None, model: Optional[str]=None, functions: Optional[list[Callable]]=None, force_function: Optional[str | Callable]=None, num_calls: Optional[int]=100) -> str:
     """
     Sends a message to the language model and processes the response, responding to tool call requests until a text response is received.
     Can be called without a content argument to just use current messages.
 
     content: Optional, the content of the message.
     role: Optional, the role of the message, defaults to 'user'.
     functions: Optional, the list of functions to use, defaults to the list of functions passed to the constructor.
@@ -171,12 +171,14 @@
     if not functions:
        functions = self.functions
     if callable(force_function):
        force_function = force_function.__name__
     if not model:
         model = self.model
     done = False
+    i = 0
     # Only force_function for the first call to avoid tool call loops
     done = self.__send_message(functions, force_function, model=model)
-    while not done:
+    i += 1
+    while not done and i < num_calls:
       done = self.__send_message(functions, model=model)
     return self.messages[-1]['content']
```

### Comparing `llmfunctionclient-0.1.3/PKG-INFO` & `llmfunctionclient-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfunctionclient
-Version: 0.1.3
+Version: 0.1.5
 Summary: 
 Author: James Mills
 Author-email: jimmyemills@gmail.com
 Requires-Python: >=3.4,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -41,15 +41,15 @@
   Gets the weather
 
   location: where to get the forecast for
   """
   return f"The weather in {location} is 75 degrees"
 ```
 
-This function will have "Gets the weather" as the function description and the location parameter will have the description "where to get the forecase for"
+This function will have "Gets the weather" as the function description and the location parameter will have the description "where to get the forecast for"
 
 ## FunctionClient
 
 The `FunctionClient` class is made to abstract away the logic of passing along tool calls by taking in a list of functions that are allowed to be called by the LLM client, running any tool calls required by LLM client responses until it is left with just text to respond with.
 
 ```python
 from llmfunctionclient import FunctionClient
@@ -66,16 +66,16 @@
 client = FunctionClient(OpenAI(), "gpt-3.5-turbo", [get_weather])
 client.add_message("You are a helpful weather assistant.", "system")
 response = client.send_message("What's the weather in LA?", "user")
 print(response) # "The current weather in Los Angeles is 75 degrees"
 ```
 
 When this is run, the following happens under the hood:  
-1. The two message specified here will be submitted to the LLM Client
-2. The LLM Client responds with a tool call for "get_weather"
+1. The two messages specified here will be submitted to the LLM Client
+2. The LLM Client responds with a tool called for "get_weather"
 3. The get_weather function is called and the result is appended as a message
 4. The LLM Client is called again with the function result.
 5. The LLM Client Responds with an informed answer.
 6. This response text is passed back.
 
 You can pass functions into the constructor of the client to create the default set of tools for every message as well as pass in the `functions` kwarg to `send_message` to specify a specific set of functions for that portion of the conversation.
 
@@ -115,7 +115,8 @@
 completion = client.chat.completions.create(
   model="gpt-3.5-turbo",
   messages=messages,
   tools=[to_tool(get_weather)],
   tool_choice="auto"
 )
 ```
+
```

