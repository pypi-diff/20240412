# Comparing `tmp/johnsnowlabs-5.3.4rc1.tar.gz` & `tmp/johnsnowlabs-5.3.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-5.3.4rc1.tar", last modified: Fri Apr  5 16:20:39 2024, max compression
+gzip compressed data, was "johnsnowlabs-5.3.4rc2.tar", last modified: Fri Apr 12 10:51:20 2024, max compression
```

## Comparing `johnsnowlabs-5.3.4rc1.tar` & `johnsnowlabs-5.3.4rc2.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.298606 johnsnowlabs-5.3.4rc1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.282606 johnsnowlabs-5.3.4rc1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.286606 johnsnowlabs-5.3.4rc1/.github/workflows/
--rw-rw-r--   0 root         (0) root         (0)     3388 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/.github/workflows/create_search_index.yml
--rw-rw-r--   0 root         (0) root         (0)     5379 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/.gitignore
--rw-rw-r--   0 root         (0) root         (0)    11356 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9321 2024-04-05 16:20:39.298606 johnsnowlabs-5.3.4rc1/PKG-INFO
--r--r--r--   0 root         (0) root         (0)     8310 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.282606 johnsnowlabs-5.3.4rc1/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.286606 johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/
--rw-rw-r--   0 root         (0) root         (0)     1178 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/Dockerfile
--rw-rw-r--   0 root         (0) root         (0)     1075 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/README.md
--rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/docker-compose.yaml
--rw-rw-r--   0 root         (0) root         (0)     1566 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/fastapi_app.py
--rw-rw-r--   0 root         (0) root         (0)       34 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/license.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.286606 johnsnowlabs-5.3.4rc1/johnsnowlabs/
--rw-rw-r--   0 root         (0) root         (0)     1042 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.286606 johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      395 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/base_enum.py
--rw-rw-r--   0 root         (0) root         (0)     9794 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/lib_resolver.py
--rw-rw-r--   0 root         (0) root         (0)      733 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/pydantic_model.py
--rw-rw-r--   0 root         (0) root         (0)     9326 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/software_product.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.286606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2680 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/dbfs.py
--rw-rw-r--   0 root         (0) root         (0)    28916 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/endpoints.py
--rw-rw-r--   0 root         (0) root         (0)    20814 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     7591 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/marketplace.py
--rw-rw-r--   0 root         (0) root         (0)    21829 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/marketplace_offering.py
--rw-rw-r--   0 root         (0) root         (0)    12197 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-25 19:19:42.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4093 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/app.py
--rw-rw-r--   0 root         (0) root         (0)     1058 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/base_dockerfile
--rw-rw-r--   0 root         (0) root         (0)     1347 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/installer.py
--rw-rw-r--   0 root         (0) root         (0)       84 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/docker_template.py
--rw-rw-r--   0 root         (0) root         (0)    13516 2024-04-05 07:12:08.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      376 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/enums.py
--rw-rw-r--   0 root         (0) root         (0)    11474 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1850 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/utils.py
--rw-rw-r--   0 root         (0) root         (0)     4164 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/work_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/glue/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/glue/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2809 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/glue/install_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3191 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/glue/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        1 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/benchmark_test.py
--rw-rw-r--   0 root         (0) root         (0)     6100 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/endpoint_test.py
--rw-rw-r--   0 root         (0) root         (0)      690 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/generate_test.py
--rw-rw-r--   0 root         (0) root         (0)      832 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/hc_test.py
--rw-rw-r--   0 root         (0) root         (0)      317 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/load_predict_test.py
--rw-rw-r--   0 root         (0) root         (0)      908 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/nlp_test.py
--rw-rw-r--   0 root         (0) root         (0)     2124 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/ocr_test.py
--rw-rw-r--   0 root         (0) root         (0)     3496 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/report.py
--rw-rw-r--   0 root         (0) root         (0)    20668 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/install_flow.py
--rw-rw-r--   0 root         (0) root         (0)    11364 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/install_software.py
--rw-rw-r--   0 root         (0) root         (0)    12178 2024-03-05 14:57:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/jsl_home.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/
--rw-rw-r--   0 root         (0) root         (0)      124 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2061 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
--rw-rw-r--   0 root         (0) root         (0)     3192 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
--rw-rw-r--   0 root         (0) root         (0)     2105 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
--rw-rw-r--   0 root         (0) root         (0)     9118 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/offline_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/snowflake/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/snowflake/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11410 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/snowflake/work_utils.py
--rw-rw-r--   0 root         (0) root         (0)     9133 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/softwares.py
--rw-rw-r--   0 root         (0) root         (0)     5619 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/finance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/
--rw-rw-r--   0 root         (0) root         (0)      547 2024-03-25 19:19:32.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18435 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
--rw-rw-r--   0 root         (0) root         (0)    14001 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
--rw-rw-r--   0 root         (0) root         (0)     6757 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/utils.py
--rw-rw-r--   0 root         (0) root         (0)      212 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/lab.py
--rw-rw-r--   0 root         (0) root         (0)     5560 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/legal.py
--rw-rw-r--   0 root         (0) root         (0)       56 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/llm.py
--rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/medical.py
--rw-rw-r--   0 root         (0) root         (0)     1849 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/nlp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4945 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/install_info.py
--rw-rw-r--   0 root         (0) root         (0)    34057 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/jsl_secrets.py
--rw-rw-r--   0 root         (0) root         (0)     4168 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/lib_version.py
--rw-rw-r--   0 root         (0) root         (0)        2 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/license_info.py
--rw-rw-r--   0 root         (0) root         (0)      128 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/primitive.py
--rw-rw-r--   0 root         (0) root         (0)     2077 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/url_dependency.py
--rw-rw-r--   0 root         (0) root         (0)      121 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/serve.py
--rw-rw-r--   0 root         (0) root         (0)     2938 2024-04-05 16:20:37.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.290606 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      997 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/boto_utils.py
--rw-rw-r--   0 root         (0) root         (0)     6668 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/enums.py
--rw-rw-r--   0 root         (0) root         (0)     4845 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/env_utils.py
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/file_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1005 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/functional.py
--rw-rw-r--   0 root         (0) root         (0)     3221 2024-04-05 16:19:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/modelhub_markdown.py
--rw-rw-r--   0 root         (0) root         (0)    10596 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/my_jsl_api.py
--rw-rw-r--   0 root         (0) root         (0)    10654 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/notebooks.py
--rw-rw-r--   0 root         (0) root         (0)     5856 2024-04-01 23:43:41.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/pip_utils.py
--rw-rw-r--   0 root         (0) root         (0)      982 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/print_messages.py
--rw-rw-r--   0 root         (0) root         (0)     4964 2024-04-05 16:20:27.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/py_process.py
--rw-rw-r--   0 root         (0) root         (0)     3109 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/s3_utils.py
--rw-rw-r--   0 root         (0) root         (0)     8495 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/sparksession_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.294607 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4050 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/jsl_pre_processor.py
--rw-rw-r--   0 root         (0) root         (0)     1778 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/nb_code_match.py
--rw-rw-r--   0 root         (0) root         (0)     1132 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/nb_nodes.py
--rw-rw-r--   0 root         (0) root         (0)     3460 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/test_settings.py
--rw-rw-r--   0 root         (0) root         (0)     4353 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/venv_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1332 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/visual.py
--rw-rw-r--   0 root         (0) root         (0)      408 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.286606 johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9321 2024-04-05 16:20:39.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5322 2024-04-05 16:20:39.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-05 16:20:39.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      141 2024-04-05 16:20:39.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2024-04-05 16:20:39.000000 johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.294607 johnsnowlabs-5.3.4rc1/notebooks/
--rw-rw-r--   0 root         (0) root         (0)     6777 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/notebooks/create_databricks_cluster.ipynb
--rw-rw-r--   0 root         (0) root         (0)     8273 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/notebooks/create_emr_cluster.ipynb
--rw-rw-r--   0 root         (0) root         (0)   145269 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/notebooks/databricks_endpoints_tutorial.ipynb
--rw-rw-r--   0 root         (0) root         (0)    19726 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/notebooks/databricks_model_marketplace.ipynb
--rw-rw-r--   0 root         (0) root         (0)    41449 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/notebooks/haystack_with_johnsnowlabs.ipynb
--rw-rw-r--   0 root         (0) root         (0)    11963 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/notebooks/langchain_with_johnsnowlabs.ipynb
--rw-rw-r--   0 root         (0) root         (0)     3685 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/notebooks/parameterized_nb_example.ipynb
--rw-rw-r--   0 root         (0) root         (0)     7837 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/notebooks/setup_glue_notebook.ipynb
--rw-rw-r--   0 root         (0) root         (0)      251 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc1/pytest.ini
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 16:20:39.298606 johnsnowlabs-5.3.4rc1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2216 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc1/setup_johnsnowlabs.py
--rw-rw-r--   0 root         (0) root         (0)     2028 2024-02-23 06:25:49.000000 johnsnowlabs-5.3.4rc1/setup_johnsnowlabs_for_databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.294607 johnsnowlabs-5.3.4rc1/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6943 2024-04-05 05:01:43.000000 johnsnowlabs-5.3.4rc1/tests/auto_install.py
--rw-rw-r--   0 root         (0) root         (0)     1527 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/backward_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.294607 johnsnowlabs-5.3.4rc1/tests/databricks/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/databricks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1599 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/databricks/db_infos_test.py
--rw-rw-r--   0 root         (0) root         (0)    13529 2024-03-05 01:02:38.000000 johnsnowlabs-5.3.4rc1/tests/databricks/db_test_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4385 2024-02-23 06:25:49.000000 johnsnowlabs-5.3.4rc1/tests/databricks/endpoint_tests.py
--rw-rw-r--   0 root         (0) root         (0)      724 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/databricks/hdfs_tests.py
--rw-rw-r--   0 root         (0) root         (0)     2541 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/tests/databricks/install_tests.py
--rw-rw-r--   0 root         (0) root         (0)     3531 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/databricks/parameterized_nb_example.ipynb
--rw-rw-r--   0 root         (0) root         (0)     1003 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/databricks/sample.ipynb
--rw-rw-r--   0 root         (0) root         (0)     4533 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/databricks/submit_tests.py
--rw-rw-r--   0 root         (0) root         (0)      948 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/file_models.py
--rw-rw-r--   0 root         (0) root         (0)     3158 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/install.py
--rw-rw-r--   0 root         (0) root         (0)     3368 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/jsl_dependency_resolver.py
--rw-rw-r--   0 root         (0) root         (0)     2986 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/jsl_secrets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 16:20:39.294607 johnsnowlabs-5.3.4rc1/tests/llm_frameworks/
--rw-rw-r--   0 root         (0) root         (0)     2696 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/tests/llm_frameworks/test_haystack.py
--rw-rw-r--   0 root         (0) root         (0)     3057 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/tests/llm_frameworks/test_langchain.py
--rw-rw-r--   0 root         (0) root         (0)     1648 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/markdown_tests.py
--rw-rw-r--   0 root         (0) root         (0)     2272 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/notebook_tests.py
--rw-rw-r--   0 root         (0) root         (0)     9066 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc1/tests/spark_session.py
--rw-rw-r--   0 root         (0) root         (0)     1798 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc1/tests/venv_wrapper_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.677354 johnsnowlabs-5.3.4rc2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.677354 johnsnowlabs-5.3.4rc2/.github/workflows/
+-rw-rw-r--   0 root         (0) root         (0)     3388 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/.github/workflows/create_search_index.yml
+-rw-rw-r--   0 root         (0) root         (0)     5379 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)    11356 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9321 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/PKG-INFO
+-r--r--r--   0 root         (0) root         (0)     8310 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.677354 johnsnowlabs-5.3.4rc2/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/
+-rw-rw-r--   0 root         (0) root         (0)     1178 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/Dockerfile
+-rw-rw-r--   0 root         (0) root         (0)     1075 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/README.md
+-rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/docker-compose.yaml
+-rw-rw-r--   0 root         (0) root         (0)     1566 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/fastapi_app.py
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-02-14 23:45:57.000000 johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/license.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/
+-rw-rw-r--   0 root         (0) root         (0)     1042 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      395 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/base_enum.py
+-rw-rw-r--   0 root         (0) root         (0)     9794 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/lib_resolver.py
+-rw-rw-r--   0 root         (0) root         (0)      733 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/pydantic_model.py
+-rw-rw-r--   0 root         (0) root         (0)     9326 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/software_product.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2680 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/dbfs.py
+-rw-rw-r--   0 root         (0) root         (0)    28916 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)    20814 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/install_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     7591 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace.py
+-rw-rw-r--   0 root         (0) root         (0)    21829 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace_offering.py
+-rw-rw-r--   0 root         (0) root         (0)    12197 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/work_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-25 19:19:42.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4093 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/app.py
+-rw-rw-r--   0 root         (0) root         (0)     1058 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/base_dockerfile
+-rw-rw-r--   0 root         (0) root         (0)     1347 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/installer.py
+-rw-rw-r--   0 root         (0) root         (0)       84 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/docker_template.py
+-rw-rw-r--   0 root         (0) root         (0)    13516 2024-04-05 07:12:08.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/work_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      376 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/enums.py
+-rw-rw-r--   0 root         (0) root         (0)    11474 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/install_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1850 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4164 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/work_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2809 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/install_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3191 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/benchmark_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6100 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/endpoint_test.py
+-rw-rw-r--   0 root         (0) root         (0)      690 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/generate_test.py
+-rw-rw-r--   0 root         (0) root         (0)      832 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/hc_test.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/load_predict_test.py
+-rw-rw-r--   0 root         (0) root         (0)      908 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/nlp_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2124 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/ocr_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3496 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/report.py
+-rw-rw-r--   0 root         (0) root         (0)    20668 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_flow.py
+-rw-rw-r--   0 root         (0) root         (0)    11364 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_software.py
+-rw-rw-r--   0 root         (0) root         (0)    12178 2024-03-05 14:57:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/jsl_home.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/
+-rw-rw-r--   0 root         (0) root         (0)      124 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2061 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py
+-rw-rw-r--   0 root         (0) root         (0)     3192 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py
+-rw-rw-r--   0 root         (0) root         (0)     2105 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py
+-rw-rw-r--   0 root         (0) root         (0)     9118 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/offline_install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11410 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/work_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     9133 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/softwares.py
+-rw-rw-r--   0 root         (0) root         (0)     5619 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/finance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.685355 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/
+-rw-rw-r--   0 root         (0) root         (0)      547 2024-03-25 19:19:32.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18435 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py
+-rw-rw-r--   0 root         (0) root         (0)    14001 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py
+-rw-rw-r--   0 root         (0) root         (0)     6757 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/utils.py
+-rw-rw-r--   0 root         (0) root         (0)      212 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/lab.py
+-rw-rw-r--   0 root         (0) root         (0)     5560 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/legal.py
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/llm.py
+-rw-rw-r--   0 root         (0) root         (0)     5440 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/medical.py
+-rw-rw-r--   0 root         (0) root         (0)     1849 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/nlp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.689355 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4945 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/install_info.py
+-rw-rw-r--   0 root         (0) root         (0)    34057 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/jsl_secrets.py
+-rw-rw-r--   0 root         (0) root         (0)     4168 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/lib_version.py
+-rw-rw-r--   0 root         (0) root         (0)        2 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/license_info.py
+-rw-rw-r--   0 root         (0) root         (0)      128 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/primitive.py
+-rw-rw-r--   0 root         (0) root         (0)     2077 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/url_dependency.py
+-rw-rw-r--   0 root         (0) root         (0)      121 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/serve.py
+-rw-rw-r--   0 root         (0) root         (0)     2938 2024-04-12 10:51:01.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.689355 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      997 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/boto_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6668 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     4845 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/env_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/file_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1005 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/functional.py
+-rw-rw-r--   0 root         (0) root         (0)     3221 2024-04-05 16:19:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/modelhub_markdown.py
+-rw-rw-r--   0 root         (0) root         (0)    10596 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/my_jsl_api.py
+-rw-rw-r--   0 root         (0) root         (0)    10654 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/notebooks.py
+-rw-rw-r--   0 root         (0) root         (0)     5856 2024-04-01 23:43:41.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/pip_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      982 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/print_messages.py
+-rw-rw-r--   0 root         (0) root         (0)     4964 2024-04-05 16:20:27.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/py_process.py
+-rw-rw-r--   0 root         (0) root         (0)     3109 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/s3_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8495 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/sparksession_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.689355 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4050 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/jsl_pre_processor.py
+-rw-rw-r--   0 root         (0) root         (0)     1778 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_code_match.py
+-rw-rw-r--   0 root         (0) root         (0)     1132 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_nodes.py
+-rw-rw-r--   0 root         (0) root         (0)     3460 2024-04-12 10:46:30.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/test_settings.py
+-rw-rw-r--   0 root         (0) root         (0)     4353 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/venv_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1332 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/visual.py
+-rw-rw-r--   0 root         (0) root         (0)      408 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.681354 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9321 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5322 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      141 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2024-04-12 10:51:20.000000 johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/notebooks/
+-rw-rw-r--   0 root         (0) root         (0)     6777 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/create_databricks_cluster.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     8273 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/create_emr_cluster.ipynb
+-rw-rw-r--   0 root         (0) root         (0)   145269 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/databricks_endpoints_tutorial.ipynb
+-rw-rw-r--   0 root         (0) root         (0)    19726 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/notebooks/databricks_model_marketplace.ipynb
+-rw-rw-r--   0 root         (0) root         (0)    41449 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/haystack_with_johnsnowlabs.ipynb
+-rw-rw-r--   0 root         (0) root         (0)    11963 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/langchain_with_johnsnowlabs.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     3685 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/parameterized_nb_example.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     7837 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/notebooks/setup_glue_notebook.ipynb
+-rw-rw-r--   0 root         (0) root         (0)      251 2024-02-14 23:45:59.000000 johnsnowlabs-5.3.4rc2/pytest.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2216 2024-04-05 07:10:43.000000 johnsnowlabs-5.3.4rc2/setup_johnsnowlabs.py
+-rw-rw-r--   0 root         (0) root         (0)     2028 2024-02-23 06:25:49.000000 johnsnowlabs-5.3.4rc2/setup_johnsnowlabs_for_databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6871 2024-04-12 10:48:03.000000 johnsnowlabs-5.3.4rc2/tests/auto_install.py
+-rw-rw-r--   0 root         (0) root         (0)     1527 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/backward_compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/tests/databricks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1599 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/db_infos_test.py
+-rw-rw-r--   0 root         (0) root         (0)    13529 2024-03-05 01:02:38.000000 johnsnowlabs-5.3.4rc2/tests/databricks/db_test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4385 2024-02-23 06:25:49.000000 johnsnowlabs-5.3.4rc2/tests/databricks/endpoint_tests.py
+-rw-rw-r--   0 root         (0) root         (0)      724 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/hdfs_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     2541 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/databricks/install_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     3531 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/parameterized_nb_example.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     1003 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/sample.ipynb
+-rw-rw-r--   0 root         (0) root         (0)     4533 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/databricks/submit_tests.py
+-rw-rw-r--   0 root         (0) root         (0)      948 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/file_models.py
+-rw-rw-r--   0 root         (0) root         (0)     3158 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/install.py
+-rw-rw-r--   0 root         (0) root         (0)     3368 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/jsl_dependency_resolver.py
+-rw-rw-r--   0 root         (0) root         (0)     2986 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/jsl_secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:51:20.693355 johnsnowlabs-5.3.4rc2/tests/llm_frameworks/
+-rw-rw-r--   0 root         (0) root         (0)     2696 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/llm_frameworks/test_haystack.py
+-rw-rw-r--   0 root         (0) root         (0)     3057 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/llm_frameworks/test_langchain.py
+-rw-rw-r--   0 root         (0) root         (0)     1648 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/markdown_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     2272 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/notebook_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     9066 2024-03-23 03:19:52.000000 johnsnowlabs-5.3.4rc2/tests/spark_session.py
+-rw-rw-r--   0 root         (0) root         (0)     1798 2024-02-15 00:31:00.000000 johnsnowlabs-5.3.4rc2/tests/venv_wrapper_tests.py
```

### Comparing `johnsnowlabs-5.3.4rc1/.github/workflows/create_search_index.yml` & `johnsnowlabs-5.3.4rc2/.github/workflows/create_search_index.yml`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/.gitignore` & `johnsnowlabs-5.3.4rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/LICENSE` & `johnsnowlabs-5.3.4rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/PKG-INFO` & `johnsnowlabs-5.3.4rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 5.3.4rc1
+Version: 5.3.4rc2
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 License: UNKNOWN
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Platform: UNKNOWN
```

