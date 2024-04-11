# Comparing `tmp/fsm_utils-0.1.0.tar.gz` & `tmp/fsm_utils-0.1.1.tar.gz`

## Comparing `fsm_utils-0.1.0.tar` & `fsm_utils-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 fsm_utils-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     3165 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/.gitignore
--rw-r--r--   0     1001      127      296 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127    11357 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/LICENSE
--rw-r--r--   0     1001      127     5572 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/README.md
--rw-r--r--   0     1001      127      454 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/__init__.py
--rw-r--r--   0     1001      127     1132 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/cache.py
--rw-r--r--   0     1001      127      126 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/config/__init__.py
--rw-r--r--   0     1001      127      633 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/config/config.py
--rw-r--r--   0     1001      127     3065 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/config/token_mapper.py
--rw-r--r--   0     1001      127     3825 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/config/utils.py
--rw-r--r--   0     1001      127      170 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/fsm/__init__.py
--rw-r--r--   0     1001      127     6197 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/fsm/fsm.py
--rw-r--r--   0     1001      127      307 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/fsm/fsm_utils/src/lib.rs
--rw-r--r--   0     1001      127     5227 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/fsm/fsm_utils/src/tokenizer_index.rs
--rw-r--r--   0     1001      127     7133 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/fsm/regex.py
--rw-r--r--   0     1001      127     3255 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/fsm/tokenizer_fsm_patch.py
--rw-r--r--   0     1001      127      658 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/fsm/utils.py
--rw-r--r--   0     1001      127    14619 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/json.py
--rw-r--r--   0     1001      127      330 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/logger.py
--rw-r--r--   0     1001      127     2640 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/regex_constants.py
--rw-r--r--   0     1001      127    14631 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/sampler.py
--rw-r--r--   0     1001      127     5636 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/function_sampler/utils.py
--rw-r--r--   0     1001      127     7984 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/notebooks/Tool_Call_Sampler_demo.ipynb
--rw-r--r--   0     1001      127   266603 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/poetry.lock
--rw-r--r--   0     1001      127     4066 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/tests/test_fsm_comp_time.py
--rw-r--r--   0     1001      127     9247 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127     1079 2024-04-11 22:09:07.000000 fsm_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5695 1970-01-01 00:00:00.000000 fsm_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 fsm_utils-0.1.1/Cargo.toml
+-rw-rw-rw-   0     1000     1000     3409 2024-04-11 22:03:30.000000 fsm_utils-0.1.1/.github/workflows/CI.yml
+-rw-rw-rw-   0     1000        0     3165 2024-04-04 23:27:06.000000 fsm_utils-0.1.1/.gitignore
+-rw-rw-rw-   0     1000     1000      296 2024-04-09 23:48:32.000000 fsm_utils-0.1.1/.pre-commit-config.yaml
+-rw-rw-rw-   0     1000        0    11357 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/LICENSE
+-rw-rw-rw-   0     1000        0     5572 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/README.md
+-rw-rw-rw-   0     1000        0      454 2024-04-09 23:20:22.000000 fsm_utils-0.1.1/function_sampler/__init__.py
+-rw-rw-rw-   0     1000        0     1132 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/function_sampler/cache.py
+-rw-rw-rw-   0     1000        0      126 2024-04-09 23:20:55.000000 fsm_utils-0.1.1/function_sampler/config/__init__.py
+-rw-rw-rw-   0     1000        0      633 2024-04-09 23:21:38.000000 fsm_utils-0.1.1/function_sampler/config/config.py
+-rw-rw-rw-   0     1000     1000     3065 2024-04-09 23:49:00.000000 fsm_utils-0.1.1/function_sampler/config/token_mapper.py
+-rw-rw-rw-   0     1000        0     3825 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/function_sampler/config/utils.py
+-rw-rw-rw-   0     1000        0      170 2024-04-09 23:20:39.000000 fsm_utils-0.1.1/function_sampler/fsm/__init__.py
+-rw-rw-rw-   0     1000     1000     6197 2024-04-11 22:03:30.000000 fsm_utils-0.1.1/function_sampler/fsm/fsm.py
+-rw-rw-rw-   0     1000     1000      307 2024-04-11 22:03:30.000000 fsm_utils-0.1.1/function_sampler/fsm/fsm_utils/src/lib.rs
+-rw-rw-rw-   0     1000     1000     5227 2024-04-11 22:03:30.000000 fsm_utils-0.1.1/function_sampler/fsm/fsm_utils/src/tokenizer_index.rs
+-rw-rw-rw-   0     1000     1000     7133 2024-04-11 22:03:30.000000 fsm_utils-0.1.1/function_sampler/fsm/regex.py
+-rw-rw-rw-   0     1000     1000     3255 2024-04-11 22:03:30.000000 fsm_utils-0.1.1/function_sampler/fsm/tokenizer_fsm_patch.py
+-rw-rw-rw-   0     1000     1000      658 2024-04-10 23:50:29.000000 fsm_utils-0.1.1/function_sampler/fsm/utils.py
+-rw-rw-rw-   0     1000        0    14619 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/function_sampler/json.py
+-rw-rw-rw-   0     1000        0      330 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/function_sampler/logger.py
+-rw-rw-rw-   0     1000        0     2640 2024-04-09 22:08:19.000000 fsm_utils-0.1.1/function_sampler/regex_constants.py
+-rw-rw-rw-   0     1000     1000    14631 2024-04-09 23:49:00.000000 fsm_utils-0.1.1/function_sampler/sampler.py
+-rw-rw-rw-   0     1000        0     5636 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/function_sampler/utils.py
+-rw-rw-rw-   0     1000        0     7984 2024-04-01 12:34:26.000000 fsm_utils-0.1.1/notebooks/Tool_Call_Sampler_demo.ipynb
+-rw-rw-rw-   0     1000        0   266603 2024-04-09 23:07:33.000000 fsm_utils-0.1.1/poetry.lock
+-rw-rw-rw-   0     1000     1000     4066 2024-04-10 23:24:53.000000 fsm_utils-0.1.1/tests/test_fsm_comp_time.py
+-rw-rw-rw-   0     1000     1000     9247 2024-04-11 22:34:04.000000 fsm_utils-0.1.1/Cargo.lock
+-rw-rw-rw-   0     1000     1000     1079 2024-04-11 22:33:32.000000 fsm_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5695 1970-01-01 00:00:00.000000 fsm_utils-0.1.1/PKG-INFO
```

### Comparing `fsm_utils-0.1.0/.github/workflows/CI.yml` & `fsm_utils-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/.gitignore` & `fsm_utils-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/LICENSE` & `fsm_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/README.md` & `fsm_utils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/cache.py` & `fsm_utils-0.1.1/function_sampler/cache.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/config/config.py` & `fsm_utils-0.1.1/function_sampler/config/config.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/config/token_mapper.py` & `fsm_utils-0.1.1/function_sampler/config/token_mapper.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/config/utils.py` & `fsm_utils-0.1.1/function_sampler/config/utils.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/fsm/fsm.py` & `fsm_utils-0.1.1/function_sampler/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/fsm/fsm_utils/src/tokenizer_index.rs` & `fsm_utils-0.1.1/function_sampler/fsm/fsm_utils/src/tokenizer_index.rs`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/fsm/regex.py` & `fsm_utils-0.1.1/function_sampler/fsm/regex.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/fsm/tokenizer_fsm_patch.py` & `fsm_utils-0.1.1/function_sampler/fsm/tokenizer_fsm_patch.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/fsm/utils.py` & `fsm_utils-0.1.1/function_sampler/fsm/utils.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/json.py` & `fsm_utils-0.1.1/function_sampler/json.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/regex_constants.py` & `fsm_utils-0.1.1/function_sampler/regex_constants.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/sampler.py` & `fsm_utils-0.1.1/function_sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/function_sampler/utils.py` & `fsm_utils-0.1.1/function_sampler/utils.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/notebooks/Tool_Call_Sampler_demo.ipynb` & `fsm_utils-0.1.1/notebooks/Tool_Call_Sampler_demo.ipynb`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/poetry.lock` & `fsm_utils-0.1.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/tests/test_fsm_comp_time.py` & `fsm_utils-0.1.1/tests/test_fsm_comp_time.py`

 * *Files identical despite different names*

### Comparing `fsm_utils-0.1.0/Cargo.lock` & `fsm_utils-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "fsm_utils"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "rayon",
 ]
 
 [[package]]
 name = "heck"
```

### Comparing `fsm_utils-0.1.0/pyproject.toml` & `fsm_utils-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "function-sampler"
 packages = [
     { include = "function_sampler" },
 ]
-version = "0.1.4"
+version = "0.1.5"
 description = "Function calling Logit Sampler"
 authors = ["Nathan Hoos <thwackyy.y@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `fsm_utils-0.1.0/PKG-INFO` & `fsm_utils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fsm_utils
-Version: 0.1.0
+Version: 0.1.1
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Function Sampler
 
 <a target="_blank" href="https://colab.research.google.com/github/unaidedelf8777/function-sampler/blob/main/notebooks/Tool_Call_Sampler_demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
```

