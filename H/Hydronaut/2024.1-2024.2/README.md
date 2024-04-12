# Comparing `tmp/hydronaut-2024.1.tar.gz` & `tmp/hydronaut-2024.2.tar.gz`

## Comparing `hydronaut-2024.1.tar` & `hydronaut-2024.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hydronaut-2024.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hydronaut-2024.1/.gitmodules
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hydronaut-2024.1/CITATION.cff
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 hydronaut-2024.1/TODO.md
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 hydronaut-2024.1/codemeta.json
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 hydronaut-2024.1/env.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hydronaut-2024.1/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hydronaut-2024.1/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydronaut-2024.1/doc/requirements.txt
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 hydronaut-2024.1/doc/source/conf.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hydronaut-2024.1/doc/source/index.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hydronaut-2024.1/doc/source/readme.md
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/README.md
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/README.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/decorated_class/README.md
--rwxr-xr-x   0        0        0     1338 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/decorated_class/decorated_class.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/decorated_class/conf/config.yaml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/decorated_function/README.md
--rwxr-xr-x   0        0        0      750 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/decorated_function/decorated_function.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/experiment_subclass/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/dummy/experiment_subclass/src/experiment.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/basic_mnist/README.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/basic_mnist/requirements.txt
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/basic_mnist/conf/config.yaml
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/basic_mnist/src/experiment.py
--rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/basic_mnist/src/model.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/lighting-mnist/README.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/lighting-mnist/requirements.txt
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/lighting-mnist/conf/config.yaml
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/lighting-mnist/src/data.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/lighting-mnist/src/experiment.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 hydronaut-2024.1/examples/pytorch/lighting-mnist/src/model.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 hydronaut-2024.1/img/hydronaut_icon.svg
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 hydronaut-2024.1/img/hydronaut_logo.svg
--rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 hydronaut-2024.1/scripts/hydronaut-build_documentation.sh
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hydronaut-2024.1/scripts/hydronaut-initialize.sh
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 hydronaut-2024.1/scripts/hydronaut-install_in_venv.sh
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hydronaut-2024.1/scripts/hydronaut-lint.sh
--rwxr-xr-x   0        0        0     1422 2020-02-02 00:00:00.000000 hydronaut-2024.1/scripts/hydronaut-rsync-results.sh
--rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 hydronaut-2024.1/scripts/hydronaut-run_in_venv.sh
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/__init__.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/decorator.py
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/experiment.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/file.py
--rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/init.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/log.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/mlflow.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/paths.py
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/run.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/types.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/version.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/hydra/__init__.py
--rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/hydra/config.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/hydra/info.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/hydra/omegaconf.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/hydra/resolvers.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 hydronaut-2024.1/src/hydronaut/lightning/experiment.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hydronaut-2024.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 hydronaut-2024.1/LICENSE.txt
--rw-r--r--   0        0        0    31407 2020-02-02 00:00:00.000000 hydronaut-2024.1/README.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 hydronaut-2024.1/pyproject.toml
--rw-r--r--   0        0        0    33572 2020-02-02 00:00:00.000000 hydronaut-2024.1/PKG-INFO
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 hydronaut-2024.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hydronaut-2024.2/.gitmodules
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 hydronaut-2024.2/CITATION.cff
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 hydronaut-2024.2/TODO.md
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 hydronaut-2024.2/codemeta.json
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 hydronaut-2024.2/env.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hydronaut-2024.2/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hydronaut-2024.2/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydronaut-2024.2/doc/requirements.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 hydronaut-2024.2/doc/source/conf.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hydronaut-2024.2/doc/source/index.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hydronaut-2024.2/doc/source/readme.md
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/README.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/README.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/decorated_class/README.md
+-rwxr-xr-x   0        0        0     1338 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/decorated_class/decorated_class.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/decorated_class/conf/config.yaml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/decorated_function/README.md
+-rwxr-xr-x   0        0        0      750 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/decorated_function/decorated_function.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/experiment_subclass/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/dummy/experiment_subclass/src/experiment.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/basic_mnist/README.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/basic_mnist/requirements.txt
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/basic_mnist/conf/config.yaml
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/basic_mnist/src/experiment.py
+-rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/basic_mnist/src/model.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/lighting-mnist/README.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/lighting-mnist/requirements.txt
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/lighting-mnist/conf/config.yaml
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/lighting-mnist/src/data.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/lighting-mnist/src/experiment.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 hydronaut-2024.2/examples/pytorch/lighting-mnist/src/model.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 hydronaut-2024.2/img/hydronaut_icon.svg
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 hydronaut-2024.2/img/hydronaut_logo.svg
+-rwxr-xr-x   0        0        0      887 2020-02-02 00:00:00.000000 hydronaut-2024.2/scripts/hydronaut-build_documentation.sh
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hydronaut-2024.2/scripts/hydronaut-initialize.sh
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 hydronaut-2024.2/scripts/hydronaut-install_in_venv.sh
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hydronaut-2024.2/scripts/hydronaut-lint.sh
+-rwxr-xr-x   0        0        0     1422 2020-02-02 00:00:00.000000 hydronaut-2024.2/scripts/hydronaut-rsync-results.sh
+-rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 hydronaut-2024.2/scripts/hydronaut-run_in_venv.sh
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/__init__.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/decorator.py
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/experiment.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/file.py
+-rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/init.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/log.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/mlflow.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/paths.py
+-rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/run.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/types.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/version.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/hydra/__init__.py
+-rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/hydra/config.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/hydra/info.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/hydra/omegaconf.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/hydra/resolvers.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 hydronaut-2024.2/src/hydronaut/lightning/experiment.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hydronaut-2024.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 hydronaut-2024.2/LICENSE.txt
+-rw-r--r--   0        0        0    31407 2020-02-02 00:00:00.000000 hydronaut-2024.2/README.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 hydronaut-2024.2/pyproject.toml
+-rw-r--r--   0        0        0    33568 2020-02-02 00:00:00.000000 hydronaut-2024.2/PKG-INFO
```

### Comparing `hydronaut-2024.1/.gitlab-ci.yml` & `hydronaut-2024.2/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   tags: *id001
 release_job:
   image: registry.gitlab.com/gitlab-org/release-cli:latest
   release:
     description: Release $CI_COMMIT_TAG
     tag_name: $CI_COMMIT_TAG
   rules:
