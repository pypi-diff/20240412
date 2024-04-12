# Comparing `tmp/exasol_script_languages_container_ci-1.3.3.tar.gz` & `tmp/exasol_script_languages_container_ci-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_script_languages_container_ci-1.3.3.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_ci-1.3.4.tar", max compression
```

## Comparing `exasol_script_languages_container_ci-1.3.3.tar` & `exasol_script_languages_container_ci-1.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1063 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/LICENSE
--rw-r--r--   0        0        0       95 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/__init__.py
--rw-r--r--   0        0        0        0 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/cli/__init__.py
--rw-r--r--   0        0        0       50 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/cli/cli.py
--rw-r--r--   0        0        0        0 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/cli/commands/__init__.py
--rw-r--r--   0        0        0     1926 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/cli/commands/run_ci.py
--rw-r--r--   0        0        0     2703 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/cli/commands/run_release.py
--rw-r--r--   0        0        0        0 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/__init__.py
--rw-r--r--   0        0        0     1304 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/asset_uploader.py
--rw-r--r--   0        0        0     1677 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/branch_config.py
--rw-r--r--   0        0        0     4705 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci.py
--rw-r--r--   0        0        0     3075 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_build.py
--rw-r--r--   0        0        0     1091 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_export.py
--rw-r--r--   0        0        0      493 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_prepare.py
--rw-r--r--   0        0        0     1250 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_push.py
--rw-r--r--   0        0        0     1305 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_security_scan.py
--rw-r--r--   0        0        0     1309 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_step_output_printer.py
--rw-r--r--   0        0        0     4893 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_test.py
--rw-r--r--   0        0        0      334 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/common.py
--rw-r--r--   0        0        0        0 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/config/__init__.py
--rw-r--r--   0        0        0      584 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/config/config_data_model.py
--rw-r--r--   0        0        0     2153 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/config/data_model_generator.py
--rw-r--r--   0        0        0     1501 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/git_access.py
--rw-r--r--   0        0        0     1223 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
--rw-r--r--   0        0        0     2906 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/release.py
--rw-r--r--   0        0        0     2443 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/release_uploader.py
--rw-r--r--   0        0        0      321 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/render_template.py
--rwxr-xr-x   0        0        0      125 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/main.py
--rw-r--r--   0        0        0      950 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/templates/config_schema.json
--rw-r--r--   0        0        0      822 2023-11-22 14:45:32.693009 exasol_script_languages_container_ci-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/LICENSE
+-rw-r--r--   0        0        0       95 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1926 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/cli/commands/run_ci.py
+-rw-r--r--   0        0        0     2703 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/cli/commands/run_release.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/__init__.py
+-rw-r--r--   0        0        0     1304 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/asset_uploader.py
+-rw-r--r--   0        0        0     1677 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/branch_config.py
+-rw-r--r--   0        0        0     4705 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci.py
+-rw-r--r--   0        0        0     3075 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_build.py
+-rw-r--r--   0        0        0     1091 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_export.py
+-rw-r--r--   0        0        0      493 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_prepare.py
+-rw-r--r--   0        0        0     1250 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_push.py
+-rw-r--r--   0        0        0     1305 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_security_scan.py
+-rw-r--r--   0        0        0     1309 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_step_output_printer.py
+-rw-r--r--   0        0        0     4893 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_test.py
+-rw-r--r--   0        0        0      334 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/common.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/config/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/config/config_data_model.py
+-rw-r--r--   0        0        0     2153 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/config/data_model_generator.py
+-rw-r--r--   0        0        0     1501 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/git_access.py
+-rw-r--r--   0        0        0     1223 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
+-rw-r--r--   0        0        0     2906 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/release.py
+-rw-r--r--   0        0        0     2443 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/release_uploader.py
+-rw-r--r--   0        0        0      321 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/render_template.py
+-rwxr-xr-x   0        0        0      125 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/main.py
+-rw-r--r--   0        0        0      950 2024-04-12 07:32:01.825919 exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/templates/config_schema.json
+-rw-r--r--   0        0        0      831 2024-04-12 07:32:01.829919 exasol_script_languages_container_ci-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci-1.3.4/PKG-INFO
```

### Comparing `exasol_script_languages_container_ci-1.3.3/LICENSE` & `exasol_script_languages_container_ci-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/cli/commands/run_ci.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/cli/commands/run_ci.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/cli/commands/run_release.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/cli/commands/run_release.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/asset_uploader.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/branch_config.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/branch_config.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_build.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_export.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_export.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_push.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_push.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_security_scan.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_step_output_printer.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_step_output_printer.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/ci_test.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/ci_test.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/config/config_data_model.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/config/config_data_model.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/config/data_model_generator.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/config/data_model_generator.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/git_access.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/git_access.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/release.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/release.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/lib/release_uploader.py` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/lib/release_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/exasol_script_languages_container_ci/templates/config_schema.json` & `exasol_script_languages_container_ci-1.3.4/exasol_script_languages_container_ci/templates/config_schema.json`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.3/pyproject.toml` & `exasol_script_languages_container_ci-1.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exasol-script-languages-container-ci"
-version = "1.3.3"
+version = "1.3.4"
 description = "Implements CI builds for script-language-container."
 
 license = "MIT"
 
 authors = [
     "Thomas Uebensee <ext.thomas.uebensee@exasol.com>"
 ]
@@ -13,15 +13,15 @@
 python = ">=3.8.0,<4.0"
 click = "^8.0.3"
 GitPython = ">=3.1.0"
 exasol-script-languages-container-tool = "^0.18.0"
 exasol-integration-test-docker-environment = "^1.7.1"
 PyGithub = "^1.55.0"
 setuptools = "^68.0.0"
-datamodel-code-generator = "^0.21.0"
+datamodel-code-generator = ">=0.25.5 <0.30.0"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
 toml = ">=0.10.2"
```

### Comparing `exasol_script_languages_container_ci-1.3.3/PKG-INFO` & `exasol_script_languages_container_ci-1.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: exasol-script-languages-container-ci
-Version: 1.3.3
+Version: 1.3.4
 Summary: Implements CI builds for script-language-container.
 License: MIT
 Author: Thomas Uebensee
 Author-email: ext.thomas.uebensee@exasol.com
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.0)
 Requires-Dist: PyGithub (>=1.55.0,<2.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: datamodel-code-generator (>=0.21.0,<0.22.0)
+Requires-Dist: datamodel-code-generator (>=0.25.5,<0.30.0)
 Requires-Dist: exasol-integration-test-docker-environment (>=1.7.1,<2.0.0)
 Requires-Dist: exasol-script-languages-container-tool (>=0.18.0,<0.19.0)
 Requires-Dist: setuptools (>=68.0.0,<69.0.0)
```

