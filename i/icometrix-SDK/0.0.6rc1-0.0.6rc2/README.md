# Comparing `tmp/icometrix_sdk-0.0.6rc1.tar.gz` & `tmp/icometrix_sdk-0.0.6rc2.tar.gz`

## Comparing `icometrix_sdk-0.0.6rc1.tar` & `icometrix_sdk-0.0.6rc2.tar`

### file list

```diff
@@ -1,72 +1,101 @@
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/Jenkinsfile
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/catalog-info.yaml
--rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/gh-version.sh
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/requirements.txt
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/.github/workflows/gh-pages-docs.yml
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/Makefile
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/conf.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/make.bat
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/make.sh
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/quickstart.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/requirements.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/developer_guide/index.rst
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/developer_guide/model_relations.mmd
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/developer_guide/models.rst
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/developer_guide/paginators.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/developer_guide/session.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/base.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/customer_report.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/customer_result.rst
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/index.rst
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/patient.rst
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/project.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/upload.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/models/user.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/resources/customer_reports.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/resources/customer_results.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/resources/index.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/resources/patients.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/resources/profile.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/resources/projects.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/docs/resources/uploads.rst
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/anonymized_upload_files.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/get_all_projects.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/get_customer_reports.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/sync_directory.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/upload_and_download.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/upload_directory.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/upload_files.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/authentication/auto_auth.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/authentication/custom_auth.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/examples/authentication/password_auth.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/_version.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/authentication.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/exceptions.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/base.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/customer_report_entity.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/customer_result_entity.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/patient_entity.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/project_entity.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/study_entity.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/upload_entity.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/models/user_entity.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/customer_reports.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/customer_results.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/patients.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/profile.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/projects.py
--rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/uploads.py
--rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/anonymizer.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/api_client.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/file_upload.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/hash_factory.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/paginator.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/requests_api_client.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/LICENSE
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/README.rst
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/pyproject.toml
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc1/PKG-INFO
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/Jenkinsfile
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/catalog-info.yaml
+-rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/gh-version.sh
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/requirements.txt
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/.github/workflows/gh-pages-docs.yml
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/Makefile
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/conf.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/make.bat
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/make.sh
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/quickstart.rst
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/requirements.txt
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/developer_guide/anonymization.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/developer_guide/index.rst
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/developer_guide/model_relations.mmd
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/developer_guide/models.rst
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/developer_guide/paginators.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/developer_guide/session.rst
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/anonymizer.rst
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/base.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/customer_report.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/customer_result.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/index.rst
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/patient.rst
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/project.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/upload.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/models/user.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/resources/customer_reports.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/resources/customer_results.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/resources/index.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/resources/patients.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/resources/profile.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/resources/projects.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/docs/resources/uploads.rst
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/anonymize.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/anonymized_upload_files.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/get_all_projects.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/get_customer_reports.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/get_customer_results.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/sync_directory.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/upload_and_download.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/upload_directory.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/upload_files.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/authentication/auto_auth.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/authentication/custom_auth.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/examples/authentication/password_auth.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/_version.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/authentication.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/__init__.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/anonymizer.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/config.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/exceptions.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/hash_factory.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/models.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/policy.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/__init__.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_anonimizer.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_hash.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_hash_factory.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_policy.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_policy_group.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_replace.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_round.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/test_utils.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/utils.py
+-rw-r--r--   0        0        0   272942 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/datasets/anonymized_md5.dcm
+-rw-r--r--   0        0        0   591692 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/datasets/anonymized_sha3.dcm
+-rw-r--r--   0        0        0   276290 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/datasets/ib_anonymized.dcm
+-rw-r--r--   0        0        0   273244 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/tests/datasets/original.dcm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/base.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/customer_report_entity.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/customer_result_entity.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/patient_entity.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/pipeline_result_entity.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/project_entity.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/study_entity.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/upload_entity.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/models/user_entity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/__init__.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/customer_reports.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/customer_results.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/patients.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/pipeline_results.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/profile.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/projects.py
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/uploads.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/api_client.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/file_upload.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/paginator.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/requests_api_client.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/LICENSE
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/README.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/pyproject.toml
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 icometrix_sdk-0.0.6rc2/PKG-INFO
```

