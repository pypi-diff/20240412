# Comparing `tmp/xtrain-0.1.3.tar.gz` & `tmp/xtrain-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtrain-0.1.3.tar", max compression
+gzip compressed data, was "xtrain-0.2.0.tar", max compression
```

## Comparing `xtrain-0.1.3.tar` & `xtrain-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,9 @@
--rw-r--r--   0        0        0     1241 2023-08-24 17:42:08.716548 xtrain-0.1.3/README.md
--rw-r--r--   0        0        0      804 2023-09-07 14:35:27.673045 xtrain-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      195 2023-08-25 14:11:54.440237 xtrain-0.1.3/xtrain/__init__.py
--rw-r--r--   0        0        0      300 2023-08-21 19:39:54.862974 xtrain-0.1.3/xtrain/data/__init__.py
--rw-r--r--   0        0        0      647 2023-08-25 14:11:53.356729 xtrain-0.1.3/xtrain/data/tf_dataset_adapter.py
--rw-r--r--   0        0        0      936 2023-08-25 14:11:53.364708 xtrain-0.1.3/xtrain/data/torch_dataloader_adapter.py
--rw-r--r--   0        0        0      802 2023-08-21 19:39:54.880479 xtrain-0.1.3/xtrain/data/utils.py
--rw-r--r--   0        0        0     1978 2023-08-25 14:11:54.493580 xtrain-0.1.3/xtrain/loss.py
--rw-r--r--   0        0        0     4281 2023-08-25 14:11:54.504598 xtrain-0.1.3/xtrain/strategy.py
--rw-r--r--   0        0        0    12898 2023-09-07 14:25:36.491888 xtrain-0.1.3/xtrain/trainer.py
--rw-r--r--   0        0        0     1024 2023-09-05 13:48:52.833837 xtrain-0.1.3/xtrain/types.py
--rw-r--r--   0        0        0     2292 2023-08-25 14:11:54.539041 xtrain-0.1.3/xtrain/utils.py
--rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 xtrain-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-12 13:52:13.296116 xtrain-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1231 2024-04-12 13:52:13.296116 xtrain-0.2.0/README.md
+-rw-r--r--   0        0        0      833 2024-04-12 13:52:31.264183 xtrain-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/__init__.py
+-rw-r--r--   0        0        0    10295 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/base_trainer.py
+-rw-r--r--   0        0        0     1289 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/loss.py
+-rw-r--r--   0        0        0     4564 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/strategy.py
+-rw-r--r--   0        0        0     5517 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/utils.py
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.0/PKG-INFO
```

### Comparing `xtrain-0.1.3/README.md` & `xtrain-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 ### General workflow
 
 #### Step 1: define your model
 
 ```
 class MyFlaxModule(nn.Module):
+  @nn.compact
   def __call__(self, x):
     ...
 ```
 
 #### Step 2: define loss function
 
 ```
-def my_loss_func(**kwargs):
-    model_out = kwargs["preds"]
-    labels = kwargs["labels"]
+def my_loss_func(batch, prediction):
+    x, y_true = batch
     loss = ....
     return loss
 ```
 
 #### Step 3: create an iterator that supplies training data
 
 ```
@@ -37,24 +37,24 @@
 #### Step 4: train
 
 ```
 # create and initialize a Trainer object
 trainer = xtrain.Trainer(
   model = MyFlaxModule(),
   losses = my_loss_func,
+  optimizer = optax.adam(1e-4),
 )
-trainer.initialize(my_data, tx=my_optax_optimizer)
 
-train_iter = trainer.train(my_data) # returns a python iterator
+train_iter = trainer.train(my_data) # returns a iterable object
 
 # iterate the train_iter trains the model
 for step in range(train_steps):
-    avg_loss = next(train_iter)
+    model_out = next(train_iter)
     if step // 1000 == 0:
-        print(avg_loss)
-        trainer.reset()
+        print(train_iter.loss_logs)
+        train_iter.reset_loss_logs()
 ```
 
 ### Full documentation
 
 https://jiyuuchc.github.io/xtrain/
```

### Comparing `xtrain-0.1.3/pyproject.toml` & `xtrain-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "xtrain"
-version = "0.1.3"
+version = "0.2.0"
 description = "A Flax trainer"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9 <3.11"
-flax = "^0.7.2"
-
-[tool.poetry.group.dev]
-optional = true
+python = "^3.10"
+flax = "^0.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
-jax = {extras = ["cuda11-pip"], version = "^0.4.14"}
-tensorflow-cpu = "^2.13.0"
+jax = {extras = ["cuda11_pip"], version = "^0.4, <=0.4.24"}
+nvidia-cudnn-cu11 = "^8.0" # bypass jax packaging error
+tensorflow = "^2.16.1"
+orbax-checkpoint = "0.5.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.2.3"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
@@ -28,9 +27,8 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "jax"
 url = "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
-default = false
-secondary = false
+priority = "supplemental"
```

### Comparing `xtrain-0.1.3/PKG-INFO` & `xtrain-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: xtrain
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Flax trainer
 Author: Ji Yu
 Author-email: jyu@uchc.edu
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: flax (>=0.7.2,<0.8.0)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: flax (>=0.8,<0.9)
 Description-Content-Type: text/markdown
 
 ## XTRAIN: a tiny library for training [Flax](https://github.com/google/flax) models.
 
 Design goals:
 
   - Help avoiding boiler-plate code
@@ -21,24 +22,24 @@
 
 ### General workflow
 
 #### Step 1: define your model
 
 ```
 class MyFlaxModule(nn.Module):
+  @nn.compact
   def __call__(self, x):
     ...
 ```
 
 #### Step 2: define loss function
 
 ```
-def my_loss_func(**kwargs):
-    model_out = kwargs["preds"]
-    labels = kwargs["labels"]
+def my_loss_func(batch, prediction):
+    x, y_true = batch
     loss = ....
     return loss
 ```
 
 #### Step 3: create an iterator that supplies training data
 
 ```
@@ -50,25 +51,25 @@
 #### Step 4: train
 
 ```
 # create and initialize a Trainer object
 trainer = xtrain.Trainer(
   model = MyFlaxModule(),
   losses = my_loss_func,
+  optimizer = optax.adam(1e-4),
 )
-trainer.initialize(my_data, tx=my_optax_optimizer)
 
-train_iter = trainer.train(my_data) # returns a python iterator
+train_iter = trainer.train(my_data) # returns a iterable object
 
 # iterate the train_iter trains the model
 for step in range(train_steps):
-    avg_loss = next(train_iter)
+    model_out = next(train_iter)
     if step // 1000 == 0:
-        print(avg_loss)
-        trainer.reset()
+        print(train_iter.loss_logs)
+        train_iter.reset_loss_logs()
 ```
 
 ### Full documentation
 
 https://jiyuuchc.github.io/xtrain/
```