-  - if: $CI_COMMIT_TAG
+  - if: $CI_COMMIT_TAG =~ /^v./
   script:
   - echo "running release_job"
   stage: release
   tags: *id001
 stages:
 - release
 - deploy
```

### Comparing `hydronaut-2024.1/CITATION.cff` & `hydronaut-2024.2/CITATION.cff`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,22 @@
   and MLflow.
 authors:
 - email: jan-michael.rye@inria.fr
   family-names: Rye
   given-names: Jan-Michael
   orcid: https://orcid.org/0009-0005-0109-6598
 cff-version: 1.2.0
-date-released: '2021-07-18'
 identifiers:
 - description: The Software Heritage URL.
   type: url
   value: https://archive.softwareheritage.org/browse/origin/?origin_url=https%3A//gitlab.inria.fr/jrye/hydronaut.git
 - description: HAL open science URL.
   type: url
   value: https://hal.science/hal-04246627
 - description: HAL open science identifier.
   type: other
   value: hal-04246627
 license: MIT
 message: If you use this software, please cite it using these metadata.
 repository-code: https://gitlab.inria.fr/jrye/hydronaut.git
 title: Hydronaut
-version: '2024.1'
+version: '2024.2'
```

### Comparing `hydronaut-2024.1/TODO.md` & `hydronaut-2024.2/TODO.md`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/codemeta.json` & `hydronaut-2024.2/codemeta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2024.2'"}*

```diff
@@ -94,9 +94,9 @@
             "description": "Run an experiment.",
             "executableName": "hydronaut-run",
             "name": "hydronaut-run",
             "runtimePlatform": "Python 3"
         }
     ],
     "url": "https://gitlab.inria.fr/jrye/hydronaut",
-    "version": "2024.1"
+    "version": "2024.2"
 }
```

