# Comparing `tmp/truefoundry-0.2.0rc2.tar.gz` & `tmp/truefoundry-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.0rc2.tar", max compression
+gzip compressed data, was "truefoundry-0.2.0rc3.tar", max compression
```

## Comparing `truefoundry-0.2.0rc2.tar` & `truefoundry-0.2.0rc3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      871 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/README.md
--rw-r--r--   0        0        0     1147 2024-04-12 07:12:28.672483 truefoundry-0.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4428 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2348 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    10660 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0      435 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0       54 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      854 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5890 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     5076 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     1751 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0     5358 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0     1585 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       29 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0       39 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      151 2024-04-12 07:12:18.760489 truefoundry-0.2.0rc2/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/README.md
+-rw-r--r--   0        0        0     1147 2024-04-12 09:01:53.023285 truefoundry-0.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4428 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2348 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    10572 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0      435 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0       54 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5890 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5076 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     1751 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0     5358 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0     1585 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-12 09:01:42.827275 truefoundry-0.2.0rc3/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc3/PKG-INFO
```

### Comparing `truefoundry-0.2.0rc2/README.md` & `truefoundry-0.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/pyproject.toml` & `truefoundry-0.2.0rc3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.0rc2"
+version = "0.2.0rc3"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
 servicefoundry = "0.10.6"
```

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/agents/tester.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,16 @@
         else:
             console.print(
                 f"[bold magenta]TFY-Agent:[/] Continuing on [green]{current_active_branch!r}[/]"
             )
 
     except InvalidGitRepositoryError:
         console.print(
-            "[red]Error:[/] This operation can only be performed inside a Git repository."
+            "[red]Error:[/] This operation can only be performed inside a Git repository.\n"
+            "Execute 'git init' to create a new repository."
         )
         sys.exit(1)
 
     except GitCommandError as gce:
         console.print(
             f"Command execution failed due to the following error:[red]{gce.stderr}[/]".replace(
                 "\n  stderr:", ""
@@ -194,17 +195,16 @@
     docker_client = docker.from_env()
     project_root_path = os.path.abspath(project_root_path)
     console = Console()
     console.print(
         "[bold magenta]TFY-Agent[/]: A tool for building and deploying [magenta]Jobs/Services[/] to the Truefoundry platform."
     )
     console.print(
-        "[bold reverse red]DISCLAIMER:[/] The [bold magenta]TFY-Agent[/] may use LLM resources outside of your organization. Please proceed only if you accept this."
+        "[bold reverse red]DISCLAIMER:[/] The contents of the project will be sent to OpenAI."
     )
-    console.print("Let's get started! Please answer the following questions:")
     console.print(
         "[bold cyan]Note:[/] All changes will be committed to a new branch. Please ensure you have a repository."
     )
     _check_repo(project_root_path=project_root_path, console=console)
 
     component_type = ComponentType[
         Prompt.ask(
@@ -294,15 +294,15 @@
 @click.option(
     "--path", type=click.STRING, required=True, help="The root path of the project"
 )
 @click.option(
     "--deploy",
     type=click.BOOL,
     is_flag=True,
-    default=False,
+    default=True,
     show_default=True,
     help="Deploy the project after successfully building it.",
 )
 def autodeploy_cli(path: str, deploy: bool):
     """
     Build and deploy projects using Truefoundry
     """
```

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/ask.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/commit.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/docker_run.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/list_files.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/send_request.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.0rc3/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/truefoundry/cli/__main__.py` & `truefoundry-0.2.0rc3/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc2/PKG-INFO` & `truefoundry-0.2.0rc3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

