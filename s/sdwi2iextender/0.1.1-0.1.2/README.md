# Comparing `tmp/sdwi2iextender-0.1.1.tar.gz` & `tmp/sdwi2iextender-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdwi2iextender-0.1.1.tar", last modified: Mon Apr  8 23:15:00 2024, max compression
+gzip compressed data, was "sdwi2iextender-0.1.2.tar", last modified: Fri Apr 12 17:51:16 2024, max compression
```

## Comparing `sdwi2iextender-0.1.1.tar` & `sdwi2iextender-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 23:15:00.080861 sdwi2iextender-0.1.1/
--rw-rw-rw-   0        0        0     1083 2024-01-20 11:18:02.000000 sdwi2iextender-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6191 2024-04-08 23:15:00.079862 sdwi2iextender-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5822 2024-04-08 21:29:24.000000 sdwi2iextender-0.1.1/README.md
--rw-rw-rw-   0        0        0      358 2024-04-08 23:14:15.000000 sdwi2iextender-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-08 23:14:59.869491 sdwi2iextender-0.1.1/sdwi2iextender/
--rw-rw-rw-   0        0        0      242 2024-04-08 23:14:23.000000 sdwi2iextender-0.1.1/sdwi2iextender/__init__.py
--rw-rw-rw-   0        0        0     1507 2024-04-06 14:57:11.000000 sdwi2iextender-0.1.1/sdwi2iextender/gradio_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 23:15:00.076865 sdwi2iextender-0.1.1/sdwi2iextender/lib/
--rw-rw-rw-   0        0        0     5303 2024-04-07 00:18:16.000000 sdwi2iextender-0.1.1/sdwi2iextender/lib/img2img_component_injector.py
--rw-rw-rw-   0        0        0     5912 2024-04-08 21:32:58.000000 sdwi2iextender-0.1.1/sdwi2iextender/lib/img2img_tab_extender.py
--rw-rw-rw-   0        0        0      224 2023-11-04 03:21:41.000000 sdwi2iextender-0.1.1/sdwi2iextender/lib/one_time_callable.py
--rw-rw-rw-   0        0        0      443 2024-04-08 16:38:50.000000 sdwi2iextender-0.1.1/sdwi2iextender/lib/operation_mode.py
-drwxrwxrwx   0        0        0        0 2024-04-08 23:15:00.078862 sdwi2iextender-0.1.1/sdwi2iextender.egg-info/
--rw-rw-rw-   0        0        0     6191 2024-04-08 23:14:59.000000 sdwi2iextender-0.1.1/sdwi2iextender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-04-08 23:14:59.000000 sdwi2iextender-0.1.1/sdwi2iextender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 23:14:59.000000 sdwi2iextender-0.1.1/sdwi2iextender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 23:14:59.000000 sdwi2iextender-0.1.1/sdwi2iextender.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 23:15:00.080861 sdwi2iextender-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 17:51:16.942827 sdwi2iextender-0.1.2/
+-rw-rw-rw-   0        0        0     1083 2024-01-20 11:18:02.000000 sdwi2iextender-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6191 2024-04-12 17:51:16.940683 sdwi2iextender-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5822 2024-04-12 17:42:16.000000 sdwi2iextender-0.1.2/README.md
+-rw-rw-rw-   0        0        0      358 2024-04-12 17:47:55.000000 sdwi2iextender-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-12 17:51:16.917683 sdwi2iextender-0.1.2/sdwi2iextender/
+-rw-rw-rw-   0        0        0      242 2024-04-12 17:42:16.000000 sdwi2iextender-0.1.2/sdwi2iextender/__init__.py
+-rw-rw-rw-   0        0        0     1507 2024-04-12 17:42:16.000000 sdwi2iextender-0.1.2/sdwi2iextender/gradio_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:51:16.936682 sdwi2iextender-0.1.2/sdwi2iextender/lib/
+-rw-rw-rw-   0        0        0     5976 2024-04-12 17:42:25.000000 sdwi2iextender-0.1.2/sdwi2iextender/lib/img2img_component_injector.py
+-rw-rw-rw-   0        0        0     5912 2024-04-12 17:42:16.000000 sdwi2iextender-0.1.2/sdwi2iextender/lib/img2img_tab_extender.py
+-rw-rw-rw-   0        0        0      224 2023-11-04 03:21:41.000000 sdwi2iextender-0.1.2/sdwi2iextender/lib/one_time_callable.py
+-rw-rw-rw-   0        0        0      443 2024-04-12 17:42:16.000000 sdwi2iextender-0.1.2/sdwi2iextender/lib/operation_mode.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:51:16.938683 sdwi2iextender-0.1.2/sdwi2iextender.egg-info/
+-rw-rw-rw-   0        0        0     6191 2024-04-12 17:51:16.000000 sdwi2iextender-0.1.2/sdwi2iextender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-04-12 17:51:16.000000 sdwi2iextender-0.1.2/sdwi2iextender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 17:51:16.000000 sdwi2iextender-0.1.2/sdwi2iextender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 17:51:16.000000 sdwi2iextender-0.1.2/sdwi2iextender.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 17:51:16.942827 sdwi2iextender-0.1.2/setup.cfg
```

### Comparing `sdwi2iextender-0.1.1/LICENSE` & `sdwi2iextender-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdwi2iextender-0.1.1/PKG-INFO` & `sdwi2iextender-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdwi2iextender
-Version: 0.1.1
+Version: 0.1.2
 Summary: Stable Diffusion Webui Img2img Tab Extender
 Author: Plads
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `sdwi2iextender-0.1.1/README.md` & `sdwi2iextender-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sdwi2iextender-0.1.1/sdwi2iextender/gradio_helpers.py` & `sdwi2iextender-0.1.2/sdwi2iextender/gradio_helpers.py`

 * *Files identical despite different names*