### Comparing `hydronaut-2024.1/doc/Makefile` & `hydronaut-2024.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/doc/make.bat` & `hydronaut-2024.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/doc/source/conf.py` & `hydronaut-2024.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/dummy/decorated_class/decorated_class.py` & `hydronaut-2024.2/examples/dummy/decorated_class/decorated_class.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/dummy/decorated_class/conf/config.yaml` & `hydronaut-2024.2/examples/dummy/decorated_class/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/dummy/decorated_function/decorated_function.py` & `hydronaut-2024.2/examples/dummy/decorated_function/decorated_function.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/dummy/experiment_subclass/src/experiment.py` & `hydronaut-2024.2/examples/dummy/experiment_subclass/src/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/basic_mnist/README.md` & `hydronaut-2024.2/examples/pytorch/basic_mnist/README.md`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/basic_mnist/conf/config.yaml` & `hydronaut-2024.2/examples/pytorch/basic_mnist/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/basic_mnist/src/experiment.py` & `hydronaut-2024.2/examples/pytorch/basic_mnist/src/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/basic_mnist/src/model.py` & `hydronaut-2024.2/examples/pytorch/basic_mnist/src/model.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/lighting-mnist/README.md` & `hydronaut-2024.2/examples/pytorch/lighting-mnist/README.md`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/lighting-mnist/conf/config.yaml` & `hydronaut-2024.2/examples/pytorch/lighting-mnist/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/lighting-mnist/src/data.py` & `hydronaut-2024.2/examples/pytorch/lighting-mnist/src/data.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/lighting-mnist/src/experiment.py` & `hydronaut-2024.2/examples/pytorch/lighting-mnist/src/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/examples/pytorch/lighting-mnist/src/model.py` & `hydronaut-2024.2/examples/pytorch/lighting-mnist/src/model.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/img/hydronaut_icon.svg` & `hydronaut-2024.2/img/hydronaut_icon.svg`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/img/hydronaut_logo.svg` & `hydronaut-2024.2/img/hydronaut_logo.svg`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/scripts/hydronaut-build_documentation.sh` & `hydronaut-2024.2/scripts/hydronaut-build_documentation.sh`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/scripts/hydronaut-rsync-results.sh` & `hydronaut-2024.2/scripts/hydronaut-rsync-results.sh`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/scripts/hydronaut-run_in_venv.sh` & `hydronaut-2024.2/scripts/hydronaut-run_in_venv.sh`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/decorator.py` & `hydronaut-2024.2/src/hydronaut/decorator.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/experiment.py` & `hydronaut-2024.2/src/hydronaut/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/file.py` & `hydronaut-2024.2/src/hydronaut/file.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/init.py` & `hydronaut-2024.2/src/hydronaut/init.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/mlflow.py` & `hydronaut-2024.2/src/hydronaut/mlflow.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/paths.py` & `hydronaut-2024.2/src/hydronaut/paths.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/run.py` & `hydronaut-2024.2/src/hydronaut/run.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/types.py` & `hydronaut-2024.2/src/hydronaut/types.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/hydra/config.py` & `hydronaut-2024.2/src/hydronaut/hydra/config.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/hydra/omegaconf.py` & `hydronaut-2024.2/src/hydronaut/hydra/omegaconf.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/hydra/resolvers.py` & `hydronaut-2024.2/src/hydronaut/hydra/resolvers.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/src/hydronaut/lightning/experiment.py` & `hydronaut-2024.2/src/hydronaut/lightning/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/LICENSE.txt` & `hydronaut-2024.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/README.md` & `hydronaut-2024.2/README.md`

 * *Files identical despite different names*

### Comparing `hydronaut-2024.1/pyproject.toml` & `hydronaut-2024.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 full = [
     "lightning",
     "torch",
     "torchvision",
 ]
 
 [project.urls]
-homepage = "https://gitlab.inria.fr/jrye/hydronaut"
-repository = "https://gitlab.inria.fr/jrye/hydronaut.git"
-documentation = "https://jrye.gitlabpages.inria.fr/hydronaut"
-issues = "https://gitlab.inria.fr/jrye/hydronaut/-/issues"
+Homepage = "https://gitlab.inria.fr/jrye/hydronaut"
+Source = "https://gitlab.inria.fr/jrye/hydronaut.git"
+Documentation = "https://jrye.gitlabpages.inria.fr/hydronaut"
+Issues = "https://gitlab.inria.fr/jrye/hydronaut/-/issues"
 
 [project.scripts]
 hydronaut-run = "hydronaut.run:script_main"
 hydronaut-init = "hydronaut.init:main"
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `hydronaut-2024.1/PKG-INFO` & `hydronaut-2024.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: Hydronaut
-Version: 2024.1
+Version: 2024.2
 Summary: A framework for exploring the depths of hyperparameter space with Hydra and MLflow.
-Project-URL: homepage, https://gitlab.inria.fr/jrye/hydronaut
-Project-URL: repository, https://gitlab.inria.fr/jrye/hydronaut.git
-Project-URL: documentation, https://jrye.gitlabpages.inria.fr/hydronaut
-Project-URL: issues, https://gitlab.inria.fr/jrye/hydronaut/-/issues
+Project-URL: Homepage, https://gitlab.inria.fr/jrye/hydronaut
+Project-URL: Source, https://gitlab.inria.fr/jrye/hydronaut.git
+Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/hydronaut
+Project-URL: Issues, https://gitlab.inria.fr/jrye/hydronaut/-/issues
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License: MIT License
         
         Copyright (c) 2022, Inria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

