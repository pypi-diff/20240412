# Comparing `tmp/composio_autogen-0.1.88.tar.gz` & `tmp/composio_autogen-0.1.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.88.tar", last modified: Thu Apr 11 15:13:28 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.89.tar", last modified: Fri Apr 12 06:30:08 2024, max compression
```

## Comparing `composio_autogen-0.1.88.tar` & `composio_autogen-0.1.89.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:28.237318 composio_autogen-0.1.88/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 15:13:28.237112 composio_autogen-0.1.88/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.88/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:28.235679 composio_autogen-0.1.88/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.88/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     8397 2024-04-11 12:39:00.000000 composio_autogen-0.1.88/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:28.236902 composio_autogen-0.1.88/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 15:12:31.000000 composio_autogen-0.1.88/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 15:13:28.237362 composio_autogen-0.1.88/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-11 15:12:31.000000 composio_autogen-0.1.88/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:30:08.075084 composio_autogen-0.1.89/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-12 06:30:08.074908 composio_autogen-0.1.89/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.89/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:30:08.073778 composio_autogen-0.1.89/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      100 2024-04-12 06:26:15.000000 composio_autogen-0.1.89/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     8467 2024-04-12 06:26:15.000000 composio_autogen-0.1.89/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:30:08.074721 composio_autogen-0.1.89/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-12 06:30:08.000000 composio_autogen-0.1.89/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-12 06:30:08.000000 composio_autogen-0.1.89/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-12 06:30:08.000000 composio_autogen-0.1.89/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-12 06:30:08.000000 composio_autogen-0.1.89/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-12 06:30:08.000000 composio_autogen-0.1.89/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-12 06:28:28.000000 composio_autogen-0.1.89/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-12 06:30:08.075122 composio_autogen-0.1.89/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-12 06:28:28.000000 composio_autogen-0.1.89/setup.py
```

### Comparing `composio_autogen-0.1.88/PKG-INFO` & `composio_autogen-0.1.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.88
+Version: 0.1.89
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.88
+Requires-Dist: composio_core===0.1.89
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.88/README.md` & `composio_autogen-0.1.89/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.88/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.89/composio_autogen/autogen_toolspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,37 +92,38 @@
             else :
                 optional_parameters.append(param)
         except Exception as e:
             logger.error(f"Error while processing param {param_name} with schema {param_schema}")
             pass
     return required_parameters + optional_parameters
 
+client = ComposioCore(framework=FrameworkEnum.AUTOGEN)
+ComposioSDK = client.sdk
 
 class ComposioToolset:
-    def __init__(self, caller = None, executor = None):
+    def __init__(self, caller = None, executor = None, entity_id: str = None):
         self.caller = caller
         self.executor = executor
-        self.client =  ComposioCore(framework=FrameworkEnum.AUTOGEN)
-
+        self.entity_id = entity_id
 
     def register_tools(
             self,
             tools: Union[App, List[App]],
             caller: ConversableAgent = None,
             executor: ConversableAgent = None
         ):
         if isinstance(tools, App):
             tools = [tools]
         assert caller or self.caller, "If caller hasn't been specified during initialization, has to be specified during registration"
         assert executor or self.executor, "If executor hasn't been specified during initialization, has to be specified during registration"
 
-        if self.client.is_authenticated() == False:
+        if client.is_authenticated() == False:
             raise Exception("User not authenticated. Please authenticate using composio-cli add <app_name>")
     
-        action_schemas = self.client.sdk.get_list_of_actions(
+        action_schemas = client.sdk.get_list_of_actions(
                                                 apps=tools)
         
         for schema in action_schemas:
             self._register_schema_to_autogen(action_schema=schema,
                                             caller = caller if caller else self.caller,
                                             executor = executor if executor else self.executor)
 
@@ -135,15 +136,15 @@
         ):
         if isinstance(actions, Action):
             actions = [actions]
 
         assert caller or self.caller, "If caller hasn't been specified during initialization, has to be specified during registration"
         assert executor or self.executor, "If executor hasn't been specified during initialization, has to be specified during registration"
 
-        action_schemas = self.client.sdk.get_list_of_actions(
+        action_schemas = client.sdk.get_list_of_actions(
                                                 actions=actions)
         
         for schema in action_schemas:
             self._register_schema_to_autogen(action_schema=schema,
                                             caller = caller if caller else self.caller,
                                             executor = executor if executor else self.executor)
 
@@ -169,17 +170,17 @@
         description = action_schema["description"]
 
         parameters = get_signature_format_from_schema_params(
                                             action_schema["parameters"])
         action_signature = Signature(parameters=parameters)
         
         def placeholder_function(**kwargs):
-            return self.client.execute_action(
-                        self.client.get_action_enum(name, appName), 
-                        kwargs)
+            return client.execute_action(
+                        client.get_action_enum(name, appName), 
+                        kwargs, entity_id=self.entity_id)
         action_func = types.FunctionType(
                                     placeholder_function.__code__, 
                                     globals=globals(), 
                                     name=processed_name, 
                                     closure=placeholder_function.__closure__
                           )
         action_func.__signature__ = action_signature
```

### Comparing `composio_autogen-0.1.88/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.89/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.88
+Version: 0.1.89
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.88
+Requires-Dist: composio_core===0.1.89
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.88/setup.py` & `composio_autogen-0.1.89/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.88",
+    version="0.1.89",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

