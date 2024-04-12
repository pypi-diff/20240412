# Comparing `tmp/types-aiobotocore-chatbot-2.12.2.tar.gz` & `tmp/types-aiobotocore-chatbot-2.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chatbot-2.12.2.tar", last modified: Wed Apr  3 01:14:47 2024, max compression
+gzip compressed data, was "types-aiobotocore-chatbot-2.12.3.tar", last modified: Fri Apr 12 01:17:01 2024, max compression
```

## Comparing `types-aiobotocore-chatbot-2.12.2.tar` & `types-aiobotocore-chatbot-2.12.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:47.323358 types-aiobotocore-chatbot-2.12.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-03 01:14:47.323358 types-aiobotocore-chatbot-2.12.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:14:47.323358 types-aiobotocore-chatbot-2.12.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:47.323358 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-03 00:59:38.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-03 00:59:38.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 00:59:37.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:14:47.323358 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-03 01:14:47.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-03 01:14:47.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:14:47.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:14:47.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 01:14:47.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 01:14:47.000000 types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chatbot-2.12.2/LICENSE` & `types-aiobotocore-chatbot-2.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chatbot-2.12.2/PKG-INFO` & `types-aiobotocore-chatbot-2.12.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chatbot
-Version: 2.12.2
-Summary: Type annotations for aiobotocore.chatbot 2.12.2 service generated with mypy-boto3-builder 7.23.2
+Version: 2.12.3
+Summary: Type annotations for aiobotocore.Chatbot 2.12.3 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chatbot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chatbot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chatbot)](https://pepy.tech/project/types-aiobotocore-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.chatbot 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
+[aiobotocore.Chatbot 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -91,15 +91,15 @@
 
 ## How to install
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `types-aiobotocore` for `chatbot` service.
+Install `types-aiobotocore` for `Chatbot` service.
 
 ```bash
 # install with aiobotocore type annotations
 python -m pip install 'types-aiobotocore[chatbot]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -246,52 +246,52 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`chatbotClient` provides annotations for `session.create_client("chatbot")`.
+`ChatbotClient` provides annotations for `session.create_client("chatbot")`.
 
 ```python
 from aiobotocore.session import get_session
 
-from types_aiobotocore_chatbot import chatbotClient
+from types_aiobotocore_chatbot import ChatbotClient
 
 session = get_session()
 async with session.create_client("chatbot") as client:
-    client: chatbotClient
+    client: ChatbotClient
     # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_chatbot.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
-Full list of `chatbot` Literals can be found in
+Full list of `Chatbot` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/literals/).
 
 ```python
-from types_aiobotocore_chatbot.literals import chatbotServiceName
+from types_aiobotocore_chatbot.literals import ChatbotServiceName
 
 
-def check_value(value: chatbotServiceName) -> bool: ...
+def check_value(value: ChatbotServiceName) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_chatbot.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
-Full list of `chatbot` TypeDefs can be found in
+Full list of `Chatbot` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/type_defs/).
 
 ```python
 from types_aiobotocore_chatbot.type_defs import AccountPreferencesTypeDef
 
 
 def get_value() -> AccountPreferencesTypeDef:
```

### Comparing `types-aiobotocore-chatbot-2.12.2/README.md` & `types-aiobotocore-chatbot-2.12.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chatbot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chatbot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chatbot)](https://pepy.tech/project/types-aiobotocore-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.chatbot 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
+[aiobotocore.Chatbot 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -58,15 +58,15 @@
 
 ## How to install
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `types-aiobotocore` for `chatbot` service.
+Install `types-aiobotocore` for `Chatbot` service.
 
 ```bash
 # install with aiobotocore type annotations
 python -m pip install 'types-aiobotocore[chatbot]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -213,52 +213,52 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`chatbotClient` provides annotations for `session.create_client("chatbot")`.
+`ChatbotClient` provides annotations for `session.create_client("chatbot")`.
 
 ```python
 from aiobotocore.session import get_session
 
-from types_aiobotocore_chatbot import chatbotClient
+from types_aiobotocore_chatbot import ChatbotClient
 
 session = get_session()
 async with session.create_client("chatbot") as client:
-    client: chatbotClient
+    client: ChatbotClient
     # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_chatbot.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
-Full list of `chatbot` Literals can be found in
+Full list of `Chatbot` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/literals/).
 
 ```python
-from types_aiobotocore_chatbot.literals import chatbotServiceName
+from types_aiobotocore_chatbot.literals import ChatbotServiceName
 
 
-def check_value(value: chatbotServiceName) -> bool: ...
+def check_value(value: ChatbotServiceName) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_chatbot.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
-Full list of `chatbot` TypeDefs can be found in
+Full list of `Chatbot` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/type_defs/).
 
 ```python
 from types_aiobotocore_chatbot.type_defs import AccountPreferencesTypeDef
 
 
 def get_value() -> AccountPreferencesTypeDef:
```

### Comparing `types-aiobotocore-chatbot-2.12.2/setup.py` & `types-aiobotocore-chatbot-2.12.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chatbot",
-    version="2.12.2",
+    version="2.12.3",
     packages=["types_aiobotocore_chatbot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore.chatbot 2.12.2 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for aiobotocore.Chatbot 2.12.3 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/__main__.py` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.chatbot 2.12.2\n"
-        "Version:         2.12.2\n"
+        "Type annotations for aiobotocore.Chatbot 2.12.3\n"
+        "Version:         2.12.3\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot//\n"
-        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.12.2")
+    print("2.12.3")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/client.py` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
 
 Usage::
 
     ```python
     from aiobotocore.session import get_session
-    from types_aiobotocore_chatbot.client import chatbotClient
+    from types_aiobotocore_chatbot.client import ChatbotClient
 
     session = get_session()
     async with session.create_client("chatbot") as client:
-        client: chatbotClient
+        client: ChatbotClient
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
@@ -35,15 +35,15 @@
     ListTeamsChannelConfigurationsResultTypeDef,
     UpdateAccountPreferencesResultTypeDef,
     UpdateChimeWebhookConfigurationResultTypeDef,
     UpdateSlackChannelConfigurationResultTypeDef,
     UpdateTeamsChannelConfigurationResultTypeDef,
 )
 
-__all__ = ("chatbotClient",)
+__all__ = ("ChatbotClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -78,44 +78,44 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     UpdateAccountPreferencesException: Type[BotocoreClientError]
     UpdateChimeWebhookConfigurationException: Type[BotocoreClientError]
     UpdateSlackChannelConfigurationException: Type[BotocoreClientError]
     UpdateTeamsChannelConfigurationException: Type[BotocoreClientError]
 
 
-class chatbotClient(AioBaseClient):
+class ChatbotClient(AioBaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        chatbotClient exceptions.
+        ChatbotClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#exceptions)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#can_paginate)
         """
 
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#close)
         """
 
     async def create_chime_webhook_configuration(
         self,
         *,
         WebhookDescription: str,
@@ -125,15 +125,15 @@
         ConfigurationName: str,
         LoggingLevel: str = ...,
     ) -> CreateChimeWebhookConfigurationResultTypeDef:
         """
         Creates Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_chime_webhook_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#create_chime_webhook_configuration)
         """
 
     async def create_microsoft_teams_channel_configuration(
         self,
         *,
         ChannelId: str,
@@ -148,15 +148,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateTeamsChannelConfigurationResultTypeDef:
         """
         Creates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#create_microsoft_teams_channel_configuration)
         """
 
     async def create_slack_channel_configuration(
         self,
         *,
         SlackTeamId: str,
@@ -169,213 +169,213 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateSlackChannelConfigurationResultTypeDef:
         """
         Creates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#create_slack_channel_configuration)
         """
 
     async def delete_chime_webhook_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_chime_webhook_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_chime_webhook_configuration)
         """
 
     async def delete_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_microsoft_teams_channel_configuration)
         """
 
     async def delete_microsoft_teams_configured_team(self, *, TeamId: str) -> Dict[str, Any]:
         """
         Deletes the Microsoft Teams team authorization allowing for channels to be
         configured in that Microsoft Teams
         team.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_configured_team)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_configured_team)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_microsoft_teams_configured_team)
         """
 
     async def delete_microsoft_teams_user_identity(
         self, *, ChatConfigurationArn: str, UserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Teams user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_user_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_microsoft_teams_user_identity)
         """
 
     async def delete_slack_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_slack_channel_configuration)
         """
 
     async def delete_slack_user_identity(
         self, *, ChatConfigurationArn: str, SlackTeamId: str, SlackUserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Slack user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_user_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_slack_user_identity)
         """
 
     async def delete_slack_workspace_authorization(self, *, SlackTeamId: str) -> Dict[str, Any]:
         """
         Deletes the Slack workspace authorization that allows channels to be configured
         in that
         workspace.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_workspace_authorization)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_workspace_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_slack_workspace_authorization)
         """
 
     async def describe_chime_webhook_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeChimeWebhookConfigurationsResultTypeDef:
         """
         Lists Chime Webhook Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeChimeWebhookConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_chime_webhook_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_chime_webhook_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_chime_webhook_configurations)
         """
 
     async def describe_slack_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeSlackChannelConfigurationsResultTypeDef:
         """
         Lists Slack Channel Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_channel_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_slack_channel_configurations)
         """
 
     async def describe_slack_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeSlackUserIdentitiesResultTypeDef:
         """
         Lists all Slack user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_user_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_slack_user_identities)
         """
 
     async def describe_slack_workspaces(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeSlackWorkspacesResultTypeDef:
         """
         Lists all authorized Slack Workspaces for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackWorkspaces).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_workspaces)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_slack_workspaces)
         """
 
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#generate_presigned_url)
         """
 
     async def get_account_preferences(self) -> GetAccountPreferencesResultTypeDef:
         """
         Get Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_account_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#get_account_preferences)
         """
 
     async def get_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> GetTeamsChannelConfigurationResultTypeDef:
         """
         Get a single MS Teams Channel Configurations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#get_microsoft_teams_channel_configuration)
         """
 
     async def list_microsoft_teams_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., TeamId: str = ...
     ) -> ListTeamsChannelConfigurationsResultTypeDef:
         """
         Lists MS Teams Channel Configurations optionally filtered by TeamId See also:
         [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_channel_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#list_microsoft_teams_channel_configurations)
         """
 
     async def list_microsoft_teams_configured_teams(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMicrosoftTeamsConfiguredTeamsResultTypeDef:
         """
         Lists all authorized MS teams for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsConfiguredTeams).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_configured_teams)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_configured_teams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#list_microsoft_teams_configured_teams)
         """
 
     async def list_microsoft_teams_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListMicrosoftTeamsUserIdentitiesResultTypeDef:
         """
         Lists all Microsoft Teams user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_user_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#list_microsoft_teams_user_identities)
         """
 
     async def update_account_preferences(
         self, *, UserAuthorizationRequired: bool = ..., TrainingDataCollectionEnabled: bool = ...
     ) -> UpdateAccountPreferencesResultTypeDef:
         """
         Update Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_account_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_account_preferences)
         """
 
     async def update_chime_webhook_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -385,15 +385,15 @@
         IamRoleArn: str = ...,
         LoggingLevel: str = ...,
     ) -> UpdateChimeWebhookConfigurationResultTypeDef:
         """
         Updates a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_chime_webhook_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_chime_webhook_configuration)
         """
 
     async def update_microsoft_teams_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -405,15 +405,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateTeamsChannelConfigurationResultTypeDef:
         """
         Updates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_microsoft_teams_channel_configuration)
         """
 
     async def update_slack_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -425,22 +425,22 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateSlackChannelConfigurationResultTypeDef:
         """
         Updates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_slack_channel_configuration)
         """
 