### Comparing `johnsnowlabs-5.3.4rc1/README.md` & `johnsnowlabs-5.3.4rc2/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/Dockerfile` & `johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/Dockerfile`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/README.md` & `johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/README.md`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/docker/johnsnowlabs_fastapi/fastapi_app.py` & `johnsnowlabs-5.3.4rc2/docker/johnsnowlabs_fastapi/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/__init__.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/lib_resolver.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/lib_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/pydantic_model.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/abstract_base/software_product.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/abstract_base/software_product.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/dbfs.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/dbfs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/endpoints.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/endpoints.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/install_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/marketplace.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/marketplace_offering.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/marketplace_offering.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/databricks/work_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/databricks/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/app.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/app.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/base_dockerfile` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/base_dockerfile`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/build/installer.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/build/installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/docker/work_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/docker/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/install_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/emr/work_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/emr/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/glue/install_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/install_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/glue/utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/glue/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/endpoint_test.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/generate_test.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/generate_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/hc_test.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/hc_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/nlp_test.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/nlp_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/ocr_test.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/ocr_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/health_checks/report.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/health_checks/report.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/install_flow.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_flow.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/install_software.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/install_software.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/jsl_home.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/jsl_home.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/hc_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/nlp_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/lib_resolvers/ocr_installer.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/offline_install.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/offline_install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/snowflake/work_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/snowflake/work_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/auto_install/softwares.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/auto_install/softwares.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/finance.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/finance.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/__init__.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/haystack_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/langchain_node.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/frameworks/embedding_retrieval/utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/frameworks/embedding_retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/legal.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/legal.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/medical.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/medical.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/nlp.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/nlp.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/install_info.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/install_info.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/jsl_secrets.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/lib_version.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/lib_version.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/py_models/url_dependency.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/py_models/url_dependency.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/settings.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     set_py4j_logger_to_error_on_databricks,
 )
 
 # These versions are used for auto-installs and version  checks
 
 
 