### Comparing `sdwi2iextender-0.1.1/sdwi2iextender/lib/img2img_component_injector.py` & `sdwi2iextender-0.1.2/sdwi2iextender/lib/img2img_component_injector.py`

 * *Files 15% similar despite different names*

```diff
@@ -109,15 +109,19 @@
 
 @one_time_callable
 def activate_generation_component_injector():
     add_nasty_patches()
 
 
 def add_nasty_patches():
-    print("[sdwi2iextender]", "Applying img2img patch")
+    print("[sdwi2iextender]", "\033[0;33mDevelopper warning:\033[0m")
+    print("[sdwi2iextender]", "\033[0;33m./modules/img2img.py is being recompiled at run time with a patch. Your debugger will not work in this file.\033[0m")
+    print("[sdwi2iextender]", "\033[0;33mIf you need debug tools in this file, disable all extensions that use the sdwi2iextender library.\033[0m")
+    print("[sdwi2iextender]", "\033[0;33mThis patch is temporary and will be removed when v1.9 will be released.\033[0m")
+
     import_patch = "import sdwi2iextender"
     code_patch = f"""
 if (script_instance := sdwi2iextender.get_script_class().img2img_instance) and (script_args := args[script_instance.args_from:script_instance.args_to]) and script_instance.should_intercept_generation(*script_args):
     script_instance.resolve_image_and_mask(*script_args)
     image = script_instance.image
     mask = script_instance.mask
 else:
@@ -125,28 +129,35 @@
     mask = None
 """
     parsed_module = ast.parse(inspect.getsource(img2img))
     parsed_module.body[0:0] = ast.parse(import_patch).body[0:1]
 
     parsed_function = get_ast_function(parsed_module, "img2img")
     ast_if = get_ast_if_mode(parsed_function)
+    if ast_if is None: # Forge support
+        parsed_function = get_ast_function(parsed_module, "img2img_function")
+        ast_if = get_ast_if_mode(parsed_function)
+
     last_ast_if = get_last_ast_if(ast_if)
     last_ast_if.orelse[:] = ast.parse(code_patch).body[0:1]
     exec(compile(parsed_module, '<string>', 'exec'), img2img.__dict__)
 
 
 def get_ast_function(parsed_object, function_name):
     res = [exp for exp in parsed_object.body if getattr(exp, 'name', None) == function_name]
     if not res:
-        raise RuntimeError(f'Cannot find function {function_name} in parsed ast')
+        return None
 
     return res[0]
 
 
 def get_ast_if_mode(parsed_img2img_function):
+    if parsed_img2img_function is None:
+        return None
+    
     for node in parsed_img2img_function.body:
         if not hasattr(node, "test"):
             continue
         
         if not hasattr(node.test, "left"):
             continue
 
@@ -154,11 +165,14 @@
             continue
 
         if node.test.left.id == "mode":
             return node
 
 
 def get_last_ast_if(ast_if):
+    if ast_if is None:
+        return None
+
     while(hasattr(ast_if, "orelse") and len(ast_if.orelse) == 1):
         ast_if = ast_if.orelse[0]
     
     return ast_if
```

### Comparing `sdwi2iextender-0.1.1/sdwi2iextender/lib/img2img_tab_extender.py` & `sdwi2iextender-0.1.2/sdwi2iextender/lib/img2img_tab_extender.py`

 * *Files identical despite different names*

### Comparing `sdwi2iextender-0.1.1/sdwi2iextender.egg-info/PKG-INFO` & `sdwi2iextender-0.1.2/sdwi2iextender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdwi2iextender
-Version: 0.1.1
+Version: 0.1.2
 Summary: Stable Diffusion Webui Img2img Tab Extender
 Author: Plads
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