-    async def __aenter__(self) -> "chatbotClient":
+    async def __aenter__(self) -> "ChatbotClient":
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
         """
 
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
         """
```

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/client.pyi` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
 
 Usage::
 
     ```python
     from aiobotocore.session import get_session
-    from types_aiobotocore_chatbot.client import chatbotClient
+    from types_aiobotocore_chatbot.client import ChatbotClient
 
     session = get_session()
     async with session.create_client("chatbot") as client:
-        client: chatbotClient
+        client: ChatbotClient
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
@@ -35,15 +35,15 @@
     ListTeamsChannelConfigurationsResultTypeDef,
     UpdateAccountPreferencesResultTypeDef,
     UpdateChimeWebhookConfigurationResultTypeDef,
     UpdateSlackChannelConfigurationResultTypeDef,
     UpdateTeamsChannelConfigurationResultTypeDef,
 )
 
-__all__ = ("chatbotClient",)
+__all__ = ("ChatbotClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
@@ -75,44 +75,44 @@
     ListTeamsChannelConfigurationsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     UpdateAccountPreferencesException: Type[BotocoreClientError]
     UpdateChimeWebhookConfigurationException: Type[BotocoreClientError]
     UpdateSlackChannelConfigurationException: Type[BotocoreClientError]
     UpdateTeamsChannelConfigurationException: Type[BotocoreClientError]
 
-class chatbotClient(AioBaseClient):
+class ChatbotClient(AioBaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        chatbotClient exceptions.
+        ChatbotClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#exceptions)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#can_paginate)
         """
 
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#close)
         """
 
     async def create_chime_webhook_configuration(
         self,
         *,
         WebhookDescription: str,
@@ -122,15 +122,15 @@
         ConfigurationName: str,
         LoggingLevel: str = ...,
     ) -> CreateChimeWebhookConfigurationResultTypeDef:
         """
         Creates Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_chime_webhook_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#create_chime_webhook_configuration)
         """
 
     async def create_microsoft_teams_channel_configuration(
         self,
         *,
         ChannelId: str,
@@ -145,15 +145,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateTeamsChannelConfigurationResultTypeDef:
         """
         Creates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#create_microsoft_teams_channel_configuration)
         """
 
     async def create_slack_channel_configuration(
         self,
         *,
         SlackTeamId: str,
@@ -166,213 +166,213 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateSlackChannelConfigurationResultTypeDef:
         """
         Creates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#create_slack_channel_configuration)
         """
 
     async def delete_chime_webhook_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_chime_webhook_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_chime_webhook_configuration)
         """
 
     async def delete_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_microsoft_teams_channel_configuration)
         """
 
     async def delete_microsoft_teams_configured_team(self, *, TeamId: str) -> Dict[str, Any]:
         """
         Deletes the Microsoft Teams team authorization allowing for channels to be
         configured in that Microsoft Teams
         team.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_configured_team)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_configured_team)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_microsoft_teams_configured_team)
         """
 
     async def delete_microsoft_teams_user_identity(
         self, *, ChatConfigurationArn: str, UserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Teams user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_user_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_microsoft_teams_user_identity)
         """
 
     async def delete_slack_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_slack_channel_configuration)
         """
 
     async def delete_slack_user_identity(
         self, *, ChatConfigurationArn: str, SlackTeamId: str, SlackUserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Slack user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_user_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_slack_user_identity)
         """
 
     async def delete_slack_workspace_authorization(self, *, SlackTeamId: str) -> Dict[str, Any]:
         """
         Deletes the Slack workspace authorization that allows channels to be configured
         in that
         workspace.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_workspace_authorization)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_workspace_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#delete_slack_workspace_authorization)
         """
 
     async def describe_chime_webhook_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeChimeWebhookConfigurationsResultTypeDef:
         """
         Lists Chime Webhook Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeChimeWebhookConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_chime_webhook_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_chime_webhook_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_chime_webhook_configurations)
         """
 
     async def describe_slack_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeSlackChannelConfigurationsResultTypeDef:
         """
         Lists Slack Channel Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_channel_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_slack_channel_configurations)
         """
 
     async def describe_slack_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeSlackUserIdentitiesResultTypeDef:
         """
         Lists all Slack user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_user_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_slack_user_identities)
         """
 
     async def describe_slack_workspaces(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeSlackWorkspacesResultTypeDef:
         """
         Lists all authorized Slack Workspaces for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackWorkspaces).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_workspaces)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#describe_slack_workspaces)
         """
 
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#generate_presigned_url)
         """
 
     async def get_account_preferences(self) -> GetAccountPreferencesResultTypeDef:
         """
         Get Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_account_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#get_account_preferences)
         """
 
     async def get_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> GetTeamsChannelConfigurationResultTypeDef:
         """
         Get a single MS Teams Channel Configurations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#get_microsoft_teams_channel_configuration)
         """
 
     async def list_microsoft_teams_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., TeamId: str = ...
     ) -> ListTeamsChannelConfigurationsResultTypeDef:
         """
         Lists MS Teams Channel Configurations optionally filtered by TeamId See also:
         [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_channel_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#list_microsoft_teams_channel_configurations)
         """
 
     async def list_microsoft_teams_configured_teams(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMicrosoftTeamsConfiguredTeamsResultTypeDef:
         """
         Lists all authorized MS teams for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsConfiguredTeams).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_configured_teams)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_configured_teams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#list_microsoft_teams_configured_teams)
         """
 
     async def list_microsoft_teams_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListMicrosoftTeamsUserIdentitiesResultTypeDef:
         """
         Lists all Microsoft Teams user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_user_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#list_microsoft_teams_user_identities)
         """
 
     async def update_account_preferences(
         self, *, UserAuthorizationRequired: bool = ..., TrainingDataCollectionEnabled: bool = ...
     ) -> UpdateAccountPreferencesResultTypeDef:
         """
         Update Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_account_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_account_preferences)
         """
 
     async def update_chime_webhook_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -382,15 +382,15 @@
         IamRoleArn: str = ...,
         LoggingLevel: str = ...,
     ) -> UpdateChimeWebhookConfigurationResultTypeDef:
         """
         Updates a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_chime_webhook_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_chime_webhook_configuration)
         """
 
     async def update_microsoft_teams_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -402,15 +402,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateTeamsChannelConfigurationResultTypeDef:
         """
         Updates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_microsoft_teams_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_microsoft_teams_channel_configuration)
         """
 
     async def update_slack_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -422,22 +422,22 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateSlackChannelConfigurationResultTypeDef:
         """
         Updates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_slack_channel_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/#update_slack_channel_configuration)
         """
 
-    async def __aenter__(self) -> "chatbotClient":
+    async def __aenter__(self) -> "ChatbotClient":
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
         """
 
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/client/)
         """
```

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/literals.py` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 Type annotations for chatbot service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_chatbot.literals import chatbotServiceName
+    from types_aiobotocore_chatbot.literals import ChatbotServiceName
 
-    data: chatbotServiceName = "chatbot"
+    data: ChatbotServiceName = "chatbot"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = ("chatbotServiceName", "ServiceName", "ResourceServiceName")
+__all__ = ("ChatbotServiceName", "ServiceName", "ResourceServiceName")
 
-chatbotServiceName = Literal["chatbot"]
+ChatbotServiceName = Literal["chatbot"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
@@ -187,15 +187,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -375,14 +374,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/literals.pyi` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 Type annotations for chatbot service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_chatbot.literals import chatbotServiceName
+    from types_aiobotocore_chatbot.literals import ChatbotServiceName
 