-raw_version_jsl_lib = "5.3.4rc1"
+raw_version_jsl_lib = "5.3.4rc2"
 
 
 raw_version_nlp = "5.3.1"
 
 raw_version_nlu = "5.3.0"
 
 
 raw_version_pyspark = "3.4.0"
 raw_version_nlp_display = "5.0"
 
-raw_version_medical = "5.3.0"
-raw_version_secret_medical = "5.3.0"
+raw_version_medical = "5.3.1"
+raw_version_secret_medical = "5.3.1"
 
-raw_version_secret_ocr = "5.3.0"
-raw_version_ocr = "5.3.0"
+raw_version_secret_ocr = "5.3.1"
+raw_version_ocr = "5.3.1"
 
 raw_version_pydantic = "1.10.11"
 
 pypi_page = "https://pypi.org/project/johnsnowlabs"
 json_indent = 4
 enforce_secret_on_version = False
 enforce_versions = True
```

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/boto_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/boto_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/enums.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/enums.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/env_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/file_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/functional.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/functional.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/modelhub_markdown.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/modelhub_markdown.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/my_jsl_api.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/my_jsl_api.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/notebooks.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/pip_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/pip_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/print_messages.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/print_messages.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/py_process.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/py_process.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/s3_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/sparksession_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/sparksession_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/jsl_pre_processor.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/jsl_pre_processor.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/nb_code_match.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_code_match.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/nb_nodes.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/nb_nodes.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/testing/test_settings.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/testing/test_settings.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/utils/venv_utils.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/utils/venv_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs/visual.py` & `johnsnowlabs-5.3.4rc2/johnsnowlabs/visual.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/PKG-INFO` & `johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: johnsnowlabs
-Version: 5.3.4rc1
+Version: 5.3.4rc2
 Summary: The John Snow Labs Library gives you access to all of John Snow Labs Enterprise And Open Source products in an easy and simple manner. Access 10000+ state-of-the-art NLP and OCR models for Finance, Legal and Medical domains. Easily scalable to Spark Cluster 
 Home-page: https://www.johnsnowlabs.com/
 Author: John Snow Labs
 Author-email: christian@johnsnowlabs.com
 License: UNKNOWN
 Keywords: Spark NLP OCR Finance Legal Medical John Snow Labs
 Platform: UNKNOWN
```

