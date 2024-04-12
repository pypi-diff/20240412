# Comparing `tmp/pogema-toolbox-0.0.2.tar.gz` & `tmp/pogema-toolbox-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogema-toolbox-0.0.2.tar", last modified: Fri Apr 12 13:53:32 2024, max compression
+gzip compressed data, was "pogema-toolbox-0.0.3a1.tar", last modified: Fri Apr 12 16:14:02 2024, max compression
```

## Comparing `pogema-toolbox-0.0.2.tar` & `pogema-toolbox-0.0.3a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.828540 pogema-toolbox-0.0.2/
--rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/LICENSE
--rw-r--r--   0 skrynnik   (503) staff       (20)      718 2024-04-12 13:53:32.826687 pogema-toolbox-0.0.2/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema-toolbox-0.0.2/README.md
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.798082 pogema-toolbox-0.0.2/pogema_toolbox/
--rw-r--r--   0 skrynnik   (503) staff       (20)       22 2024-04-12 13:46:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      370 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.2/pogema_toolbox/algorithm_config.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.2/pogema_toolbox/config_variant_generator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2209 2024-04-12 13:30:32.000000 pogema-toolbox-0.0.2/pogema_toolbox/create_env.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.2/pogema_toolbox/eval_utils.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    11912 2024-04-12 13:51:28.000000 pogema-toolbox-0.0.2/pogema_toolbox/evaluator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema-toolbox-0.0.2/pogema_toolbox/fix_num_threads_issue.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.810210 pogema-toolbox-0.0.2/pogema_toolbox/maps/
--rw-r--r--   0 skrynnik   (503) staff       (20)      870 2024-04-12 09:29:53.000000 pogema-toolbox-0.0.2/pogema_toolbox/maps/default-maps.yaml
--rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/registry.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema-toolbox-0.0.2/pogema_toolbox/results_holder.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.822619 pogema-toolbox-0.0.2/pogema_toolbox/views/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_multi_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_tabular.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.2/pogema_toolbox/views/view_utils.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 13:53:32.824612 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/
--rw-r--r--   0 skrynnik   (503) staff       (20)      718 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/requires.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-04-12 13:53:32.000000 pogema-toolbox-0.0.2/pogema_toolbox.egg-info/top_level.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-12 13:53:32.828818 pogema-toolbox-0.0.2/setup.cfg
--rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema-toolbox-0.0.2/setup.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:14:02.533568 pogema-toolbox-0.0.3a1/
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a1/LICENSE
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-12 16:14:02.531844 pogema-toolbox-0.0.3a1/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema-toolbox-0.0.3a1/README.md
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:14:02.508091 pogema-toolbox-0.0.3a1/pogema_toolbox/
+-rw-r--r--   0 skrynnik   (503) staff       (20)       25 2024-04-12 16:13:34.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      370 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/algorithm_config.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/config_variant_generator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2209 2024-04-12 13:30:32.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/create_env.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/eval_utils.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11780 2024-04-12 16:13:34.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/evaluator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/fix_num_threads_issue.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:14:02.519940 pogema-toolbox-0.0.3a1/pogema_toolbox/maps/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      870 2024-04-12 09:29:53.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/maps/default-maps.yaml
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/registry.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/results_holder.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:14:02.529055 pogema-toolbox-0.0.3a1/pogema_toolbox/views/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/views/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_multi_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_tabular.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_utils.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:14:02.530894 pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-12 16:14:02.000000 pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-04-12 16:14:02.000000 pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-12 16:14:02.000000 pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-04-12 16:14:02.000000 pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/requires.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-04-12 16:14:02.000000 pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-12 16:14:02.533683 pogema-toolbox-0.0.3a1/setup.cfg
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema-toolbox-0.0.3a1/setup.py
```

### Comparing `pogema-toolbox-0.0.2/LICENSE` & `pogema-toolbox-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/PKG-INFO` & `pogema-toolbox-0.0.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.2
+Version: 0.0.3a1
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/config_variant_generator.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/config_variant_generator.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/create_env.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/create_env.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/eval_utils.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/eval_utils.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/evaluator.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,30 +57,28 @@
     """
     registry = ToolboxRegistry
     if registry_state is not None:
         registry.recreate_from_state(registry_state)
 
     results = []
     algo_name = algo_config['name']
-    # algo_cfg = toolbox_registry.make_config(algo_name, **algo_config)
-    # algo = toolbox_registry.make(algo_name, **algo_config)
     algo = registry.create_algorithm(algo_name, **algo_config)
     algo_cfg = registry.create_algorithm_config(algo_name, **algo_config)
     for idx, env_config in enumerate(env_configs):
         logger.info(f'Running: {full_algo_name} [{idx + 1}/{len(env_configs)}]')
         env = registry.create_env(env_config['name'], **env_config)
         if algo_cfg.preprocessing:
             logger.debug('Adding preprocessing')
             env = registry.create_algorithm_preprocessing(env, algo_name, **algo_config)
         results.append(run_episode(env, algo))
 
         if env_config.get('with_animation', None):
             from pathlib import Path
 
-            directory = Path(f'renders/{algo_cfg.name}/')
+            directory = Path(f'renders/{full_algo_name}/')
             name = env.pick_name(env.grid_config)
 
             directory.mkdir(parents=True, exist_ok=True)
             logger.info(f'Saving animation to "{directory / name}"')
             env.save_animation(name=directory / name)
     return results
```

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/maps/default-maps.yaml` & `pogema-toolbox-0.0.3a1/pogema_toolbox/maps/default-maps.yaml`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/registry.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/registry.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/views/view_multi_plot.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_multi_plot.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/views/view_plot.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_plot.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/views/view_tabular.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_tabular.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox/views/view_utils.py` & `pogema-toolbox-0.0.3a1/pogema_toolbox/views/view_utils.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox.egg-info/PKG-INFO` & `pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.2
+Version: 0.0.3a1
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-toolbox-0.0.2/pogema_toolbox.egg-info/SOURCES.txt` & `pogema-toolbox-0.0.3a1/pogema_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.2/setup.py` & `pogema-toolbox-0.0.3a1/setup.py`

 * *Files identical despite different names*