-    data: chatbotServiceName = "chatbot"
+    data: ChatbotServiceName = "chatbot"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = ("chatbotServiceName", "ServiceName", "ResourceServiceName")
+__all__ = ("ChatbotServiceName", "ServiceName", "ResourceServiceName")
 
-chatbotServiceName = Literal["chatbot"]
+ChatbotServiceName = Literal["chatbot"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
@@ -187,15 +187,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -375,14 +374,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/type_defs.py` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot/type_defs.pyi` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/PKG-INFO` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chatbot
-Version: 2.12.2
-Summary: Type annotations for aiobotocore.chatbot 2.12.2 service generated with mypy-boto3-builder 7.23.2
+Version: 2.12.3
+Summary: Type annotations for aiobotocore.Chatbot 2.12.3 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chatbot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chatbot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chatbot)](https://pepy.tech/project/types-aiobotocore-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.chatbot 2.12.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
+[aiobotocore.Chatbot 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -91,15 +91,15 @@
 
 ## How to install
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `types-aiobotocore` for `chatbot` service.
+Install `types-aiobotocore` for `Chatbot` service.
 
 ```bash
 # install with aiobotocore type annotations
 python -m pip install 'types-aiobotocore[chatbot]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -246,52 +246,52 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`chatbotClient` provides annotations for `session.create_client("chatbot")`.
+`ChatbotClient` provides annotations for `session.create_client("chatbot")`.
 
 ```python
 from aiobotocore.session import get_session
 
-from types_aiobotocore_chatbot import chatbotClient
+from types_aiobotocore_chatbot import ChatbotClient
 
 session = get_session()
 async with session.create_client("chatbot") as client:
-    client: chatbotClient
+    client: ChatbotClient
     # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_chatbot.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
-Full list of `chatbot` Literals can be found in
+Full list of `Chatbot` Literals can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/literals/).
 
 ```python
-from types_aiobotocore_chatbot.literals import chatbotServiceName
+from types_aiobotocore_chatbot.literals import ChatbotServiceName
 
 
-def check_value(value: chatbotServiceName) -> bool: ...
+def check_value(value: ChatbotServiceName) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_chatbot.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
-Full list of `chatbot` TypeDefs can be found in
+Full list of `Chatbot` TypeDefs can be found in
 [docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/type_defs/).
 
 ```python
 from types_aiobotocore_chatbot.type_defs import AccountPreferencesTypeDef
 
 
 def get_value() -> AccountPreferencesTypeDef:
```

### Comparing `types-aiobotocore-chatbot-2.12.2/types_aiobotocore_chatbot.egg-info/SOURCES.txt` & `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