### Comparing `johnsnowlabs-5.3.4rc1/johnsnowlabs.egg-info/SOURCES.txt` & `johnsnowlabs-5.3.4rc2/johnsnowlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/create_databricks_cluster.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/create_databricks_cluster.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/create_emr_cluster.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/create_emr_cluster.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/databricks_endpoints_tutorial.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/databricks_endpoints_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/databricks_model_marketplace.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/databricks_model_marketplace.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/haystack_with_johnsnowlabs.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/haystack_with_johnsnowlabs.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/langchain_with_johnsnowlabs.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/langchain_with_johnsnowlabs.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/parameterized_nb_example.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/parameterized_nb_example.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/notebooks/setup_glue_notebook.ipynb` & `johnsnowlabs-5.3.4rc2/notebooks/setup_glue_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/setup_johnsnowlabs.py` & `johnsnowlabs-5.3.4rc2/setup_johnsnowlabs.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/setup_johnsnowlabs_for_databricks.py` & `johnsnowlabs-5.3.4rc2/setup_johnsnowlabs_for_databricks.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/auto_install.py` & `johnsnowlabs-5.3.4rc2/tests/auto_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             offline=True,
             offline_zip_dir=self.zip_dir,
             install_optional=True,
             include_dependencies=True,
         )
 
     def test_browser_install(self):
