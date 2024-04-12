# Comparing `tmp/pyqqq_cli-0.1.8.tar.gz` & `tmp/pyqqq_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.1.8.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.1.9.tar", max compression
```

## Comparing `pyqqq_cli-0.1.8.tar` & `pyqqq_cli-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      937 2024-03-27 03:34:24.848115 pyqqq_cli-0.1.8/README.md
--rw-r--r--   0        0        0      620 2024-03-29 04:04:02.934354 pyqqq_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      358 2024-03-29 03:28:42.002454 pyqqq_cli-0.1.8/qupiato/cli/config.py
--rw-r--r--   0        0        0     4673 2024-03-29 04:00:38.797164 pyqqq_cli-0.1.8/qupiato/cli/main.py
--rw-r--r--   0        0        0     3759 2024-03-29 03:42:46.535223 pyqqq_cli-0.1.8/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1732 1970-01-01 00:00:00.000000 pyqqq_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      937 2024-03-26 03:56:47.680900 pyqqq_cli-0.1.9/README.md
+-rw-r--r--   0        0        0      655 2024-04-12 07:50:19.019879 pyqqq_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-04-12 07:34:36.984208 pyqqq_cli-0.1.9/qupiato/cli/config.py
+-rw-r--r--   0        0        0     6353 2024-04-12 07:50:13.466796 pyqqq_cli-0.1.9/qupiato/cli/main.py
+-rw-r--r--   0        0        0     4459 2024-04-12 02:18:24.801494 pyqqq_cli-0.1.9/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.1.9/PKG-INFO
```

### Comparing `pyqqq_cli-0.1.8/README.md` & `pyqqq_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.1.8/pyproject.toml` & `pyqqq_cli-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.1.8"
+version = "0.1.9"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 websockets = "^12.0"
 python-dotenv = "^1.0.1"
 requests = "^2.31.0"
+pyqqq = "^0.7.4"
+pyyaml = "^6.0.1"
 
 [tool.poetry.scripts]
 qqq = 'qupiato.cli.main:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyqqq_cli-0.1.8/qupiato/cli/main.py` & `pyqqq_cli-0.1.9/qupiato/cli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from pyqqq.executors.hook import HookExecutor
+from qupiato.cli.utils import create_and_upload_to_gcs_bucket, get_token, ws_api_call, get_version, get_agent, encode_secret
 import asyncio
-import sys
 import click
 import datetime as dtm
+import importlib
 import os
-import re
 import qupiato.cli.config as c
-
-from qupiato.cli.utils import create_and_upload_to_gcs_bucket, get_token, ws_api_call, get_version, get_agent
+import re
+import subprocess
+import sys
+import yaml
 
 
 @click.group()
 def main():
     pass
 
 
@@ -44,25 +47,27 @@
     click.echo(f"Deploying {entryfile} as {strategy_name}")
 
     asyncio.run(deploy_strategy(entryfile, strategy_name))
 
 
 async def deploy_strategy(entryfile, strategy_name):
     click.echo(f"Uploading {entryfile} to GCS bucket")
+    secret = encode_secret()
     zipfile = create_and_upload_to_gcs_bucket()
 
     req = {
         "action": "deploy",
         "strategy_name": strategy_name,
         "token": get_token(),
         "zipfile": zipfile,
-        "entryfile": os.path.basename(entryfile),
+        "entryfile": entryfile,
         "agent": {
             **get_agent()
-        }
+        },
+        "secret": secret
     }
 
     async for line in ws_api_call(req):
         if 'text' in line:
             click.echo(line['text'])
 
 
@@ -102,15 +107,14 @@
         click.echo(f"{'DEPLOYMENT ID':<{name_width}} {'STRATEGY NAME':<{strategy_width}} {'STATUS':<{status_width}} CREATED AT")
 
         for e in data:
             created_at = dtm.datetime.fromtimestamp(e['created_at']/1000).strftime('%Y-%m-%d %H:%M:%S')
             click.echo(f"{e['name']:<{name_width}} {e['strategy_name']:<{strategy_width}} {e['status']:<{status_width}} {created_at}")
 
 
