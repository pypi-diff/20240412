# Comparing `tmp/pve_cli-0.4.0a0.tar.gz` & `tmp/pve_cli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pve_cli-0.4.0a0.tar", max compression
+gzip compressed data, was "pve_cli-0.4.1.tar", max compression
```

## Comparing `pve_cli-0.4.0a0.tar` & `pve_cli-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    16725 2023-12-25 02:44:02.622926 pve_cli-0.4.0a0/LICENSE
--rw-r--r--   0        0        0      594 2023-12-25 02:44:02.626926 pve_cli-0.4.0a0/README.md
--rw-r--r--   0        0        0      198 2023-12-25 02:44:02.626926 pve_cli-0.4.0a0/pve_cli/__init__.py
--rw-r--r--   0        0        0     3727 2024-02-05 19:02:35.494526 pve_cli-0.4.0a0/pve_cli/guest_cmd.py
--rw-r--r--   0        0        0     1880 2024-01-21 23:14:01.996698 pve_cli-0.4.0a0/pve_cli/main.py
--rw-r--r--   0        0        0     5646 2023-12-25 02:44:02.634926 pve_cli-0.4.0a0/pve_cli/nodes_cmd.py
--rw-r--r--   0        0        0      233 2023-12-25 02:44:02.634926 pve_cli-0.4.0a0/pve_cli/proxmox/__init__.py
--rw-r--r--   0        0        0     3849 2024-02-22 15:55:23.646926 pve_cli-0.4.0a0/pve_cli/proxmox/api.py
--rw-r--r--   0        0        0      449 2023-12-25 02:44:02.638926 pve_cli-0.4.0a0/pve_cli/proxmox/exceptions.py
--rw-r--r--   0        0        0       96 2023-12-25 02:44:02.638926 pve_cli-0.4.0a0/pve_cli/proxmox/types.py
--rw-r--r--   0        0        0        0 2024-02-22 15:59:48.224110 pve_cli-0.4.0a0/pve_cli/util/__init__.py
--rw-r--r--   0        0        0      910 2024-01-21 23:14:01.996698 pve_cli-0.4.0a0/pve_cli/util/callbacks.py
--rw-r--r--   0        0        0      129 2023-12-25 02:44:02.638926 pve_cli-0.4.0a0/pve_cli/util/exceptions.py
--rw-r--r--   0        0        0     1574 2023-12-26 03:06:30.801607 pve_cli-0.4.0a0/pve_cli/util/validators.py
--rw-r--r--   0        0        0     1936 2024-02-22 15:46:56.936585 pve_cli-0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 pve_cli-0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-12-25 02:44:02.622926 pve_cli-0.4.1/LICENSE
+-rw-r--r--   0        0        0      594 2023-12-25 02:44:02.626926 pve_cli-0.4.1/README.md
+-rw-r--r--   0        0        0      198 2023-12-25 02:44:02.626926 pve_cli-0.4.1/pve_cli/__init__.py
+-rw-r--r--   0        0        0     3727 2024-02-05 19:02:35.494526 pve_cli-0.4.1/pve_cli/guest_cmd.py
+-rw-r--r--   0        0        0     1880 2024-01-21 23:14:01.996698 pve_cli-0.4.1/pve_cli/main.py
+-rw-r--r--   0        0        0     5646 2023-12-25 02:44:02.634926 pve_cli-0.4.1/pve_cli/nodes_cmd.py
+-rw-r--r--   0        0        0      233 2023-12-25 02:44:02.634926 pve_cli-0.4.1/pve_cli/proxmox/__init__.py
+-rw-r--r--   0        0        0     3849 2024-02-22 15:55:23.646926 pve_cli-0.4.1/pve_cli/proxmox/api.py
+-rw-r--r--   0        0        0      449 2023-12-25 02:44:02.638926 pve_cli-0.4.1/pve_cli/proxmox/exceptions.py
+-rw-r--r--   0        0        0       96 2023-12-25 02:44:02.638926 pve_cli-0.4.1/pve_cli/proxmox/types.py
+-rw-r--r--   0        0        0        0 2024-02-26 02:54:23.682469 pve_cli-0.4.1/pve_cli/util/__init__.py
+-rw-r--r--   0        0        0      910 2024-01-21 23:14:01.996698 pve_cli-0.4.1/pve_cli/util/callbacks.py
+-rw-r--r--   0        0        0      129 2023-12-25 02:44:02.638926 pve_cli-0.4.1/pve_cli/util/exceptions.py
+-rw-r--r--   0        0        0     1574 2023-12-26 03:06:30.801607 pve_cli-0.4.1/pve_cli/util/validators.py
+-rw-r--r--   0        0        0     1935 2024-02-26 02:09:37.038606 pve_cli-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 pve_cli-0.4.1/PKG-INFO
```

### Comparing `pve_cli-0.4.0a0/LICENSE` & `pve_cli-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/README.md` & `pve_cli-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/pve_cli/guest_cmd.py` & `pve_cli-0.4.1/pve_cli/guest_cmd.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/pve_cli/main.py` & `pve_cli-0.4.1/pve_cli/main.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/pve_cli/nodes_cmd.py` & `pve_cli-0.4.1/pve_cli/nodes_cmd.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/pve_cli/proxmox/api.py` & `pve_cli-0.4.1/pve_cli/proxmox/api.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/pve_cli/util/callbacks.py` & `pve_cli-0.4.1/pve_cli/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/pve_cli/util/validators.py` & `pve_cli-0.4.1/pve_cli/util/validators.py`

 * *Files identical despite different names*

### Comparing `pve_cli-0.4.0a0/pyproject.toml` & `pve_cli-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "pve-cli"
-version = "0.4.0a0"
+version = "0.4.1"
 description = "CLI Tool to manage VMs and more on proxmox clusters"
 license = "MPL-2.0"
 authors = ["Dominik Rimpf <dev@drimpf.de>"]
 readme = "README.md"
-packages = [{include = "pve_cli"}]
 
 [tool.poetry.scripts]
 pve-cli = "pve_cli.main:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 proxmoxer = "^2.0.1"
 requests = "^2.31.0"
 typer = {extras = ["all"], version = "^0.9.0"}
 toml = "^0.10.2"
 requests-toolbelt = "^1.0.0"
 
 [tool.poetry.group.lint.dependencies]
 bandit = {extras = ["toml"], version = "^1.7.4"}
-ruff = "^0.1.7"
-mypy = "^0.991"
+ruff = "^0.2.2"
+mypy = "^1.8.0"
 types-toml = "^0.10.8.1" # for mypy
 types-requests = "^2.28.11.7" # for mypy
+mypy-gitlab-code-quality = "^1.1.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.0"
+pytest = "^8.0.2"
 pytest-cov = "^4.0.0"
 
 [tool.ruff]
 # 80 chars aren't enough in 21 century
 line-length = 128
 indent-width = 2
```

### Comparing `pve_cli-0.4.0a0/PKG-INFO` & `pve_cli-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pve-cli
-Version: 0.4.0a0
+Version: 0.4.1
 Summary: CLI Tool to manage VMs and more on proxmox clusters
 License: MPL-2.0
 Author: Dominik Rimpf
 Author-email: dev@drimpf.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

