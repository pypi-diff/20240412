# Comparing `tmp/azure-communication-chat-1.2.0.tar.gz` & `tmp/azure-communication-chat-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-communication-chat-1.2.0.tar", last modified: Mon Dec  4 22:42:58 2023, max compression
+gzip compressed data, was "azure-communication-chat-1.3.0.tar", last modified: Thu Apr 11 20:50:27 2024, max compression
```

## Comparing `azure-communication-chat-1.2.0.tar` & `azure-communication-chat-1.3.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.608323 azure-communication-chat-1.2.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4011 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      197 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    22863 2023-12-04 22:42:58.608323 azure-communication-chat-1.2.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21790 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/communication/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/communication/chat/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1576 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9581 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_chat_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22414 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_chat_thread_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/communication/chat/_common/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_common/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2526 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_communication_identifier_serializer.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/communication/chat/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4801 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/_azure_communication_chat_service.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2535 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79052 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4928 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/_azure_communication_chat_service.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2545 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      860 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18295 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/_chat_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    72999 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/_chat_thread_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.600323 azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3293 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1451 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/_azure_communication_chat_service_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46702 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.604323 azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      860 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21248 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/_chat_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    87427 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/_chat_thread_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_generated/py.typed
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12678 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_models.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.604323 azure-communication-chat-1.2.0/azure/communication/chat/_shared/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      310 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2595 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/auth_policy_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14198 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4651 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6575 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/user_credential.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6865 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/user_credential_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3356 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1008 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_shared/utils_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2693 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      397 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.604323 azure-communication-chat-1.2.0/azure/communication/chat/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      414 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9530 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/aio/_chat_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22002 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/aio/_chat_thread_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/azure/communication/chat/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.608323 azure-communication-chat-1.2.0/azure_communication_chat.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    22863 2023-12-04 22:42:58.000000 azure-communication-chat-1.2.0/azure_communication_chat.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2023-12-04 22:42:58.000000 azure-communication-chat-1.2.0/azure_communication_chat.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-04 22:42:58.000000 azure-communication-chat-1.2.0/azure_communication_chat.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-12-04 22:42:58.000000 azure-communication-chat-1.2.0/azure_communication_chat.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       73 2023-12-04 22:42:58.000000 azure-communication-chat-1.2.0/azure_communication_chat.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-12-04 22:42:58.000000 azure-communication-chat-1.2.0/azure_communication_chat.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       99 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.604323 azure-communication-chat-1.2.0/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5979 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/samples/chat_client_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6451 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/samples/chat_client_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16380 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/samples/chat_thread_client_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18452 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/samples/chat_thread_client_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3865 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/samples/user_credential_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4011 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/samples/user_credential_sample_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-12-04 22:42:58.608323 azure-communication-chat-1.2.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2590 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.608323 azure-communication-chat-1.2.0/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-12-04 22:42:58.608323 azure-communication-chat-1.2.0/tests/_shared/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      326 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/_shared/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/_shared/async_fake_token_credential.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      436 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/_shared/communication_service_preparer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      537 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/_shared/fake_token_credential.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      920 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/_shared/helper.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2615 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/_shared/utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1539 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/chat_e2e_helper.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2040 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8550 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5509 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5618 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_client_e2e.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5847 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_client_e2e_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30573 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_thread_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27909 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_thread_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11318 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_thread_client_e2e.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15584 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_chat_thread_client_e2e_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5721 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/test_communication_identifier_serializer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      889 2023-12-04 22:42:15.000000 azure-communication-chat-1.2.0/tests/unittest_helpers.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.913874 azure-communication-chat-1.3.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4263 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      197 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/MANIFEST.in
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    22799 2024-04-11 20:50:27.913874 azure-communication-chat-1.3.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21790 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.901874 azure-communication-chat-1.3.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.901874 azure-communication-chat-1.3.0/azure/communication/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.901874 azure-communication-chat-1.3.0/azure/communication/chat/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1712 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9581 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_chat_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22418 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_chat_thread_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.901874 azure-communication-chat-1.3.0/azure/communication/chat/_common/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_common/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2526 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_communication_identifier_serializer.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.901874 azure-communication-chat-1.3.0/azure/communication/chat/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4801 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/_azure_communication_chat_service.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2535 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.905875 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4928 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/_azure_communication_chat_service.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2545 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.905875 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      860 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17746 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/_chat_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    69718 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/_chat_thread_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.905875 azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3391 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1515 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/_azure_communication_chat_service_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48834 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.905875 azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      860 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20699 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/_chat_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    84146 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/_chat_thread_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_generated/py.typed
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12689 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_models.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.905875 azure-communication-chat-1.3.0/azure/communication/chat/_shared/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      310 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2595 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/auth_policy_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15664 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4651 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6594 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/user_credential.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6885 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/user_credential_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3356 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1008 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_shared/utils_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2693 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      397 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.909875 azure-communication-chat-1.3.0/azure/communication/chat/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      414 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9542 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/aio/_chat_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21998 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/aio/_chat_thread_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/azure/communication/chat/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.913874 azure-communication-chat-1.3.0/azure_communication_chat.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    22799 2024-04-11 20:50:27.000000 azure-communication-chat-1.3.0/azure_communication_chat.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3521 2024-04-11 20:50:27.000000 azure-communication-chat-1.3.0/azure_communication_chat.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-11 20:50:27.000000 azure-communication-chat-1.3.0/azure_communication_chat.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-11 20:50:27.000000 azure-communication-chat-1.3.0/azure_communication_chat.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       59 2024-04-11 20:50:27.000000 azure-communication-chat-1.3.0/azure_communication_chat.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-11 20:50:27.000000 azure-communication-chat-1.3.0/azure_communication_chat.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      120 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.909875 azure-communication-chat-1.3.0/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5979 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/samples/chat_client_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6451 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/samples/chat_client_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17030 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/samples/chat_thread_client_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19165 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/samples/chat_thread_client_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3865 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/samples/user_credential_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4011 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/samples/user_credential_sample_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-11 20:50:27.913874 azure-communication-chat-1.3.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2527 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.913874 azure-communication-chat-1.3.0/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-11 20:50:27.913874 azure-communication-chat-1.3.0/tests/_shared/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      326 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/_shared/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/_shared/async_fake_token_credential.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      436 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/_shared/communication_service_preparer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      537 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/_shared/fake_token_credential.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      920 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/_shared/helper.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2615 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/_shared/utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1539 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/chat_e2e_helper.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2040 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8550 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5509 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5800 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_client_e2e.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6089 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_client_e2e_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31005 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_thread_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27909 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_thread_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11659 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_thread_client_e2e.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16048 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_chat_thread_client_e2e_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5721 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/test_communication_identifier_serializer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      889 2024-04-11 20:49:06.000000 azure-communication-chat-1.3.0/tests/unittest_helpers.py
```

### Comparing `azure-communication-chat-1.2.0/CHANGELOG.md` & `azure-communication-chat-1.3.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release History
 
+## 1.3.0 (2024-04-10)
+
+### Features Added
+
+- Updated `chat_attachment.attachment_type`to include type `file` to support ACS users to recieve files shared by Teams user.
+- Added support for a new communication identifier `MicrosoftTeamsAppIdentifier`.
+
 ## 1.2.0 (2023-12-04)
 
 ### Features Added
 
 - Added the support to receive inline images from Microsoft Teams users in an interoperability Chat with new type `ChatAttachment`
 - Added support for proactive refreshing of tokens
 - `CommunicationTokenCredential` exposes a new boolean keyword argument `proactive_refresh` that defaults to `False`. If set to `True`, the refreshing of the token will be scheduled in the background ensuring continuous authentication state.
```

### Comparing `azure-communication-chat-1.2.0/LICENSE` & `azure-communication-chat-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/PKG-INFO` & `azure-communication-chat-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: azure-communication-chat
-Version: 1.2.0
+Version: 1.3.0
 Summary: Microsoft Azure Communication Chat Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-core<2.0.0,>=1.29.5
+Requires-Dist: isodate>=0.6.1
+Requires-Dist: azure-core>=1.29.5
 Requires-Dist: typing-extensions>=4.3.0
 
 # Azure Communication Chat Package client library for Python
 
 This package contains a Python SDK for Azure Communication Services for Chat.
 Read more about Azure Communication Services [here](https://docs.microsoft.com/azure/communication-services/overview)
```

### Comparing `azure-communication-chat-1.2.0/README.md` & `azure-communication-chat-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/__init__.py` & `azure-communication-chat-1.3.0/azure/communication/chat/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     CommunicationIdentifier,
     CommunicationIdentifierKind,
     CommunicationUserIdentifier,
     CommunicationUserProperties,
     identifier_from_raw_id,
     PhoneNumberIdentifier,
     PhoneNumberProperties,
+    MicrosoftTeamsAppIdentifier,
+    MicrosoftTeamsAppProperties,
     MicrosoftTeamsUserIdentifier,
     MicrosoftTeamsUserProperties,
     UnknownIdentifier
 )
 
 __all__ = [
     'ChatClient',
@@ -49,14 +51,16 @@
     'CreateChatThreadResult',
     'ChatError',
     'CommunicationTokenCredential',
     'CommunicationIdentifier',
     'CommunicationIdentifierKind',
     'CommunicationUserIdentifier',
     'CommunicationUserProperties',
+    'MicrosoftTeamsAppIdentifier',
+    'MicrosoftTeamsAppProperties',
     'MicrosoftTeamsUserIdentifier',
     'MicrosoftTeamsUserProperties',
     'identifier_from_raw_id',
     'PhoneNumberIdentifier',
     'PhoneNumberProperties',
     'UnknownIdentifier'
 ]
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_chat_client.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_chat_client.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_chat_thread_client.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_chat_thread_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
         **kwargs  # type: Any
     ):
         # type: (...) -> ItemPaged[ChatMessage]
         """Gets a list of messages from a thread.
 
         :keyword int results_per_page: The maximum number of messages to be returned per page.
         :keyword ~datetime.datetime start_time: The earliest point in time to get messages up to.
-        The timestamp should be in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
+            The timestamp should be in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``.
         :return: An iterator like instance of ChatMessage
         :rtype: ~azure.core.paging.ItemPaged[~azure.communication.chat.ChatMessage]
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample.py
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_communication_identifier_serializer.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_communication_identifier_serializer.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/__init__.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/_azure_communication_chat_service.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/_azure_communication_chat_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     :ivar chat_thread: ChatThreadOperations operations
     :vartype chat_thread: azure.communication.chat.operations.ChatThreadOperations
     :ivar chat: ChatOperations operations
     :vartype chat: azure.communication.chat.operations.ChatOperations
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2023-11-07". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-07". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, **kwargs: Any
     ) -> None:
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/_configuration.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     """Configuration for AzureCommunicationChatService.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2023-11-07". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-07". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2023-11-07")
+        api_version: str = kwargs.pop("api_version", "2024-03-07")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "azurecommunicationchatservice/{}".format(VERSION))
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/_patch.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/_serialization.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,21 +166,14 @@
             content_type = "application/json"
 
         if body_bytes:
             return cls.deserialize_from_text(body_bytes, content_type)
         return None
 
 
-try:
-    basestring  # type: ignore
-    unicode_str = unicode  # type: ignore
-except NameError:
-    basestring = str
-    unicode_str = str
-
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
 
@@ -541,15 +534,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -557,15 +550,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -645,15 +638,15 @@
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
                             serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
-                            local_node.text = unicode_str(new_attr)
+                            local_node.text = str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
                             new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
@@ -741,15 +734,15 @@
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str
+        :rtype: str, list
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
@@ -990,15 +983,15 @@
         if isinstance(attr, ET.Element):
             return attr
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.serialize_basic(attr, self.basic_types[obj_type], **kwargs)
         if obj_type is _long_type:
             return self.serialize_long(attr)
-        if obj_type is unicode_str:
+        if obj_type is str:
             return self.serialize_unicode(attr)
         if obj_type is datetime.datetime:
             return self.serialize_iso(attr)
         if obj_type is datetime.date:
             return self.serialize_date(attr)
         if obj_type is datetime.time:
             return self.serialize_time(attr)
@@ -1366,15 +1359,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1386,15 +1379,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1439,15 +1432,15 @@
                     setattr(data, attr, self._deserialize(local_type, value))
                 return data
             except AttributeError:
                 return
 
         response, class_name = self._classify_target(target_obj, data)
 
-        if isinstance(response, basestring):
+        if isinstance(response, str):
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
@@ -1510,22 +1503,22 @@
 
         :param str target: The target object type to deserialize to.
         :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
-        if isinstance(target, basestring):
+        if isinstance(target, str):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
-            target = target._classify(data, self.dependencies)
+            target = target._classify(data, self.dependencies)  # type: ignore
         except AttributeError:
             pass  # Target is not a Model, no classify
         return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