### Comparing `icometrix_sdk-0.0.6rc1/Jenkinsfile` & `icometrix_sdk-0.0.6rc2/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/.github/workflows/gh-pages-docs.yml` & `icometrix_sdk-0.0.6rc2/.github/workflows/gh-pages-docs.yml`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/.github/workflows/python-publish.yml` & `icometrix_sdk-0.0.6rc2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/docs/Makefile` & `icometrix_sdk-0.0.6rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/docs/conf.py` & `icometrix_sdk-0.0.6rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/docs/make.bat` & `icometrix_sdk-0.0.6rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/docs/quickstart.rst` & `icometrix_sdk-0.0.6rc2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/docs/developer_guide/models.rst` & `icometrix_sdk-0.0.6rc2/docs/developer_guide/models.rst`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 - :attr:`~icometrix_sdk.models.base.BackendEntity.creation_timestamp`: The creation timestamp
 - :attr:`~icometrix_sdk.models.base.BackendEntity.uri`: The uri to point to the location of the object
 
 Collections
 -----------
 
 When fetching a collection of models from the API; you will always get a subset of that collection in combination with
-<<<<<<< HEAD
 some extra meta data. See: :doc:`paginators`
 
 Relations
 ---------
 
 High level overview of the relations between the available entities
```

### Comparing `icometrix_sdk-0.0.6rc1/docs/developer_guide/paginators.rst` & `icometrix_sdk-0.0.6rc2/docs/developer_guide/paginators.rst`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/examples/anonymized_upload_files.py` & `icometrix_sdk-0.0.6rc2/examples/anonymized_upload_files.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 import os
 from io import BytesIO
 
 import pydicom
-from pydicom import FileDataset
+from pydicom import FileDataset, Dataset
 from pydicom.errors import InvalidDicomError
 
 from icometrix_sdk import IcometrixApi
+from icometrix_sdk.anonymizer.anonymizer import Anonymizer
+from icometrix_sdk.anonymizer.policy import policy, group_policy
 from icometrix_sdk.models.upload_entity import StartUploadDto
-from icometrix_sdk.utils.anonymizer import Anonymizer
-from icometrix_sdk.utils.hash_factory import SHA3
+from icometrix_sdk.anonymizer.hash_factory import SHA3, HashFactory
 
 PROJECT_ID = "uuid"
 DICOM_DIR_PATH = "<path>"
 
+# file_paths = ["IM-0007-0106.dcm"]
+#
+# hash_algo = HashFactory.create_hash_method("ico_md5")
+# anon = AnonymizerP(policy, group_policy, hash_algo)
+#
+# for file_path in file_paths:
+#     dataset = pydicom.dcmread(file_path)
+#     anon.anonymize(dataset).save_as(f"anon-{file_path}")
+
 if __name__ == '__main__':
-    hash_method = SHA3(size=512)
-    anonymizer = Anonymizer(hash_method)
+    hash_algo = HashFactory.create_hash_method("ico_md5")
+    anonymizer = Anonymizer(policy, group_policy, hash_algo)
 
     os.environ["API_HOST"] = "https://icobrain-test.icometrix.com"
 
     # Initialize the icometrix API
     ico_api = IcometrixApi()
 
     # Get the project, to make sure its there (will throw a 404 in case the project is not found)
@@ -36,15 +46,15 @@
 
             file_path = os.path.join(path, name)
             try:
                 dicom_file = pydicom.dcmread(file_path)
             except InvalidDicomError:
                 continue
 
-            anonymized_dicom: FileDataset = anonymizer.anonymize(dicom_file)
+            anonymized_dicom: Dataset = anonymizer.anonymize(dicom_file)
             buffer = BytesIO()
             anonymized_dicom.save_as(buffer)
             buffer.seek(0)
             fields = {"file": (file_path, buffer.read(), "application/octet-stream")}
             ico_api.uploads.upload_dicom(upload.uri, fields=fields)
 
     # Once all files have been uploaded, signal that they are all there and start the import/processing
```

### Comparing `icometrix_sdk-0.0.6rc1/examples/get_customer_reports.py` & `icometrix_sdk-0.0.6rc2/examples/get_customer_reports.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/examples/sync_directory.py` & `icometrix_sdk-0.0.6rc2/examples/sync_directory.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/examples/upload_and_download.py` & `icometrix_sdk-0.0.6rc2/examples/upload_and_download.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/examples/upload_directory.py` & `icometrix_sdk-0.0.6rc2/examples/upload_directory.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/examples/upload_files.py` & `icometrix_sdk-0.0.6rc2/examples/upload_files.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/examples/authentication/custom_auth.py` & `icometrix_sdk-0.0.6rc2/examples/authentication/custom_auth.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/examples/authentication/password_auth.py` & `icometrix_sdk-0.0.6rc2/examples/authentication/password_auth.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/__init__.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/authentication.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/authentication.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/exceptions.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/models/base.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/models/customer_report_entity.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/models/customer_report_entity.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/models/patient_entity.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/models/patient_entity.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/models/study_entity.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/models/study_entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from typing import Optional, Union
 
 from pydantic import field_validator
 