-
 @main.command()
 @click.argument('deployment_id')
 def delete(deployment_id):
     """ Delete a deployed strategy """
 
     asyncio.run(delete_strategy(deployment_id))
 
@@ -169,9 +173,64 @@
 
 @main.command()
 def version():
     """ Show version number and quit """
     version = get_version()
     click.echo(f"v{version}")
 
+@main.command()
+@click.argument('filename')
+def run(filename):
+    """ Run a strategy """
+
+    if not os.path.exists(filename):
+        click.echo(f"File {filename} does not exist")
+        sys.exit(1)
+
+    if os.path.exists("requirements.txt"):
+        subprocess.run(["pip", "install", "-r", "requirements.txt"])
+
+    app = None
+    if os.path.exists("app.yaml"):
+        with open("app.yaml", "r") as f:
+            app = yaml.safe_load(f)
+
+    spec = importlib.util.spec_from_file_location(os.getcwd(), filename)
+    module = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+
+    loop = asyncio.get_event_loop()
+
+    if app is not None and app.get("executor") == "hook":
+        task = loop.create_task(maybe_awaitable(HookExecutor(module).run()))
+    else:
+        if not has_callable(module, "run"):
+            click.echo("Module does not have a callable run()")
+            sys.exit(1)
+
+        task = loop.create_task(maybe_awaitable(module.run()))
+
+    try:
+        loop.run_until_complete(task)
+    except asyncio.CancelledError:
+        click.echo(f"Got keyboard interrupt, cancelling tasks...")
+        task.cancel()
+        loop.run_until_complete(task)
+    finally:
+        loop.close()
+
+
+async def maybe_awaitable(result):
+    if asyncio.iscoroutine(result) or isinstance(result, asyncio.Future):
+        return await result
+    else:
+        return result
+
+
+def has_callable(module, name):
+    try:
+        return callable(getattr(module, name))
+    except AttributeError:
+        return False
+
 if __name__ == '__main__':
     main()
```

### Comparing `pyqqq_cli-0.1.8/qupiato/cli/utils.py` & `pyqqq_cli-0.1.9/qupiato/cli/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import platform
 import qupiato.cli.config as c
 import requests
 import tempfile
 import uuid
 import websockets
 import zipfile
+import base64
 
 async def ws_api_call(req: Dict):
     async with websockets.connect(c.DEPLOYER_WS_URL) as ws:
         await ws.send(json.dumps(req))
 
         while True:
             try:
@@ -22,24 +23,40 @@
                 yield data
             except websockets.exceptions.ConnectionClosedOK:
                 break
 
             except websockets.exceptions.ConnectionClosedError:
                 break
 
+def encode_secret():
+    for root, _, files in os.walk('.'):
+        for file in files:
+            file_path = os.path.join(root, file)
+            norm_path = os.path.normpath(file_path)
+
+            if os.path.basename(norm_path) == '.env':
+                with open(norm_path, 'r') as file:
+                    env = file.read()
+                    env_bytes = base64.b64encode(env.encode('utf-8'))
+                    env_string = env_bytes.decode('utf-8')
+                    return env_string
 
 # 현재 디렉토리와 하위 디렉토리에 있는 모든 파일 압축
 def create_zip_archive(zip_filename):
     with zipfile.ZipFile(zip_filename, 'w', zipfile.ZIP_DEFLATED) as zipf:
         for root, _, files in os.walk('.'):
             for file in files:
                 file_path = os.path.join(root, file)
                 norm_path = os.path.normpath(file_path)
                 d_name = os.path.dirname(norm_path)
 
+                if os.path.basename(norm_path).startswith('.env'):
+                    continue
+                if os.path.basename(norm_path) == 'db.json':
+                    continue
                 if os.path.basename(norm_path).startswith('.bash'):
                     continue
                 if d_name and d_name.startswith('.'):
                     continue
                 if d_name and os.path.basename(d_name) == '__pycache__':
                     continue
                 if d_name and os.path.basename(d_name).startswith('.'):
```

### Comparing `pyqqq_cli-0.1.8/PKG-INFO` & `pyqqq_cli-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: pyqqq (>=0.7.4,<0.8.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
 
 ## pyqqq-cli
```