@@ -1573,15 +1566,15 @@
         if hasattr(raw_data, "body"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
-        if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
+        if isinstance(raw_data, (str, bytes)) or hasattr(raw_data, "read"):
             return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
@@ -1695,15 +1688,15 @@
         :raises: TypeError if non-builtin datatype encountered.
         """
         if attr is None:
             return None
         if isinstance(attr, ET.Element):
             # Do no recurse on XML, just return the tree as-is
             return attr
-        if isinstance(attr, basestring):
+        if isinstance(attr, str):
             return self.deserialize_basic(attr, "str")
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.deserialize_basic(attr, self.basic_types[obj_type])
         if obj_type is _long_type:
             return self.deserialize_long(attr)
 
@@ -1752,15 +1745,15 @@
                     # None or '', node <a/> with a strong type is None.
                     # Don't try to model "empty bool" or "empty int"
                     return None
 
         if data_type == "bool":
             if attr in [True, False, 1, 0]:
                 return bool(attr)
-            elif isinstance(attr, basestring):
+            elif isinstance(attr, str):
                 if attr.lower() in ["true", "1"]:
                     return True
                 elif attr.lower() in ["false", "0"]:
                     return False
             raise TypeError("Invalid boolean value: {}".format(attr))
 
         if data_type == "str":
@@ -1856,15 +1849,15 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)  # type: ignore
+            return decimal.Decimal(str(attr))  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
             raise DeserializationError(msg) from err
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
@@ -1992,13 +1985,14 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
+            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise DeserializationError(msg) from err
         else:
             return date_obj
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/_vendor.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/__init__.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/_azure_communication_chat_service.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/_azure_communication_chat_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     :ivar chat_thread: ChatThreadOperations operations
     :vartype chat_thread: azure.communication.chat.aio.operations.ChatThreadOperations
     :ivar chat: ChatOperations operations
     :vartype chat: azure.communication.chat.aio.operations.ChatOperations
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2023-11-07". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-07". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, **kwargs: Any
     ) -> None:
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/_configuration.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     """Configuration for AzureCommunicationChatService.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param endpoint: The endpoint of the Azure Communication resource. Required.
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2023-11-07". Note that overriding this
+    :keyword api_version: Api Version. Default value is "2024-03-07". Note that overriding this
      default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2023-11-07")
+        api_version: str = kwargs.pop("api_version", "2024-03-07")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "azurecommunicationchatservice/{}".format(VERSION))
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/_patch.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/__init__.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/_chat_operations.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/_chat_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -79,77 +79,71 @@
          request multiple times. The value of the Repeatability-Request-Id is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :type repeatability_request_id: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CreateChatThreadResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.CreateChatThreadResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_chat_thread(
         self,
-        create_chat_thread_request: IO,
+        create_chat_thread_request: IO[bytes],
         repeatability_request_id: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CreateChatThreadResult:
         """Creates a chat thread.
 
         Creates a chat thread.
 
         :param create_chat_thread_request: Request payload for creating a chat thread. Required.
-        :type create_chat_thread_request: IO
+        :type create_chat_thread_request: IO[bytes]
         :param repeatability_request_id: If specified, the client directs that the request is
          repeatable; that is, that the client can make the request multiple times with the same
          Repeatability-Request-Id and get back an appropriate response without the server executing the
          request multiple times. The value of the Repeatability-Request-Id is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :type repeatability_request_id: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CreateChatThreadResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.CreateChatThreadResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_chat_thread(
         self,
-        create_chat_thread_request: Union[_models.CreateChatThreadRequest, IO],
+        create_chat_thread_request: Union[_models.CreateChatThreadRequest, IO[bytes]],
         repeatability_request_id: Optional[str] = None,
         **kwargs: Any
     ) -> _models.CreateChatThreadResult:
         """Creates a chat thread.
 
         Creates a chat thread.
 
         :param create_chat_thread_request: Request payload for creating a chat thread. Is either a
-         CreateChatThreadRequest type or a IO type. Required.
+         CreateChatThreadRequest type or a IO[bytes] type. Required.
         :type create_chat_thread_request: ~azure.communication.chat.models.CreateChatThreadRequest or
-         IO
+         IO[bytes]
         :param repeatability_request_id: If specified, the client directs that the request is
          repeatable; that is, that the client can make the request multiple times with the same
          Repeatability-Request-Id and get back an appropriate response without the server executing the
          request multiple times. The value of the Repeatability-Request-Id is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :type repeatability_request_id: str
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CreateChatThreadResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.CreateChatThreadResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -203,15 +197,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("CreateChatThreadResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -227,15 +221,14 @@
 
         :param max_page_size: The maximum number of chat threads returned per page. Default value is
          None.
         :type max_page_size: int
         :param start_time: The earliest point in time to get chat threads up to. The timestamp should
          be in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``. Default value is None.
         :type start_time: ~datetime.datetime
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatThreadItem or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.communication.chat.models.ChatThreadItem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -316,15 +309,15 @@
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     @distributed_trace_async
@@ -333,15 +326,14 @@
     ) -> None:
         """Deletes a thread.
 
         Deletes a thread.
 
         :param chat_thread_id: Id of the thread to be deleted. Required.
         :type chat_thread_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -383,12 +375,12 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/_chat_thread_operations.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/_chat_thread_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -80,15 +80,14 @@
         :type chat_thread_id: str
         :param max_page_size: The maximum number of chat message read receipts to be returned per page.
          Default value is None.
         :type max_page_size: int
         :param skip: Skips chat message read receipts up to a specified position in response. Default
          value is None.
         :type skip: int
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatMessageReadReceipt or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.communication.chat.models.ChatMessageReadReceipt]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -171,15 +170,15 @@
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     @overload
@@ -198,63 +197,61 @@
         :param chat_thread_id: Thread id to send the read receipt event to. Required.
         :type chat_thread_id: str
         :param send_read_receipt_request: Read receipt details. Required.
         :type send_read_receipt_request: ~azure.communication.chat.models.SendReadReceiptRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def send_chat_read_receipt(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        send_read_receipt_request: IO,
+        send_read_receipt_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Sends a read receipt event to a thread, on behalf of a user.
 
         Sends a read receipt event to a thread, on behalf of a user.
 
         :param chat_thread_id: Thread id to send the read receipt event to. Required.
         :type chat_thread_id: str
         :param send_read_receipt_request: Read receipt details. Required.
-        :type send_read_receipt_request: IO
+        :type send_read_receipt_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def send_chat_read_receipt(  # pylint: disable=inconsistent-return-statements
-        self, chat_thread_id: str, send_read_receipt_request: Union[_models.SendReadReceiptRequest, IO], **kwargs: Any
+        self,
+        chat_thread_id: str,
+        send_read_receipt_request: Union[_models.SendReadReceiptRequest, IO[bytes]],
+        **kwargs: Any
     ) -> None:
         """Sends a read receipt event to a thread, on behalf of a user.
 
         Sends a read receipt event to a thread, on behalf of a user.
 
         :param chat_thread_id: Thread id to send the read receipt event to. Required.
         :type chat_thread_id: str
         :param send_read_receipt_request: Read receipt details. Is either a SendReadReceiptRequest type
-         or a IO type. Required.
-        :type send_read_receipt_request: ~azure.communication.chat.models.SendReadReceiptRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         or a IO[bytes] type. Required.
+        :type send_read_receipt_request: ~azure.communication.chat.models.SendReadReceiptRequest or
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -308,15 +305,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
     async def send_chat_message(
@@ -334,63 +331,61 @@
         :param chat_thread_id: The thread id to send the message to. Required.
         :type chat_thread_id: str
         :param send_chat_message_request: Details of the message to send. Required.
         :type send_chat_message_request: ~azure.communication.chat.models.SendChatMessageRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SendChatMessageResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.SendChatMessageResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def send_chat_message(
         self,
         chat_thread_id: str,
-        send_chat_message_request: IO,
+        send_chat_message_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.SendChatMessageResult:
         """Sends a message to a thread.
 
         Sends a message to a thread.
 
         :param chat_thread_id: The thread id to send the message to. Required.
         :type chat_thread_id: str
         :param send_chat_message_request: Details of the message to send. Required.
-        :type send_chat_message_request: IO
+        :type send_chat_message_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SendChatMessageResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.SendChatMessageResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def send_chat_message(
-        self, chat_thread_id: str, send_chat_message_request: Union[_models.SendChatMessageRequest, IO], **kwargs: Any
+        self,
+        chat_thread_id: str,
+        send_chat_message_request: Union[_models.SendChatMessageRequest, IO[bytes]],
+        **kwargs: Any
     ) -> _models.SendChatMessageResult:
         """Sends a message to a thread.
 
         Sends a message to a thread.
 
         :param chat_thread_id: The thread id to send the message to. Required.
         :type chat_thread_id: str
         :param send_chat_message_request: Details of the message to send. Is either a
-         SendChatMessageRequest type or a IO type. Required.
-        :type send_chat_message_request: ~azure.communication.chat.models.SendChatMessageRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         SendChatMessageRequest type or a IO[bytes] type. Required.
+        :type send_chat_message_request: ~azure.communication.chat.models.SendChatMessageRequest or
+         IO[bytes]
         :return: SendChatMessageResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.SendChatMessageResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -444,15 +439,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("SendChatMessageResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -474,15 +469,14 @@
         :type chat_thread_id: str
         :param max_page_size: The maximum number of messages to be returned per page. Default value is
          None.
         :type max_page_size: int
         :param start_time: The earliest point in time to get messages up to. The timestamp should be in
          RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``. Default value is None.
         :type start_time: ~datetime.datetime
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatMessage or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.communication.chat.models.ChatMessage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -563,15 +557,15 @@
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     @distributed_trace_async
@@ -580,15 +574,14 @@
 
         Gets a message by id.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ChatMessage or the result of cls(response)
         :rtype: ~azure.communication.chat.models.ChatMessage
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -631,15 +624,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("ChatMessage", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -664,73 +657,67 @@
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
         :param update_chat_message_request: Details of the request to update the message. Required.
         :type update_chat_message_request: ~azure.communication.chat.models.UpdateChatMessageRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update_chat_message(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
         chat_message_id: str,
-        update_chat_message_request: IO,
+        update_chat_message_request: IO[bytes],
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> None:
         """Updates a message.
 
         Updates a message.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
         :param update_chat_message_request: Details of the request to update the message. Required.
-        :type update_chat_message_request: IO
+        :type update_chat_message_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update_chat_message(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
         chat_message_id: str,
-        update_chat_message_request: Union[_models.UpdateChatMessageRequest, IO],
+        update_chat_message_request: Union[_models.UpdateChatMessageRequest, IO[bytes]],
         **kwargs: Any
     ) -> None:
         """Updates a message.
 
         Updates a message.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
         :param update_chat_message_request: Details of the request to update the message. Is either a
-         UpdateChatMessageRequest type or a IO type. Required.
+         UpdateChatMessageRequest type or a IO[bytes] type. Required.
         :type update_chat_message_request: ~azure.communication.chat.models.UpdateChatMessageRequest or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are:
-         'application/merge-patch+json'. Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -785,15 +772,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
     async def delete_chat_message(  # pylint: disable=inconsistent-return-statements
@@ -803,15 +790,14 @@
 
         Deletes a message.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -854,15 +840,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def list_chat_participants(
@@ -875,15 +861,14 @@
         :param chat_thread_id: Thread id to get participants for. Required.
         :type chat_thread_id: str
         :param max_page_size: The maximum number of participants to be returned per page. Default value
          is None.
         :type max_page_size: int
         :param skip: Skips participants up to a specified position in response. Default value is None.
         :type skip: int
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatParticipant or the result of cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.communication.chat.models.ChatParticipant]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -965,15 +950,15 @@
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     @overload
@@ -994,69 +979,63 @@
         :param participant_communication_identifier: Id of the thread participant to remove from the
          thread. Required.
         :type participant_communication_identifier:
          ~azure.communication.chat.models.CommunicationIdentifierModel
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def remove_chat_participant(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        participant_communication_identifier: IO,
+        participant_communication_identifier: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Remove a participant from a thread.
 
         Remove a participant from a thread.
 
         :param chat_thread_id: Thread id to remove the participant from. Required.
         :type chat_thread_id: str
         :param participant_communication_identifier: Id of the thread participant to remove from the
          thread. Required.
-        :type participant_communication_identifier: IO
+        :type participant_communication_identifier: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Known values are: 'application/json', 'application/merge-patch+json'. Default value is
          "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def remove_chat_participant(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        participant_communication_identifier: Union[_models.CommunicationIdentifierModel, IO],
+        participant_communication_identifier: Union[_models.CommunicationIdentifierModel, IO[bytes]],
         **kwargs: Any
     ) -> None:
         """Remove a participant from a thread.
 
         Remove a participant from a thread.
 
         :param chat_thread_id: Thread id to remove the participant from. Required.
         :type chat_thread_id: str
         :param participant_communication_identifier: Id of the thread participant to remove from the
-         thread. Is either a CommunicationIdentifierModel type or a IO type. Required.
+         thread. Is either a CommunicationIdentifierModel type or a IO[bytes] type. Required.
         :type participant_communication_identifier:
-         ~azure.communication.chat.models.CommunicationIdentifierModel or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
-         'application/merge-patch+json'. Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.communication.chat.models.CommunicationIdentifierModel or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1110,15 +1089,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
     async def add_chat_participants(
@@ -1137,67 +1116,61 @@
         :type chat_thread_id: str
         :param add_chat_participants_request: Thread participants to be added to the thread. Required.
         :type add_chat_participants_request:
          ~azure.communication.chat.models.AddChatParticipantsRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AddChatParticipantsResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.AddChatParticipantsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def add_chat_participants(
         self,
         chat_thread_id: str,
-        add_chat_participants_request: IO,
+        add_chat_participants_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.AddChatParticipantsResult:
         """Adds thread participants to a thread. If participants already exist, no change occurs.
 
         Adds thread participants to a thread. If participants already exist, no change occurs.
 
         :param chat_thread_id: Id of the thread to add participants to. Required.
         :type chat_thread_id: str
         :param add_chat_participants_request: Thread participants to be added to the thread. Required.
-        :type add_chat_participants_request: IO
+        :type add_chat_participants_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AddChatParticipantsResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.AddChatParticipantsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def add_chat_participants(
         self,
         chat_thread_id: str,
-        add_chat_participants_request: Union[_models.AddChatParticipantsRequest, IO],
+        add_chat_participants_request: Union[_models.AddChatParticipantsRequest, IO[bytes]],
         **kwargs: Any
     ) -> _models.AddChatParticipantsResult:
         """Adds thread participants to a thread. If participants already exist, no change occurs.
 
         Adds thread participants to a thread. If participants already exist, no change occurs.
 
         :param chat_thread_id: Id of the thread to add participants to. Required.
         :type chat_thread_id: str
         :param add_chat_participants_request: Thread participants to be added to the thread. Is either
-         a AddChatParticipantsRequest type or a IO type. Required.
+         a AddChatParticipantsRequest type or a IO[bytes] type. Required.
         :type add_chat_participants_request:
-         ~azure.communication.chat.models.AddChatParticipantsRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.communication.chat.models.AddChatParticipantsRequest or IO[bytes]
         :return: AddChatParticipantsResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.AddChatParticipantsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1251,15 +1224,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("AddChatParticipantsResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -1281,64 +1254,61 @@
         :param chat_thread_id: The id of the thread to update. Required.
         :type chat_thread_id: str
         :param update_chat_thread_request: Request payload for updating a chat thread. Required.
         :type update_chat_thread_request: ~azure.communication.chat.models.UpdateChatThreadRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update_chat_thread_properties(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        update_chat_thread_request: IO,
+        update_chat_thread_request: IO[bytes],
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> None:
         """Updates a thread's properties.
 
         Updates a thread's properties.
 
         :param chat_thread_id: The id of the thread to update. Required.
         :type chat_thread_id: str
         :param update_chat_thread_request: Request payload for updating a chat thread. Required.
-        :type update_chat_thread_request: IO
+        :type update_chat_thread_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update_chat_thread_properties(  # pylint: disable=inconsistent-return-statements
-        self, chat_thread_id: str, update_chat_thread_request: Union[_models.UpdateChatThreadRequest, IO], **kwargs: Any
+        self,
+        chat_thread_id: str,
+        update_chat_thread_request: Union[_models.UpdateChatThreadRequest, IO[bytes]],
+        **kwargs: Any
     ) -> None:
         """Updates a thread's properties.
 
         Updates a thread's properties.
 
         :param chat_thread_id: The id of the thread to update. Required.
         :type chat_thread_id: str
         :param update_chat_thread_request: Request payload for updating a chat thread. Is either a
-         UpdateChatThreadRequest type or a IO type. Required.
+         UpdateChatThreadRequest type or a IO[bytes] type. Required.
         :type update_chat_thread_request: ~azure.communication.chat.models.UpdateChatThreadRequest or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are:
-         'application/merge-patch+json'. Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1392,29 +1362,28 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace_async
     async def get_chat_thread_properties(self, chat_thread_id: str, **kwargs: Any) -> _models.ChatThreadProperties:
         """Gets a chat thread's properties.
 
         Gets a chat thread's properties.
 
         :param chat_thread_id: Id of the thread. Required.
         :type chat_thread_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ChatThreadProperties or the result of cls(response)
         :rtype: ~azure.communication.chat.models.ChatThreadProperties
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1456,15 +1425,15 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("ChatThreadProperties", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -1488,68 +1457,62 @@
         :param send_typing_notification_request: Details of the typing notification request. Default
          value is None.
         :type send_typing_notification_request:
          ~azure.communication.chat.models.SendTypingNotificationRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def send_typing_notification(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        send_typing_notification_request: Optional[IO] = None,
+        send_typing_notification_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Posts a typing event to a thread, on behalf of a user.
 
         Posts a typing event to a thread, on behalf of a user.
 
         :param chat_thread_id: Id of the thread. Required.
         :type chat_thread_id: str
         :param send_typing_notification_request: Details of the typing notification request. Default
          value is None.
-        :type send_typing_notification_request: IO
+        :type send_typing_notification_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def send_typing_notification(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        send_typing_notification_request: Optional[Union[_models.SendTypingNotificationRequest, IO]] = None,
+        send_typing_notification_request: Optional[Union[_models.SendTypingNotificationRequest, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         """Posts a typing event to a thread, on behalf of a user.
 
         Posts a typing event to a thread, on behalf of a user.
 
         :param chat_thread_id: Id of the thread. Required.
         :type chat_thread_id: str
         :param send_typing_notification_request: Details of the typing notification request. Is either
-         a SendTypingNotificationRequest type or a IO type. Default value is None.
+         a SendTypingNotificationRequest type or a IO[bytes] type. Default value is None.
         :type send_typing_notification_request:
-         ~azure.communication.chat.models.SendTypingNotificationRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.communication.chat.models.SendTypingNotificationRequest or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1606,12 +1569,12 @@
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/aio/operations/_patch.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/__init__.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from ._models_py3 import ChatThreadProperties
 from ._models_py3 import ChatThreadsItemCollection
 from ._models_py3 import CommunicationErrorResponse
 from ._models_py3 import CommunicationIdentifierModel
 from ._models_py3 import CommunicationUserIdentifierModel
 from ._models_py3 import CreateChatThreadRequest
 from ._models_py3 import CreateChatThreadResult
+from ._models_py3 import MicrosoftTeamsAppIdentifierModel
 from ._models_py3 import MicrosoftTeamsUserIdentifierModel
 from ._models_py3 import PhoneNumberIdentifierModel
 from ._models_py3 import SendChatMessageRequest
 from ._models_py3 import SendChatMessageResult
 from ._models_py3 import SendReadReceiptRequest
 from ._models_py3 import SendTypingNotificationRequest
 from ._models_py3 import UpdateChatMessageRequest
@@ -58,14 +59,15 @@
     "ChatThreadProperties",
     "ChatThreadsItemCollection",
     "CommunicationErrorResponse",
     "CommunicationIdentifierModel",
     "CommunicationUserIdentifierModel",
     "CreateChatThreadRequest",
     "CreateChatThreadResult",
+    "MicrosoftTeamsAppIdentifierModel",
     "MicrosoftTeamsUserIdentifierModel",
     "PhoneNumberIdentifierModel",
     "SendChatMessageRequest",
     "SendChatMessageResult",
     "SendReadReceiptRequest",
     "SendTypingNotificationRequest",
     "UpdateChatMessageRequest",
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/_azure_communication_chat_service_enums.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/_azure_communication_chat_service_enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from azure.core import CaseInsensitiveEnumMeta
 
 
 class ChatAttachmentType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The type of attachment."""
 
     IMAGE = "image"
+    FILE = "file"
 
 
 class ChatMessageType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The chat message type."""
 
     TEXT = "text"
     HTML = "html"
@@ -37,7 +38,8 @@
 class CommunicationIdentifierModelKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The identifier kind, for example 'communicationUser' or 'phoneNumber'."""
 
     UNKNOWN = "unknown"
     COMMUNICATION_USER = "communicationUser"
     PHONE_NUMBER = "phoneNumber"
     MICROSOFT_TEAMS_USER = "microsoftTeamsUser"
+    MICROSOFT_TEAMS_APP = "microsoftTeamsApp"
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/_models_py3.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/_models_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 class ChatAttachment(_serialization.Model):
     """An attachment in a chat message.
 
     All required parameters must be populated in order to send to server.
 
     :ivar id: Id of the attachment. Required.
     :vartype id: str
-    :ivar attachment_type: The type of attachment. Required. "image"
+    :ivar attachment_type: The type of attachment. Required. Known values are: "image" and "file".
     :vartype attachment_type: str or ~azure.communication.chat.models.ChatAttachmentType
     :ivar name: The name of the attachment content.
     :vartype name: str
     :ivar url: The URL where the attachment can be downloaded.
     :vartype url: str
     :ivar preview_url: The URL where the preview of attachment can be downloaded.
     :vartype preview_url: str
@@ -105,15 +105,16 @@
         url: Optional[str] = None,
         preview_url: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Id of the attachment. Required.
         :paramtype id: str
-        :keyword attachment_type: The type of attachment. Required. "image"
+        :keyword attachment_type: The type of attachment. Required. Known values are: "image" and
+         "file".
         :paramtype attachment_type: str or ~azure.communication.chat.models.ChatAttachmentType
         :keyword name: The name of the attachment content.
         :paramtype name: str
         :keyword url: The URL where the attachment can be downloaded.
         :paramtype url: str
         :keyword preview_url: The URL where the preview of attachment can be downloaded.
         :paramtype preview_url: str
@@ -782,66 +783,74 @@
 
 class CommunicationIdentifierModel(_serialization.Model):
     """Identifies a participant in Azure Communication services. A participant is, for example, a
     phone number or an Azure communication user. This model is polymorphic: Apart from kind and
     rawId, at most one further property may be set which must match the kind enum value.
 
     :ivar kind: The identifier kind. Only required in responses. Known values are: "unknown",
-     "communicationUser", "phoneNumber", and "microsoftTeamsUser".
+     "communicationUser", "phoneNumber", "microsoftTeamsUser", and "microsoftTeamsApp".
     :vartype kind: str or ~azure.communication.chat.models.CommunicationIdentifierModelKind
     :ivar raw_id: Raw Id of the identifier. Optional in requests, required in responses.
     :vartype raw_id: str
     :ivar communication_user: The communication user.
     :vartype communication_user: ~azure.communication.chat.models.CommunicationUserIdentifierModel
     :ivar phone_number: The phone number.
     :vartype phone_number: ~azure.communication.chat.models.PhoneNumberIdentifierModel
     :ivar microsoft_teams_user: The Microsoft Teams user.
     :vartype microsoft_teams_user:
      ~azure.communication.chat.models.MicrosoftTeamsUserIdentifierModel
+    :ivar microsoft_teams_app: The Microsoft Teams application.
+    :vartype microsoft_teams_app: ~azure.communication.chat.models.MicrosoftTeamsAppIdentifierModel
     """
 
     _attribute_map = {
         "kind": {"key": "kind", "type": "str"},
         "raw_id": {"key": "rawId", "type": "str"},
         "communication_user": {"key": "communicationUser", "type": "CommunicationUserIdentifierModel"},
         "phone_number": {"key": "phoneNumber", "type": "PhoneNumberIdentifierModel"},
         "microsoft_teams_user": {"key": "microsoftTeamsUser", "type": "MicrosoftTeamsUserIdentifierModel"},
+        "microsoft_teams_app": {"key": "microsoftTeamsApp", "type": "MicrosoftTeamsAppIdentifierModel"},
     }
 
     def __init__(
         self,
         *,
         kind: Optional[Union[str, "_models.CommunicationIdentifierModelKind"]] = None,
         raw_id: Optional[str] = None,
         communication_user: Optional["_models.CommunicationUserIdentifierModel"] = None,
         phone_number: Optional["_models.PhoneNumberIdentifierModel"] = None,
         microsoft_teams_user: Optional["_models.MicrosoftTeamsUserIdentifierModel"] = None,
+        microsoft_teams_app: Optional["_models.MicrosoftTeamsAppIdentifierModel"] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword kind: The identifier kind. Only required in responses. Known values are: "unknown",
-         "communicationUser", "phoneNumber", and "microsoftTeamsUser".
+         "communicationUser", "phoneNumber", "microsoftTeamsUser", and "microsoftTeamsApp".
         :paramtype kind: str or ~azure.communication.chat.models.CommunicationIdentifierModelKind
         :keyword raw_id: Raw Id of the identifier. Optional in requests, required in responses.
         :paramtype raw_id: str
         :keyword communication_user: The communication user.
         :paramtype communication_user:
          ~azure.communication.chat.models.CommunicationUserIdentifierModel
         :keyword phone_number: The phone number.
         :paramtype phone_number: ~azure.communication.chat.models.PhoneNumberIdentifierModel
         :keyword microsoft_teams_user: The Microsoft Teams user.
         :paramtype microsoft_teams_user:
          ~azure.communication.chat.models.MicrosoftTeamsUserIdentifierModel
+        :keyword microsoft_teams_app: The Microsoft Teams application.
+        :paramtype microsoft_teams_app:
+         ~azure.communication.chat.models.MicrosoftTeamsAppIdentifierModel
         """
         super().__init__(**kwargs)
         self.kind = kind
         self.raw_id = raw_id
         self.communication_user = communication_user
         self.phone_number = phone_number
         self.microsoft_teams_user = microsoft_teams_user
+        self.microsoft_teams_app = microsoft_teams_app
 
 
 class CommunicationUserIdentifierModel(_serialization.Model):
     """A user that got created with an Azure Communication Services resource.
 
     All required parameters must be populated in order to send to server.
 
@@ -926,14 +935,54 @@
         :paramtype chat_thread: ~azure.communication.chat.models.ChatThreadProperties
         """
         super().__init__(**kwargs)
         self.chat_thread = chat_thread
         self.invalid_participants = None
 
 
+class MicrosoftTeamsAppIdentifierModel(_serialization.Model):
+    """A Microsoft Teams application.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar app_id: The Id of the Microsoft Teams application. Required.
+    :vartype app_id: str
+    :ivar cloud: The cloud that the Microsoft Teams application belongs to. By default 'public' if
+     missing. Known values are: "public", "dod", and "gcch".
+    :vartype cloud: str or ~azure.communication.chat.models.CommunicationCloudEnvironmentModel
+    """
+
+    _validation = {
+        "app_id": {"required": True},
+    }
+
+    _attribute_map = {
+        "app_id": {"key": "appId", "type": "str"},
+        "cloud": {"key": "cloud", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        app_id: str,
+        cloud: Optional[Union[str, "_models.CommunicationCloudEnvironmentModel"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword app_id: The Id of the Microsoft Teams application. Required.
+        :paramtype app_id: str
+        :keyword cloud: The cloud that the Microsoft Teams application belongs to. By default 'public'
+         if missing. Known values are: "public", "dod", and "gcch".
+        :paramtype cloud: str or ~azure.communication.chat.models.CommunicationCloudEnvironmentModel
+        """
+        super().__init__(**kwargs)
+        self.app_id = app_id
+        self.cloud = cloud
+
+
 class MicrosoftTeamsUserIdentifierModel(_serialization.Model):
     """A Microsoft Teams user.
 
     All required parameters must be populated in order to send to server.
 
     :ivar user_id: The Id of the Microsoft Teams user. If not anonymous, this is the AAD object Id
      of the user. Required.
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/models/_patch.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/__init__.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/_chat_operations.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/_chat_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -38,15 +38,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_chat_thread_request(*, repeatability_request_id: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads")
 
     # Construct parameters
@@ -66,15 +66,15 @@
 
 def build_list_chat_threads_request(
     *, max_page_size: Optional[int] = None, start_time: Optional[datetime.datetime] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads")
 
     # Construct parameters
     if max_page_size is not None:
@@ -89,15 +89,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_chat_thread_request(chat_thread_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
     }
@@ -153,77 +153,71 @@
          request multiple times. The value of the Repeatability-Request-Id is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :type repeatability_request_id: str
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CreateChatThreadResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.CreateChatThreadResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_chat_thread(
         self,
-        create_chat_thread_request: IO,
+        create_chat_thread_request: IO[bytes],
         repeatability_request_id: Optional[str] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.CreateChatThreadResult:
         """Creates a chat thread.
 
         Creates a chat thread.
 
         :param create_chat_thread_request: Request payload for creating a chat thread. Required.
-        :type create_chat_thread_request: IO
+        :type create_chat_thread_request: IO[bytes]
         :param repeatability_request_id: If specified, the client directs that the request is
          repeatable; that is, that the client can make the request multiple times with the same
          Repeatability-Request-Id and get back an appropriate response without the server executing the
          request multiple times. The value of the Repeatability-Request-Id is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :type repeatability_request_id: str
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CreateChatThreadResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.CreateChatThreadResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_chat_thread(
         self,
-        create_chat_thread_request: Union[_models.CreateChatThreadRequest, IO],
+        create_chat_thread_request: Union[_models.CreateChatThreadRequest, IO[bytes]],
         repeatability_request_id: Optional[str] = None,
         **kwargs: Any
     ) -> _models.CreateChatThreadResult:
         """Creates a chat thread.
 
         Creates a chat thread.
 
         :param create_chat_thread_request: Request payload for creating a chat thread. Is either a
-         CreateChatThreadRequest type or a IO type. Required.
+         CreateChatThreadRequest type or a IO[bytes] type. Required.
         :type create_chat_thread_request: ~azure.communication.chat.models.CreateChatThreadRequest or
-         IO
+         IO[bytes]
         :param repeatability_request_id: If specified, the client directs that the request is
          repeatable; that is, that the client can make the request multiple times with the same
          Repeatability-Request-Id and get back an appropriate response without the server executing the
          request multiple times. The value of the Repeatability-Request-Id is an opaque string
          representing a client-generated, globally unique for all time, identifier for the request. It
          is recommended to use version 4 (random) UUIDs. Default value is None.
         :type repeatability_request_id: str
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: CreateChatThreadResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.CreateChatThreadResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -277,15 +271,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("CreateChatThreadResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -301,15 +295,14 @@
 
         :param max_page_size: The maximum number of chat threads returned per page. Default value is
          None.
         :type max_page_size: int
         :param start_time: The earliest point in time to get chat threads up to. The timestamp should
          be in RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``. Default value is None.
         :type start_time: ~datetime.datetime
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatThreadItem or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.communication.chat.models.ChatThreadItem]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -389,15 +382,15 @@
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     @distributed_trace
@@ -406,15 +399,14 @@
     ) -> None:
         """Deletes a thread.
 
         Deletes a thread.
 
         :param chat_thread_id: Id of the thread to be deleted. Required.
         :type chat_thread_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -456,12 +448,12 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/_chat_thread_operations.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/_chat_thread_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -39,15 +39,15 @@
 
 def build_list_chat_read_receipts_request(
     chat_thread_id: str, *, max_page_size: Optional[int] = None, skip: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/readReceipts")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
     }
@@ -67,15 +67,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_send_chat_read_receipt_request(chat_thread_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/readReceipts")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
@@ -94,15 +94,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_send_chat_message_request(chat_thread_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/messages")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
@@ -127,15 +127,15 @@
     max_page_size: Optional[int] = None,
     start_time: Optional[datetime.datetime] = None,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/messages")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
     }
@@ -155,15 +155,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_chat_message_request(chat_thread_id: str, chat_message_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/messages/{chatMessageId}")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
         "chatMessageId": _SERIALIZER.url("chat_message_id", chat_message_id, "str"),
@@ -180,15 +180,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_chat_message_request(chat_thread_id: str, chat_message_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/messages/{chatMessageId}")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
@@ -208,15 +208,15 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_chat_message_request(chat_thread_id: str, chat_message_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/messages/{chatMessageId}")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
         "chatMessageId": _SERIALIZER.url("chat_message_id", chat_message_id, "str"),
@@ -235,15 +235,15 @@
 
 def build_list_chat_participants_request(
     chat_thread_id: str, *, max_page_size: Optional[int] = None, skip: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/participants")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
     }
@@ -263,15 +263,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_remove_chat_participant_request(chat_thread_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/participants/:remove")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
@@ -290,15 +290,15 @@
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_add_chat_participants_request(chat_thread_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/participants/:add")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
@@ -319,15 +319,15 @@
 
 def build_update_chat_thread_properties_request(  # pylint: disable=name-too-long
     chat_thread_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
@@ -346,15 +346,15 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_chat_thread_properties_request(chat_thread_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
     }
@@ -370,15 +370,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_send_typing_notification_request(chat_thread_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-11-07"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-07"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/chat/threads/{chatThreadId}/typing")
     path_format_arguments = {
         "chatThreadId": _SERIALIZER.url("chat_thread_id", chat_thread_id, "str"),
@@ -428,15 +428,14 @@
         :type chat_thread_id: str
         :param max_page_size: The maximum number of chat message read receipts to be returned per page.
          Default value is None.
         :type max_page_size: int
         :param skip: Skips chat message read receipts up to a specified position in response. Default
          value is None.
         :type skip: int
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatMessageReadReceipt or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.communication.chat.models.ChatMessageReadReceipt]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -518,15 +517,15 @@
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     @overload
@@ -545,63 +544,61 @@
         :param chat_thread_id: Thread id to send the read receipt event to. Required.
         :type chat_thread_id: str
         :param send_read_receipt_request: Read receipt details. Required.
         :type send_read_receipt_request: ~azure.communication.chat.models.SendReadReceiptRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def send_chat_read_receipt(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        send_read_receipt_request: IO,
+        send_read_receipt_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Sends a read receipt event to a thread, on behalf of a user.
 
         Sends a read receipt event to a thread, on behalf of a user.
 
         :param chat_thread_id: Thread id to send the read receipt event to. Required.
         :type chat_thread_id: str
         :param send_read_receipt_request: Read receipt details. Required.
-        :type send_read_receipt_request: IO
+        :type send_read_receipt_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def send_chat_read_receipt(  # pylint: disable=inconsistent-return-statements
-        self, chat_thread_id: str, send_read_receipt_request: Union[_models.SendReadReceiptRequest, IO], **kwargs: Any
+        self,
+        chat_thread_id: str,
+        send_read_receipt_request: Union[_models.SendReadReceiptRequest, IO[bytes]],
+        **kwargs: Any
     ) -> None:
         """Sends a read receipt event to a thread, on behalf of a user.
 
         Sends a read receipt event to a thread, on behalf of a user.
 
         :param chat_thread_id: Thread id to send the read receipt event to. Required.
         :type chat_thread_id: str
         :param send_read_receipt_request: Read receipt details. Is either a SendReadReceiptRequest type
-         or a IO type. Required.
-        :type send_read_receipt_request: ~azure.communication.chat.models.SendReadReceiptRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         or a IO[bytes] type. Required.
+        :type send_read_receipt_request: ~azure.communication.chat.models.SendReadReceiptRequest or
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -655,15 +652,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
     def send_chat_message(
@@ -681,63 +678,61 @@
         :param chat_thread_id: The thread id to send the message to. Required.
         :type chat_thread_id: str
         :param send_chat_message_request: Details of the message to send. Required.
         :type send_chat_message_request: ~azure.communication.chat.models.SendChatMessageRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SendChatMessageResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.SendChatMessageResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def send_chat_message(
         self,
         chat_thread_id: str,
-        send_chat_message_request: IO,
+        send_chat_message_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.SendChatMessageResult:
         """Sends a message to a thread.
 
         Sends a message to a thread.
 
         :param chat_thread_id: The thread id to send the message to. Required.
         :type chat_thread_id: str
         :param send_chat_message_request: Details of the message to send. Required.
-        :type send_chat_message_request: IO
+        :type send_chat_message_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: SendChatMessageResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.SendChatMessageResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def send_chat_message(
-        self, chat_thread_id: str, send_chat_message_request: Union[_models.SendChatMessageRequest, IO], **kwargs: Any
+        self,
+        chat_thread_id: str,
+        send_chat_message_request: Union[_models.SendChatMessageRequest, IO[bytes]],
+        **kwargs: Any
     ) -> _models.SendChatMessageResult:
         """Sends a message to a thread.
 
         Sends a message to a thread.
 
         :param chat_thread_id: The thread id to send the message to. Required.
         :type chat_thread_id: str
         :param send_chat_message_request: Details of the message to send. Is either a
-         SendChatMessageRequest type or a IO type. Required.
-        :type send_chat_message_request: ~azure.communication.chat.models.SendChatMessageRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         SendChatMessageRequest type or a IO[bytes] type. Required.
+        :type send_chat_message_request: ~azure.communication.chat.models.SendChatMessageRequest or
+         IO[bytes]
         :return: SendChatMessageResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.SendChatMessageResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -791,15 +786,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("SendChatMessageResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -821,15 +816,14 @@
         :type chat_thread_id: str
         :param max_page_size: The maximum number of messages to be returned per page. Default value is
          None.
         :type max_page_size: int
         :param start_time: The earliest point in time to get messages up to. The timestamp should be in
          RFC3339 format: ``yyyy-MM-ddTHH:mm:ssZ``. Default value is None.
         :type start_time: ~datetime.datetime
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatMessage or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.communication.chat.models.ChatMessage]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -910,15 +904,15 @@
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     @distributed_trace
@@ -927,15 +921,14 @@
 
         Gets a message by id.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ChatMessage or the result of cls(response)
         :rtype: ~azure.communication.chat.models.ChatMessage
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -978,15 +971,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("ChatMessage", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -1011,73 +1004,67 @@
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
         :param update_chat_message_request: Details of the request to update the message. Required.
         :type update_chat_message_request: ~azure.communication.chat.models.UpdateChatMessageRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update_chat_message(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
         chat_message_id: str,
-        update_chat_message_request: IO,
+        update_chat_message_request: IO[bytes],
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> None:
         """Updates a message.
 
         Updates a message.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
         :param update_chat_message_request: Details of the request to update the message. Required.
-        :type update_chat_message_request: IO
+        :type update_chat_message_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update_chat_message(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
         chat_message_id: str,
-        update_chat_message_request: Union[_models.UpdateChatMessageRequest, IO],
+        update_chat_message_request: Union[_models.UpdateChatMessageRequest, IO[bytes]],
         **kwargs: Any
     ) -> None:
         """Updates a message.
 
         Updates a message.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
         :param update_chat_message_request: Details of the request to update the message. Is either a
-         UpdateChatMessageRequest type or a IO type. Required.
+         UpdateChatMessageRequest type or a IO[bytes] type. Required.
         :type update_chat_message_request: ~azure.communication.chat.models.UpdateChatMessageRequest or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are:
-         'application/merge-patch+json'. Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1132,15 +1119,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def delete_chat_message(  # pylint: disable=inconsistent-return-statements
@@ -1150,15 +1137,14 @@
 
         Deletes a message.
 
         :param chat_thread_id: The thread id to which the message was sent. Required.
         :type chat_thread_id: str
         :param chat_message_id: The message id. Required.
         :type chat_message_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1201,15 +1187,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def list_chat_participants(
@@ -1222,15 +1208,14 @@
         :param chat_thread_id: Thread id to get participants for. Required.
         :type chat_thread_id: str
         :param max_page_size: The maximum number of participants to be returned per page. Default value
          is None.
         :type max_page_size: int
         :param skip: Skips participants up to a specified position in response. Default value is None.
         :type skip: int
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ChatParticipant or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.communication.chat.models.ChatParticipant]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -1311,15 +1296,15 @@
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
-                map_error(status_code=response.status_code, response=response, error_map=error_map)
+                map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
                 raise HttpResponseError(response=response)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     @overload
@@ -1340,69 +1325,63 @@
         :param participant_communication_identifier: Id of the thread participant to remove from the
          thread. Required.
         :type participant_communication_identifier:
          ~azure.communication.chat.models.CommunicationIdentifierModel
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def remove_chat_participant(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        participant_communication_identifier: IO,
+        participant_communication_identifier: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Remove a participant from a thread.
 
         Remove a participant from a thread.
 
         :param chat_thread_id: Thread id to remove the participant from. Required.
         :type chat_thread_id: str
         :param participant_communication_identifier: Id of the thread participant to remove from the
          thread. Required.
-        :type participant_communication_identifier: IO
+        :type participant_communication_identifier: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Known values are: 'application/json', 'application/merge-patch+json'. Default value is
          "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def remove_chat_participant(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        participant_communication_identifier: Union[_models.CommunicationIdentifierModel, IO],
+        participant_communication_identifier: Union[_models.CommunicationIdentifierModel, IO[bytes]],
         **kwargs: Any
     ) -> None:
         """Remove a participant from a thread.
 
         Remove a participant from a thread.
 
         :param chat_thread_id: Thread id to remove the participant from. Required.
         :type chat_thread_id: str
         :param participant_communication_identifier: Id of the thread participant to remove from the
-         thread. Is either a CommunicationIdentifierModel type or a IO type. Required.
+         thread. Is either a CommunicationIdentifierModel type or a IO[bytes] type. Required.
         :type participant_communication_identifier:
-         ~azure.communication.chat.models.CommunicationIdentifierModel or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json',
-         'application/merge-patch+json'. Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.communication.chat.models.CommunicationIdentifierModel or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1456,15 +1435,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @overload
     def add_chat_participants(
@@ -1483,67 +1462,61 @@
         :type chat_thread_id: str
         :param add_chat_participants_request: Thread participants to be added to the thread. Required.
         :type add_chat_participants_request:
          ~azure.communication.chat.models.AddChatParticipantsRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AddChatParticipantsResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.AddChatParticipantsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def add_chat_participants(
         self,
         chat_thread_id: str,
-        add_chat_participants_request: IO,
+        add_chat_participants_request: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.AddChatParticipantsResult:
         """Adds thread participants to a thread. If participants already exist, no change occurs.
 
         Adds thread participants to a thread. If participants already exist, no change occurs.
 
         :param chat_thread_id: Id of the thread to add participants to. Required.
         :type chat_thread_id: str
         :param add_chat_participants_request: Thread participants to be added to the thread. Required.
-        :type add_chat_participants_request: IO
+        :type add_chat_participants_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: AddChatParticipantsResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.AddChatParticipantsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def add_chat_participants(
         self,
         chat_thread_id: str,
-        add_chat_participants_request: Union[_models.AddChatParticipantsRequest, IO],
+        add_chat_participants_request: Union[_models.AddChatParticipantsRequest, IO[bytes]],
         **kwargs: Any
     ) -> _models.AddChatParticipantsResult:
         """Adds thread participants to a thread. If participants already exist, no change occurs.
 
         Adds thread participants to a thread. If participants already exist, no change occurs.
 
         :param chat_thread_id: Id of the thread to add participants to. Required.
         :type chat_thread_id: str
         :param add_chat_participants_request: Thread participants to be added to the thread. Is either
-         a AddChatParticipantsRequest type or a IO type. Required.
+         a AddChatParticipantsRequest type or a IO[bytes] type. Required.
         :type add_chat_participants_request:
-         ~azure.communication.chat.models.AddChatParticipantsRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.communication.chat.models.AddChatParticipantsRequest or IO[bytes]
         :return: AddChatParticipantsResult or the result of cls(response)
         :rtype: ~azure.communication.chat.models.AddChatParticipantsResult
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1597,15 +1570,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [201]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("AddChatParticipantsResult", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -1627,64 +1600,61 @@
         :param chat_thread_id: The id of the thread to update. Required.
         :type chat_thread_id: str
         :param update_chat_thread_request: Request payload for updating a chat thread. Required.
         :type update_chat_thread_request: ~azure.communication.chat.models.UpdateChatThreadRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update_chat_thread_properties(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        update_chat_thread_request: IO,
+        update_chat_thread_request: IO[bytes],
         *,
         content_type: str = "application/merge-patch+json",
         **kwargs: Any
     ) -> None:
         """Updates a thread's properties.
 
         Updates a thread's properties.
 
         :param chat_thread_id: The id of the thread to update. Required.
         :type chat_thread_id: str
         :param update_chat_thread_request: Request payload for updating a chat thread. Required.
-        :type update_chat_thread_request: IO
+        :type update_chat_thread_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/merge-patch+json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update_chat_thread_properties(  # pylint: disable=inconsistent-return-statements
-        self, chat_thread_id: str, update_chat_thread_request: Union[_models.UpdateChatThreadRequest, IO], **kwargs: Any
+        self,
+        chat_thread_id: str,
+        update_chat_thread_request: Union[_models.UpdateChatThreadRequest, IO[bytes]],
+        **kwargs: Any
     ) -> None:
         """Updates a thread's properties.
 
         Updates a thread's properties.
 
         :param chat_thread_id: The id of the thread to update. Required.
         :type chat_thread_id: str
         :param update_chat_thread_request: Request payload for updating a chat thread. Is either a
-         UpdateChatThreadRequest type or a IO type. Required.
+         UpdateChatThreadRequest type or a IO[bytes] type. Required.
         :type update_chat_thread_request: ~azure.communication.chat.models.UpdateChatThreadRequest or
-         IO
-        :keyword content_type: Body Parameter content-type. Known values are:
-         'application/merge-patch+json'. Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1738,29 +1708,28 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [204]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
 
     @distributed_trace
     def get_chat_thread_properties(self, chat_thread_id: str, **kwargs: Any) -> _models.ChatThreadProperties:
         """Gets a chat thread's properties.
 
         Gets a chat thread's properties.
 
         :param chat_thread_id: Id of the thread. Required.
         :type chat_thread_id: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ChatThreadProperties or the result of cls(response)
         :rtype: ~azure.communication.chat.models.ChatThreadProperties
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1802,15 +1771,15 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         deserialized = self._deserialize("ChatThreadProperties", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
@@ -1834,68 +1803,62 @@
         :param send_typing_notification_request: Details of the typing notification request. Default
          value is None.
         :type send_typing_notification_request:
          ~azure.communication.chat.models.SendTypingNotificationRequest
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def send_typing_notification(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        send_typing_notification_request: Optional[IO] = None,
+        send_typing_notification_request: Optional[IO[bytes]] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> None:
         """Posts a typing event to a thread, on behalf of a user.
 
         Posts a typing event to a thread, on behalf of a user.
 
         :param chat_thread_id: Id of the thread. Required.
         :type chat_thread_id: str
         :param send_typing_notification_request: Details of the typing notification request. Default
          value is None.
-        :type send_typing_notification_request: IO
+        :type send_typing_notification_request: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def send_typing_notification(  # pylint: disable=inconsistent-return-statements
         self,
         chat_thread_id: str,
-        send_typing_notification_request: Optional[Union[_models.SendTypingNotificationRequest, IO]] = None,
+        send_typing_notification_request: Optional[Union[_models.SendTypingNotificationRequest, IO[bytes]]] = None,
         **kwargs: Any
     ) -> None:
         """Posts a typing event to a thread, on behalf of a user.
 
         Posts a typing event to a thread, on behalf of a user.
 
         :param chat_thread_id: Id of the thread. Required.
         :type chat_thread_id: str
         :param send_typing_notification_request: Details of the typing notification request. Is either
-         a SendTypingNotificationRequest type or a IO type. Default value is None.
+         a SendTypingNotificationRequest type or a IO[bytes] type. Default value is None.
         :type send_typing_notification_request:
-         ~azure.communication.chat.models.SendTypingNotificationRequest or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ~azure.communication.chat.models.SendTypingNotificationRequest or IO[bytes]
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             404: ResourceNotFoundError,
             409: ResourceExistsError,
@@ -1952,12 +1915,12 @@
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
-            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            map_error(status_code=response.status_code, response=response, error_map=error_map)  # type: ignore
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})  # type: ignore
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_generated/operations/_patch.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_models.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 class ChatAttachment:
     """An attachment in a chat message.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: Id of the attachment. Required.
     :vartype id: str
-    :ivar attachment_type: The type of attachment. Required. Known values are: "image".
+    :ivar attachment_type: The type of attachment. Required. Known values are: "image" and "file".
     :vartype attachment_type: str or ~azure.communication.chat.models.ChatAttachmentType
     :ivar name: The name of the attachment content.
     :vartype name: str or None
     :ivar url: The URL where the attachment can be downloaded.
     :vartype url: str or None
     :ivar preview_url: The URL where the preview of attachment can be downloaded.
     :vartype preview_url: str or None
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_shared/auth_policy_utils.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_shared/auth_policy_utils.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_shared/models.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_shared/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,323 +1,335 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 from enum import Enum
-from typing import Mapping, Optional, Union, Any
 import warnings
-from typing_extensions import TypedDict, Protocol
+from typing import Mapping, Optional, Union, Any, cast
+from typing_extensions import Literal, TypedDict, Protocol, runtime_checkable
+
 from azure.core import CaseInsensitiveEnumMeta
 
 
 class DeprecatedEnumMeta(CaseInsensitiveEnumMeta):
 
     def __getattribute__(cls, item):
         if item.upper() == "MICROSOFT_BOT":
-            warnings.warn("MICROSOFT_BOT is deprecated and should not be used.", DeprecationWarning)
-        return CaseInsensitiveEnumMeta.__getattribute__(cls, item)
+            warnings.warn("MICROSOFT_BOT is deprecated and has been replaced by \
+                          MICROSOFT_TEAMS_APP identifier.", DeprecationWarning)
+            item = "MICROSOFT_TEAMS_APP"
+        return super().__getattribute__(item)
 
 
-# The Chat SDK is diverging to not use the DeprecatedEnumMeta until the new
-# replacement for the BotIdentifier is released to prevent exposing the deprecated
-# enum value.
-class CommunicationIdentifierKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+class CommunicationIdentifierKind(str, Enum, metaclass=DeprecatedEnumMeta):
     """Communication Identifier Kind.
 
     For checking yet unknown identifiers it is better to rely on the presence of the `raw_id` property,
     as new or existing distinct type identifiers always contain the `raw_id` property.
     It is not advisable to rely on the `kind` property with a value `unknown`,
     as it could become a new or existing distinct type in the future.
     """
 
     UNKNOWN = "unknown"
     COMMUNICATION_USER = "communication_user"
     PHONE_NUMBER = "phone_number"
     MICROSOFT_TEAMS_USER = "microsoft_teams_user"
+    MICROSOFT_TEAMS_APP = "microsoft_teams_app"
 
 
 class CommunicationCloudEnvironment(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The cloud environment that the identifier belongs to"""
 
     PUBLIC = "PUBLIC"
     DOD = "DOD"
     GCCH = "GCCH"
 
 
+@runtime_checkable
 class CommunicationIdentifier(Protocol):
-    """Communication Identifier.
-
-    :ivar str raw_id: Optional raw ID of the identifier.
-    :ivar kind: The type of identifier.
-    :vartype kind: str or CommunicationIdentifierKind
-    :ivar Mapping[str, Any] properties: The properties of the identifier.
-    """
-
-    raw_id = None  # type: Optional[str]
-    kind = None  # type: Optional[Union[CommunicationIdentifierKind, str]]
-    properties = {}  # type: Mapping[str, Any]
+    """Communication Identifier."""
+    @property
+    def raw_id(self) -> str:
+        """The raw ID of the identifier."""
+        ...
+    @property
+    def kind(self) -> CommunicationIdentifierKind:
+        """The type of identifier."""
+        ...
+    @property
+    def properties(self) -> Mapping[str, Any]:
+        """The properties of the identifier."""
+        ...
 
 
-CommunicationUserProperties = TypedDict("CommunicationUserProperties", {"id": str})
-
 PHONE_NUMBER_PREFIX = "4:"
 BOT_PREFIX = "28:"
 BOT_PUBLIC_CLOUD_PREFIX = "28:orgid:"
 BOT_DOD_CLOUD_PREFIX = "28:dod:"
 BOT_DOD_CLOUD_GLOBAL_PREFIX = "28:dod-global:"
 BOT_GCCH_CLOUD_PREFIX = "28:gcch:"
 BOT_GCCH_CLOUD_GLOBAL_PREFIX = "28:gcch-global:"
+TEAMS_APP_PUBLIC_CLOUD_PREFIX = "28:orgid:"
+TEAMS_APP_DOD_CLOUD_PREFIX = "28:dod:"
+TEAMS_APP_GCCH_CLOUD_PREFIX = "28:gcch:"
 TEAMS_USER_ANONYMOUS_PREFIX = "8:teamsvisitor:"
 TEAMS_USER_PUBLIC_CLOUD_PREFIX = "8:orgid:"
 TEAMS_USER_DOD_CLOUD_PREFIX = "8:dod:"
 TEAMS_USER_GCCH_CLOUD_PREFIX = "8:gcch:"
 ACS_USER_PREFIX = "8:acs:"
 ACS_USER_DOD_CLOUD_PREFIX = "8:dod-acs:"
 ACS_USER_GCCH_CLOUD_PREFIX = "8:gcch-acs:"
 SPOOL_USER_PREFIX = "8:spool:"
 
 
-class CommunicationUserIdentifier:
-    """Represents a user in Azure Communication Service.
-
-    :ivar str raw_id: Optional raw ID of the identifier.
-    :ivar kind: The type of identifier.
-    :vartype kind: str or CommunicationIdentifierKind
-    :ivar Mapping[str, Any] properties: The properties of the identifier.
-     The keys in this mapping include:
-        - `id`(str): ID of the Communication user as returned from Azure Communication Identity.
+class CommunicationUserProperties(TypedDict):
+    """Dictionary of properties for a CommunicationUserIdentifier."""
+    id: str
+    """ID of the Communication user as returned from Azure Communication Identity."""
 
-    :param str id: ID of the Communication user as returned from Azure Communication Identity.
-    """
 
-    kind = CommunicationIdentifierKind.COMMUNICATION_USER
+class CommunicationUserIdentifier:
+    """Represents a user in Azure Communication Service."""
+    kind: Literal[CommunicationIdentifierKind.COMMUNICATION_USER] = CommunicationIdentifierKind.COMMUNICATION_USER
+    """The type of identifier."""
+    properties: CommunicationUserProperties
+    """The properties of the identifier."""
+    raw_id: str
+    """The raw ID of the identifier."""
 
     def __init__(self, id: str, **kwargs: Any) -> None:
-        self.raw_id = kwargs.get("raw_id", id)
+        """
+        :param str id: ID of the Communication user as returned from Azure Communication Identity.
+        :keyword str raw_id: The raw ID of the identifier. If not specified, the 'id' value will be used.
+        """
         self.properties = CommunicationUserProperties(id=id)
-        if self.raw_id is None:
-            self.raw_id = _communication_user_raw_id(self)
+        raw_id: Optional[str] = kwargs.get("raw_id")
+        self.raw_id = raw_id if raw_id is not None else id
 
     def __eq__(self, other):
         try:
+            if other.raw_id:
+                return self.raw_id == other.raw_id
             return self.raw_id == other.properties["id"]
         except Exception:  # pylint: disable=broad-except
             return False
 
 
-def _communication_user_raw_id(identifier: CommunicationUserIdentifier) -> str:
-    if identifier.raw_id:
-        return str(identifier.raw_id)
-    return str(identifier.properties["id"])
-
-
-PhoneNumberProperties = TypedDict("PhoneNumberProperties", {"value": str})
+class PhoneNumberProperties(TypedDict):
+    """Dictionary of properties for a PhoneNumberIdentifier."""
+    value: str
+    """The phone number in E.164 format."""
 
 
 class PhoneNumberIdentifier:
-    """Represents a phone number.
-
-    :ivar str raw_id: Optional raw ID of the identifier.
-    :ivar kind: The type of identifier.
-    :vartype kind: str or CommunicationIdentifierKind
-    :ivar Mapping properties: The properties of the identifier.
-     The keys in this mapping include:
-        - `value`(str): The phone number in E.164 format.
-
-    :param str value: The phone number.
-    """
-
-    kind = CommunicationIdentifierKind.PHONE_NUMBER
+    """Represents a phone number."""
+    kind: Literal[CommunicationIdentifierKind.PHONE_NUMBER] = CommunicationIdentifierKind.PHONE_NUMBER
+    """The type of identifier."""
+    properties: PhoneNumberProperties
+    """The properties of the identifier."""
+    raw_id: str
+    """The raw ID of the identifier."""
 
     def __init__(self, value: str, **kwargs: Any) -> None:
-        self.raw_id = kwargs.get("raw_id")
+        """
+        :param str value: The phone number.
+        :keyword str raw_id: The raw ID of the identifier. If not specified, this will be constructed from
+          the 'value' parameter.
+        """
         self.properties = PhoneNumberProperties(value=value)
-        if self.raw_id is None:
-            self.raw_id = _phone_number_raw_id(self)
+        raw_id: Optional[str] = kwargs.get("raw_id")
+        self.raw_id = raw_id if raw_id is not None else self._format_raw_id(self.properties)
 
     def __eq__(self, other):
         try:
-            return self.raw_id == _phone_number_raw_id(other)
-        except Exception:  # pylint: disable=broad-except
+            if other.raw_id:
+                return self.raw_id == other.raw_id
+            return self.raw_id == self._format_raw_id(other.properties)
+        except Exception:  # pylint:disable=broad-except
             return False
 
-
-def _phone_number_raw_id(identifier: PhoneNumberIdentifier) -> str:
-    if identifier.raw_id:
-        return str(identifier.raw_id)
-    value = identifier.properties["value"]
-    # We just assume correct E.164 format here because
-    # validation should only happen server-side, not client-side.
-    return f"{PHONE_NUMBER_PREFIX}{value}"
+    def _format_raw_id(self, properties: PhoneNumberProperties) -> str:
+        # We just assume correct E.164 format here because
+        # validation should only happen server-side, not client-side.
+        value = properties["value"]
+        return f"{PHONE_NUMBER_PREFIX}{value}"
 
 
 class UnknownIdentifier:
     """Represents an identifier of an unknown type.
 
     It will be encountered in communications with endpoints that are not
     identifiable by this version of the SDK.
 
     For checking yet unknown identifiers it is better to rely on the presence of the `raw_id` property,
     as new or existing distinct type identifiers always contain the `raw_id` property.
     It is not advisable to rely on the `kind` property with a value `unknown`,
     as it could become a new or existing distinct type in the future.
-
-    :ivar str raw_id: Optional raw ID of the identifier.
-    :ivar kind: The type of identifier.
-    :vartype kind: str or CommunicationIdentifierKind
-    :ivar Mapping properties: The properties of the identifier.
-    :param str identifier: The ID of the identifier.
     """
-
-    kind = CommunicationIdentifierKind.UNKNOWN
+    kind: Literal[CommunicationIdentifierKind.UNKNOWN] = CommunicationIdentifierKind.UNKNOWN
+    """The type of identifier."""
+    properties: Mapping[str, Any]
+    """The properties of the identifier."""
+    raw_id: str
+    """The raw ID of the identifier."""
 
     def __init__(self, identifier: str) -> None:
+        """
+        :param str identifier: The ID of the identifier.
+        """
         self.raw_id = identifier
-        self.properties = {}  # type: Any
+        self.properties = {}
 
     def __eq__(self, other):
         try:
             return self.raw_id == other.raw_id
-        except Exception:  # pylint: disable=broad-except
+        except AttributeError:
             return False
 
 
-MicrosoftTeamsUserProperties = TypedDict(
-    "MicrosoftTeamsUserProperties",
-    {
-        "user_id": str,
-        "is_anonymous": bool,
-        "cloud": Union[CommunicationCloudEnvironment, str],
-    },
-)
+class MicrosoftTeamsUserProperties(TypedDict):
+    """Dictionary of properties for a MicrosoftTeamsUserIdentifier."""
+    user_id: str
+    """The id of the Microsoft Teams user. If the user isn't anonymous, the id is the AAD object id of the user."""
+    is_anonymous: bool
+    """Set this to true if the user is anonymous for example when joining a meeting with a share link."""
+    cloud: Union[CommunicationCloudEnvironment, str]
+    """Cloud environment that this identifier belongs to."""
 
 
 class MicrosoftTeamsUserIdentifier:
-    """Represents an identifier for a Microsoft Teams user.
-
-    :ivar str raw_id: Optional raw ID of the identifier.
-    :ivar kind: The type of identifier.
-    :vartype kind: str or CommunicationIdentifierKind
-    :ivar Mapping properties: The properties of the identifier.
-     The keys in this mapping include:
-        - `user_id`(str): The id of the Microsoft Teams user. If the user isn't anonymous,
-          the id is the AAD object id of the user.
-        - `is_anonymous` (bool): Set this to true if the user is anonymous for example when joining
-          a meeting with a share link.
-        - `cloud` (str): Cloud environment that this identifier belongs to.
-
-    :param str user_id: Microsoft Teams user id.
-    :keyword bool is_anonymous: `True` if the identifier is anonymous. Default value is `False`.
-    :keyword cloud: Cloud environment that the user belongs to. Default value is `PUBLIC`.
-    :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
-    """
-
-    kind = CommunicationIdentifierKind.MICROSOFT_TEAMS_USER
+    """Represents an identifier for a Microsoft Teams user."""
+    kind: Literal[CommunicationIdentifierKind.MICROSOFT_TEAMS_USER] = CommunicationIdentifierKind.MICROSOFT_TEAMS_USER
+    """The type of identifier."""
+    properties: MicrosoftTeamsUserProperties
+    """The properties of the identifier."""
+    raw_id: str
+    """The raw ID of the identifier."""
 
     def __init__(self, user_id: str, **kwargs: Any) -> None:
-        self.raw_id = kwargs.get("raw_id")
+        """
+        :param str user_id: Microsoft Teams user id.
+        :keyword bool is_anonymous: `True` if the identifier is anonymous. Default value is `False`.
+        :keyword cloud: Cloud environment that the user belongs to. Default value is `PUBLIC`.
+        :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
+        :keyword str raw_id: The raw ID of the identifier. If not specified, this value will be constructed from
+         the other properties.
+        """
         self.properties = MicrosoftTeamsUserProperties(
             user_id=user_id,
             is_anonymous=kwargs.get("is_anonymous", False),
             cloud=kwargs.get("cloud") or CommunicationCloudEnvironment.PUBLIC,
         )
-        if self.raw_id is None:
-            self.raw_id = _microsoft_teams_user_raw_id(self)
+        raw_id: Optional[str] = kwargs.get("raw_id")
+        self.raw_id = raw_id if raw_id is not None else self._format_raw_id(self.properties)
 
     def __eq__(self, other):
         try:
-            return self.raw_id == _microsoft_teams_user_raw_id(other)
+            if other.raw_id:
+                return self.raw_id == other.raw_id
+            return self.raw_id == self._format_raw_id(other.properties)
         except Exception:  # pylint: disable=broad-except
             return False
 
-
-def _microsoft_teams_user_raw_id(identifier: MicrosoftTeamsUserIdentifier) -> str:
-    if identifier.raw_id:
-        return str(identifier.raw_id)
-    user_id = identifier.properties["user_id"]
-    if identifier.properties["is_anonymous"]:
-        return f"{TEAMS_USER_ANONYMOUS_PREFIX}{user_id}"
-    cloud = identifier.properties["cloud"]
-    if cloud == CommunicationCloudEnvironment.DOD:
-        return f"{TEAMS_USER_DOD_CLOUD_PREFIX}{user_id}"
-    if cloud == CommunicationCloudEnvironment.GCCH:
-        return f"{TEAMS_USER_GCCH_CLOUD_PREFIX}{user_id}"
-    if cloud == CommunicationCloudEnvironment.PUBLIC:
+    def _format_raw_id(self, properties: MicrosoftTeamsUserProperties) -> str:
+        user_id = properties["user_id"]
+        if properties["is_anonymous"]:
+            return f"{TEAMS_USER_ANONYMOUS_PREFIX}{user_id}"
+        cloud = properties["cloud"]
+        if cloud == CommunicationCloudEnvironment.DOD:
+            return f"{TEAMS_USER_DOD_CLOUD_PREFIX}{user_id}"
+        if cloud == CommunicationCloudEnvironment.GCCH:
+            return f"{TEAMS_USER_GCCH_CLOUD_PREFIX}{user_id}"
+        if cloud == CommunicationCloudEnvironment.PUBLIC:
+            return f"{TEAMS_USER_PUBLIC_CLOUD_PREFIX}{user_id}"
         return f"{TEAMS_USER_PUBLIC_CLOUD_PREFIX}{user_id}"
-    return f"{TEAMS_USER_PUBLIC_CLOUD_PREFIX}{user_id}"
 
 
-# _MicrosoftBotProperties = TypedDict(
-#     "MicrosoftBotProperties",
-#     {
-#         "bot_id": str,
-#         "is_resource_account_configured": bool,
-#         "cloud": Union[CommunicationCloudEnvironment, str],
-#     },
-# )
-
-
-# class _MicrosoftBotIdentifier:
-#     """Represents an identifier for a Microsoft bot.
-
-#     :ivar str raw_id: Optional raw ID of the identifier.
-#     :ivar kind: The type of identifier.
-#     :vartype kind: str or CommunicationIdentifierKind
-#     :ivar MicrosoftBotProperties: The properties of the identifier.
-#      The keys in this mapping include:
-#         - `bot_id`(str): The id of the Microsoft bot.
-#         - `is_resource_account_configured` (bool): Set this to false if the bot is global.
-#         The default is `true` for tennantized bots.
-#         - `cloud` (str): Cloud environment that this identifier belongs to.
-
-#     :param str bot_id: Microsoft bot id.
-#     :keyword bool is_resource_account_configured: `False` if the identifier is global.
-#     Default value is `True` for tennantzed bots.
-#     :keyword cloud: Cloud environment that the bot belongs to. Default value is `PUBLIC`.
-#     :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
-#     """
-
-#     kind = CommunicationIdentifierKind.MICROSOFT_BOT
-
-#     def __init__(self, bot_id: str, **kwargs: Any) -> None:
-#         self.raw_id = kwargs.get("raw_id")
-#         self.properties = _MicrosoftBotProperties(
-#             bot_id=bot_id,
-#             is_resource_account_configured=kwargs.get(
-#                 "is_resource_account_configured", True
-#             ),
-#             cloud=kwargs.get("cloud") or CommunicationCloudEnvironment.PUBLIC,
-#         )
-#         if self.raw_id is None:
-#             self.raw_id = _microsoft_bot_raw_id(self)
-
-#     def __eq__(self, other):
-#         try:
-#             return self.raw_id == _microsoft_bot_raw_id(other)
-#         except Exception:  # pylint: disable=broad-except
-#             return False
-
-
-# def _microsoft_bot_raw_id(identifier: _MicrosoftBotIdentifier) -> str:  # pylint: disable=too-many-return-statements
-#     if identifier.raw_id:
-#         return str(identifier.raw_id)
-#     bot_id = identifier.properties["bot_id"]
-#     cloud = identifier.properties["cloud"]
-#     if identifier.properties["is_resource_account_configured"] is False:
-#         if cloud == CommunicationCloudEnvironment.DOD:
-#             return f"{BOT_DOD_CLOUD_GLOBAL_PREFIX}{bot_id}"
-#         if cloud == CommunicationCloudEnvironment.GCCH:
-#             return f"{BOT_GCCH_CLOUD_GLOBAL_PREFIX}{bot_id}"
-#         return f"{BOT_PREFIX}{bot_id}"
-
-#     if cloud == CommunicationCloudEnvironment.DOD:
-#         return f"{BOT_DOD_CLOUD_PREFIX}{bot_id}"
-#     if cloud == CommunicationCloudEnvironment.GCCH:
-#         return f"{BOT_GCCH_CLOUD_PREFIX}{bot_id}"
-#     return f"{BOT_PUBLIC_CLOUD_PREFIX}{bot_id}"
+class MicrosoftTeamsAppProperties(TypedDict):
+    """Dictionary of properties for a MicrosoftTeamsAppIdentifier."""
+    app_id: str
+    """The id of the Microsoft Teams application."""
+    cloud: Union[CommunicationCloudEnvironment, str]
+    """Cloud environment that this identifier belongs to."""
+
+
+class _botbackcompatdict(dict):
+    """Backwards compatible properties."""
+    def __getitem__(self, __key: Any) -> Any:
+        try:
+            return super().__getitem__(__key)
+        except KeyError:
+            if __key == "bot_id":
+                return super().__getitem__("app_id")
+            if __key == "is_resource_account_configured":
+                return True
+            raise
+
+
+class MicrosoftTeamsAppIdentifier:
+    """Represents an identifier for a Microsoft Teams application."""
+    kind: Literal[CommunicationIdentifierKind.MICROSOFT_TEAMS_APP] = CommunicationIdentifierKind.MICROSOFT_TEAMS_APP
+    """The type of identifier."""
+    properties: MicrosoftTeamsAppProperties
+    """The properties of the identifier."""
+    raw_id: str
+    """The raw ID of the identifier."""
+
+    def __init__(self, app_id: str, **kwargs: Any) -> None:
+        """
+        :param str app_id: Microsoft Teams application id.
+        :keyword cloud: Cloud environment that the application belongs to. Default value is `PUBLIC`.
+        :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
+        :keyword str raw_id: The raw ID of the identifier. If not specified, this value will be constructed
+         from the other properties.
+        """
+        self.properties = cast(MicrosoftTeamsAppProperties, _botbackcompatdict(
+            app_id=app_id,
+            cloud=kwargs.get("cloud") or CommunicationCloudEnvironment.PUBLIC,
+        ))
+        raw_id: Optional[str] = kwargs.get("raw_id")
+        self.raw_id = raw_id if raw_id is not None else self._format_raw_id(self.properties)
+
+    def __eq__(self, other):
+        try:
+            if other.raw_id:
+                return self.raw_id == other.raw_id
+            return self.raw_id == self._format_raw_id(other.properties)
+        except Exception:  # pylint: disable=broad-except
+            return False
+
+    def _format_raw_id(self, properties: MicrosoftTeamsAppProperties) -> str:
+        app_id = properties["app_id"]
+        cloud = properties["cloud"]
+        if cloud == CommunicationCloudEnvironment.DOD:
+            return f"{TEAMS_APP_DOD_CLOUD_PREFIX}{app_id}"
+        if cloud == CommunicationCloudEnvironment.GCCH:
+            return f"{TEAMS_APP_GCCH_CLOUD_PREFIX}{app_id}"
+        return f"{TEAMS_APP_PUBLIC_CLOUD_PREFIX}{app_id}"
+
+
+class _MicrosoftBotIdentifier(MicrosoftTeamsAppIdentifier):
+    """Represents an identifier for a Microsoft bot.
+
+    DEPRECATED. Only used in cases of backwards compatibility.
+    """
+
+    def __init__(self, bot_id, **kwargs):
+        """
+        :param str bot_id: Microsoft bot id.
+        :keyword bool is_resource_account_configured: `False` if the identifier is global.
+         Default value is `True` for tennantzed bots.
+        :keyword cloud: Cloud environment that the bot belongs to. Default value is `PUBLIC`.
+        :paramtype cloud: str or ~azure.communication.chat.CommunicationCloudEnvironment
+        """
+        warnings.warn(
+            "The MicrosoftBotIdentifier is deprecated and has been replaced by MicrosoftTeamsAppIdentifier.",
+            DeprecationWarning
+        )
+        super().__init__(bot_id, **kwargs)
 
 
 def identifier_from_raw_id(raw_id: str) -> CommunicationIdentifier:  # pylint: disable=too-many-return-statements
     """
     Creates a CommunicationIdentifier from a given raw ID.
 
     When storing raw IDs use this function to restore the identifier that was encoded in the raw ID.
@@ -325,48 +337,66 @@
     :param str raw_id: A raw ID to construct the CommunicationIdentifier from.
     :return: The CommunicationIdentifier parsed from the raw_id.
     :rtype: CommunicationIdentifier
     """
     if raw_id.startswith(PHONE_NUMBER_PREFIX):
         return PhoneNumberIdentifier(
             value=raw_id[len(PHONE_NUMBER_PREFIX) :], raw_id=raw_id
-        )  # type: ignore
+        )
 
     segments = raw_id.split(":", maxsplit=2)
     if len(segments) < 3:
-        return UnknownIdentifier(identifier=raw_id)  # type: ignore
+        return UnknownIdentifier(identifier=raw_id)
 
     prefix = f"{segments[0]}:{segments[1]}:"
     suffix = segments[2]
     if prefix == TEAMS_USER_ANONYMOUS_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix, is_anonymous=True, raw_id=raw_id
-        )  # type: ignore
+        )
     if prefix == TEAMS_USER_PUBLIC_CLOUD_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix,
             is_anonymous=False,
             cloud=CommunicationCloudEnvironment.PUBLIC,
             raw_id=raw_id,
-        )  # type: ignore
+        )
     if prefix == TEAMS_USER_DOD_CLOUD_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix,
             is_anonymous=False,
             cloud=CommunicationCloudEnvironment.DOD,
             raw_id=raw_id,
-        )  # type: ignore
+        )
     if prefix == TEAMS_USER_GCCH_CLOUD_PREFIX:
         return MicrosoftTeamsUserIdentifier(
             user_id=suffix,
             is_anonymous=False,
             cloud=CommunicationCloudEnvironment.GCCH,
             raw_id=raw_id,
-        )  # type: ignore
+        )
+    if prefix == TEAMS_APP_PUBLIC_CLOUD_PREFIX:
+        return MicrosoftTeamsAppIdentifier(
+            app_id=suffix,
+            cloud=CommunicationCloudEnvironment.PUBLIC,
+            raw_id=raw_id,
+        )
+    if prefix == TEAMS_APP_DOD_CLOUD_PREFIX:
+        return MicrosoftTeamsAppIdentifier(
+            app_id=suffix,
+            cloud=CommunicationCloudEnvironment.DOD,
+            raw_id=raw_id,
+        )
+    if prefix == TEAMS_APP_GCCH_CLOUD_PREFIX:
+        return MicrosoftTeamsAppIdentifier(
+            app_id=suffix,
+            cloud=CommunicationCloudEnvironment.GCCH,
+            raw_id=raw_id,
+        )
     if prefix in [
         ACS_USER_PREFIX,
         ACS_USER_DOD_CLOUD_PREFIX,
         ACS_USER_GCCH_CLOUD_PREFIX,
         SPOOL_USER_PREFIX,
     ]:
-        return CommunicationUserIdentifier(id=raw_id, raw_id=raw_id)  # type: ignore
-    return UnknownIdentifier(identifier=raw_id)  # type: ignore
+        return CommunicationUserIdentifier(id=raw_id, raw_id=raw_id)
+    return UnknownIdentifier(identifier=raw_id)
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_shared/policy.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_shared/policy.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_shared/user_credential.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_shared/user_credential.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 
 from .utils import get_current_utc_as_int
 from .utils import create_access_token
 
 
 class CommunicationTokenCredential(object):
     """Credential type used for authenticating to an Azure Communication service.
+
     :param str token: The token used to authenticate to an Azure Communication service.
     :keyword token_refresher: The sync token refresher to provide capacity to fetch a fresh token.
-     The returned token must be valid (expiration date must be in the future).
+        The returned token must be valid (expiration date must be in the future).
     :paramtype token_refresher: Callable[[], AccessToken]
     :keyword bool proactive_refresh: Whether to refresh the token proactively or not.
-     If the proactive refreshing is enabled ('proactive_refresh' is true), the credential will use
-     a background thread to attempt to refresh the token within 10 minutes before the cached token expires,
-     the proactive refresh will request a new token by calling the 'token_refresher' callback.
-     When 'proactive_refresh' is enabled, the Credential object must be either run within a context manager
-     or the 'close' method must be called once the object usage has been finished.
+        If the proactive refreshing is enabled ('proactive_refresh' is true), the credential will use
+        a background thread to attempt to refresh the token within 10 minutes before the cached token expires,
+        the proactive refresh will request a new token by calling the 'token_refresher' callback.
+        When 'proactive_refresh' is enabled, the Credential object must be either run within a context manager
+        or the 'close' method must be called once the object usage has been finished.
     :raises: TypeError if paramater 'token' is not a string
     :raises: ValueError if the 'proactive_refresh' is enabled without providing the 'token_refresher' callable.
     """
 
     _ON_DEMAND_REFRESHING_INTERVAL_MINUTES = 2
     _DEFAULT_AUTOREFRESH_INTERVAL_MINUTES = 10
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_shared/user_credential_async.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_shared/user_credential_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 from .utils import get_current_utc_as_int
 from .utils import create_access_token
 from .utils_async import AsyncTimer
 
 
 class CommunicationTokenCredential(object):
     """Credential type used for authenticating to an Azure Communication service.
+
     :param str token: The token used to authenticate to an Azure Communication service.
     :keyword token_refresher: The async token refresher to provide capacity to fetch a fresh token.
-     The returned token must be valid (expiration date must be in the future).
+        The returned token must be valid (expiration date must be in the future).
     :paramtype token_refresher: Callable[[], Awaitable[AccessToken]]
     :keyword bool proactive_refresh: Whether to refresh the token proactively or not.
-     If the proactive refreshing is enabled ('proactive_refresh' is true), the credential will use
-     a background thread to attempt to refresh the token within 10 minutes before the cached token expires,
-     the proactive refresh will request a new token by calling the 'token_refresher' callback.
-     When 'proactive_refresh is enabled', the Credential object must be either run within a context manager
-     or the 'close' method must be called once the object usage has been finished.
+        If the proactive refreshing is enabled ('proactive_refresh' is true), the credential will use
+        a background thread to attempt to refresh the token within 10 minutes before the cached token expires,
+        the proactive refresh will request a new token by calling the 'token_refresher' callback.
+        When 'proactive_refresh is enabled', the Credential object must be either run within a context manager
+        or the 'close' method must be called once the object usage has been finished.
     :raises: TypeError if paramater 'token' is not a string
     :raises: ValueError if the 'proactive_refresh' is enabled without providing the 'token_refresher' function.
     """
 
     _ON_DEMAND_REFRESHING_INTERVAL_MINUTES = 2
     _DEFAULT_AUTOREFRESH_INTERVAL_MINUTES = 10
 
@@ -51,14 +52,15 @@
         self._lock = Condition(self._async_mutex)
         self._some_thread_refreshing = False
         self._is_closed = Event()
 
     async def get_token(self, *scopes, **kwargs):  # pylint: disable=unused-argument
         # type (*str, **Any) -> AccessToken
         """The value of the configured token.
+
         :param any scopes: Scopes to be added to the token.
         :return: AccessToken
         :rtype: ~azure.core.credentials.AccessToken
         """
         if self._proactive_refresh and self._is_closed.is_set():
             raise RuntimeError(
                 "An instance of CommunicationTokenCredential cannot be reused once it has been closed."
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_shared/utils.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_shared/utils.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_shared/utils_async.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_shared/utils_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/_utils.py` & `azure-communication-chat-1.3.0/azure/communication/chat/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/aio/_chat_client_async.py` & `azure-communication-chat-1.3.0/azure/communication/chat/aio/_chat_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,31 +125,31 @@
         """Creates a chat thread.
 
         :param topic: Required. The thread topic.
         :type topic: str
         :keyword thread_participants: Optional. Participants to be added to the thread.
         :paramtype thread_participants: List[~azure.communication.chat.ChatParticipant]
         :keyword idempotency_token: Optional. If specified, the client directs that the request is
-         repeatable; that is, the client can make the request multiple times with the same
-         Idempotency_Token and get back an appropriate response without the server executing the
-         request multiple times. The value of the Idempotency_Token is an opaque string
-         representing a client-generated, globally unique for all time, identifier for the request. If not
-         specified, a new unique id would be generated.
+            repeatable; that is, the client can make the request multiple times with the same
+            Idempotency_Token and get back an appropriate response without the server executing the
+            request multiple times. The value of the Idempotency_Token is an opaque string
+            representing a client-generated, globally unique for all time, identifier for the request. If not
+            specified, a new unique id would be generated.
         :paramtype idempotency_token: str
         :return: CreateChatThreadResult
         :rtype: ~azure.communication.chat.CreateChatThreadResult
         :raises: ~azure.core.exceptions.HttpResponseError, ValueError
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_client_sample_async.py
                 :start-after: [START create_thread]
                 :end-before: [END create_thread]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Creating a new chat thread.
         """
         if not topic:
             raise ValueError("topic cannot be None.")
 
         idempotency_token = kwargs.pop('idempotency_token', None)
         if idempotency_token is None:
@@ -201,15 +201,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_client_sample_async.py
                 :start-after: [START list_threads]
                 :end-before: [END list_threads]
                 :language: python
-                :dedent: 12
+                :dedent: 4
                 :caption: Listing chat threads.
         """
         results_per_page = kwargs.pop("results_per_page", None)
         start_time = kwargs.pop("start_time", None)
 
         return self._client.chat.list_chat_threads(
             max_page_size=results_per_page,
@@ -232,15 +232,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_client_sample_async.py
                 :start-after: [START delete_thread]
                 :end-before: [END delete_thread]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Deleting a chat thread.
         """
         if not thread_id:
             raise ValueError("thread_id cannot be None.")
 
         return await self._client.chat.delete_chat_thread(thread_id, **kwargs)
```

### Comparing `azure-communication-chat-1.2.0/azure/communication/chat/aio/_chat_thread_client_async.py` & `azure-communication-chat-1.3.0/azure/communication/chat/aio/_chat_thread_client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 
 class ChatThreadClient(object): # pylint: disable=client-accepts-api-version-keyword
     """A client to interact with the AzureCommunicationService Chat gateway.
     Instances of this class is normally retrieved by ChatClient.get_chat_thread_client()
 
     This client provides operations to add participant(s) to chat thread, remove participant from
-    chat thread, send message, delete message, update message, send typing notifications,
-    send and list read receipt
+        chat thread, send message, delete message, update message, send typing notifications,
+        send and list read receipt
 
     :ivar thread_id: Chat thread id.
     :vartype thread_id: str
 
     :param str endpoint:
         The endpoint of the Azure Communication resource.
     :param CommunicationTokenCredential credential:
@@ -124,15 +124,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START get_thread]
                 :end-before: [END get_thread]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Retrieving chat thread properties by chat thread id.
         """
 
         chat_thread = await self._client.chat_thread.get_chat_thread_properties(self._thread_id, **kwargs)
         return ChatThreadProperties._from_generated(chat_thread)  # pylint:disable=protected-access
 
 
@@ -153,15 +153,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START update_topic]
                 :end-before: [END update_topic]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Updating chat thread.
         """
 
         update_topic_request = UpdateChatThreadRequest(topic=topic)
         return await self._client.chat_thread.update_chat_thread_properties(
             chat_thread_id=self._thread_id,
             update_chat_thread_request=update_topic_request,
@@ -183,15 +183,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START send_read_receipt]
                 :end-before: [END send_read_receipt]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Sending read receipt of a chat message.
         """
         if not message_id:
             raise ValueError("message_id cannot be None.")
 
         post_read_receipt_request = SendReadReceiptRequest(chat_message_id=message_id)
         return await self._client.chat_thread.send_chat_read_receipt(
@@ -214,15 +214,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START list_read_receipts]
                 :end-before: [END list_read_receipts]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Listing read receipts.
         """
         results_per_page = kwargs.pop("results_per_page", None)
         skip = kwargs.pop("skip", None)
 
         return self._client.chat_thread.list_chat_read_receipts(
             self._thread_id,
@@ -248,15 +248,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START send_typing_notification]
                 :end-before: [END send_typing_notification]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Send typing notification.
         """
 
         send_typing_notification_request = SendTypingNotificationRequest(sender_display_name=sender_display_name)
 
         return await self._client.chat_thread.send_typing_notification(
             chat_thread_id=self._thread_id,
@@ -287,15 +287,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START send_message]
                 :end-before: [END send_message]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Sending a message.
         """
         if not content:
             raise ValueError("content cannot be None.")
 
         chat_message_type = kwargs.pop("chat_message_type", None)
         if chat_message_type is None:
@@ -342,15 +342,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START get_message]
                 :end-before: [END get_message]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Retrieving a message by message id.
         """
         if not message_id:
             raise ValueError("message_id cannot be None.")
 
         chat_message = await self._client.chat_thread.get_chat_message(self._thread_id, message_id, **kwargs)
         return ChatMessage._from_generated(chat_message)  # pylint:disable=protected-access
@@ -370,15 +370,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START list_messages]
                 :end-before: [END list_messages]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Listing messages of a chat thread.
         """
         results_per_page = kwargs.pop("results_per_page", None)
         start_time = kwargs.pop("start_time", None)
 
         return self._client.chat_thread.list_chat_messages(
             self._thread_id,
@@ -408,15 +408,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START update_message]
                 :end-before: [END update_message]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Updating an already sent message.
         """
         if not message_id:
             raise ValueError("message_id cannot be None.")
 
         update_message_request = UpdateChatMessageRequest(content=content, metadata=metadata)
 
@@ -442,15 +442,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START delete_message]
                 :end-before: [END delete_message]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Deleting a message.
         """
         if not message_id:
             raise ValueError("message_id cannot be None.")
 
         return await self._client.chat_thread.delete_chat_message(
             chat_thread_id=self._thread_id,
@@ -472,15 +472,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START list_participants]
                 :end-before: [END list_participants]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Listing participants of chat thread.
         """
 
         results_per_page = kwargs.pop("results_per_page", None)
         skip = kwargs.pop("skip", None)
 
         return self._client.chat_thread.list_chat_participants(
@@ -511,15 +511,15 @@
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/chat_thread_client_sample_async.py
                 :start-after: [START add_participants]
                 :end-before: [END add_participants]
                 :language: python
-                :dedent: 12
+                :dedent: 8
                 :caption: Adding participants to chat thread.
         """
         response = []
         if thread_participants:
             participants = [m._to_generated() for m in thread_participants]  # pylint:disable=protected-access
             add_thread_participants_request = AddChatParticipantsRequest(participants=participants)
```

### Comparing `azure-communication-chat-1.2.0/azure_communication_chat.egg-info/PKG-INFO` & `azure-communication-chat-1.3.0/azure_communication_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: azure-communication-chat
-Version: 1.2.0
+Version: 1.3.0
 Summary: Microsoft Azure Communication Chat Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-core<2.0.0,>=1.29.5
+Requires-Dist: isodate>=0.6.1
+Requires-Dist: azure-core>=1.29.5
 Requires-Dist: typing-extensions>=4.3.0
 
 # Azure Communication Chat Package client library for Python
 
 This package contains a Python SDK for Azure Communication Services for Chat.
 Read more about Azure Communication Services [here](https://docs.microsoft.com/azure/communication-services/overview)
```

### Comparing `azure-communication-chat-1.2.0/azure_communication_chat.egg-info/SOURCES.txt` & `azure-communication-chat-1.3.0/azure_communication_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/samples/chat_client_sample.py` & `azure-communication-chat-1.3.0/samples/chat_client_sample.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/samples/chat_client_sample_async.py` & `azure-communication-chat-1.3.0/samples/chat_client_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/samples/chat_thread_client_sample.py` & `azure-communication-chat-1.3.0/samples/chat_thread_client_sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,14 +175,23 @@
         start_time = datetime.utcnow() - timedelta(days=1)
         chat_messages = chat_thread_client.list_messages(results_per_page=1, start_time=start_time)
 
         print("list_messages succeeded with results_per_page is 1, and start time is yesterday UTC")
         for chat_message_page in chat_messages.by_page():
             for chat_message in chat_message_page:
                 print("ChatMessage: message=", chat_message.content.message)
+                for attachment in chat_message.content.attachments:
+                    if attachment.type == "image":
+                        print("image attachment: ", attachment.name, " with ID: ", attachment.id, "received.")
+                        # render `attachment.preview_url` as the thumbnail
+                        # render `attachment.url` as the full image
+                    elif attachment.type == "file":
+                        print("file attachment: ", attachment.name, " with ID: ", attachment.id, "received.")
+                        # render a button that will navigate user to the URL provided in `attachment.preview_url`
+
         # [END list_messages]
         print("list_messages succeeded")
 
     def update_message(self):
         thread_id = self._thread_id
         chat_client = self._chat_client
         message_id = self._message_id
```

### Comparing `azure-communication-chat-1.2.0/samples/chat_thread_client_sample_async.py` & `azure-communication-chat-1.3.0/samples/chat_thread_client_sample_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,14 +182,22 @@
             async with chat_thread_client:
                 start_time = datetime.utcnow() - timedelta(days=1)
                 chat_messages = chat_thread_client.list_messages(results_per_page=1, start_time=start_time)
                 print("list_messages succeeded with results_per_page is 1, and start time is yesterday UTC")
                 async for chat_message_page in chat_messages.by_page():
                     async for chat_message in chat_message_page:
                         print("ChatMessage: message=", chat_message.content.message)
+                        for attachment in chat_message.content.attachments:
+                            if attachment.type == "image":
+                                print("image attachment: ", attachment.name, " with ID: ", attachment.id, "received.")
+                                # render `attachment.preview_url` as the thumbnail
+                                # render `attachment.url` as the full image
+                            elif attachment.type == "file":
+                                print("file attachment: ", attachment.name, " with ID: ", attachment.id, "received.")
+                                # render a button that will navigate user to the URL provided in `attachment.preview_url`
         # [END list_messages]
         print("list_messages_async succeeded")
 
     async def update_message_async(self):
         thread_id = self._thread_id
         chat_client = self._chat_client
         message_id = self._message_id
```

### Comparing `azure-communication-chat-1.2.0/samples/user_credential_sample.py` & `azure-communication-chat-1.3.0/samples/user_credential_sample.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/samples/user_credential_sample_async.py` & `azure-communication-chat-1.3.0/samples/user_credential_sample_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/setup.py` & `azure-communication-chat-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,33 +40,32 @@
     url='https://github.com/Azure/azure-sdk-for-python',
     keywords="azure, azure sdk",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         'Programming Language :: Python',
         "Programming Language :: Python :: 3 :: Only",
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.communication'
     ]),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     include_package_data=True,
     package_data={
         'pytyped': ['py.typed'],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
-        "azure-core<2.0.0,>=1.29.5",
+        "isodate>=0.6.1",
+        "azure-core>=1.29.5",
         "typing-extensions>=4.3.0",
     ]
 )
```

### Comparing `azure-communication-chat-1.2.0/tests/_shared/async_fake_token_credential.py` & `azure-communication-chat-1.3.0/tests/_shared/async_fake_token_credential.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/_shared/fake_token_credential.py` & `azure-communication-chat-1.3.0/tests/_shared/fake_token_credential.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/_shared/helper.py` & `azure-communication-chat-1.3.0/tests/_shared/helper.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/_shared/utils.py` & `azure-communication-chat-1.3.0/tests/_shared/utils.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/chat_e2e_helper.py` & `azure-communication-chat-1.3.0/tests/chat_e2e_helper.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/conftest.py` & `azure-communication-chat-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_client.py` & `azure-communication-chat-1.3.0/tests/test_chat_client.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_client_async.py` & `azure-communication-chat-1.3.0/tests/test_chat_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_client_e2e.py` & `azure-communication-chat-1.3.0/tests/test_chat_client_e2e.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import pytest
 import time
 from datetime import datetime, timezone
-from devtools_testutils import AzureRecordedTestCase, is_live
+from devtools_testutils import AzureRecordedTestCase, is_live, recorded_by_proxy
 from uuid import uuid4
 
 from azure.communication.identity import CommunicationIdentityClient
 from azure.communication.chat import (
     ChatClient,
     CommunicationTokenCredential,
     ChatParticipant
@@ -58,14 +58,15 @@
         )]
         create_chat_thread_result = self.chat_client.create_chat_thread(topic,
                                                                         thread_participants=participants,
                                                                         idempotency_token=idempotency_token)
         self.thread_id = create_chat_thread_result.chat_thread.id
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_access_token_validation(self):
         """
         This is to make sure that consecutive calls made using the same chat_client or chat_thread_client
         does not throw an exception due to mismatch in the generation of azure.core.credentials.AccessToken
         """
 
         # create ChatClient
@@ -91,54 +92,60 @@
                     print("ChatThreadInfo: ", chat_thread_info)
         except:
            raised = True
 
         assert raised is False
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_create_chat_thread(self):
         self._create_thread()
         assert self.thread_id is not None
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_create_chat_thread_w_no_participants(self):
         # create chat thread
         topic = "test topic"
         create_chat_thread_result = self.chat_client.create_chat_thread(topic)
         self.thread_id = create_chat_thread_result.chat_thread.id
         assert create_chat_thread_result.chat_thread is not None
-        assert create_chat_thread_result.errors is None
+        assert len(create_chat_thread_result.errors) == 0
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_create_chat_thread_w_repeatability_request_id(self):
         idempotency_token = str(uuid4())
         # create thread
         self._create_thread(idempotency_token=idempotency_token)
         thread_id = self.thread_id
 
         # re-create thread with same idempotency_token
         self._create_thread(idempotency_token=idempotency_token)
 
         # test idempotency
         assert thread_id == self.thread_id
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_list_chat_threads(self):
         self._create_thread()
         if self.is_live:
             time.sleep(2)
 
         chat_threads = self.chat_client.list_chat_threads(results_per_page=1)
         for chat_thread_item_page in chat_threads.by_page():
             li = list(chat_thread_item_page)
             assert len(li) <= 1
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_get_thread_client(self):
         self._create_thread()
         chat_thread_client = self.chat_client.get_chat_thread_client(self.thread_id)
         assert chat_thread_client.thread_id == self.thread_id
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_delete_chat_thread(self):
         self._create_thread()
         self.chat_client.delete_chat_thread(self.thread_id)
```

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_client_e2e_async.py` & `azure-communication-chat-1.3.0/tests/test_chat_client_e2e_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import pytest
 import asyncio
 from datetime import datetime, timezone
 from devtools_testutils import AzureRecordedTestCase, is_live
+from devtools_testutils.aio import recorded_by_proxy_async
 from uuid import uuid4
 
 from azure.communication.identity import CommunicationIdentityClient
 from azure.communication.chat.aio import (
     ChatClient,
     CommunicationTokenCredential
 )
@@ -57,43 +58,46 @@
             display_name='name',
             share_history_time=share_history_time
         )]
         create_chat_thread_result = await self.chat_client.create_chat_thread(topic,
                                                                               thread_participants=participants,
                                                                               idempotency_token=idempotency_token)
         self.thread_id = create_chat_thread_result.chat_thread.id
-
+    
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_create_chat_thread_async(self):
         async with self.chat_client:
             await self._create_thread()
             assert self.thread_id is not None
 
             # delete created users and chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_create_chat_thread_w_no_participants_async(self):
         async with self.chat_client:
             # create chat thread
             topic = "test topic"
             create_chat_thread_result = await self.chat_client.create_chat_thread(topic)
 
             assert create_chat_thread_result.chat_thread is not None
-            assert create_chat_thread_result.errors is None
+            assert len(create_chat_thread_result.errors) == 0
 
             # delete created users and chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(create_chat_thread_result.chat_thread.id)
-
+    
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_create_chat_thread_w_repeatability_request_id_async(self):
         async with self.chat_client:
             idempotency_token = str(uuid4())
 
             # create thread
             await self._create_thread(idempotency_token=idempotency_token)
             assert self.thread_id is not None
@@ -104,17 +108,17 @@
             assert thread_id == self.thread_id
 
 
             # delete created users and chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
-
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_list_chat_threads(self):
         async with self.chat_client:
             await self._create_thread()
             if self.is_live:
                 await asyncio.sleep(2)
 
             chat_threads = self.chat_client.list_chat_threads(results_per_page=1)
@@ -126,26 +130,28 @@
 
             # delete created users and chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_get_thread_client(self):
         async with self.chat_client:
             await self._create_thread()
             chat_thread_client = self.chat_client.get_chat_thread_client(self.thread_id)
             assert chat_thread_client.thread_id == self.thread_id
 
             # delete created users and chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_delete_chat_thread(self):
         async with self.chat_client:
             await self._create_thread()
             await self.chat_client.delete_chat_thread(self.thread_id)
 
             # delete created users and chat threads
             if not self.is_playback():
```

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_thread_client.py` & `azure-communication-chat-1.3.0/tests/test_chat_thread_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,20 @@
                             "attachments": [
                                 {
                                     "id": "id",
                                     "attachmentType": "image",
                                     "name": "name.png",
                                     "url": "https://endpoint/threads/chatThreadId/images/imageId/views/original",
                                     "previewUrl": "https://endpoint/threads/chatThreadId/images/imageId/views/preview",
+                                },
+                                {
+                                    "id": "id",
+                                    "attachmentType": "file",
+                                    "name": "name.pdf",
+                                    "previewUrl": "https://contoso.sharepoint.com/teams/TeamName/DocumentLibrary/FileName",
                                 }
                             ]
                         },
                         "senderDisplayName": "Bob",
                         "createdOn": "2021-01-27T01:37:33Z",
                         "senderCommunicationIdentifier": {"rawId": "string", "communicationUser": {
                             "id": "8:acs:8540c0de-899f-5cce-acb5-3ec493af3800_0e59221d-0c1d-46ae-9544-c963ce56c10b"}},
@@ -214,16 +220,17 @@
 
         self.assertFalse(raised, 'Expected is no excpetion raised')
         assert message.id == message_id
         assert message.content.message == message_str
         assert message.type == ChatMessageType.TEXT
         assert message.metadata["tags"] == "tag"
         assert len(message.content.participants) > 0
-        assert len(message.content.attachments) > 0
+        assert len(message.content.attachments) == 2
         assert message.content.attachments[0].attachment_type == "image"
+        assert message.content.attachments[1].attachment_type == "file"
 
     def test_list_messages(self):
         thread_id = "19:bcaebfba0d314c2aa3e920d38fa3df08@thread.v2"
         message_id='1596823919339'
         message_str = "Hi I am Bob."
         raised = False
```

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_thread_client_async.py` & `azure-communication-chat-1.3.0/tests/test_chat_thread_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_thread_client_e2e.py` & `azure-communication-chat-1.3.0/tests/test_chat_thread_client_e2e.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import pytest
 import time
 from datetime import datetime, timezone
-from devtools_testutils import AzureRecordedTestCase, is_live
+from devtools_testutils import AzureRecordedTestCase, is_live, recorded_by_proxy
 
 from azure.communication.identity import CommunicationIdentityClient
 from azure.communication.chat import (
     ChatClient,
     ChatParticipant,
     ChatMessageType,
     CommunicationTokenCredential
@@ -106,69 +106,76 @@
         create_message_result = self.chat_thread_client.send_message(
             content,
             sender_display_name=sender_display_name)
         message_id = create_message_result.id
         return message_id
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_update_topic(self):
         self._create_thread()
         topic = "update topic"
         self.chat_thread_client.update_topic(topic=topic)
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_send_message(self):
         self._create_thread()
 
         content = 'hello world'
         sender_display_name = 'sender name'
 
         create_message_result = self.chat_thread_client.send_message(
             content,
             sender_display_name=sender_display_name)
         create_message_result_id = create_message_result.id
 
         assert create_message_result_id is not None
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_get_message(self):
         self._create_thread()
         message_id = self._send_message()
         message = self.chat_thread_client.get_message(message_id)
         assert message.id == message_id
         assert message.type == ChatMessageType.TEXT
         assert message.content.message == 'hello world'
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_list_messages(self):
         self._create_thread()
         self._send_message()
 
         chat_messages = self.chat_thread_client.list_messages(results_per_page=1)
 
         for chat_message in chat_messages.by_page():
             li = list(chat_message)
             assert len(li) <= 1
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_update_message(self):
         self._create_thread()
         message_id = self._send_message()
 
         content = "updated message content"
         self.chat_thread_client.update_message(message_id, content=content)
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_delete_message(self):
         self._create_thread()
         message_id = self._send_message()
 
         self.chat_thread_client.delete_message(message_id)
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_list_participants(self):
         self._create_thread()
 
         # add another participant
         share_history_time = datetime.utcnow()
         share_history_time = share_history_time.replace(tzinfo=timezone.utc)
         new_participant = ChatParticipant(
@@ -188,14 +195,15 @@
             assert len(li) <= 1
             participant_count += len(li)
             li[0].identifier.properties['id'] = self.user.properties['id']
         assert participant_count == 1
 
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_add_participants(self):
         self._create_thread()
 
         share_history_time = datetime.utcnow()
         share_history_time = share_history_time.replace(tzinfo=timezone.utc)
         new_participant = ChatParticipant(
                 identifier=self.new_user,
@@ -206,14 +214,15 @@
         failed_participants = self.chat_thread_client.add_participants(participants)
 
         # no error occured while adding participants
         assert len(failed_participants) == 0
 
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_remove_participant(self):
         self._create_thread()
 
         # add participant first
         share_history_time = datetime.utcnow()
         share_history_time = share_history_time.replace(tzinfo=timezone.utc)
         new_participant = ChatParticipant(
@@ -224,26 +233,29 @@
 
         self.chat_thread_client.add_participants(participants)
 
         # test remove participant
         self.chat_thread_client.remove_participant(self.new_user)
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_send_typing_notification(self):
         self._create_thread()
 
         self.chat_thread_client.send_typing_notification()
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_send_typing_notification_with_display_name(self):
         self._create_thread()
 
         self.chat_thread_client.send_typing_notification(sender_display_name="John")
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_send_read_receipt(self):
         self._create_thread()
         message_id = self._send_message()
 
         self.chat_thread_client.send_read_receipt(message_id)
 
 
@@ -262,14 +274,15 @@
             else:
                 print("Sleeping for additional 2 secs")
                 time.sleep(2)
         raise Exception("Read receipts not updated in 20 seconds. Failing.")
 
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_list_read_receipts(self):
         self._create_thread_w_two_users()
 
         # first user send 2 messages
         # send messages and read receipts
         for i in range(2):
             message_id = self._send_message()
@@ -298,11 +311,12 @@
         for page in read_receipts.by_page():
             for item in page:
                 items.append(item)
 
         assert len(items) == 2
 
     @pytest.mark.live_test_only
+    @recorded_by_proxy
     def test_get_properties(self):
         self._create_thread()
         get_thread_result = self.chat_thread_client.get_properties()
         assert get_thread_result.id == self.thread_id
```

### Comparing `azure-communication-chat-1.2.0/tests/test_chat_thread_client_e2e_async.py` & `azure-communication-chat-1.3.0/tests/test_chat_thread_client_e2e_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import pytest
 import asyncio
 from datetime import datetime, timezone
 from devtools_testutils import AzureRecordedTestCase, is_live
+from devtools_testutils.aio import recorded_by_proxy_async
 
 from azure.communication.identity import CommunicationIdentityClient
 from azure.communication.chat.aio import (
     ChatClient,
     CommunicationTokenCredential
 )
 from azure.communication.chat import (
@@ -107,28 +108,30 @@
             content,
             sender_display_name=sender_display_name)
         message_id = create_message_result.id
         return message_id
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_update_topic(self):
         async with self.chat_client:
             await self._create_thread()
             topic = "update topic"
 
             async with self.chat_thread_client:
                 await self.chat_thread_client.update_topic(topic=topic)
 
             # delete chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_send_message(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 content = 'hello world'
                 sender_display_name = 'sender name'
@@ -142,14 +145,15 @@
 
             # delete chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_get_message(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 message_id = await self._send_message()
                 message = await self.chat_thread_client.get_message(message_id)
@@ -159,14 +163,15 @@
 
             # delete chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_list_messages(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 await self._send_message()
 
@@ -180,14 +185,15 @@
 
             # delete chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_update_message(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 message_id = await self._send_message()
 
@@ -196,14 +202,15 @@
 
             # delete chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_delete_message(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 message_id = await self._send_message()
 
@@ -211,14 +218,15 @@
 
             # delete chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_list_participants(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 # add another participant
                 share_history_time = datetime.utcnow()
@@ -240,14 +248,15 @@
 
             # delete chat threads
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_add_participants(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 share_history_time = datetime.utcnow()
                 share_history_time = share_history_time.replace(tzinfo=timezone.utc)
@@ -263,14 +272,15 @@
                 assert len(failed_participants) == 0
 
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_remove_participant(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 # add participant first
                 share_history_time = datetime.utcnow()
@@ -287,42 +297,44 @@
                 await self.chat_thread_client.remove_participant(self.new_user)
 
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_send_typing_notification(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 await self.chat_thread_client.send_typing_notification()
 
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_send_typing_notification_with_sender_display_name(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 await self.chat_thread_client.send_typing_notification(sender_display_name="John")
 
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_send_read_receipt(self):
         async with self.chat_client:
             await self._create_thread()
-
             async with self.chat_thread_client:
                 message_id = await self._send_message()
 
                 await self.chat_thread_client.send_read_receipt(message_id)
 
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
@@ -342,14 +354,15 @@
             else:
                 print("Sleeping for additional 2 secs")
                 await asyncio.sleep(2)
         raise Exception("Read receipts not updated in 20 seconds. Failing.")
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_list_read_receipts(self):
         async with self.chat_client:
             await self._create_thread_w_two_users()
 
             async with self.chat_thread_client:
 
                 # first user sends 2 messages
@@ -388,14 +401,15 @@
                 assert len(items) == 2
 
             if not self.is_playback():
                 await self.chat_client.delete_chat_thread(self.thread_id)
 
     @pytest.mark.live_test_only
     @pytest.mark.asyncio
+    @recorded_by_proxy_async
     async def test_get_properties(self):
         async with self.chat_client:
             await self._create_thread()
 
             async with self.chat_thread_client:
                 get_thread_result = await self.chat_thread_client.get_properties()
                 assert get_thread_result.id == self.thread_id
```

### Comparing `azure-communication-chat-1.2.0/tests/test_communication_identifier_serializer.py` & `azure-communication-chat-1.3.0/tests/test_communication_identifier_serializer.py`

 * *Files identical despite different names*

### Comparing `azure-communication-chat-1.2.0/tests/unittest_helpers.py` & `azure-communication-chat-1.3.0/tests/unittest_helpers.py`

 * *Files identical despite different names*

