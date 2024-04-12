# Comparing `tmp/pipepal-0.1.2.tar.gz` & `tmp/pipepal-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipepal-0.1.2.tar", max compression
+gzip compressed data, was "pipepal-0.1.3.tar", max compression
```

## Comparing `pipepal-0.1.2.tar` & `pipepal-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,59 @@
--rw-r--r--   0        0        0     9161 2024-03-29 03:07:21.407356 pipepal-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1471 2024-03-29 03:07:21.407356 pipepal-0.1.2/README.md
--rw-r--r--   0        0        0     2373 2024-03-29 03:07:49.831494 pipepal-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       48 2024-03-29 03:07:21.407356 pipepal-0.1.2/src/pipepal/__init__.py
--rw-r--r--   0        0        0      288 2024-03-29 03:07:21.407356 pipepal-0.1.2/src/pipepal/app.py
--rw-r--r--   0        0        0      365 2024-03-29 03:07:21.407356 pipepal-0.1.2/src/pipepal/cli.py
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 pipepal-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     9161 2024-04-12 17:36:19.388369 pipepal-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     3683 2024-04-12 17:36:19.388369 pipepal-0.1.3/README.md
+-rw-r--r--   0        0        0     2619 2024-04-12 17:39:15.145901 pipepal-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/app.py
+-rw-r--r--   0        0        0        0 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/pipes/.gitkeep
+-rw-r--r--   0        0        0      209 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/__init__.py
+-rw-r--r--   0        0        0      121 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/__init__.py
+-rw-r--r--   0        0        0     1050 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/abstract_service.py
+-rw-r--r--   0        0        0     5180 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/interface.py
+-rw-r--r--   0        0        0      690 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/schemas/run/input.json
+-rw-r--r--   0        0        0      332 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/schemas/run/output.json
+-rw-r--r--   0        0        0      148 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/services/__init__.py
+-rw-r--r--   0        0        0      134 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/services/example_service/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/services/example_service/config.json
+-rw-r--r--   0        0        0     4128 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/example_task/services/example_service/service.py
+-rw-r--r--   0        0        0      123 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/__init__.py
+-rw-r--r--   0        0        0     3157 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/abstract_service.py
+-rw-r--r--   0        0        0     4705 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/interface.py
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/read_HF_dataset_from_HF_hub/input.json
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/read_HF_dataset_from_HF_hub/output.json
+-rw-r--r--   0        0        0     1167 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/read_audios_from_disk/input.json
+-rw-r--r--   0        0        0      210 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/read_audios_from_disk/output.json
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/read_local_HF_dataset/input.json
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/read_local_HF_dataset/output.json
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/save_HF_dataset_to_disk/input.json
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/save_HF_dataset_to_disk/output.json
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/upload_HF_dataset_to_HF_hub copy 2/input.json
+-rw-r--r--   0        0        0      258 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/schemas/upload_HF_dataset_to_HF_hub copy 2/output.json
+-rw-r--r--   0        0        0      145 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/services/__init__.py
+-rw-r--r--   0        0        0      130 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/services/datasets/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/services/datasets/config.json
+-rw-r--r--   0        0        0     5458 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio/tasks/input_output/services/datasets/service.py
+-rw-r--r--   0        0        0        0 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/audio-cli/.gitkeep
+-rw-r--r--   0        0        0      365 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/cli.py
+-rw-r--r--   0        0        0      152 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/utils/__init__.py
+-rw-r--r--   0        0        0     4861 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/utils/abstract_component.py
+-rw-r--r--   0        0        0       43 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/utils/functions.py
+-rw-r--r--   0        0        0        0 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/pipes/.gitkeep
+-rw-r--r--   0        0        0      209 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/__init__.py
+-rw-r--r--   0        0        0      121 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/__init__.py
+-rw-r--r--   0        0        0     1050 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/abstract_service.py
+-rw-r--r--   0        0        0     5180 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/interface.py
+-rw-r--r--   0        0        0      690 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/schemas/run/input.json
+-rw-r--r--   0        0        0      332 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/schemas/run/output.json
+-rw-r--r--   0        0        0      148 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/services/__init__.py
+-rw-r--r--   0        0        0      134 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/services/example_service/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/services/example_service/config.json
+-rw-r--r--   0        0        0     4128 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/example_task/services/example_service/service.py
+-rw-r--r--   0        0        0      123 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/__init__.py
+-rw-r--r--   0        0        0     1705 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/abstract_service.py
+-rw-r--r--   0        0        0     2161 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/interface.py
+-rw-r--r--   0        0        0     1945 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/schemas/extract_audios_from_videos/input.json
+-rw-r--r--   0        0        0      302 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/schemas/extract_audios_from_videos/output.json
+-rw-r--r--   0        0        0      139 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/services/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/services/ffmpeg/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/services/ffmpeg/config.json
+-rw-r--r--   0        0        0     7355 2024-04-12 17:36:19.392369 pipepal-0.1.3/src/pipepal/video/tasks/input_output/services/ffmpeg/service.py
+-rw-r--r--   0        0        0     5066 1970-01-01 00:00:00.000000 pipepal-0.1.3/PKG-INFO
```

### Comparing `pipepal-0.1.2/LICENSE.txt` & `pipepal-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pipepal-0.1.2/pyproject.toml` & `pipepal-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipepal"
-version = "0.1.2"
+version = "0.1.3"
 description = "PipePal is a Python package that simplifies building pipelines for speech and voice analysis."
 authors = [
     "Fabio Catania <fabiocat@mit.edu>",
 ]
 maintainers = [
     "Fabio Catania <fabiocat@mit.edu>",
 ]
@@ -21,23 +21,34 @@
   "Operating System :: OS Independent"
 ]
 packages = [{include = "pipepal", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
+jsonschema = "^4.21.1"
+datasets = "^2.18.0"
+torch = "^2.2.2"
+torchvision = "^0.17.2"
+torchaudio = "^2.2.2"
+transformers = "^4.39.3"
+librosa = "^0.10.1"
+soundfile = "^0.12.1"
+ffmpeg-python = "^0.2.0"
+ipykernel = "^6.29.4"
 
 [tool.poetry.group.dev]
 optional = true
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 mypy = "^1.9.0"
 pre-commit = "^3.7.0"
 pytest-cov = "^5.0.0"
 ruff = "^0.3.4"
+pytest-mock = "^3.14.0"
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 pdoc = "^14.4.0"
 
 [tool.pytest.ini_options]
@@ -71,15 +82,15 @@
   "_build",
   "buck-out",
   "build",
   "dist",
   "node_modules",
   "venv"
 ]
-line-length = 88
+line-length = 200
 indent-width = 4
 src = ["src"]
 target-version = "py310"
 
 [tool.ruff.lint]
 select = ["ANN", "D", "E", "F", "I"]
 ignore = [
```

