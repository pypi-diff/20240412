# Comparing `tmp/zabbix_utils-1.1.1.tar.gz` & `tmp/zabbix_utils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zabbix_utils-1.1.1.tar", last modified: Wed Mar  6 11:35:33 2024, max compression
+gzip compressed data, was "zabbix_utils-2.0.0.tar", last modified: Fri Apr 12 12:00:34 2024, max compression
```

## Comparing `zabbix_utils-1.1.1.tar` & `zabbix_utils-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 11:35:33.403468 zabbix_utils-1.1.1/
--rw-rw-rw-   0        0        0     1092 2023-10-13 12:06:00.000000 zabbix_utils-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     9786 2024-03-06 11:35:33.403468 zabbix_utils-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8683 2024-01-10 03:19:02.000000 zabbix_utils-1.1.1/README.md
--rw-rw-rw-   0        0        0      104 2024-03-06 11:35:33.406467 zabbix_utils-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3012 2024-03-05 11:27:09.000000 zabbix_utils-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-06 11:35:33.337384 zabbix_utils-1.1.1/zabbix_utils/
--rw-rw-rw-   0        0        0     1543 2023-11-17 07:53:09.000000 zabbix_utils-1.1.1/zabbix_utils/__init__.py
--rw-rw-rw-   0        0        0    17487 2024-03-06 10:33:14.000000 zabbix_utils-1.1.1/zabbix_utils/api.py
--rw-rw-rw-   0        0        0     9963 2024-01-19 07:14:58.000000 zabbix_utils-1.1.1/zabbix_utils/common.py
--rw-rw-rw-   0        0        0     2457 2024-01-10 00:07:16.000000 zabbix_utils-1.1.1/zabbix_utils/exceptions.py
--rw-rw-rw-   0        0        0     6214 2024-01-09 23:55:40.000000 zabbix_utils-1.1.1/zabbix_utils/getter.py
--rw-rw-rw-   0        0        0     2014 2023-12-22 13:06:49.000000 zabbix_utils-1.1.1/zabbix_utils/logger.py
--rw-rw-rw-   0        0        0    18165 2024-03-06 10:34:09.000000 zabbix_utils-1.1.1/zabbix_utils/sender.py
--rw-rw-rw-   0        0        0     1213 2024-03-06 10:37:06.000000 zabbix_utils-1.1.1/zabbix_utils/version.py
-drwxrwxrwx   0        0        0        0 2024-03-06 11:35:33.402594 zabbix_utils-1.1.1/zabbix_utils.egg-info/
--rw-rw-rw-   0        0        0     9786 2024-03-06 11:35:32.000000 zabbix_utils-1.1.1/zabbix_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-03-06 11:35:32.000000 zabbix_utils-1.1.1/zabbix_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 11:35:32.000000 zabbix_utils-1.1.1/zabbix_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-06 11:35:32.000000 zabbix_utils-1.1.1/zabbix_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 12:00:34.836562 zabbix_utils-2.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-10-13 12:06:00.000000 zabbix_utils-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    11350 2024-04-12 12:00:34.836562 zabbix_utils-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9966 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/README.md
+-rw-rw-rw-   0        0        0      104 2024-04-12 12:00:34.838579 zabbix_utils-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     3332 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:00:34.797541 zabbix_utils-2.0.0/zabbix_utils/
+-rw-rw-rw-   0        0        0     1951 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/__init__.py
+-rw-rw-rw-   0        0        0    16965 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/aioapi.py
+-rw-rw-rw-   0        0        0     5127 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/aiogetter.py
+-rw-rw-rw-   0        0        0    11885 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/aiosender.py
+-rw-rw-rw-   0        0        0    14188 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/api.py
+-rw-rw-rw-   0        0        0    11752 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/common.py
+-rw-rw-rw-   0        0        0     2457 2024-03-11 09:16:35.000000 zabbix_utils-2.0.0/zabbix_utils/exceptions.py
+-rw-rw-rw-   0        0        0     5333 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/getter.py
+-rw-rw-rw-   0        0        0     2014 2023-12-22 13:06:49.000000 zabbix_utils-2.0.0/zabbix_utils/logger.py
+-rw-rw-rw-   0        0        0    11717 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/sender.py
+-rw-rw-rw-   0        0        0    12222 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/types.py
+-rw-rw-rw-   0        0        0     1213 2024-04-12 11:59:41.000000 zabbix_utils-2.0.0/zabbix_utils/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:00:34.834947 zabbix_utils-2.0.0/zabbix_utils.egg-info/
+-rw-rw-rw-   0        0        0    11350 2024-04-12 12:00:34.000000 zabbix_utils-2.0.0/zabbix_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2024-04-12 12:00:34.000000 zabbix_utils-2.0.0/zabbix_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 12:00:34.000000 zabbix_utils-2.0.0/zabbix_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-12 12:00:34.000000 zabbix_utils-2.0.0/zabbix_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 12:00:34.000000 zabbix_utils-2.0.0/zabbix_utils.egg-info/top_level.txt
```

### Comparing `zabbix_utils-1.1.1/LICENSE` & `zabbix_utils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zabbix_utils-1.1.1/PKG-INFO` & `zabbix_utils-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,64 @@
-Metadata-Version: 2.1
-Name: zabbix_utils
-Version: 1.1.1
-Summary: A library with modules for working with Zabbix (Zabbix API, Zabbix sender, Zabbix get)
-Home-page: https://github.com/zabbix/python-zabbix-utils
-Author: Zabbix SIA
-Author-email: integrationteam@zabbix.com
-Maintainer: Aleksandr Iantsen
-Maintainer-email: aleksandr.iantsen@zabbix.com
-Project-URL: Zabbix, https://www.zabbix.com/documentation/current
-Project-URL: Source, https://github.com/zabbix/python-zabbix-utils
-Project-URL: Changes, https://github.com/zabbix/python-zabbix-utils/blob/main/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/zabbix/python-zabbix-utils/issues
-Keywords: monitoring zabbix api sender get utils tools
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: System :: Monitoring
-Classifier: Topic :: System :: Networking :: Monitoring
-Classifier: Topic :: System :: Systems Administration
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Information Technology
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Zabbix utils library
 
 [![Tests](https://github.com/zabbix/python-zabbix-utils/actions/workflows/tests.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/tests.yaml)
 [![Zabbix API](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_api.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_api.yaml)
 [![Zabbix sender](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_sender.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_sender.yaml)
-[![Zabbix get](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_get.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_get.yaml)
+[![Zabbix get](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_getter.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_getter.yaml)
 [![Zabbix 5.0](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_50.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_50.yaml)
 [![Zabbix 6.0](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_60.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_60.yaml)
 [![Zabbix 6.4](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_64.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_64.yaml)
 
 **zabbix_utils** is a Python library for working with [Zabbix API](https://www.zabbix.com/documentation/current/manual/api/reference) as well as with [Zabbix sender](https://www.zabbix.com/documentation/current/manpages/zabbix_sender) and [Zabbix get](https://www.zabbix.com/documentation/current/manpages/zabbix_get) protocols.
 
+## Get started
+* [Requirements](#requirements)
+* [Installation](#installation)
+* [Zabbix API](#to-work-with-zabbix-api)
+* [Zabbix Sender](#to-work-via-zabbix-sender-protocol)
+* [Zabbix Get](#to-work-via-zabbix-get-protocol)
+* [Debug log](#enabling-debug-log)
+
 ## Requirements
 
 Supported versions:
 
 * Zabbix 5.0+
 * Python 3.8+
 
 Tested on:
 
 * Zabbix 5.0, 6.0, 6.4 and pre-7.0
 * Python 3.8, 3.9, 3.10, 3.11 and 3.12
 
+Dependencies:
+
+* [aiohttp](https://github.com/aio-libs/aiohttp) (in case of async use)
+
 ## Documentation
 
 ### Installation
 
 Install **zabbix_utils** library using pip:
 
 ```bash
 $ pip install zabbix_utils
 ```
 
+To install the library with dependencies for asynchronous work use the following way:
+
+```bash
+$ pip install zabbix_utils[async]
+```
+
 ### Use cases
 
 ##### To work with Zabbix API
 
-To work with Zabbix API you can import and use **zabbix_utils** library as follows:
+To work with Zabbix API via synchronous I/O you can import and use **zabbix_utils** library as follows:
 
 ```python
 from zabbix_utils import ZabbixAPI
 
 api = ZabbixAPI(url="127.0.0.1")
 api.login(user="User", password="zabbix")
 
@@ -79,46 +68,56 @@
 
 for user in users:
     print(user['name'])
 
 api.logout()
 ```
 
-You can also authenticate using an API token (supported since Zabbix 5.4):
+To work with Zabbix API via asynchronous I/O you can use the following way:
 
 ```python
-from zabbix_utils import ZabbixAPI
+import asyncio
+from zabbix_utils import AsyncZabbixAPI
+
+async def main():
+    api = AsyncZabbixAPI(url="127.0.0.1")
+    await api.login(user="User", password="zabbix")
+
+    users = await api.user.get(
+        output=['userid','name']
+    )
 
+    for user in users:
+        print(user['name'])
+
+    await api.logout()
+
+asyncio.run(main())
+```
+
+You can also authenticate using an API token (supported since Zabbix 5.4):
+
+```python
 api = ZabbixAPI(url="127.0.0.1")
 api.login(token="xxxxxxxx")
+```
 
-users = api.user.get(
-    output=['userid','name']
-)
-
-for user in users:
-    print(user['name'])
+```python
+api = AsyncZabbixAPI(url="127.0.0.1")
+await api.login(token="xxxxxxxx")
 ```
 
 When token is used, calling `api.logout()` is not necessary.
 
 It is possible to specify authentication fields by the following environment variables:
 `ZABBIX_URL`, `ZABBIX_TOKEN`, `ZABBIX_USER`, `ZABBIX_PASSWORD`
 
 You can compare Zabbix API version with strings and numbers, for example:
 
 ```python
-from zabbix_utils import ZabbixAPI
-
-url = "127.0.0.1"
-user = "User"
-password = "zabbix"
-
-api = ZabbixAPI(url=url, user=user, password=password)
-
 # Method to get version
 ver = api.api_version()
 print(type(ver).__name__, ver) # APIVersion 7.0.0
 
 # ZabbixAPI prototype with version
 ver = api.version
 print(type(ver).__name__, ver) # APIVersion 7.0.0
@@ -128,19 +127,17 @@
 print(ver != 7.0)     # False
 print(ver != "7.0.0") # False
 
 # Version additional methods
 print(ver.major)    # 7.0
 print(ver.minor)    # 0
 print(ver.is_lts()) # True
-
-api.logout()
 ```
 
-In case the API object or method name matches one of Python keywords, you can use the suffix `_` in their name to execute correctly:
+In case the API object or method name matches one of Python keywords, you can use the suffix `_` in their name to execute correctly, for example:
 ```python
 from zabbix_utils import ZabbixAPI
 
 api = ZabbixAPI(url="127.0.0.1")
 api.login(token="xxxxxxxx")
 
 template_source = ''
@@ -169,15 +166,31 @@
 sender = Sender(server='127.0.0.1', port=10051)
 response = sender.send_value('host', 'item.key', 'value', 1695713666)
 
 print(response)
 # {"processed": 1, "failed": 0, "total": 1, "time": "0.000338", "chunk": 1}
 ```
 
-Or you can prepare a list of item values and send all at once:
+The asynchronous way:
+
+```python
+import asyncio
+from zabbix_utils import AsyncSender
+
+async def main():
+    sender = AsyncSender(server='127.0.0.1', port=10051)
+    response = await sender.send_value('host', 'item.key', 'value', 1695713666)
+
+    print(response)
+    # {"processed": 1, "failed": 0, "total": 1, "time": "0.000338", "chunk": 1}
+
+asyncio.run(main())
+```
+
+You can also prepare a list of item values and send all at once:
 
 ```python
 from zabbix_utils import ItemValue, Sender
 
 items = [
     ItemValue('host1', 'item.key1', 10),
     ItemValue('host1', 'item.key2', 'test message'),
@@ -218,26 +231,42 @@
 
 In such case, the value will be sent to the first available node of each cluster.
 
 > Please, refer to the [Zabbix sender protocol](https://www.zabbix.com/documentation/current/manual/appendix/protocols/zabbix_sender) and the [using examples](https://github.com/zabbix/python-zabbix-utils/tree/main/examples/sender) for more information.
 
 ##### To work via Zabbix get protocol
 
-To get a value by item key from a Zabbix agent or agent 2 you can import and use the library as follows:
+To get a value by item key from a Zabbix agent or agent 2 via synchronous I/O the library can be imported and used as follows:
 
 ```python
 from zabbix_utils import Getter
 
 agent = Getter(host='127.0.0.1', port=10050)
 resp = agent.get('system.uname')
 
 print(resp.value)
 # Linux test_server 5.15.0-3.60.5.1.el9uek.x86_64
 ```
 
+The library can be used via asynchronous I/O, as in the following example:
+
+```python
+import asyncio
+from zabbix_utils import AsyncGetter
+
+async def main():
+    agent = AsyncGetter(host='127.0.0.1', port=10050)
+    resp = await agent.get('system.uname')
+
+    print(resp.value)
+    # Linux test_server 5.15.0-3.60.5.1.el9uek.x86_64
+
+asyncio.run(main())
+```
+
 > Please, refer to the [Zabbix agent protocol](https://www.zabbix.com/documentation/current/manual/appendix/protocols/zabbix_agent) and the [using examples](https://github.com/zabbix/python-zabbix-utils/tree/main/examples/get) for more information.
 
 ### Enabling debug log
 
 If it needed to debug some issue with Zabbix API, sender or get you can enable the output of logging. The **zabbix_utils** library uses the default python logging module, but it doesn't log by default. You can define logging handler to see records from the library, for example:
 
 ```python
```

### Comparing `zabbix_utils-1.1.1/README.md` & `zabbix_utils-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,91 @@
+Metadata-Version: 2.1
+Name: zabbix_utils
+Version: 2.0.0
+Summary: A library with modules for working with Zabbix (Zabbix API, Zabbix sender, Zabbix get)
+Home-page: https://github.com/zabbix/python-zabbix-utils
+Author: Zabbix SIA
+Author-email: integrationteam@zabbix.com
+Maintainer: Aleksandr Iantsen
+Maintainer-email: aleksandr.iantsen@zabbix.com
+Project-URL: Zabbix, https://www.zabbix.com/documentation/current
+Project-URL: Source, https://github.com/zabbix/python-zabbix-utils
+Project-URL: Changes, https://github.com/zabbix/python-zabbix-utils/blob/main/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/zabbix/python-zabbix-utils/issues
+Keywords: monitoring zabbix api sender get utils tools
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Networking :: Monitoring
+Classifier: Topic :: System :: Systems Administration
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Information Technology
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: async
+License-File: LICENSE
+
 # Zabbix utils library
 
 [![Tests](https://github.com/zabbix/python-zabbix-utils/actions/workflows/tests.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/tests.yaml)
 [![Zabbix API](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_api.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_api.yaml)
 [![Zabbix sender](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_sender.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_sender.yaml)
-[![Zabbix get](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_get.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_get.yaml)
+[![Zabbix get](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_getter.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_getter.yaml)
 [![Zabbix 5.0](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_50.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_50.yaml)
 [![Zabbix 6.0](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_60.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_60.yaml)
 [![Zabbix 6.4](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_64.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_64.yaml)
 
 **zabbix_utils** is a Python library for working with [Zabbix API](https://www.zabbix.com/documentation/current/manual/api/reference) as well as with [Zabbix sender](https://www.zabbix.com/documentation/current/manpages/zabbix_sender) and [Zabbix get](https://www.zabbix.com/documentation/current/manpages/zabbix_get) protocols.
 
-## Get started
-* [Requirements](#requirements)
-* [Installation](#installation)
-* [Zabbix API](#to-work-with-zabbix-api)
-* [Zabbix Sender](#to-work-via-zabbix-sender-protocol)
-* [Zabbix Get](#to-work-via-zabbix-get-protocol)
-* [Debug log](#enabling-debug-log)
-
 ## Requirements
 
 Supported versions:
 
 * Zabbix 5.0+
 * Python 3.8+
 
 Tested on:
 
 * Zabbix 5.0, 6.0, 6.4 and pre-7.0
 * Python 3.8, 3.9, 3.10, 3.11 and 3.12
 
+Dependencies:
+
+* [aiohttp](https://github.com/aio-libs/aiohttp) (in case of async use)
+
 ## Documentation
 
 ### Installation
 
 Install **zabbix_utils** library using pip:
 
 ```bash
 $ pip install zabbix_utils
 ```
 
+To install the library with dependencies for asynchronous work use the following way:
+
+```bash
+$ pip install zabbix_utils[async]
+```
+
 ### Use cases
 
 ##### To work with Zabbix API
 
-To work with Zabbix API you can import and use **zabbix_utils** library as follows:
+To work with Zabbix API via synchronous I/O you can import and use **zabbix_utils** library as follows:
 
 ```python
 from zabbix_utils import ZabbixAPI
 
 api = ZabbixAPI(url="127.0.0.1")
 api.login(user="User", password="zabbix")
 
@@ -58,46 +95,56 @@
 
 for user in users:
     print(user['name'])
 
 api.logout()
 ```
 
-You can also authenticate using an API token (supported since Zabbix 5.4):
+To work with Zabbix API via asynchronous I/O you can use the following way:
 
 ```python
-from zabbix_utils import ZabbixAPI
+import asyncio
+from zabbix_utils import AsyncZabbixAPI
+
+async def main():
+    api = AsyncZabbixAPI(url="127.0.0.1")
+    await api.login(user="User", password="zabbix")
+
+    users = await api.user.get(
+        output=['userid','name']
+    )
 
+    for user in users:
+        print(user['name'])
+
+    await api.logout()
+
+asyncio.run(main())
+```
+
+You can also authenticate using an API token (supported since Zabbix 5.4):
+
+```python
 api = ZabbixAPI(url="127.0.0.1")
 api.login(token="xxxxxxxx")
+```
 
-users = api.user.get(
-    output=['userid','name']
-)
-
-for user in users:
-    print(user['name'])
+```python
+api = AsyncZabbixAPI(url="127.0.0.1")
+await api.login(token="xxxxxxxx")
 ```
 
 When token is used, calling `api.logout()` is not necessary.
 
 It is possible to specify authentication fields by the following environment variables:
 `ZABBIX_URL`, `ZABBIX_TOKEN`, `ZABBIX_USER`, `ZABBIX_PASSWORD`
 
 You can compare Zabbix API version with strings and numbers, for example:
 
 ```python
-from zabbix_utils import ZabbixAPI
-
-url = "127.0.0.1"
-user = "User"
-password = "zabbix"
-
-api = ZabbixAPI(url=url, user=user, password=password)
-
 # Method to get version
 ver = api.api_version()
 print(type(ver).__name__, ver) # APIVersion 7.0.0
 
 # ZabbixAPI prototype with version
 ver = api.version
 print(type(ver).__name__, ver) # APIVersion 7.0.0
@@ -107,19 +154,17 @@
 print(ver != 7.0)     # False
 print(ver != "7.0.0") # False
 
 # Version additional methods
 print(ver.major)    # 7.0
 print(ver.minor)    # 0
 print(ver.is_lts()) # True
-
-api.logout()
 ```
 
-In case the API object or method name matches one of Python keywords, you can use the suffix `_` in their name to execute correctly:
+In case the API object or method name matches one of Python keywords, you can use the suffix `_` in their name to execute correctly, for example:
 ```python
 from zabbix_utils import ZabbixAPI
 
 api = ZabbixAPI(url="127.0.0.1")
 api.login(token="xxxxxxxx")
 
 template_source = ''
@@ -148,15 +193,31 @@
 sender = Sender(server='127.0.0.1', port=10051)
 response = sender.send_value('host', 'item.key', 'value', 1695713666)
 
 print(response)
 # {"processed": 1, "failed": 0, "total": 1, "time": "0.000338", "chunk": 1}
 ```
 
-Or you can prepare a list of item values and send all at once:
+The asynchronous way:
+
+```python
+import asyncio
+from zabbix_utils import AsyncSender
+
+async def main():
+    sender = AsyncSender(server='127.0.0.1', port=10051)
+    response = await sender.send_value('host', 'item.key', 'value', 1695713666)
+
+    print(response)
+    # {"processed": 1, "failed": 0, "total": 1, "time": "0.000338", "chunk": 1}
+
+asyncio.run(main())
+```
+
+You can also prepare a list of item values and send all at once:
 
 ```python
 from zabbix_utils import ItemValue, Sender
 
 items = [
     ItemValue('host1', 'item.key1', 10),
     ItemValue('host1', 'item.key2', 'test message'),
@@ -197,26 +258,42 @@
 
 In such case, the value will be sent to the first available node of each cluster.
 
 > Please, refer to the [Zabbix sender protocol](https://www.zabbix.com/documentation/current/manual/appendix/protocols/zabbix_sender) and the [using examples](https://github.com/zabbix/python-zabbix-utils/tree/main/examples/sender) for more information.
 
 ##### To work via Zabbix get protocol
 
-To get a value by item key from a Zabbix agent or agent 2 you can import and use the library as follows:
+To get a value by item key from a Zabbix agent or agent 2 via synchronous I/O the library can be imported and used as follows:
 
 ```python
 from zabbix_utils import Getter
 
 agent = Getter(host='127.0.0.1', port=10050)
 resp = agent.get('system.uname')
 
 print(resp.value)
 # Linux test_server 5.15.0-3.60.5.1.el9uek.x86_64
 ```
 
+The library can be used via asynchronous I/O, as in the following example:
+
+```python
+import asyncio
+from zabbix_utils import AsyncGetter
+
+async def main():
+    agent = AsyncGetter(host='127.0.0.1', port=10050)
+    resp = await agent.get('system.uname')
+
+    print(resp.value)
+    # Linux test_server 5.15.0-3.60.5.1.el9uek.x86_64
+
+asyncio.run(main())
+```
+
 > Please, refer to the [Zabbix agent protocol](https://www.zabbix.com/documentation/current/manual/appendix/protocols/zabbix_agent) and the [using examples](https://github.com/zabbix/python-zabbix-utils/tree/main/examples/get) for more information.
 
 ### Enabling debug log
 
 If it needed to debug some issue with Zabbix API, sender or get you can enable the output of logging. The **zabbix_utils** library uses the default python logging module, but it doesn't log by default. You can define logging handler to see records from the library, for example:
 
 ```python
```

### Comparing `zabbix_utils-1.1.1/setup.py` & `zabbix_utils-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,25 +42,33 @@
     long_description_content_type="text/markdown",
     keywords="monitoring zabbix api sender get utils tools",
     url="https://github.com/zabbix/python-zabbix-utils",
     test_suite='tests',
     packages=["zabbix_utils"],
     tests_require=["unittest"],
     install_requires=[],
+    extras_require={
+        "async": ["aiohttp>=3,<4"],
+    },
     python_requires='>=3.8',
     project_urls={
         'Zabbix': 'https://www.zabbix.com/documentation/current',
         'Source': 'https://github.com/zabbix/python-zabbix-utils',
         'Changes': 'https://github.com/zabbix/python-zabbix-utils/blob/main/CHANGELOG.md',
         'Bug Tracker': 'https://github.com/zabbix/python-zabbix-utils/issues'
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: System :: Monitoring",
         "Topic :: System :: Networking :: Monitoring",
         "Topic :: System :: Systems Administration",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
```

### Comparing `zabbix_utils-1.1.1/zabbix_utils/__init__.py` & `zabbix_utils-2.0.0/zabbix_utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,38 @@
 # OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 
-from .api import ZabbixAPI, APIVersion
-from .sender import Sender, ItemValue
+from .api import ZabbixAPI
+from .sender import Sender
 from .getter import Getter
+from .types import ItemValue, APIVersion
 from .exceptions import ModuleBaseException, APIRequestError, APINotSupported, ProcessingError
 
+from .aiosender import AsyncSender
+from .aiogetter import AsyncGetter
+try:
+    __import__('aiohttp')
+except ModuleNotFoundError:
+    class AsyncZabbixAPI():
+        def __init__(self, *args, **kwargs):
+            raise ModuleNotFoundError("No module named 'aiohttp'")
+else:
+    from .aioapi import AsyncZabbixAPI
+
 __all__ = (
     'ZabbixAPI',
+    'AsyncZabbixAPI',
     'APIVersion',
     'Sender',
+    'AsyncSender',
     'ItemValue',
     'Getter',
+    'AsyncGetter',
     'ModuleBaseException',
     'APIRequestError',
     'APINotSupported',
     'ProcessingError'
 )
```

### Comparing `zabbix_utils-1.1.1/zabbix_utils/api.py` & `zabbix_utils-2.0.0/zabbix_utils/aioapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,34 +18,35 @@
 # OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 
-import re
 import ssl
 import json
 import base64
+import aiohttp
 import logging
-import urllib.request as ul
-from textwrap import shorten
 
 from uuid import uuid4
+import urllib.request as ul
+from textwrap import shorten
 from os import environ as env
-from urllib.error import URLError
 
-from typing import Callable, Union, Any, List
+from urllib.error import URLError
+from typing import Callable, Union, Optional, Any, List
+from aiohttp.client_exceptions import ContentTypeError
 
+from .types import APIVersion
 from .common import ModuleUtils
 from .logger import EmptyHandler, SensitiveFilter
 from .exceptions import APIRequestError, APINotSupported, ProcessingError
 from .version import __version__, __min_supported__, __max_supported__
 
-
 log = logging.getLogger(__name__)
 log.addHandler(EmptyHandler())
 log.addFilter(SensitiveFilter())
 
 
 class APIObject():
     """Zabbix API object.
@@ -72,261 +73,167 @@
             Callable: Zabbix API method.
         """
 
         # For compatibility with Python less 3.9 versions
         def removesuffix(string: str, suffix: str) -> str:
             return str(string[:-len(suffix)]) if suffix and string.endswith(suffix) else string
 
-        def func(*args: Any, **kwargs: Any) -> Any:
+        async def func(*args: Any, **kwargs: Any) -> Any:
             if args and kwargs:
-                raise TypeError("Only args or kwargs should be used.")
+                await self.__exception(TypeError("Only args or kwargs should be used."))
 
             # Support '_' suffix to avoid conflicts with python keywords
             method = removesuffix(self.object, '_') + "." + removesuffix(name, '_')
 
             log.debug("Executing %s method", method)
 
             need_auth = method not in ModuleUtils.UNAUTH_METHODS
 
-            return self.parent.send_api_request(
+            response = await self.parent.send_async_request(
                 method,
                 args or kwargs,
                 need_auth
-            ).get('result')
+            )
+            return response.get('result')
 
         return func
 
 
-class APIVersion():
-    """Zabbix API version object.
-
-    Args:
-        apiver (str): Raw version in string format.
-    """
-
-    def __init__(self, apiver: str):
-        self.__raw = apiver
-        self.__first, self.__second, self.__third = self.__parse_version(self.__raw)
-
-    def __getitem__(self, index: int) -> Any:
-        # Get a symbol from the raw version string by index
-        # For compatibility with using Zabbix version as a string
-        return self.__raw[index]
-
-    def is_lts(self) -> bool:
-        """Check if the current version is LTS.
-
-        Returns:
-            bool: `True` if the current version is LTS.
-        """
-
-        return self.__second == 0
-
-    @property
-    def major(self) -> float:
-        """Get major version number.
-
-        Returns:
-            float: A major version number.
-        """
-
-        return float(f"{self.__first}.{self.__second}")
-
-    @property
-    def minor(self) -> int:
-        """Get minor version number.
-
-        Returns:
-            int: A minor version number.
-        """
-
-        return self.__third
-
-    def __parse_version(self, ver: str) -> List[Any]:
-        # Parse the version string into a list of integers.
-        match = re.fullmatch(r'(\d+)\.(\d+)\.(\d+)', ver)
-        if match is None:
-            raise ValueError(
-                f"Unable to parse version of Zabbix API: {ver}. " +
-                f"Default '{__max_supported__}.0' format is expected."
-            ) from None
-        return list(map(int, match.groups()))
-
-    def __str__(self) -> str:
-        return self.__raw
-
-    def __repr__(self) -> str:
-        return self.__raw
-
-    def __eq__(self, other: Union[float, str]) -> bool:
-        if isinstance(other, float):
-            return self.major == other
-        if isinstance(other, str):
-            return [self.__first, self.__second, self.__third] == self.__parse_version(other)
-        raise TypeError(
-            f"'==' not supported between instances of '{type(self).__name__}' and \
-'{type(other).__name__}', only 'float' or 'str' is expected"
-        )
-
-    def __gt__(self, other: Union[float, str]) -> bool:
-        if isinstance(other, float):
-            return self.major > other
-        if isinstance(other, str):
-            return [self.__first, self.__second, self.__third] > self.__parse_version(other)
-        raise TypeError(
-            f"'>' not supported between instances of '{type(self).__name__}' and \
-'{type(other).__name__}', only 'float' or 'str' is expected"
-        )
-
-    def __lt__(self, other: Union[float, str]) -> bool:
-        if isinstance(other, float):
-            return self.major < other
-        if isinstance(other, str):
-            return [self.__first, self.__second, self.__third] < self.__parse_version(other)
-        raise TypeError(
-            f"'<' not supported between instances of '{type(self).__name__}' and \
-'{type(other).__name__}', only 'float' or 'str' is expected"
-        )
-
-    def __ne__(self, other: Any) -> bool:
-        return not self.__eq__(other)
-
-    def __ge__(self, other: Any) -> bool:
-        return not self.__lt__(other)
-
-    def __le__(self, other: Any) -> bool:
-        return not self.__gt__(other)
-
-
-class ZabbixAPI():
-    """Provide interface for working with Zabbix API.
+class AsyncZabbixAPI():
+    """Provide asynchronous interface for working with Zabbix API.
 
     Args:
         url (str, optional): Zabbix API URL. Defaults to `http://localhost/zabbix/api_jsonrpc.php`.
-        token (str, optional): Zabbix API token. Defaults to `None`.
-        user (str, optional): Zabbix API username. Defaults to `None`.
-        password (str, optional): Zabbix API user's password. Defaults to `None`.
         http_user (str, optional): Basic Authentication username. Defaults to `None`.
         http_password (str, optional): Basic Authentication password. Defaults to `None`.
         skip_version_check (bool, optional): Skip version compatibility check. Defaults to `False`.
         validate_certs (bool, optional): Specifying certificate validation. Defaults to `True`.
+        client_session (aiohttp.ClientSession, optional): Client's session. Defaults to `None`.
         timeout (int, optional): Connection timeout to Zabbix API. Defaults to `30`.
     """
 
     __version = None
     __use_token = False
     __session_id = None
-    __basic_cred = None
+    __internal_client = None
 
-    def __init__(self, url: Union[str, None] = None, token: Union[str, None] = None,
-                 user: Union[str, None] = None, password: Union[str, None] = None,
-                 http_user: Union[str, None] = None, http_password: Union[str, None] = None,
-                 skip_version_check: bool = False, validate_certs: bool = True, timeout: int = 30):
+    def __init__(self, url: Optional[str] = None,
+                 http_user: Optional[str] = None, http_password: Optional[str] = None,
+                 skip_version_check: bool = False, validate_certs: bool = True,
+                 client_session: Optional[aiohttp.ClientSession] = None, timeout: int = 30):
 
         url = url or env.get('ZABBIX_URL') or 'http://localhost/zabbix/api_jsonrpc.php'
-        user = user or env.get('ZABBIX_USER') or None
-        password = password or env.get('ZABBIX_PASSWORD') or None
-        token = token or env.get('ZABBIX_TOKEN') or None
 
         self.url = ModuleUtils.check_url(url)
         self.validate_certs = validate_certs
         self.timeout = timeout
 
-        if http_user and http_password:
-            self.__basic_auth(http_user, http_password)
+        client_params: dict = {}
 
-        self.__check_version(skip_version_check)
+        if client_session is None:
+            client_params["connector"] = aiohttp.TCPConnector(
+                ssl=self.validate_certs
+            )
+            if http_user and http_password:
+                client_params["auth"] = aiohttp.BasicAuth(
+                    login=http_user,
+                    password=http_password
+                )
+            self.__internal_client = aiohttp.ClientSession(**client_params)
+            self.client_session = self.__internal_client
+        else:
+            if http_user and http_password:
+                raise AttributeError(
+                    "Parameters http_user/http_password shouldn't be used with client_session"
+                )
+            self.client_session = client_session
 
-        if token or user or password:
-            self.login(token, user, password)
+        self.__check_version(skip_version_check)
 
     def __getattr__(self, name: str) -> Callable:
         """Dynamic creation of an API object.
 
         Args:
             name (str): Zabbix API method name.
 
         Returns:
             APIObject: Zabbix API object instance.
         """
 
         return APIObject(name, self)
 
-    def __enter__(self) -> Callable:
+    async def __aenter__(self) -> Callable:
         return self
 
-    def __exit__(self, *args) -> None:
-        self.logout()
+    async def __aexit__(self, *args) -> None:
+        await self.logout()
 
-    def __basic_auth(self, user: str, password: str) -> None:
-        """Enable Basic Authentication using.
-
-        Args:
-            user (str): Basic Authentication username.
-            password (str): Basic Authentication password.
-        """
-
-        log.debug(
-            "Enable Basic Authentication with username:%s password:%s",
-            user,
-            ModuleUtils.HIDING_MASK
-        )
-
-        self.__basic_cred = base64.b64encode(
-            f"{user}:{password}".encode()
-        ).decode()
+    async def __close_session(self) -> None:
+        if self.__internal_client:
+            await self.__internal_client.close()
+
+    async def __exception(self, exc) -> None:
+        await self.__close_session()
+        raise exc from exc
 
     def api_version(self) -> APIVersion:
         """Return object of Zabbix API version.
 
         Returns:
             APIVersion: Object of Zabbix API version
         """
 
         if self.__version is None:
-            self.__version = APIVersion(self.apiinfo.version())
+            self.__version = APIVersion(
+                self.send_sync_request('apiinfo.version', {}, False).get('result')
+            )
         return self.__version
 
     @property
     def version(self) -> APIVersion:
         """Return object of Zabbix API version.
 
         Returns:
             APIVersion: Object of Zabbix API version.
         """
 
         return self.api_version()
 
-    def login(self, token: Union[str, None] = None, user: Union[str, None] = None,
-              password: Union[str, None] = None) -> None:
+    async def login(self, token: Optional[str] = None, user: Optional[str] = None,
+                    password: Optional[str] = None) -> None:
         """Login to Zabbix API.
 
         Args:
             token (str, optional): Zabbix API token. Defaults to `None`.
             user (str, optional): Zabbix API username. Defaults to `None`.
             password (str, optional): Zabbix API user's password. Defaults to `None`.
         """
 
+        user = user or env.get('ZABBIX_USER') or None
+        password = password or env.get('ZABBIX_PASSWORD') or None
+        token = token or env.get('ZABBIX_TOKEN') or None
+
         if token:
             if self.version < 5.4:
-                raise APINotSupported(
+                await self.__exception(APINotSupported(
                     message="Token usage",
                     version=self.version
-                )
+                ))
             if user or password:
-                raise ProcessingError(
-                    "Token cannot be used with username and password")
+                await self.__exception(
+                    ProcessingError("Token cannot be used with username and password")
+                )
             self.__use_token = True
             self.__session_id = token
             return
 
         if not user:
-            raise ProcessingError("Username is missing")
+            await self.__exception(ProcessingError("Username is missing"))
         if not password:
-            raise ProcessingError("User password is missing")
+            await self.__exception(ProcessingError("User password is missing"))
 
         if self.version < 5.4:
             user_cred = {
                 "user": user,
                 "password": password
             }
         else:
@@ -335,71 +242,58 @@
                 "password": password
             }
 
         log.debug(
             "Login to Zabbix API using username:%s password:%s", user, ModuleUtils.HIDING_MASK
         )
         self.__use_token = False
-        self.__session_id = self.user.login(**user_cred)
+        self.__session_id = await self.user.login(**user_cred)
 
         log.debug("Connected to Zabbix API version %s: %s", self.version, self.url)
 
-    def logout(self) -> None:
+    async def logout(self) -> None:
         """Logout from Zabbix API."""
 
         if self.__session_id:
             if self.__use_token:
                 self.__session_id = None
                 self.__use_token = False
+                await self.__close_session()
                 return
 
             log.debug("Logout from Zabbix API")
-            self.user.logout()
+            await self.user.logout()
             self.__session_id = None
+            await self.__close_session()
         else:
             log.debug("You're not logged in Zabbix API")
 
-    def check_auth(self) -> bool:
+    async def check_auth(self) -> bool:
         """Check authentication status in Zabbix API.
 
         Returns:
             bool: User authentication status (`True`, `False`)
         """
 
         if not self.__session_id:
             log.debug("You're not logged in Zabbix API")
             return False
 
         if self.__use_token:
             log.debug("Check auth session using token in Zabbix API")
-            refresh_resp = self.user.checkAuthentication(token=self.__session_id)
+            refresh_resp = await self.user.checkAuthentication(token=self.__session_id)
         else:
             log.debug("Check auth session using sessionid in Zabbix API")
-            refresh_resp = self.user.checkAuthentication(sessionid=self.__session_id)
+            refresh_resp = await self.user.checkAuthentication(sessionid=self.__session_id)
 
         return bool(refresh_resp.get('userid'))
 
-    def send_api_request(self, method: str, params: Union[dict, None] = None,
-                         need_auth=True) -> dict:
-        """Function for sending request to Zabbix API.
-
-        Args:
-            method (str): Zabbix API method name.
-            params (dict, optional): Params for request body. Defaults to `None`.
-            need_auth (bool, optional): Authorization using flag. Defaults to `False`.
-
-        Raises:
-            ProcessingError: Wrapping built-in exceptions during request processing.
-            APIRequestError: Wrapping errors from Zabbix API.
-
-        Returns:
-            dict: Dictionary with Zabbix API response.
-        """
-
-        request_json = {
+    def __prepare_request(self, method: str, params: Optional[dict] = None,
+                          need_auth=True) -> Union[dict, dict]:
+        request = {
             'jsonrpc': '2.0',
             'method': method,
             'params': params or {},
             'id': str(uuid4()),
         }
 
         headers = {
@@ -407,27 +301,115 @@
             'Content-Type': 'application/json-rpc',
             'User-Agent': f"{__name__}/{__version__}"
         }
 
         if need_auth:
             if not self.__session_id:
                 raise ProcessingError("You're not logged in Zabbix API")
-            if self.version < 6.4 or self.__basic_cred is not None:
-                request_json['auth'] = self.__session_id
+            if self.version < 6.4 or self.client_session._default_auth is not None:
+                request['auth'] = self.__session_id
             else:
                 headers["Authorization"] = f"Bearer {self.__session_id}"
 
-        if self.__basic_cred is not None:
-            headers["Authorization"] = f"Basic {self.__basic_cred}"
-
         log.debug(
             "Sending request to %s with body: %s",
             self.url,
-            request_json
+            request
+        )
+
+        return (request, headers)
+
+    def __check_response(self, method: str, response: dict) -> dict:
+        if method not in ModuleUtils.FILES_METHODS:
+            log.debug(
+                "Received response body: %s",
+                response
+            )
+        else:
+            debug_json = response.copy()
+            if debug_json.get('result'):
+                debug_json['result'] = shorten(debug_json['result'], 200, placeholder='...')
+            log.debug(
+                "Received response body (clipped): %s",
+                json.dumps(debug_json, indent=4, separators=(',', ': '))
+            )
+
+        if 'error' in response:
+            err = response['error'].copy()
+            err['body'] = response.copy()
+            raise APIRequestError(err)
+
+        return response
+
+    async def send_async_request(self, method: str, params: Optional[dict] = None,
+                                 need_auth=True) -> dict:
+        """Function for sending asynchronous request to Zabbix API.
+
+        Args:
+            method (str): Zabbix API method name.
+            params (dict, optional): Params for request body. Defaults to `None`.
+            need_auth (bool, optional): Authorization using flag. Defaults to `False`.
+
+        Raises:
+            ProcessingError: Wrapping built-in exceptions during request processing.
+            APIRequestError: Wrapping errors from Zabbix API.
+
+        Returns:
+            dict: Dictionary with Zabbix API response.
+        """
+
+        try:
+            request_json, headers = self.__prepare_request(method, params, need_auth)
+        except ProcessingError as err:
+            await self.__exception(err)
+
+        resp = await self.client_session.post(
+            self.url,
+            json=request_json,
+            headers=headers,
+            timeout=self.timeout
         )
+        resp.raise_for_status()
+
+        try:
+            resp_json = await resp.json()
+        except ContentTypeError as err:
+            await self.__exception(ProcessingError(f"Unable to connect to {self.url}:", err))
+        except ValueError as err:
+            await self.__exception(ProcessingError("Unable to parse json:", err))
+
+        try:
+            return self.__check_response(method, resp_json)
+        except APIRequestError as err:
+            await self.__exception(err)
+
+    def send_sync_request(self, method: str, params: Optional[dict] = None,
+                          need_auth=True) -> dict:
+        """Function for sending synchronous request to Zabbix API.
+
+        Args:
+            method (str): Zabbix API method name.
+            params (dict, optional): Params for request body. Defaults to `None`.
+            need_auth (bool, optional): Authorization using flag. Defaults to `False`.
+
+        Raises:
+            ProcessingError: Wrapping built-in exceptions during request processing.
+            APIRequestError: Wrapping errors from Zabbix API.
+
+        Returns:
+            dict: Dictionary with Zabbix API response.
+        """
+
+        request_json, headers = self.__prepare_request(method, params, need_auth)
+
+        basic_auth = self.client_session._default_auth
+        if basic_auth is not None:
+            headers["Authorization"] = "Basic " + base64.b64encode(
+                f"{basic_auth.login}:{basic_auth.password}".encode()
+            ).decode()
 
         req = ul.Request(
             self.url,
             data=json.dumps(request_json).encode("utf-8"),
             headers=headers,
             method='POST'
         )
@@ -445,40 +427,22 @@
             resp = ul.urlopen(req, context=ctx)
             resp_json = json.loads(resp.read().decode('utf-8'))
         except URLError as err:
             raise ProcessingError(f"Unable to connect to {self.url}:", err) from None
         except ValueError as err:
             raise ProcessingError("Unable to parse json:", err) from None
 
-        if method not in ModuleUtils.FILES_METHODS:
-            log.debug(
-                "Received response body: %s",
-                resp_json
-            )
-        else:
-            debug_json = resp_json.copy()
-            if debug_json.get('result'):
-                debug_json['result'] = shorten(debug_json['result'], 200, placeholder='...')
-            log.debug(
-                "Received response body (clipped): %s",
-                json.dumps(debug_json, indent=4, separators=(',', ': '))
-            )
-
-        if 'error' in resp_json:
-            err = resp_json['error'].copy()
-            err['body'] = request_json.copy()
-            raise APIRequestError(err)
-
-        return resp_json
+        return self.__check_response(method, resp_json)
 
     def __check_version(self, skip_check: bool) -> None:
 
         skip_check_help = "If you're sure zabbix_utils will work properly with your current \
 Zabbix version you can skip this check by \
 specifying skip_version_check=True when create ZabbixAPI object."
+
         if self.version < __min_supported__:
             if skip_check:
                 log.debug(
                     "Version of Zabbix API [%s] is less than the library supports. %s",
                     self.version,
                     "Further library use at your own risk!"
                 )
```

### Comparing `zabbix_utils-1.1.1/zabbix_utils/common.py` & `zabbix_utils-2.0.0/zabbix_utils/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,19 +22,22 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 
 import re
 import json
 import zlib
 import struct
-from typing import Match, Union
+import asyncio
+
 from textwrap import shorten
 from logging import Logger
 from socket import socket
 
+from typing import Match, Union
+
 
 class ModuleUtils():
 
     # Hidding mask for sensitive data
     HIDING_MASK = "*" * 8
 
     # The main php-file of Zabbix API
@@ -232,16 +235,16 @@
                 log.debug("Socket connection was closed before receiving expected amount of data.")
                 break
             buf += chunk
 
         return buf
 
     @classmethod
-    def parse_packet(cls, conn: socket, log: Logger, exception) -> str:
-        """Parse a received Zabbix protocol packet.
+    def parse_sync_packet(cls, conn: socket, log: Logger, exception) -> str:
+        """Parse a received synchronously Zabbix protocol packet.
 
         Args:
             conn (socket): Opened socket connection
             log (Logger): Logger object
             exception: Exception type
 
         Raises:
@@ -276,7 +279,53 @@
         # 0x02 - Using packet compression mode
         if flags & 0x02:
             response_body = zlib.decompress(cls.receive_packet(conn, datalen, log))
         else:
             response_body = cls.receive_packet(conn, datalen, log)
 
         return response_body.decode("utf-8")
+
+    @classmethod
+    async def parse_async_packet(cls, reader: asyncio.StreamReader, log: Logger, exception) -> str:
+        """Parse a received asynchronously Zabbix protocol packet.
+
+        Args:
+            reader (StreamReader): Created asyncio.StreamReader
+            log (Logger): Logger object
+            exception: Exception type
+
+        Raises:
+            exception: Depends on input exception type
+
+        Returns:
+            str: Body of the received packet
+        """
+
+        response_header = await reader.readexactly(cls.HEADER_SIZE)
+        log.debug('Zabbix response header: %s', response_header)
+
+        if (not response_header.startswith(cls.ZABBIX_PROTOCOL) or
+                len(response_header) != cls.HEADER_SIZE):
+            log.debug('Unexpected response was received from Zabbix.')
+            raise exception('Unexpected response was received from Zabbix.')
+
+        flags, datalen, reserved = struct.unpack('<BII', response_header[4:])
+
+        # 0x01 - Zabbix communications protocol
+        if not flags & 0x01:
+            raise exception(
+                'Unexcepted flags were received. '
+                'Check debug log for more information.'
+            )
+        # 0x04 - Using large packet mode
+        if flags & 0x04:
+            raise exception(
+                'A large packet flag was received. '
+                'Current module doesn\'t support large packets.'
+            )
+        # 0x02 - Using packet compression mode
+        if flags & 0x02:
+            response_body = zlib.decompress(await reader.readexactly(datalen))
+        else:
+            response_body = await reader.readexactly(datalen)
+
+        return response_body.decode("utf-8")
```

### Comparing `zabbix_utils-1.1.1/zabbix_utils/exceptions.py` & `zabbix_utils-2.0.0/zabbix_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `zabbix_utils-1.1.1/zabbix_utils/getter.py` & `zabbix_utils-2.0.0/zabbix_utils/getter.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,61 +18,29 @@
 # OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 
-import json
 import socket
 import logging
 from typing import Callable, Union
 
 from .logger import EmptyHandler
+from .types import AgentResponse
 from .common import ZabbixProtocol
 from .exceptions import ProcessingError
 
 log = logging.getLogger(__name__)
 log.addHandler(EmptyHandler())
 
 
-class AgentResponse:
-    """Contains response from Zabbix agent/agent2.
-
-    Args:
-        response (string): Raw response from Zabbix.
-    """
-
-    def __init__(self, response: str):
-        error_code = 'ZBX_NOTSUPPORTED'
-        self.raw = response
-        if response == error_code:
-            self.value = None
-            self.error = 'Not supported by Zabbix Agent'
-        elif response.startswith(error_code + '\0'):
-            self.value = None
-            self.error = response[len(error_code)+1:]
-        else:
-            idx = response.find('\0')
-            if idx == -1:
-                self.value = response
-            else:
-                self.value = response[:idx]
-            self.error = None
-
-    def __repr__(self) -> str:
-        return json.dumps({
-            'error': self.error,
-            'raw': self.raw,
-            'value': self.value,
-        })
-
-
 class Getter():
-    """Zabbix get implementation.
+    """Zabbix get synchronous implementation.
 
     Args:
         host (str, optional): Zabbix agent address. Defaults to `'127.0.0.1'`.
 
         port (int, optional): Zabbix agent port. Defaults to `10050`.
 
         timeout (int, optional): Connection timeout value. Defaults to `10`.
@@ -95,15 +63,15 @@
 
         self.socket_wrapper = socket_wrapper
         if self.socket_wrapper:
             if not isinstance(self.socket_wrapper, Callable):
                 raise TypeError('Value "socket_wrapper" should be a function.')
 
     def __get_response(self, conn: socket) -> Union[str, None]:
-        result = ZabbixProtocol.parse_packet(conn, log, ProcessingError)
+        result = ZabbixProtocol.parse_sync_packet(conn, log, ProcessingError)
 
         log.debug('Received data: %s', result)
 
         return result
 
     def get(self, key: str) -> Union[str, None]:
         """Gets item value from Zabbix agent by specified key.
```

### Comparing `zabbix_utils-1.1.1/zabbix_utils/logger.py` & `zabbix_utils-2.0.0/zabbix_utils/logger.py`

 * *Files identical despite different names*

### Comparing `zabbix_utils-1.1.1/zabbix_utils/version.py` & `zabbix_utils-2.0.0/zabbix_utils/version.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 # OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 # HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 # OTHER DEALINGS IN THE SOFTWARE.
 
-__version__ = "1.1.1"
+__version__ = "2.0.0"
 
 __min_supported__ = 5.0
 __max_supported__ = 7.0
```

### Comparing `zabbix_utils-1.1.1/zabbix_utils.egg-info/PKG-INFO` & `zabbix_utils-2.0.0/zabbix_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 Metadata-Version: 2.1
 Name: zabbix-utils
-Version: 1.1.1
+Version: 2.0.0
 Summary: A library with modules for working with Zabbix (Zabbix API, Zabbix sender, Zabbix get)
 Home-page: https://github.com/zabbix/python-zabbix-utils
 Author: Zabbix SIA
 Author-email: integrationteam@zabbix.com
 Maintainer: Aleksandr Iantsen
 Maintainer-email: aleksandr.iantsen@zabbix.com
 Project-URL: Zabbix, https://www.zabbix.com/documentation/current
 Project-URL: Source, https://github.com/zabbix/python-zabbix-utils
 Project-URL: Changes, https://github.com/zabbix/python-zabbix-utils/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/zabbix/python-zabbix-utils/issues
 Keywords: monitoring zabbix api sender get utils tools
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Systems Administration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: async
 License-File: LICENSE
 
 # Zabbix utils library
 
 [![Tests](https://github.com/zabbix/python-zabbix-utils/actions/workflows/tests.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/tests.yaml)
 [![Zabbix API](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_api.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_api.yaml)
 [![Zabbix sender](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_sender.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_sender.yaml)
-[![Zabbix get](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_get.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_get.yaml)
+[![Zabbix get](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_getter.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/integration_getter.yaml)
 [![Zabbix 5.0](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_50.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_50.yaml)
 [![Zabbix 6.0](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_60.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_60.yaml)
 [![Zabbix 6.4](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_64.yaml/badge.svg)](https://github.com/zabbix/python-zabbix-utils/actions/workflows/compatibility_64.yaml)
 
 **zabbix_utils** is a Python library for working with [Zabbix API](https://www.zabbix.com/documentation/current/manual/api/reference) as well as with [Zabbix sender](https://www.zabbix.com/documentation/current/manpages/zabbix_sender) and [Zabbix get](https://www.zabbix.com/documentation/current/manpages/zabbix_get) protocols.
 
 ## Requirements
@@ -47,29 +53,39 @@
 * Python 3.8+
 
 Tested on:
 
 * Zabbix 5.0, 6.0, 6.4 and pre-7.0
 * Python 3.8, 3.9, 3.10, 3.11 and 3.12
 
+Dependencies:
+
+* [aiohttp](https://github.com/aio-libs/aiohttp) (in case of async use)
+
 ## Documentation
 
 ### Installation
 
 Install **zabbix_utils** library using pip:
 
 ```bash
 $ pip install zabbix_utils
 ```
 
+To install the library with dependencies for asynchronous work use the following way:
+
+```bash
+$ pip install zabbix_utils[async]
+```
+
 ### Use cases
 
 ##### To work with Zabbix API
 
-To work with Zabbix API you can import and use **zabbix_utils** library as follows:
+To work with Zabbix API via synchronous I/O you can import and use **zabbix_utils** library as follows:
 
 ```python
 from zabbix_utils import ZabbixAPI
 
 api = ZabbixAPI(url="127.0.0.1")
 api.login(user="User", password="zabbix")
 
@@ -79,46 +95,56 @@
 
 for user in users:
     print(user['name'])
 
 api.logout()
 ```
 
-You can also authenticate using an API token (supported since Zabbix 5.4):
+To work with Zabbix API via asynchronous I/O you can use the following way:
 
 ```python
-from zabbix_utils import ZabbixAPI
+import asyncio
+from zabbix_utils import AsyncZabbixAPI
+
+async def main():
+    api = AsyncZabbixAPI(url="127.0.0.1")
+    await api.login(user="User", password="zabbix")
+
+    users = await api.user.get(
+        output=['userid','name']
+    )
+
+    for user in users:
+        print(user['name'])
+
+    await api.logout()
 
+asyncio.run(main())
+```
+
+You can also authenticate using an API token (supported since Zabbix 5.4):
+
+```python
 api = ZabbixAPI(url="127.0.0.1")
 api.login(token="xxxxxxxx")
+```
 
-users = api.user.get(
-    output=['userid','name']
-)
-
-for user in users:
-    print(user['name'])
+```python
+api = AsyncZabbixAPI(url="127.0.0.1")
+await api.login(token="xxxxxxxx")
 ```
 
 When token is used, calling `api.logout()` is not necessary.
 
 It is possible to specify authentication fields by the following environment variables:
 `ZABBIX_URL`, `ZABBIX_TOKEN`, `ZABBIX_USER`, `ZABBIX_PASSWORD`
 
 You can compare Zabbix API version with strings and numbers, for example:
 
 ```python
-from zabbix_utils import ZabbixAPI
-
-url = "127.0.0.1"
-user = "User"
-password = "zabbix"
-
-api = ZabbixAPI(url=url, user=user, password=password)
-
 # Method to get version
 ver = api.api_version()
 print(type(ver).__name__, ver) # APIVersion 7.0.0
 
 # ZabbixAPI prototype with version
 ver = api.version
 print(type(ver).__name__, ver) # APIVersion 7.0.0
@@ -128,19 +154,17 @@
 print(ver != 7.0)     # False
 print(ver != "7.0.0") # False
 
 # Version additional methods
 print(ver.major)    # 7.0
 print(ver.minor)    # 0
 print(ver.is_lts()) # True
-
-api.logout()
 ```
 
-In case the API object or method name matches one of Python keywords, you can use the suffix `_` in their name to execute correctly:
+In case the API object or method name matches one of Python keywords, you can use the suffix `_` in their name to execute correctly, for example:
 ```python
 from zabbix_utils import ZabbixAPI
 
 api = ZabbixAPI(url="127.0.0.1")
 api.login(token="xxxxxxxx")
 
 template_source = ''
@@ -169,15 +193,31 @@
 sender = Sender(server='127.0.0.1', port=10051)
 response = sender.send_value('host', 'item.key', 'value', 1695713666)
 
 print(response)
 # {"processed": 1, "failed": 0, "total": 1, "time": "0.000338", "chunk": 1}
 ```
 
-Or you can prepare a list of item values and send all at once:
+The asynchronous way:
+
+```python
+import asyncio
+from zabbix_utils import AsyncSender
+
+async def main():
+    sender = AsyncSender(server='127.0.0.1', port=10051)
+    response = await sender.send_value('host', 'item.key', 'value', 1695713666)
+
+    print(response)
+    # {"processed": 1, "failed": 0, "total": 1, "time": "0.000338", "chunk": 1}
+
+asyncio.run(main())
+```
+
+You can also prepare a list of item values and send all at once:
 
 ```python
 from zabbix_utils import ItemValue, Sender
 
 items = [
     ItemValue('host1', 'item.key1', 10),
     ItemValue('host1', 'item.key2', 'test message'),
@@ -218,26 +258,42 @@
 
 In such case, the value will be sent to the first available node of each cluster.
 
 > Please, refer to the [Zabbix sender protocol](https://www.zabbix.com/documentation/current/manual/appendix/protocols/zabbix_sender) and the [using examples](https://github.com/zabbix/python-zabbix-utils/tree/main/examples/sender) for more information.
 
 ##### To work via Zabbix get protocol
 
-To get a value by item key from a Zabbix agent or agent 2 you can import and use the library as follows:
+To get a value by item key from a Zabbix agent or agent 2 via synchronous I/O the library can be imported and used as follows:
 
 ```python
 from zabbix_utils import Getter
 
 agent = Getter(host='127.0.0.1', port=10050)
 resp = agent.get('system.uname')
 
 print(resp.value)
 # Linux test_server 5.15.0-3.60.5.1.el9uek.x86_64
 ```
 
+The library can be used via asynchronous I/O, as in the following example:
+
+```python
+import asyncio
+from zabbix_utils import AsyncGetter
+
+async def main():
+    agent = AsyncGetter(host='127.0.0.1', port=10050)
+    resp = await agent.get('system.uname')
+
+    print(resp.value)
+    # Linux test_server 5.15.0-3.60.5.1.el9uek.x86_64
+
+asyncio.run(main())
+```
+
 > Please, refer to the [Zabbix agent protocol](https://www.zabbix.com/documentation/current/manual/appendix/protocols/zabbix_agent) and the [using examples](https://github.com/zabbix/python-zabbix-utils/tree/main/examples/get) for more information.
 
 ### Enabling debug log
 
 If it needed to debug some issue with Zabbix API, sender or get you can enable the output of logging. The **zabbix_utils** library uses the default python logging module, but it doesn't log by default. You can define logging handler to see records from the library, for example:
 
 ```python
```