-from exceptions import IcometrixInvalidInputDataException
+from icometrix_sdk.exceptions import IcometrixInvalidInputDataException
 from icometrix_sdk.models.base import BackendEntity, DicomModality
 
 
 class StudyEntity(BackendEntity):
     modality: DicomModality
     patient_id: str
     project_id: str
```

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/models/upload_entity.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/models/upload_entity.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/models/user_entity.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/models/user_entity.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/customer_reports.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/customer_reports.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/customer_results.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/customer_results.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/patients.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/patients.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/projects.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/projects.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/resources/uploads.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/resources/uploads.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/api_client.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/file_upload.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/hash_factory.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/anonymizer/hash_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import hashlib
 from abc import abstractmethod
-from typing import Literal
+from typing import get_args
 
-
-class UnsupportedAlgorithmException(Exception):
-    pass
-
-
-class UnsupportedSizeException(Exception):
-    pass
+from icometrix_sdk.anonymizer.exceptions import HashAlgorithmException, HashSizeException
+from icometrix_sdk.anonymizer.models import HashAlgo
 
 
 class HashFactory:
     @staticmethod
-    def create_hash_method(algo: Literal["sha3", "md5", "ico_md5"], size=256, salt=None):
+    def create_hash_method(algo: HashAlgo, size=512, salt=None):
         if algo == "sha3":
             return SHA3(size)
         elif algo == "md5":
             return MD5()
-        elif algo == "ico_md5":
-            return IcometrixMD5()
+        elif algo == "short_md5":
+            return ShortMD5()
         else:
-            raise UnsupportedAlgorithmException(f"No algorithm named {algo} is supported, "
-                                                f"valid values are \"sha3\", \'md5\"")
+            supported = ", ".join(get_args(HashAlgo))
+            raise HashAlgorithmException(f"No algorithm named {algo} is supported, valid values are {supported}")
 
 
 class HashMethod:
     @abstractmethod
     def calculate_hash_from_bytes(self, input_obj: bytes) -> str:
         pass
 
@@ -38,38 +33,39 @@
     def __init__(self, size=256):
         acceptable_capacities = [224, 256, 384, 512]
         if size not in acceptable_capacities:
             raise f"Invalid capacity for SHA3, should be any of {acceptable_capacities}"
         self.size = size
 
     def calculate_hash_from_bytes(self, input_obj: bytes):
-        hash_obj = None
         if self.size == 224:
             hash_obj = hashlib.sha3_224(input_obj)
         elif self.size == 256:
             hash_obj = hashlib.sha3_256(input_obj)
         elif self.size == 384:
             hash_obj = hashlib.sha3_384(input_obj)
         elif self.size == 512:
             hash_obj = hashlib.sha3_512(input_obj)
         else:
-            raise UnsupportedSizeException(f"SHA3 does not support size {self.size}, "
-                                           f"valid values are (224, 256, 384, 512)")
+            raise HashSizeException(f"SHA3 does not support size {self.size}, "
+                                    f"valid values are (224, 256, 384, 512)")
 
         digest = hash_obj.hexdigest()
         return digest
 
 
 class MD5(HashMethod):
     def calculate_hash_from_bytes(self, input_obj: bytes):
         return hashlib.md5(input_obj, usedforsecurity=True).hexdigest()
 
 
-class IcometrixMD5(HashMethod):
+class ShortMD5(HashMethod):
     """
     MD5 that is re-based to base10.
     """
 
+    def calculate_hash(self, input_obj: str, encoding='utf-8') -> str:
+        return self.calculate_hash_from_bytes(input_obj.encode(encoding))
+
     def calculate_hash_from_bytes(self, input_obj: bytes):
         md5_hash = MD5().calculate_hash_from_bytes(input_obj)
-        decimized = str(int(md5_hash, base=16))
-        return decimized
+        return str(int(md5_hash, base=16))[:10]
```

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/paginator.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/icometrix_sdk/utils/requests_api_client.py` & `icometrix_sdk-0.0.6rc2/icometrix_sdk/utils/requests_api_client.py`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/.gitignore` & `icometrix_sdk-0.0.6rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/LICENSE` & `icometrix_sdk-0.0.6rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/pyproject.toml` & `icometrix_sdk-0.0.6rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `icometrix_sdk-0.0.6rc1/PKG-INFO` & `icometrix_sdk-0.0.6rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: icometrix-SDK
-Version: 0.0.6rc1
+Version: 0.0.6rc2
 Summary: icometrix-SDK is a Software Development Kit (SDK) for Python, which allows Python developers to write software that interacts with the icometrix API.
 Project-URL: Homepage, https://github.com/icometrix/icometrix-sdk
 Project-URL: Issues, https://github.com/icometrix/icometrix-sdk/issues
 Author-email: Jeroen Pinxten <jeroen.pinxten@icometrix.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

