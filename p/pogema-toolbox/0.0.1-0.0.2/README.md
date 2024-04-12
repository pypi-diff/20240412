# Comparing `tmp/pogema-toolbox-0.0.1.tar.gz` & `tmp/pogema-toolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogema-toolbox-0.0.1.tar", last modified: Wed Apr  3 20:33:40 2024, max compression
+gzip compressed data, was "pogema-toolbox-0.0.2.tar", last modified: Fri Apr 12 13:53:32 2024, max compression
```

## Comparing `pogema-toolbox-0.0.1.tar` & `pogema-toolbox-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-03 20:33:40.669623 pogema-toolbox-0.0.1/
--rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/LICENSE
--rw-r--r--   0 skrynnik   (503) staff       (20)      718 2024-04-03 20:33:40.667032 pogema-toolbox-0.0.1/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema-toolbox-0.0.1/README.md
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-03 20:33:40.643504 pogema-toolbox-0.0.1/pogema_toolbox/
--rw-r--r--   0 skrynnik   (503) staff       (20)       22 2024-03-22 15:02:21.000000 pogema-toolbox-0.0.1/pogema_toolbox/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      370 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.1/pogema_toolbox/algorithm_config.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.1/pogema_toolbox/config_variant_generator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2180 2024-04-03 14:08:38.000000 pogema-toolbox-0.0.1/pogema_toolbox/create_env.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.1/pogema_toolbox/eval_utils.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    11104 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/pogema_toolbox/evaluator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema-toolbox-0.0.1/pogema_toolbox/fix_num_threads_issue.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/pogema_toolbox/registry.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema-toolbox-0.0.1/pogema_toolbox/results_holder.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-03 20:33:40.664142 pogema-toolbox-0.0.1/pogema_toolbox/views/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.1/pogema_toolbox/views/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3138 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/pogema_toolbox/views/view_multi_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/pogema_toolbox/views/view_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/pogema_toolbox/views/view_tabular.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/pogema_toolbox/views/view_utils.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-03 20:33:40.666073 pogema-toolbox-0.0.1/pogema_toolbox.egg-info/
--rw-r--r--   0 skrynnik   (503) staff       (20)      718 2024-04-03 20:33:40.000000 pogema-toolbox-0.0.1/pogema_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)      723 2024-04-03 20:33:40.000000 pogema-toolbox-0.0.1/pogema_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-03 20:33:40.000000 pogema-toolbox-0.0.1/pogema_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-04-03 20:33:40.000000 pogema-toolbox-0.0.1/pogema_toolbox.egg-info/requires.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-04-03 20:33:40.000000 pogema-toolbox-0.0.1/pogema_toolbox.egg-info/top_level.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-03 20:33:40.669740 pogema-toolbox-0.0.1/setup.cfg
--rw-r--r--   0 skrynnik   (503) staff       (20)     1687 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.1/setup.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.828540 pogema-toolbox-0.0.2/
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/LICENSE
+-rw-r--r--   0 skrynnik   (503) staff       (20)      718 2024-04-12 13:53:32.826687 pogema-toolbox-0.0.2/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema-toolbox-0.0.2/README.md
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.798082 pogema-toolbox-0.0.2/pogema_toolbox/
+-rw-r--r--   0 skrynnik   (503) staff       (20)       22 2024-04-12 13:46:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      370 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.2/pogema_toolbox/algorithm_config.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.2/pogema_toolbox/config_variant_generator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2209 2024-04-12 13:30:32.000000 pogema-toolbox-0.0.2/pogema_toolbox/create_env.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.2/pogema_toolbox/eval_utils.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11912 2024-04-12 13:51:28.000000 pogema-toolbox-0.0.2/pogema_toolbox/evaluator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema-toolbox-0.0.2/pogema_toolbox/fix_num_threads_issue.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.810210 pogema-toolbox-0.0.2/pogema_toolbox/maps/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      870 2024-04-12 09:29:53.000000 pogema-toolbox-0.0.2/pogema_toolbox/maps/default-maps.yaml
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/registry.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema-toolbox-0.0.2/pogema_toolbox/results_holder.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.822619 pogema-toolbox-0.0.2/pogema_toolbox/views/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_multi_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_tabular.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_utils.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.824612 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      718 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/requires.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-12 13:53:32.828818 pogema-toolbox-0.0.2/setup.cfg
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema-toolbox-0.0.2/setup.py
```

### Comparing `pogema-toolbox-0.0.1/LICENSE` & `pogema-toolbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.1/PKG-INFO` & `pogema-toolbox-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/config_variant_generator.py` & `pogema-toolbox-0.0.2/pogema_toolbox/config_variant_generator.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/create_env.py` & `pogema-toolbox-0.0.2/pogema_toolbox/create_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,10 +58,10 @@
 
 def create_env_base(config: Environment):
     env = pogema_v0(grid_config=config.grid_config)
     env = ProvideGlobalObstacles(env)
     if config.use_maps:
         env = MultiMapWrapper(env)
     if config.with_animation:
-        env = AnimationMonitor(env, AnimationConfig(directory='experiments/renders'))
+        env = AnimationMonitor(env, AnimationConfig(directory='experiments/renders', save_every_idx_episode=None))
 
     return env
```

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/eval_utils.py` & `pogema-toolbox-0.0.2/pogema_toolbox/eval_utils.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/evaluator.py` & `pogema-toolbox-0.0.2/pogema_toolbox/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # noinspection PyUnresolvedReferences
 from pogema_toolbox import fix_num_threads_issue
 
 import json
 from pathlib import Path
-
+from loguru import logger
 import time
 
 import numpy as np
-from loguru import logger
 
 from pogema_toolbox.config_variant_generator import generate_variants
 from pogema_toolbox.create_env import Environment
 from pogema_toolbox.registry import ToolboxRegistry
 
 from pogema_toolbox.views.view_multi_plot import process_multi_plot_view, MultiPlotView
 from pogema_toolbox.views.view_plot import process_plot_view, PlotView
@@ -69,14 +68,24 @@
     for idx, env_config in enumerate(env_configs):
         logger.info(f'Running: {full_algo_name} [{idx + 1}/{len(env_configs)}]')
         env = registry.create_env(env_config['name'], **env_config)
         if algo_cfg.preprocessing:
             logger.debug('Adding preprocessing')
             env = registry.create_algorithm_preprocessing(env, algo_name, **algo_config)
         results.append(run_episode(env, algo))
+
+        if env_config.get('with_animation', None):
+            from pathlib import Path
+
+            directory = Path(f'renders/{algo_cfg.name}/')
+            name = env.pick_name(env.grid_config)
+
+            directory.mkdir(parents=True, exist_ok=True)
+            logger.info(f'Saving animation to "{directory / name}"')
+            env.save_animation(name=directory / name)
     return results
 
 
 def split_on_chunks(size, num_chunks):
     """
     Splits the given size into equal chunks.
 
@@ -148,16 +157,15 @@
     Returns:
         List: Results of running the algorithm on the environments.
     """
     import dask.distributed as dd
     initialized_algo_config = ToolboxRegistry.create_algorithm_config(algo_config['name'], **algo_config)
 
     num_process = min(initialized_algo_config.num_process, get_num_of_available_cpus())
-    cluster = dd.LocalCluster(n_workers=num_process, threads_per_worker=1,
-                              nthreads=1, )  # Create a Dask cluster
+    cluster = dd.LocalCluster(n_workers=num_process, threads_per_worker=1, nthreads=1, )
     client = dd.Client(cluster, timeout="120s")  # Connect the client to the cluster
 
     futures = []
     for left, right in split_on_chunks(len(env_configs), initialized_algo_config.num_process):
         future = client.submit(sequential_backend, algo_config, env_configs[left:right], full_algo_name)
         futures.append(future)
 
@@ -185,15 +193,15 @@
 
     initialized_algo_config = ToolboxRegistry.create_algorithm_config(algo_config['name'], **algo_config)
 
     num_process = min(initialized_algo_config.num_process, get_num_of_available_cpus())
     balanced_buckets = get_balanced_buckets_indexes(env_configs, num_process)
 
     cluster = dd.LocalCluster(n_workers=num_process, threads_per_worker=1, nthreads=1)
-    client = dd.Client(cluster)
+    client = dd.Client(cluster, timeout="120s")  # Connect the client to the cluster
 
     futures = []
 
     # Getting maps to initialize registry (if not) and  avoid multiple loading
     ToolboxRegistry.get_maps()
     registry_state = ToolboxRegistry.get_state()
 
@@ -246,14 +254,17 @@
         evaluation_config: Configuration for the evaluation.
         eval_dir: Directory to save the views (optional).
 
     Returns:
         List: Results of running the views.
     """
     view_results = []
+    if 'results_views' not in evaluation_config:
+        logger.info("No result views provided in config")
+        return
     for key, view in evaluation_config['results_views'].items():
         save_path = Path(eval_dir if eval_dir else '.') / f'{key}.pdf'
         # create directory if not exists
         save_path.parent.mkdir(parents=True, exist_ok=True)
 
         if view['type'] == 'tabular':
             view_results.append(process_table_view(results, TabularView(**view)))
@@ -280,16 +291,20 @@
     results = []
     for key, algo_cfg in evaluation_config['algorithms'].items():
         p_algo_cfg = ToolboxRegistry.create_algorithm_config(algo_cfg['name'], **algo_cfg)
         logger.info(f'Starting: {key}, {algo_cfg}')
         start_time = time.monotonic()
         if p_algo_cfg.parallel_backend == 'sequential':
             metrics = sequential_backend(algo_cfg, environment_configs, key)
+        # elif p_algo_cfg.parallel_backend == 'multiprocessing':
+        #     metrics = multiprocess_backend(algo_cfg, environment_configs, key)
         elif p_algo_cfg.parallel_backend == 'dask':
             metrics = dask_backend(algo_cfg, environment_configs, key)
+        # elif p_algo_cfg.parallel_backend == 'balanced_multiprocessing':
+        #     metrics = balanced_multiprocess_backend(algo_cfg, environment_configs, key)
         elif p_algo_cfg.parallel_backend == 'balanced_dask':
             metrics = balanced_dask_backend(algo_cfg, environment_configs, key)
         else:
             raise ValueError(f'Unknown parallel backend: {p_algo_cfg.parallel_backend}')
         algo_results = join_metrics_and_configs(metrics, environment_configs, env_grid_search, algo_cfg, key)
         if eval_dir:
             save_path = Path(eval_dir) / f'{key}.json'
```

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/registry.py` & `pogema-toolbox-0.0.2/pogema_toolbox/registry.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/views/view_multi_plot.py` & `pogema-toolbox-0.0.2/pogema_toolbox/views/view_multi_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class MultiPlotView(PlotView):
     type: Literal['multi-plot'] = 'multi-plot'
     over: str = None
     num_cols: int = 3
     share_x: bool = False
     share_y: bool = False