-        nlp.install(force_browser=True, visual=True, local_license_number=2)
+        nlp.install(force_browser=True, visual=True)
 
     def test_upgrade_licensed_lib_via_secret_only(self):
         new_secret = secrets.random_secret
         from johnsnowlabs import settings
 
         settings.enforce_versions = False
         nlp.install(enterprise_nlp_secret=new_secret)
@@ -108,21 +108,21 @@
 
 
     def test_create_and_install_cluster(self):
         install_suite = get_install_suite_from_jsl_home()
         print(install_suite)
 
     def test_uninstall_all(self):
-        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall spark-nlp -y')
-        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall spark-nlp-display -y')
-        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall nlu -y')
-
-        # os.system(f"{sys.executable} -m pip uninstall spark-nlp-jsl -y")
-        # os.system(f"{sys.executable} -m pip uninstall spark-ocr -y")
-        # os.system(old_lic'{sys.py_executable} -py_executable pip uninstall jsl_tmp -y')
+        os.system(f'{sys.executable} -py_executable pip uninstall spark-nlp -y')
+        os.system(f'{sys.executable} -py_executable pip uninstall spark-nlp-display -y')
+        os.system(f'{sys.executable} -py_executable pip uninstall nlu -y')
+
+        os.system(f"{sys.executable} -m pip uninstall spark-nlp-jsl -y")
+        os.system(f"{sys.executable} -m pip uninstall spark-ocr -y")
+        os.system(f'{sys.executable} -py_executable pip uninstall jsl_tmp -y')
         os.system(f"{sys.executable} -m pip uninstall spark-nlp-internal -y")
 
     def test_install_to_emr(self):
         # Make sure correct aws credentials are configured
         nlp.install_to_emr(
             "us-east-1",
             bootstrap_bucket="ksh-emr-bucket",
```

### Comparing `johnsnowlabs-5.3.4rc1/tests/backward_compat.py` & `johnsnowlabs-5.3.4rc2/tests/backward_compat.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/db_infos_test.py` & `johnsnowlabs-5.3.4rc2/tests/databricks/db_infos_test.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/db_test_utils.py` & `johnsnowlabs-5.3.4rc2/tests/databricks/db_test_utils.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/endpoint_tests.py` & `johnsnowlabs-5.3.4rc2/tests/databricks/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/hdfs_tests.py` & `johnsnowlabs-5.3.4rc2/tests/databricks/hdfs_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/install_tests.py` & `johnsnowlabs-5.3.4rc2/tests/databricks/install_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/parameterized_nb_example.ipynb` & `johnsnowlabs-5.3.4rc2/tests/databricks/parameterized_nb_example.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/sample.ipynb` & `johnsnowlabs-5.3.4rc2/tests/databricks/sample.ipynb`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/databricks/submit_tests.py` & `johnsnowlabs-5.3.4rc2/tests/databricks/submit_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/file_models.py` & `johnsnowlabs-5.3.4rc2/tests/file_models.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/install.py` & `johnsnowlabs-5.3.4rc2/tests/install.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/jsl_dependency_resolver.py` & `johnsnowlabs-5.3.4rc2/tests/jsl_dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/jsl_secrets.py` & `johnsnowlabs-5.3.4rc2/tests/jsl_secrets.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/llm_frameworks/test_haystack.py` & `johnsnowlabs-5.3.4rc2/tests/llm_frameworks/test_haystack.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/llm_frameworks/test_langchain.py` & `johnsnowlabs-5.3.4rc2/tests/llm_frameworks/test_langchain.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/markdown_tests.py` & `johnsnowlabs-5.3.4rc2/tests/markdown_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/notebook_tests.py` & `johnsnowlabs-5.3.4rc2/tests/notebook_tests.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/spark_session.py` & `johnsnowlabs-5.3.4rc2/tests/spark_session.py`

 * *Files identical despite different names*

### Comparing `johnsnowlabs-5.3.4rc1/tests/venv_wrapper_tests.py` & `johnsnowlabs-5.3.4rc2/tests/venv_wrapper_tests.py`

 * *Files identical despite different names*

