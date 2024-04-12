# Comparing `tmp/igniter-1.0.1.tar.gz` & `tmp/igniter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igniter-1.0.1.tar", last modified: Mon Mar 18 23:59:40 2024, max compression
+gzip compressed data, was "igniter-1.0.2.tar", last modified: Fri Apr 12 06:06:52 2024, max compression
```

## Comparing `igniter-1.0.1.tar` & `igniter-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.023696 igniter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-18 23:59:26.000000 igniter-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-18 23:59:40.023696 igniter-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.019696 igniter-1.0.1/igniter/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.019696 igniter-1.0.1/igniter/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/configs/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.019696 igniter-1.0.1/igniter/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/datasets/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/datasets/s3_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.019696 igniter-1.0.1/igniter/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/defaults/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.023696 igniter-1.0.1/igniter/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/engine/inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/engine/trainer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.023696 igniter-1.0.1/igniter/io/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/io/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/io/s3_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/io/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/io/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-18 23:59:26.000000 igniter-1.0.1/igniter/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 23:59:40.019696 igniter-1.0.1/igniter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-18 23:59:39.000000 igniter-1.0.1/igniter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-18 23:59:39.000000 igniter-1.0.1/igniter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 23:59:39.000000 igniter-1.0.1/igniter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-18 23:59:39.000000 igniter-1.0.1/igniter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-18 23:59:39.000000 igniter-1.0.1/igniter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 23:59:39.000000 igniter-1.0.1/igniter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 23:59:39.000000 igniter-1.0.1/igniter.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-18 23:59:26.000000 igniter-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 23:59:40.023696 igniter-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-18 23:59:26.000000 igniter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.501770 igniter-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 06:06:42.000000 igniter-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-12 06:06:52.501770 igniter-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/configs/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/datasets/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/datasets/s3_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/defaults/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.501770 igniter-1.0.2/igniter/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/trainer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.501770 igniter-1.0.2/igniter/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/s3_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/io/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-12 06:06:42.000000 igniter-1.0.2/igniter/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:06:52.497770 igniter-1.0.2/igniter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:06:52.000000 igniter-1.0.2/igniter.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 06:06:42.000000 igniter-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:06:52.501770 igniter-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-12 06:06:42.000000 igniter-1.0.2/setup.py
```

### Comparing `igniter-1.0.1/PKG-INFO` & `igniter-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igniter
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/iKrishneel/igniter
 Author: Krishneel
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `igniter-1.0.1/igniter/builder.py` & `igniter-1.0.2/igniter/builder.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/cli.py` & `igniter-1.0.2/igniter/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 
-from typing import List, Dict
 import argparse
-import os
 import importlib
 import logging
+import os
+from typing import List
+
 from igniter.logger import logger
-from igniter.main import get_full_config, _run
+from igniter.main import _run, get_full_config
 
 
 def _find_files(directory: str, ext: str = 'py') -> List[str]:
     valid_files = []
     for root, _, files in os.walk(directory):
         for filename in files:
             if ext != filename.split('.')[1]:
@@ -50,28 +51,28 @@
 def main() -> None:
     parser = argparse.ArgumentParser(description='Igniter Command Line Interface (CLI)')
     parser.add_argument('config', type=str, help='Configuration filename')
     parser.add_argument('--log-level', type=str, default='INFO')
     args = parser.parse_args()
 
     logger.setLevel(getattr(logging, args.log_level))
-    
+
     config_path = os.path.abspath(args.config)
     assert config_path.split('.')[1] == 'yaml', f'Config must be a yaml file but got {config_path}'
     logger.info(f'Using config {config_path}')
 
     cfg = get_full_config(config_path)
 
     if os.path.isdir(cfg.driver):
         raise NotImplementedError
     elif _is_path(cfg.driver):
         logger.info(f'Loading: {cfg.driver}')
         load_script(cfg.driver)
     else:
         logger.info(f'Importing: {cfg.driver}')
-        import_module(cfg.driver)
+        import_modules(cfg.driver)
 
     _run(cfg)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `igniter-1.0.1/igniter/configs/config.yaml` & `igniter-1.0.2/igniter/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/datasets/coco.py` & `igniter-1.0.2/igniter/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/datasets/s3_dataset.py` & `igniter-1.0.2/igniter/datasets/s3_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,24 @@
         # TODO: Add target transforms
         if transforms:
             import warnings
 
             warnings.warn('Target transforms is not yet implemented')
 
     def __getitem__(self, index: int) -> Tuple[Any, ...]:
