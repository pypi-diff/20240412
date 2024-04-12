# Comparing `tmp/lendsmart_reva-2.6.tar.gz` & `tmp/lendsmart_reva-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_reva-2.6.tar", last modified: Tue Oct  3 14:53:51 2023, max compression
+gzip compressed data, was "lendsmart_reva-2.7.tar", last modified: Sat Oct  7 07:35:53 2023, max compression
```

## Comparing `lendsmart_reva-2.6.tar` & `lendsmart_reva-2.7.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     3095 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.464980 lendsmart_reva-2.6/lendsmart_reva.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3095 2023-10-03 14:53:51.000000 lendsmart_reva-2.6/lendsmart_reva.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3117 2023-10-03 14:53:51.000000 lendsmart_reva-2.6/lendsmart_reva.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-10-03 14:53:51.000000 lendsmart_reva-2.6/lendsmart_reva.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      647 2023-10-03 14:53:51.000000 lendsmart_reva-2.6/lendsmart_reva.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      206 2023-10-03 14:53:51.000000 lendsmart_reva-2.6/lendsmart_reva.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2023-10-03 14:53:51.000000 lendsmart_reva-2.6/lendsmart_reva.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      907 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/advisor_profile.py
--rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/autotest.py
--rw-rw-r--   0 user      (1000) user      (1000)      997 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/autotest_runner.py
--rw-rw-r--   0 user      (1000) user      (1000)      839 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/branch.py
--rw-rw-r--   0 user      (1000) user      (1000)     3548 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/cli.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/conf/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/conf/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      740 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/conf/reva.py
--rw-rw-r--   0 user      (1000) user      (1000)      953 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/exception.py
--rw-rw-r--   0 user      (1000) user      (1000)      954 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/info.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/advisor_profile/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/advisor_profile/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    10887 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/advisor_profile/create.py
--rw-rw-r--   0 user      (1000) user      (1000)      483 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/advisor_profile/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/auto/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/auto/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4014 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/auto/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/autotest_runner/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/autotest_runner/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3672 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/autotest_runner/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/base/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1840 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/base.py
--rw-rw-r--   0 user      (1000) user      (1000)       65 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/constants.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/base/errors/
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/errors/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      456 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/errors/errors.py
--rw-rw-r--   0 user      (1000) user      (1000)     1302 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/resource_delete.py
--rw-rw-r--   0 user      (1000) user      (1000)     4634 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/resource_update.py
--rw-rw-r--   0 user      (1000) user      (1000)      950 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/run_query.py
--rw-rw-r--   0 user      (1000) user      (1000)     1701 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/base/site_settings.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/branch/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/branch/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3452 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/branch/create.py
--rw-rw-r--   0 user      (1000) user      (1000)      439 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/branch/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/client/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/client/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      781 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/client/aws.py
--rw-rw-r--   0 user      (1000) user      (1000)      805 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/client/builder.py
--rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/client/graphql_client.py
--rw-rw-r--   0 user      (1000) user      (1000)     2317 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/client/lendsmart_client.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/document_access_control/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/document_access_control/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      728 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/document_access_control/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/document_access_control/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/graphql_queries/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1954 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/advisor_profiles.py
--rw-rw-r--   0 user      (1000) user      (1000)      953 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/branch.py
--rw-rw-r--   0 user      (1000) user      (1000)      806 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/document_access_control.py
--rw-rw-r--   0 user      (1000) user      (1000)      641 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)      386 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/namespace.py
--rw-rw-r--   0 user      (1000) user      (1000)     3219 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      590 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/site_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      802 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/graphql_queries/workflow.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.468980 lendsmart_reva-2.6/reva/lib/loan_productus/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/loan_productus/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      642 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/loan_productus/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/loan_productus/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/lib/permissions/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/permissions/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2559 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/permissions/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      803 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/permissions/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     2628 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/permissions/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/lib/roles/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/roles/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2244 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/roles/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      759 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/roles/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     2181 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/roles/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/lib/roles_and_permissions/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/roles_and_permissions/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      687 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/roles_and_permissions/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/roles_and_permissions/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/lib/site_settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/site_settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/site_settings/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1845 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/site_settings/update.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/lib/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      507 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/utils/address.py
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/utils/filter_data_with_id.py
--rw-rw-r--   0 user      (1000) user      (1000)     2634 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/utils/get_json_files.py
--rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/utils/get_namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)     4344 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/utils/get_paths.py
--rw-rw-r--   0 user      (1000) user      (1000)      236 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/utils/list_files.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/lib/workflow/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/workflow/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      608 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/workflow/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/lib/workflow/update.py
--rw-rw-r--   0 user      (1000) user      (1000)      878 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/loan_products.py
--rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/namespaces.py
--rw-rw-r--   0 user      (1000) user      (1000)      879 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      847 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/roles.py
--rw-rw-r--   0 user      (1000) user      (1000)      933 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/roles_and_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      853 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/site_settings.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      613 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/local_test_permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)      774 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/local_test_roles.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/tests/permissions/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/permissions/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2205 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/permissions/fake_permissions_deleter.py
--rw-rw-r--   0 user      (1000) user      (1000)     1829 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/permissions/fake_permissions_updater.py
--rw-rw-r--   0 user      (1000) user      (1000)     5458 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/permissions/test_permissions.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/reva/tests/roles/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/roles/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1900 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/roles/fake_roles_deleter.py
--rw-rw-r--   0 user      (1000) user      (1000)     1683 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/roles/fake_roles_updater.py
--rw-rw-r--   0 user      (1000) user      (1000)     5090 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/tests/roles/test_roles.py
--rw-rw-r--   0 user      (1000) user      (1000)      820 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/reva/workflow.py
--rw-rw-r--   0 user      (1000) user      (1000)       86 2023-10-03 14:53:51.472980 lendsmart_reva-2.6/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2580 2023-10-03 14:52:56.000000 lendsmart_reva-2.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.948805 lendsmart_reva-2.7/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     3469 2023-10-07 07:35:53.948805 lendsmart_reva-2.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2714 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.936805 lendsmart_reva-2.7/lendsmart_reva.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3469 2023-10-07 07:35:53.000000 lendsmart_reva-2.7/lendsmart_reva.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3117 2023-10-07 07:35:53.000000 lendsmart_reva-2.7/lendsmart_reva.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-10-07 07:35:53.000000 lendsmart_reva-2.7/lendsmart_reva.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      647 2023-10-07 07:35:53.000000 lendsmart_reva-2.7/lendsmart_reva.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      206 2023-10-07 07:35:53.000000 lendsmart_reva-2.7/lendsmart_reva.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-10-07 07:35:53.000000 lendsmart_reva-2.7/lendsmart_reva.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      907 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/advisor_profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1849 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/autotest.py
+-rw-rw-r--   0 user      (1000) user      (1000)      997 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/autotest_runner.py
+-rw-rw-r--   0 user      (1000) user      (1000)      839 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/branch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3548 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/cli.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/conf/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/conf/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      740 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/conf/reva.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1076 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)      954 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/info.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/lib/advisor_profile/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/advisor_profile/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10887 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/advisor_profile/create.py
+-rw-rw-r--   0 user      (1000) user      (1000)      483 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/advisor_profile/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/lib/auto/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/auto/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4014 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/auto/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/lib/autotest_runner/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/autotest_runner/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3672 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/autotest_runner/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/lib/base/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1840 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)       65 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/constants.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/lib/base/errors/
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/errors/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      456 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/errors/errors.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1302 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/resource_delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4634 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/resource_update.py
+-rw-rw-r--   0 user      (1000) user      (1000)      950 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/run_query.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1701 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/base/site_settings.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.940805 lendsmart_reva-2.7/reva/lib/branch/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/branch/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3452 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/branch/create.py
+-rw-rw-r--   0 user      (1000) user      (1000)      439 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/branch/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/client/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/client/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      781 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/client/aws.py
+-rw-rw-r--   0 user      (1000) user      (1000)      805 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/client/builder.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2926 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/client/graphql_client.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2317 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/client/lendsmart_client.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/document_access_control/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/document_access_control/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      728 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/document_access_control/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1599 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/document_access_control/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/graphql_queries/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1954 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/advisor_profiles.py
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/branch.py
+-rw-rw-r--   0 user      (1000) user      (1000)      806 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/document_access_control.py
+-rw-rw-r--   0 user      (1000) user      (1000)      641 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)      386 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/namespace.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3560 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      590 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/site_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      802 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/graphql_queries/workflow.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/loan_productus/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/loan_productus/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      642 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/loan_productus/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1482 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/loan_productus/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/permissions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/permissions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2559 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/permissions/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      803 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/permissions/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2628 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/permissions/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/roles/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/roles/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2421 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/roles/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      759 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/roles/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2181 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/roles/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/roles_and_permissions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/roles_and_permissions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      687 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/roles_and_permissions/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1880 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/roles_and_permissions/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/site_settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/site_settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/site_settings/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1845 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/site_settings/update.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.944805 lendsmart_reva-2.7/reva/lib/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      507 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/utils/address.py
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/utils/filter_data_with_id.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2634 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/utils/get_json_files.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2968 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/utils/get_namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4344 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/utils/get_paths.py
+-rw-rw-r--   0 user      (1000) user      (1000)      236 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/utils/list_files.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.948805 lendsmart_reva-2.7/reva/lib/workflow/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/workflow/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      608 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/workflow/main.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1386 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/lib/workflow/update.py
+-rw-rw-r--   0 user      (1000) user      (1000)      878 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/loan_products.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1125 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/namespaces.py
+-rw-rw-r--   0 user      (1000) user      (1000)      879 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      847 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/roles.py
+-rw-rw-r--   0 user      (1000) user      (1000)      933 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/roles_and_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      853 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/site_settings.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.948805 lendsmart_reva-2.7/reva/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      613 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/local_test_permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      774 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/local_test_roles.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.948805 lendsmart_reva-2.7/reva/tests/permissions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/permissions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2205 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/permissions/fake_permissions_deleter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1829 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/permissions/fake_permissions_updater.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5458 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/permissions/test_permissions.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-10-07 07:35:53.948805 lendsmart_reva-2.7/reva/tests/roles/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/roles/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2076 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/roles/fake_roles_deleter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1683 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/roles/fake_roles_updater.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5090 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/tests/roles/test_roles.py
+-rw-rw-r--   0 user      (1000) user      (1000)      820 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/reva/workflow.py
+-rw-rw-r--   0 user      (1000) user      (1000)       86 2023-10-07 07:35:53.948805 lendsmart_reva-2.7/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2580 2023-10-07 07:35:14.000000 lendsmart_reva-2.7/setup.py
```

### Comparing `lendsmart_reva-2.6/PKG-INFO` & `lendsmart_reva-2.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: lendsmart_reva
-Version: 2.6
-Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
-Home-page: https://github.com/lendsmartlabs
-Author: Lendsmart
-Author-email: accounts@lendsmart.ai
-License: MIT
-Keywords: lendsmart reva
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Reva CLI
 ==========
 ![image](https://user-images.githubusercontent.com/1402479/200783457-550bf8bc-4bc8-4571-b995-829bc2f9b2b1.png)
 
 
 
 The Reva CLI is used to manage Lendsmart deployment from the command line.
```

### Comparing `lendsmart_reva-2.6/README.md` & `lendsmart_reva-2.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: lendsmart_reva
+Version: 2.7
+Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
+Home-page: https://github.com/lendsmartlabs
+Author: Lendsmart
+Author-email: accounts@lendsmart.ai
+License: MIT
+Keywords: lendsmart reva
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: remoto>=1.1.4
+Requires-Dist: configparser; python_version < "3.0"
+Requires-Dist: setuptools<45.0.0; python_version < "3.0"
+Requires-Dist: python-graphql-client
+Requires-Dist: ramda
+Requires-Dist: lendsmart-autotest
+Requires-Dist: setuptools; python_version >= "3.0"
+Requires-Dist: PyJWT==2.7.0
+Requires-Dist: cryptography==37.0.4
+Requires-Dist: lendsmart-api
+
 Reva CLI
 ==========
 ![image](https://user-images.githubusercontent.com/1402479/200783457-550bf8bc-4bc8-4571-b995-829bc2f9b2b1.png)
 
 
 
 The Reva CLI is used to manage Lendsmart deployment from the command line.
```

### Comparing `lendsmart_reva-2.6/lendsmart_reva.egg-info/PKG-INFO` & `lendsmart_reva-2.7/lendsmart_reva.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 2.1
 Name: lendsmart-reva
-Version: 2.6
+Version: 2.7
 Summary: Lendsmart opinionated tool to mirror QA to Prod. Deploy with ease.
 Home-page: https://github.com/lendsmartlabs
 Author: Lendsmart
 Author-email: accounts@lendsmart.ai
 License: MIT
 Keywords: lendsmart reva
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: remoto>=1.1.4
+Requires-Dist: configparser; python_version < "3.0"
+Requires-Dist: setuptools<45.0.0; python_version < "3.0"
+Requires-Dist: python-graphql-client
+Requires-Dist: ramda
+Requires-Dist: lendsmart-autotest
+Requires-Dist: setuptools; python_version >= "3.0"
+Requires-Dist: PyJWT==2.7.0
+Requires-Dist: cryptography==37.0.4
+Requires-Dist: lendsmart-api
 
 Reva CLI
 ==========
 ![image](https://user-images.githubusercontent.com/1402479/200783457-550bf8bc-4bc8-4571-b995-829bc2f9b2b1.png)
```

### Comparing `lendsmart_reva-2.6/lendsmart_reva.egg-info/SOURCES.txt` & `lendsmart_reva-2.7/lendsmart_reva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/lendsmart_reva.egg-info/entry_points.txt` & `lendsmart_reva-2.7/lendsmart_reva.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/advisor_profile.py` & `lendsmart_reva-2.7/reva/advisor_profile.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/autotest.py` & `lendsmart_reva-2.7/reva/autotest.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/autotest_runner.py` & `lendsmart_reva-2.7/reva/autotest_runner.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/branch.py` & `lendsmart_reva-2.7/reva/branch.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/cli.py` & `lendsmart_reva-2.7/reva/cli.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/conf/reva.py` & `lendsmart_reva-2.7/reva/conf/reva.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/document_access_control.py` & `lendsmart_reva-2.7/reva/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/exception.py` & `lendsmart_reva-2.7/reva/exception.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/info.py` & `lendsmart_reva-2.7/reva/info.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/advisor_profile/create.py` & `lendsmart_reva-2.7/reva/lib/advisor_profile/create.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/auto/main.py` & `lendsmart_reva-2.7/reva/lib/auto/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/autotest_runner/main.py` & `lendsmart_reva-2.7/reva/lib/autotest_runner/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/base/base.py` & `lendsmart_reva-2.7/reva/lib/base/base.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/base/errors/__init__.py` & `lendsmart_reva-2.7/reva/lib/base/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/base/resource_delete.py` & `lendsmart_reva-2.7/reva/lib/base/resource_delete.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/base/resource_update.py` & `lendsmart_reva-2.7/reva/lib/base/resource_update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/base/run_query.py` & `lendsmart_reva-2.7/reva/lib/base/run_query.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/base/site_settings.py` & `lendsmart_reva-2.7/reva/lib/base/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/branch/create.py` & `lendsmart_reva-2.7/reva/lib/branch/create.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/client/aws.py` & `lendsmart_reva-2.7/reva/lib/client/aws.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/client/builder.py` & `lendsmart_reva-2.7/reva/lib/client/builder.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/client/graphql_client.py` & `lendsmart_reva-2.7/reva/lib/client/graphql_client.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/client/lendsmart_client.py` & `lendsmart_reva-2.7/reva/lib/client/lendsmart_client.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/document_access_control/main.py` & `lendsmart_reva-2.7/reva/lib/document_access_control/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/document_access_control/update.py` & `lendsmart_reva-2.7/reva/lib/document_access_control/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/graphql_queries/advisor_profiles.py` & `lendsmart_reva-2.7/reva/lib/graphql_queries/advisor_profiles.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/graphql_queries/branch.py` & `lendsmart_reva-2.7/reva/lib/graphql_queries/branch.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/graphql_queries/document_access_control.py` & `lendsmart_reva-2.7/reva/lib/graphql_queries/document_access_control.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/graphql_queries/loan_products.py` & `lendsmart_reva-2.7/reva/lib/graphql_queries/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/graphql_queries/roles_and_permissions.py` & `lendsmart_reva-2.7/reva/lib/graphql_queries/roles_and_permissions.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,14 +69,32 @@
 		}
  	""",
         "variables": {
             "role_id": id
         }
 	}
 
+def delete_permission_by_role_id(id: str):
+    """
+	Delete permission with role_id
+    """
+    return {
+		"query": """
+			mutation delete_permissions($role_id: bigint!) {
+				delete_permissions(where: {role_id: {_eq: $role_id}}) 
+    				{
+						affected_rows
+					}
+		}
+ 	""",
+        "variables": {
+            "role_id": id
+        }
+	}
+
 def delete_permission_by_id(id: str):
     """
 	Delete permission at ID
     """
     return {
 		"query": """
 			mutation delete_permissions($permission_id: bigint!) {
```

### Comparing `lendsmart_reva-2.6/reva/lib/graphql_queries/site_settings.py` & `lendsmart_reva-2.7/reva/lib/graphql_queries/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/graphql_queries/workflow.py` & `lendsmart_reva-2.7/reva/lib/graphql_queries/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/loan_productus/main.py` & `lendsmart_reva-2.7/reva/lib/loan_productus/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/loan_productus/update.py` & `lendsmart_reva-2.7/reva/lib/loan_productus/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/permissions/delete.py` & `lendsmart_reva-2.7/reva/lib/permissions/delete.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/permissions/main.py` & `lendsmart_reva-2.7/reva/lib/permissions/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/permissions/update.py` & `lendsmart_reva-2.7/reva/lib/permissions/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/roles/delete.py` & `lendsmart_reva-2.7/reva/lib/roles/delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 
 # pylint: disable=W0102, W0718, W0221, W0622, C0103
 from ramda import path_or, empty
 from reva.lib.base.resource_delete import ResourceDeleter
 from reva.lib.base.errors.errors import RolesDeleteError
 from reva.lib.graphql_queries.roles_and_permissions import (
-    delete_role_by_id, get_roles_by_namespace
+    delete_role_by_id, get_roles_by_namespace,
+    delete_permission_by_role_id
 )
 
 class RolesDeleter(ResourceDeleter):
     """
     delete the roles
     """
 
@@ -38,34 +39,38 @@
         Returns the list of ids of roles to be deleted
         """
         roles = path_or({}, ["reva", "roles"], self.deploy_json)
         return path_or([],
                        [0, "delete"],
                        list(filter(lambda x: x["namespace"] == self.arguments.namespace, roles)))
 
-    def delete(self, query):
+    def delete(self):
         """
             Delete resources
         """
         list_of_ids = self.__get_list_of_ids()
         # print("List of ids==", list_of_ids)
         query_datas = []
         for id in list_of_ids:
             if empty(self.get_resource_by_id(id, self.remote_roles)):
                 self.raise_exception(cause=f"No record found for ID: {id}.")
 
+            # delete all the permissions associated with the role
             query_datas.append(
-                query(
-                    id
-                )
+                delete_permission_by_role_id(id)
+            )
+
+            # delete the role itself
+            query_datas.append(
+                delete_role_by_id(id)
             )
 
         # print("Query Data:===", query_datas)
         self.excecute_for_list_of_query_data(query_datas)
         print("-----roles were deleted successfully!-----")
         return
 
     def start(self):
         """
         update the roles and permissions
         """
-        self.delete(query=delete_role_by_id)
+        self.delete()
```

### Comparing `lendsmart_reva-2.6/reva/lib/roles/main.py` & `lendsmart_reva-2.7/reva/lib/roles/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/roles/update.py` & `lendsmart_reva-2.7/reva/lib/roles/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/roles_and_permissions/main.py` & `lendsmart_reva-2.7/reva/lib/roles_and_permissions/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/roles_and_permissions/update.py` & `lendsmart_reva-2.7/reva/lib/roles_and_permissions/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/site_settings/main.py` & `lendsmart_reva-2.7/reva/lib/site_settings/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/site_settings/update.py` & `lendsmart_reva-2.7/reva/lib/site_settings/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/utils/get_json_files.py` & `lendsmart_reva-2.7/reva/lib/utils/get_json_files.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/utils/get_namespaces.py` & `lendsmart_reva-2.7/reva/lib/utils/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/utils/get_paths.py` & `lendsmart_reva-2.7/reva/lib/utils/get_paths.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/workflow/main.py` & `lendsmart_reva-2.7/reva/lib/workflow/main.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/lib/workflow/update.py` & `lendsmart_reva-2.7/reva/lib/workflow/update.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/loan_products.py` & `lendsmart_reva-2.7/reva/loan_products.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/namespaces.py` & `lendsmart_reva-2.7/reva/namespaces.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/permissions.py` & `lendsmart_reva-2.7/reva/permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/roles.py` & `lendsmart_reva-2.7/reva/roles.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/roles_and_permissions.py` & `lendsmart_reva-2.7/reva/roles_and_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/site_settings.py` & `lendsmart_reva-2.7/reva/site_settings.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/tests/local_test_permissions.py` & `lendsmart_reva-2.7/reva/tests/local_test_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/tests/local_test_roles.py` & `lendsmart_reva-2.7/reva/tests/local_test_roles.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/tests/permissions/fake_permissions_deleter.py` & `lendsmart_reva-2.7/reva/tests/permissions/fake_permissions_deleter.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/tests/permissions/fake_permissions_updater.py` & `lendsmart_reva-2.7/reva/tests/permissions/fake_permissions_updater.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/tests/permissions/test_permissions.py` & `lendsmart_reva-2.7/reva/tests/permissions/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/tests/roles/fake_roles_deleter.py` & `lendsmart_reva-2.7/reva/tests/roles/fake_roles_deleter.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 # pylint: disable=W0102, W0718, W0221, W0622, C0103
 from ramda import path_or, empty
 from reva.lib.base.resource_delete import ResourceDeleter
 from reva.lib.base.errors.errors import RolesDeleteError
 from reva.lib.fixtures.roles import DELETE_TEST_CASES
 from reva.lib.graphql_queries.roles_and_permissions import (
-    delete_role_by_id, get_roles_by_namespace
+    delete_role_by_id, get_roles_by_namespace,
+    delete_permission_by_role_id
 )
 
 class FakeRolesDeleter(ResourceDeleter):
     """
     delete the roles
     """
 
@@ -30,34 +31,37 @@
             Gets the roles from database using graphql query
         """
         query_response = self.get_resource_from_database(
             get_roles_by_namespace(self.arguments.namespace))
 
         return path_or([], ["data", "roles"], query_response)
 
-    def delete(self, query):
+    def delete(self):
         """
             Delete resources
         """
         # print("JSON DATA: ====", self.deploy_json)
         list_of_ids = path_or([], ["delete_roles"],self.deploy_json)
 
         query_datas = []
 
         for id in list_of_ids:
             if empty(self.get_resource_by_id(id, self.remote_roles)):
                 self.raise_exception(cause=f"No record found for ID: {id}.")
 
+            # delete all the permissions associated with the role
             query_datas.append(
-                query(
-                    id
-                )
+                delete_permission_by_role_id(id)
+            )
+            # delete the role itself
+            query_datas.append(
+                delete_role_by_id(id)
             )
 
         print("-----roles were deleted successfully!-----")
         return query_datas
 
     def start(self):
         """
         update the roles and permissions
         """
-        return self.delete(query=delete_role_by_id)
+        return self.delete()
```

### Comparing `lendsmart_reva-2.6/reva/tests/roles/fake_roles_updater.py` & `lendsmart_reva-2.7/reva/tests/roles/fake_roles_updater.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/tests/roles/test_roles.py` & `lendsmart_reva-2.7/reva/tests/roles/test_roles.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/reva/workflow.py` & `lendsmart_reva-2.7/reva/workflow.py`

 * *Files identical despite different names*

### Comparing `lendsmart_reva-2.6/setup.py` & `lendsmart_reva-2.7/setup.py`

 * *Files identical despite different names*