-    remove_individual_titles: bool = False
+    remove_individual_titles: bool = True
     legend_bbox_to_anchor: Tuple[float, float] = (0.5, -0.05)
     legend_loc: str = 'lower center'
     legend_columns: int = 5
     width: float = 2.0
     height: float = 2.0
```

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/views/view_plot.py` & `pogema-toolbox-0.0.2/pogema_toolbox/views/view_plot.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/views/view_tabular.py` & `pogema-toolbox-0.0.2/pogema_toolbox/views/view_tabular.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox/views/view_utils.py` & `pogema-toolbox-0.0.2/pogema_toolbox/views/view_utils.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox.egg-info/PKG-INFO` & `pogema-toolbox-0.0.2/pogema_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-toolbox-0.0.1/pogema_toolbox.egg-info/SOURCES.txt` & `pogema-toolbox-0.0.2/pogema_toolbox.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 ./pogema_toolbox/registry.py
 ./pogema_toolbox/results_holder.py
 ./pogema_toolbox.egg-info/PKG-INFO
 ./pogema_toolbox.egg-info/SOURCES.txt
 ./pogema_toolbox.egg-info/dependency_links.txt
 ./pogema_toolbox.egg-info/requires.txt
 ./pogema_toolbox.egg-info/top_level.txt
+./pogema_toolbox/maps/default-maps.yaml
 ./pogema_toolbox/views/__init__.py
 ./pogema_toolbox/views/view_multi_plot.py
 ./pogema_toolbox/views/view_plot.py
 ./pogema_toolbox/views/view_tabular.py
 ./pogema_toolbox/views/view_utils.py
```

### Comparing `pogema-toolbox-0.0.1/setup.py` & `pogema-toolbox-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,8 +55,11 @@
     extras_require={
 
     },
     package_dir={'': './'},
     packages=find_packages(where='./', include='pogema_toolbox*'),
     include_package_data=True,
     python_requires='>=3.8',
+    package_data={
+        'pogema_toolbox': ['maps/*.yaml'],
+    },
 )
```

