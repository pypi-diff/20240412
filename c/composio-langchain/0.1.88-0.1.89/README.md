# Comparing `tmp/composio_langchain-0.1.88.tar.gz` & `tmp/composio_langchain-0.1.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.88.tar", last modified: Thu Apr 11 15:13:14 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.89.tar", last modified: Fri Apr 12 06:29:48 2024, max compression
```

## Comparing `composio_langchain-0.1.88.tar` & `composio_langchain-0.1.89.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:14.403248 composio_langchain-0.1.88/
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:29:17.000000 composio_langchain-0.1.88/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-11 15:13:14.403043 composio_langchain-0.1.88/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-02 18:29:17.000000 composio_langchain-0.1.88/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:14.401778 composio_langchain-0.1.88/composio_langchain/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       88 2024-04-02 18:29:17.000000 composio_langchain-0.1.88/composio_langchain/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     5405 2024-04-07 18:28:35.000000 composio_langchain-0.1.88/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-02 18:29:17.000000 composio_langchain-0.1.88/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:14.402788 composio_langchain-0.1.88/composio_langchain.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-11 15:13:14.000000 composio_langchain-0.1.88/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-11 15:13:14.000000 composio_langchain-0.1.88/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 15:13:14.000000 composio_langchain-0.1.88/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      149 2024-04-11 15:13:14.000000 composio_langchain-0.1.88/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-11 15:13:14.000000 composio_langchain-0.1.88/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      455 2024-04-11 15:12:31.000000 composio_langchain-0.1.88/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 15:13:14.403296 composio_langchain-0.1.88/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-11 15:12:31.000000 composio_langchain-0.1.88/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:48.158383 composio_langchain-0.1.89/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:29:17.000000 composio_langchain-0.1.89/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-12 06:29:48.158206 composio_langchain-0.1.89/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-02 18:29:17.000000 composio_langchain-0.1.89/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:48.156917 composio_langchain-0.1.89/composio_langchain/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      101 2024-04-12 06:26:15.000000 composio_langchain-0.1.89/composio_langchain/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5518 2024-04-12 06:26:15.000000 composio_langchain-0.1.89/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-02 18:29:17.000000 composio_langchain-0.1.89/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:48.158015 composio_langchain-0.1.89/composio_langchain.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-12 06:29:48.000000 composio_langchain-0.1.89/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-12 06:29:48.000000 composio_langchain-0.1.89/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-12 06:29:48.000000 composio_langchain-0.1.89/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      149 2024-04-12 06:29:48.000000 composio_langchain-0.1.89/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-12 06:29:48.000000 composio_langchain-0.1.89/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      455 2024-04-12 06:28:28.000000 composio_langchain-0.1.89/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-12 06:29:48.158424 composio_langchain-0.1.89/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-12 06:28:28.000000 composio_langchain-0.1.89/setup.py
```

### Comparing `composio_langchain-0.1.88/PKG-INFO` & `composio_langchain-0.1.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.88
+Version: 0.1.89
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.88
+Requires-Dist: composio_core===0.1.89
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.88/README.md` & `composio_langchain-0.1.89/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.88/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.89/composio_langchain/composio_tool_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,22 +87,22 @@
         if is_required:
             required_parameters.append(param)
         else :
             optional_parameters.append(param)
     return required_parameters + optional_parameters
 
     
-def ComposioTool(client : ComposioCore, action_schema: dict[str, any]) ->  StructuredTool:
+def ComposioTool(client : ComposioCore, action_schema: dict[str, any], entity_id: str = None) ->  StructuredTool:
     name = action_schema["name"]
     description = action_schema["description"]
     parameters = json_schema_to_model(action_schema["parameters"])
     appName = action_schema["appName"]
     func_params = get_signature_format_from_schema_params(action_schema["parameters"])
     action_signature = Signature(parameters=func_params)
-    placeholder_function = lambda **kwargs: client.execute_action(client.get_action_enum(name, appName), kwargs)
+    placeholder_function = lambda **kwargs: client.execute_action(client.get_action_enum(name, appName), kwargs, entity_id=entity_id)
     action_func = types.FunctionType(
                                     placeholder_function.__code__, 
                                     globals=globals(), 
                                     name=name, 
                                     closure=placeholder_function.__closure__
                           )
     action_func.__signature__ = action_signature
@@ -113,15 +113,16 @@
         args_schema=parameters,
         return_schema=True,
         # TODO use execute action here
         func = action_func
     )
 
 client = ComposioCore(framework=FrameworkEnum.LANGCHAIN)
+ComposioSDK = client.sdk
 
-def ComposioToolset(apps: List[App] = [], actions: List[Action] = []) -> List[StructuredTool]:
+def ComposioToolset(apps: List[App] = [], actions: List[Action] = [], entity_id: str = None) -> List[StructuredTool]:
     if len(apps) >0 and len(actions) > 0:
         raise ValueError("You must provide either a list of tools or a list of actions, not both")
     if client.is_authenticated() == False:
         raise Exception("User not authenticated. Please authenticate using composio-cli add <app_name>")
     actions_list = client.sdk.get_list_of_actions(apps, actions)
-    return [ComposioTool(client, action) for action in actions_list]
+    return [ComposioTool(client, action, entity_id=entity_id) for action in actions_list]
```

### Comparing `composio_langchain-0.1.88/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.89/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.88/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.89/composio_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.88
+Version: 0.1.89
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.88
+Requires-Dist: composio_core===0.1.89
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.88/setup.py` & `composio_langchain-0.1.89/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.88",
+    version="0.1.89",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