-        iid = self.ids[index]
         while True:
             try:
+                iid = self.ids[index]
                 image, target = self._load(iid)
                 if self.transforms and self.apply_transforms:
                     image = self.transforms(image)
                 return image, target
             except Exception as e:
                 logger.warning(f'{e} for iid: {iid}')
-                iid = np.random.choice(iid)
+                index = np.random.choice(np.arange(len(self.ids)))
 
     def _load(self, iid: int) -> Tuple[Any, ...]:
         file_name = osp.join(self.root, self.coco.loadImgs(iid)[0]['file_name'])
         image = self.load_image(file_name)
         image = Image.fromarray(image).convert('RGB') if not isinstance(image, Image.Image) else image  # type: ignore
         target = self.coco.loadAnns(self.coco.getAnnIds(iid))
         return image, target
```

### Comparing `igniter-1.0.1/igniter/defaults/defaults.py` & `igniter-1.0.2/igniter/defaults/defaults.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/engine/inference_engine.py` & `igniter-1.0.2/igniter/engine/inference_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
         self.device = cfg.get('device', 'cuda' if torch.cuda.is_available() else 'cpu')
         logger.info(f'Using device: {self.device}')
 
         model = build_model(cfg) if model is None else model
         load_weights(model, cfg, strict=kwargs.get('strict', True))
         model.to(self.device)
+        model.to(getattr(torch, cfg.dtype))
         model.eval()
         self._model = model
 
         logger.info('Inference Engine is Ready!')
 
     @torch.inference_mode()
     def __call__(self, image: Union[np.ndarray, Image.Image, torch.Tensor], **kwargs: Dict[str, Any]):
```

### Comparing `igniter-1.0.1/igniter/engine/trainer_engine.py` & `igniter-1.0.2/igniter/engine/trainer_engine.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/engine/utils.py` & `igniter-1.0.2/igniter/engine/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
     state_dict = model.state_dict()
     wpth = _remap_keys(weight_dict['model'])
 
     for key in state_dict:
         if key not in wpth or state_dict[key].shape == wpth[key].shape:
             continue
-        logger.info(f'Removing shape missmatch key {key}')
-        wpth.pop(key)
+        logger.warning(f'Shape missmatch key {key} {state_dict[key].shape} != {wpth[key].shape}')
+        # wpth.pop(key)
 
     load_status = model.load_state_dict(wpth, strict=kwargs.get('strict', False))
     logger.info(f'{load_status}')
 
 
 def load_weights_from_s3(path: str, decoder: Union[Callable[..., Any], str, None] = None) -> Dict[str, Any]:
     bucket_name = path[5:].split('/')[0]
```

### Comparing `igniter-1.0.1/igniter/io/s3_client.py` & `igniter-1.0.2/igniter/io/s3_client.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/io/s3_io.py` & `igniter-1.0.2/igniter/io/s3_io.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/io/s3_utils.py` & `igniter-1.0.2/igniter/io/s3_utils.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/logger.py` & `igniter-1.0.2/igniter/logger.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/main.py` & `igniter-1.0.2/igniter/main.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/registry.py` & `igniter-1.0.2/igniter/registry.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/utils.py` & `igniter-1.0.2/igniter/utils.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter/visualizer.py` & `igniter-1.0.2/igniter/visualizer.py`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/igniter.egg-info/PKG-INFO` & `igniter-1.0.2/igniter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igniter
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://github.com/iKrishneel/igniter
 Author: Krishneel
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `igniter-1.0.1/igniter.egg-info/SOURCES.txt` & `igniter-1.0.2/igniter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `igniter-1.0.1/setup.py` & `igniter-1.0.2/setup.py`

 * *Files identical despite different names*

