# Comparing `tmp/llm-quantkit-0.24.tar.gz` & `tmp/llm_quantkit-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-quantkit-0.24.tar", last modified: Sat Apr  6 06:53:26 2024, max compression
+gzip compressed data, was "llm_quantkit-0.25.tar", last modified: Fri Apr 12 21:36:27 2024, max compression
```

## Comparing `llm-quantkit-0.24.tar` & `llm_quantkit-0.25.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:53:26.845376 llm-quantkit-0.24/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-06 06:53:17.000000 llm-quantkit-0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-06 06:53:26.845376 llm-quantkit-0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-06 06:53:17.000000 llm-quantkit-0.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:53:26.845376 llm-quantkit-0.24/llm_quantkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 06:53:26.000000 llm-quantkit-0.24/llm_quantkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-06 06:53:17.000000 llm-quantkit-0.24/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:53:26.845376 llm-quantkit-0.24/quantkit/
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    64290 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/quantkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-06 06:53:17.000000 llm-quantkit-0.24/quantkit/safetensor.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:53:26.845376 llm-quantkit-0.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:36:27.417880 llm_quantkit-0.25/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 21:36:14.000000 llm_quantkit-0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-12 21:36:27.417880 llm_quantkit-0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-12 21:36:14.000000 llm_quantkit-0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:36:27.417880 llm_quantkit-0.25/llm_quantkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 21:36:27.000000 llm_quantkit-0.25/llm_quantkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 21:36:15.000000 llm_quantkit-0.25/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:36:27.413880 llm_quantkit-0.25/quantkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64290 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15979 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/quantkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-12 21:36:15.000000 llm_quantkit-0.25/quantkit/safetensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:36:27.417880 llm_quantkit-0.25/setup.cfg
```

### Comparing `llm-quantkit-0.24/LICENSE` & `llm_quantkit-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.24/PKG-INFO` & `llm_quantkit-0.25/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.24
+Version: 0.25
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
@@ -96,14 +96,22 @@
 ```
 quantkit download mistralai/Mistral-7B-v0.1 --no-cache --safetensors-only -out mistral7b
 ```
 
 <br/>
 
 
+Download from specific revision of a huggingface repo:
+```
+uantkit download turboderp/TinyLlama-1B-32k-exl2 --branch 6.0bpw --no-cache -out TinyLlama-1B-32k-exl2-b6
+```
+
+<br/>
+
+
 Download and convert a model to safetensor, deleting the original pytorch bins:
 ```
 quantkit safetensor migtissera/Tess-10.7B-v1.5b --delete-original
 ```
 
 <br/>
 
@@ -180,8 +188,8 @@
 |70B|GPTQ|24GB|:x:|
 |70B|HQQ|24GB|?|
 
 <br />
 
 # Notes
 
-Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the revelant command but replace llama-cpp-python with llama-cpp-conv.
+Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the relevant command but replace llama-cpp-python with llama-cpp-conv.
```

### Comparing `llm-quantkit-0.24/README.md` & `llm_quantkit-0.25/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,22 @@
 ```
 quantkit download mistralai/Mistral-7B-v0.1 --no-cache --safetensors-only -out mistral7b
 ```
 
 <br/>
 
 
+Download from specific revision of a huggingface repo:
+```
+uantkit download turboderp/TinyLlama-1B-32k-exl2 --branch 6.0bpw --no-cache -out TinyLlama-1B-32k-exl2-b6
+```
+
+<br/>
+
+
 Download and convert a model to safetensor, deleting the original pytorch bins:
 ```
 quantkit safetensor migtissera/Tess-10.7B-v1.5b --delete-original
 ```
 
 <br/>
 
@@ -156,8 +164,8 @@
 |70B|GPTQ|24GB|:x:|
 |70B|HQQ|24GB|?|
 
 <br />
 
 # Notes
 
-Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the revelant command but replace llama-cpp-python with llama-cpp-conv.
+Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the relevant command but replace llama-cpp-python with llama-cpp-conv.
```

### Comparing `llm-quantkit-0.24/llm_quantkit.egg-info/PKG-INFO` & `llm_quantkit-0.25/llm_quantkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.24
+Version: 0.25
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
@@ -96,14 +96,22 @@
 ```
 quantkit download mistralai/Mistral-7B-v0.1 --no-cache --safetensors-only -out mistral7b
 ```
 
 <br/>
 
 
+Download from specific revision of a huggingface repo:
+```
+uantkit download turboderp/TinyLlama-1B-32k-exl2 --branch 6.0bpw --no-cache -out TinyLlama-1B-32k-exl2-b6
+```
+
+<br/>
+
+
 Download and convert a model to safetensor, deleting the original pytorch bins:
 ```
 quantkit safetensor migtissera/Tess-10.7B-v1.5b --delete-original
 ```
 
 <br/>
 
@@ -180,8 +188,8 @@
 |70B|GPTQ|24GB|:x:|
 |70B|HQQ|24GB|?|
 
 <br />
 
 # Notes
 
-Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the revelant command but replace llama-cpp-python with llama-cpp-conv.
+Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the relevant command but replace llama-cpp-python with llama-cpp-conv.
```

### Comparing `llm-quantkit-0.24/pyproject.toml` & `llm_quantkit-0.25/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm-quantkit"
 description = "cli tool for downloading and quantizing LLMs"
 readme = "README.md"
 license = { text = "MIT License" }
-version = "0.24"
+version = "0.25"
 authors = [{ name = "xhedit", email = "jevd@protonmail.com" }]
 dependencies = [
     "click",
     "torch>=2.0.0",
     "einops",
     "tqdm",
     "transformers",
```

### Comparing `llm-quantkit-0.24/quantkit/cli.py` & `llm_quantkit-0.25/quantkit/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 @run.command()
 @click.argument('model', required=True)
 @click.option('--output', '-out')
 @click.option('--hf-cache/--no-cache', default=True, help='Use huggingface cache dir.')
 @click.option('--force-download/--no-force-download', default=False, help='Download again even if model is in hf cache.')
 @click.option('--resume/--no-resume', default=True, help='Resume a previously incomplete download.')
 @click.option('--safetensors-only/--everything', default=False, help='Ignore pytorch model-*.bin and pytorch_model.bin.index.json')
-def download(model, output, hf_cache, force_download, resume, safetensors_only):
+@click.option('--branch', '--revision', default=None, help='Branch/revision of hf repo to download')
+def download(model, output, hf_cache, force_download, resume, safetensors_only, branch):
     """Download model from huggingface."""
-    click.echo(f"download | model: {model} | use hf cache: {hf_cache} | out: {output} | force_download: {force_download} | resume: {resume} | safetensors_only: {safetensors_only}")
-    run_download(model, output, hf_cache, force_download, resume, safetensors_only)
+    click.echo(f"download | model: {model} | use hf cache: {hf_cache} | out: {output} | force_download: {force_download} | resume: {resume} | safetensors_only: {safetensors_only} | branch: {branch}")
+    run_download(model, output, hf_cache, force_download, resume, safetensors_only, branch)
 
 @run.command()
 @click.argument('model', required=True)
 @click.option('--delete-original/--save-original', default=False, help='Delete pytorch model files after conversion')
 #@click.option('--output', '-out')
 def safetensor(model, delete_original):
     """Download and/or convert a pytorch model to safetensor format."""
```

### Comparing `llm-quantkit-0.24/quantkit/convert.py` & `llm_quantkit-0.25/quantkit/convert.py`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.24/quantkit/quantkit.py` & `llm_quantkit-0.25/quantkit/quantkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import time
 import datetime
 
 from pathlib import Path
 from quantkit.safetensor import convert_multi
 from quantkit.convert import do_gguf_conversion
 
-def run_download(model, output, hf_cache, force_download, resume_download, safetensors_only):
+def run_download(model, output, hf_cache, force_download, resume_download, safetensors_only, branch):
     if output is None:
         model_dir = model.split("/")[1]
         path = Path(model_dir)
     else:
         path = Path(output)
 
     from huggingface_hub import snapshot_download
-    snapshot_download(model, local_dir=path, local_dir_use_symlinks=hf_cache, force_download=force_download, resume_download=resume_download, ignore_patterns=['pytorch_model*', 'consolidated*.pt'] if safetensors_only else None)
+    snapshot_download(model, revision=branch, local_dir=path, local_dir_use_symlinks=hf_cache, force_download=force_download, resume_download=resume_download, ignore_patterns=['pytorch_model*', 'consolidated*.pt'] if safetensors_only else None)
 
 def run_safetensor(model, delete_original):
     path = Path(model)
     if path.is_dir():
         if Path(path / "config.json").is_file():
             # convert
             convert_multi(model, del_pytorch_model=delete_original)
```

### Comparing `llm-quantkit-0.24/quantkit/safetensor.py` & `llm_quantkit-0.25/quantkit/safetensor.py`

 * *Files identical despite different names*

