# Comparing `tmp/signal_bot_framework-0.1.0.tar.gz` & `tmp/signal_bot_framework-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal_bot_framework-0.1.0.tar", last modified: Fri Sep  1 18:54:25 2023, max compression
+gzip compressed data, was "signal_bot_framework-0.2.tar", last modified: Fri Apr 12 19:28:56 2024, max compression
```

## Comparing `signal_bot_framework-0.1.0.tar` & `signal_bot_framework-0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-09-01 18:54:25.680081 signal_bot_framework-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-09-01 18:09:06.000000 signal_bot_framework-0.1.0/COPYING
--rw-rw-rw-   0        0        0    35823 2023-09-01 18:09:06.000000 signal_bot_framework-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    45936 2023-09-01 18:54:25.680081 signal_bot_framework-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3826 2023-09-01 18:44:38.000000 signal_bot_framework-0.1.0/README.md
--rw-rw-rw-   0        0        0     1274 2023-09-01 18:42:56.000000 signal_bot_framework-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-01 18:54:25.680081 signal_bot_framework-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-01 18:54:25.663563 signal_bot_framework-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-09-01 18:54:25.675084 signal_bot_framework-0.1.0/src/signal_bot_framework/
--rw-rw-rw-   0        0        0     2031 2023-09-01 18:49:45.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/__init__.py
--rw-rw-rw-   0        0        0     9821 2023-08-06 17:33:48.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/_signal_impl.py
--rw-rw-rw-   0        0        0      963 2023-09-01 18:06:25.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/_util.py
--rw-rw-rw-   0        0        0     1861 2023-09-01 18:50:22.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/aliases.py
--rw-rw-rw-   0        0        0     2283 2023-07-30 17:36:14.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/args.py
--rw-rw-rw-   0        0        0      407 2023-09-01 18:50:26.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/constants.py
--rw-rw-rw-   0        0        0      396 2023-09-01 18:50:32.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/exceptions.py
--rw-rw-rw-   0        0        0     8388 2023-09-01 18:50:47.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/personality.py
--rw-rw-rw-   0        0        0     6964 2023-09-01 18:51:04.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/protocol.py
--rw-rw-rw-   0        0        0     6854 2023-09-01 18:51:05.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/transport.py
--rw-rw-rw-   0        0        0     5289 2023-09-01 18:51:07.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/types.py
--rw-rw-rw-   0        0        0      178 2023-08-06 17:33:48.000000 signal_bot_framework-0.1.0/src/signal_bot_framework/version.py
-drwxrwxrwx   0        0        0        0 2023-09-01 18:54:25.679077 signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/
--rw-rw-rw-   0        0        0    45936 2023-09-01 18:54:25.000000 signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      722 2023-09-01 18:54:25.000000 signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-01 18:54:25.000000 signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-09-01 18:54:25.000000 signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-09-01 18:54:25.000000 signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 19:28:56.032011 signal_bot_framework-0.2/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 18:09:06.000000 signal_bot_framework-0.2/COPYING
+-rw-rw-rw-   0        0        0    35823 2023-09-01 18:09:06.000000 signal_bot_framework-0.2/LICENSE
+-rw-rw-rw-   0        0        0    46548 2024-04-12 19:28:56.030269 signal_bot_framework-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3838 2024-04-12 18:07:42.000000 signal_bot_framework-0.2/README.md
+-rw-rw-rw-   0        0        0     1301 2024-04-12 19:23:44.000000 signal_bot_framework-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 19:28:56.032011 signal_bot_framework-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 19:28:56.007315 signal_bot_framework-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 19:28:56.023301 signal_bot_framework-0.2/src/signal_bot_framework/
+-rw-rw-rw-   0        0        0     2003 2024-04-12 18:07:24.000000 signal_bot_framework-0.2/src/signal_bot_framework/__init__.py
+-rw-rw-rw-   0        0        0     9715 2024-04-12 17:52:44.000000 signal_bot_framework-0.2/src/signal_bot_framework/_signal_impl.py
+-rw-rw-rw-   0        0        0      963 2023-09-01 18:06:25.000000 signal_bot_framework-0.2/src/signal_bot_framework/_util.py
+-rw-rw-rw-   0        0        0     1861 2024-04-12 18:47:49.000000 signal_bot_framework-0.2/src/signal_bot_framework/aliases.py
+-rw-rw-rw-   0        0        0     2283 2023-07-30 17:36:14.000000 signal_bot_framework-0.2/src/signal_bot_framework/args.py
+-rw-rw-rw-   0        0        0      407 2023-09-01 18:50:26.000000 signal_bot_framework-0.2/src/signal_bot_framework/constants.py
+-rw-rw-rw-   0        0        0      396 2023-09-01 18:50:32.000000 signal_bot_framework-0.2/src/signal_bot_framework/exceptions.py
+-rw-rw-rw-   0        0        0     8305 2024-04-12 18:15:39.000000 signal_bot_framework-0.2/src/signal_bot_framework/personality.py
+-rw-rw-rw-   0        0        0     7553 2024-04-12 19:04:20.000000 signal_bot_framework-0.2/src/signal_bot_framework/protocol.py
+-rw-rw-rw-   0        0        0     6854 2023-09-01 18:51:05.000000 signal_bot_framework-0.2/src/signal_bot_framework/transport.py
+-rw-rw-rw-   0        0        0     5395 2024-04-12 19:15:30.000000 signal_bot_framework-0.2/src/signal_bot_framework/types.py
+-rw-rw-rw-   0        0        0      172 2024-04-12 17:52:44.000000 signal_bot_framework-0.2/src/signal_bot_framework/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 19:28:56.028530 signal_bot_framework-0.2/src/signal_bot_framework.egg-info/
+-rw-rw-rw-   0        0        0    46548 2024-04-12 19:28:55.000000 signal_bot_framework-0.2/src/signal_bot_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2024-04-12 19:28:56.000000 signal_bot_framework-0.2/src/signal_bot_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 19:28:55.000000 signal_bot_framework-0.2/src/signal_bot_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      225 2024-04-12 19:28:55.000000 signal_bot_framework-0.2/src/signal_bot_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-12 19:28:55.000000 signal_bot_framework-0.2/src/signal_bot_framework.egg-info/top_level.txt
```

### Comparing `signal_bot_framework-0.1.0/COPYING` & `signal_bot_framework-0.2/COPYING`

 * *Files identical despite different names*

### Comparing `signal_bot_framework-0.1.0/LICENSE` & `signal_bot_framework-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `signal_bot_framework-0.1.0/PKG-INFO` & `signal_bot_framework-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal_bot_framework
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python module for building Signal.org bots that interact with signal-cli.
 Author-email: Sidneys1 <sidneys1@proton.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,18 +686,31 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Communications :: Chat
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
 License-File: LICENSE
 License-File: COPYING
+Requires-Dist: cron-converter~=1.0.2
+Requires-Dist: humanize~=4.6.0
+Provides-Extra: dev
+Requires-Dist: pylint~=2.17.5; extra == "dev"
+Requires-Dist: yapf~=0.40.1; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: sphinx~=7.2.6; extra == "docs"
+Requires-Dist: myst-parser~=2.0.0; extra == "docs"
+Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
+Requires-Dist: sphinx-paramlinks~=0.6.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints~=1.23.0; extra == "docs"
+Requires-Dist: setuptools; extra == "docs"
 
 # Signal-Bot
 
 An `asyncio` Python 3.11 module for building [Signal][signal] bots that interact with [AsamK/signal-cli][signal-cli].
 
 ## Features
 
@@ -720,29 +733,29 @@
 ## Usage
 
 For development: `python3.11 -m pip install signal_bot_framework`.
 
 ```py
 # test_bot.py
 import asyncio
-from signal_bot_framework import create, Account
+from signal_bot_framework import create, AccountNumber
 
 async def crabby_callback(signal: Signal, context: Context, message: DataMessage) -> bool:
         to = context[1]
         await signal.send_reaction(message, "🦀")
         await signal.send_message(to, f"Sorry, just feeling a little crabby, {message.sender_name}.",
                                   args=SendMessageArgs(mention=[f"37:{len(message.sender_name)}:{message.sender}"]))
         return True
 
 async def main():
     # The default, finds `signal-cli` on path and launches it as a subprocess
     connection = 'ipc://'
     # or, use TCP: connection = 'tcp://HOST:PORT'
 
-    signal = await create(Account('+12345678900'), connection)
+    signal = await create(AccountNumber('+12345678900'), connection)
     signal.on_keyword('ok?', crabby_callback)
     await signal.run()
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
```

### Comparing `signal_bot_framework-0.1.0/README.md` & `signal_bot_framework-0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 ## Usage
 
 For development: `python3.11 -m pip install signal_bot_framework`.
 
 ```py
 # test_bot.py
 import asyncio
-from signal_bot_framework import create, Account
+from signal_bot_framework import create, AccountNumber
 
 async def crabby_callback(signal: Signal, context: Context, message: DataMessage) -> bool:
         to = context[1]
         await signal.send_reaction(message, "🦀")
         await signal.send_message(to, f"Sorry, just feeling a little crabby, {message.sender_name}.",
                                   args=SendMessageArgs(mention=[f"37:{len(message.sender_name)}:{message.sender}"]))
         return True
 
 async def main():
     # The default, finds `signal-cli` on path and launches it as a subprocess
     connection = 'ipc://'
     # or, use TCP: connection = 'tcp://HOST:PORT'
 
-    signal = await create(Account('+12345678900'), connection)
+    signal = await create(AccountNumber('+12345678900'), connection)
     signal.on_keyword('ok?', crabby_callback)
     await signal.run()
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
```

### Comparing `signal_bot_framework-0.1.0/pyproject.toml` & `signal_bot_framework-0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,56 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "signal_bot_framework"
-version = "0.1.0"
-authors = [
-  { name="Sidneys1", email="sidneys1@proton.me" },
-]
-description = "A Python module for building Signal.org bots that interact with signal-cli."
-readme = "README.md"
-license = {file = "LICENSE"}
-requires-python = ">=3.11"
-keywords = ["signal", "signal-cli", "bot"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Topic :: Communications :: Chat",
-    "Typing :: Typed",
-]
-dependencies = [
-  "cron-converter~=1.0.2",
-  "humanize~=4.6.0"
-]
-
-[project.optional-dependencies]
-dev = [
-  "pylint~=2.17.5",
-  "yapf~=0.40.1"
-]
-
-docs = [
-  "sphinx~=6.2.1",
-  "myst-parser~=2.0.0",
-  "sphinx-paramlinks~=0.5.4",
-  "sphinx-autodoc-typehints~=1.23.0"
-]
-
-[project.urls]
-Documentation = "https://signal-bot.readthedocs.io/"
-Repository = "https://github.com/Sidneys1/signal-bot"
-"Bug Tracker" = "https://github.com/Sidneys1/signal-bot/issues"
-
-[tool.yapf]
-"COLUMN_LIMIT" = 120
-
-[tool.pydocstyle]
-ignore = "D107"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "signal_bot_framework"
+version = "0.2.0"
+authors = [
+  { name="Sidneys1", email="sidneys1@proton.me" },
+]
+description = "A Python module for building Signal.org bots that interact with signal-cli."
+readme = "README.md"
+license = {file = "LICENSE"}
+requires-python = ">=3.11"
+keywords = ["signal", "signal-cli", "bot"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Operating System :: OS Independent",
+    "Development Status :: 3 - Alpha",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Topic :: Communications :: Chat",
+    "Typing :: Typed",
+]
+dependencies = [
+  "cron-converter~=1.0.2",
+  "humanize~=4.6.0"
+]
+
+[project.optional-dependencies]
+dev = [
+  "pylint~=2.17.5",
+  "yapf~=0.40.1",
+  "wheel",
+  "build",
+  "twine"
+]
+
+docs = [
+  "sphinx~=7.2.6",
+  "myst-parser~=2.0.0",
+  "sphinx-rtd-theme~=2.0.0",
+  "sphinx-paramlinks~=0.6.0",
+  "sphinx-autodoc-typehints~=1.23.0",
+  "setuptools"
+]
+
+[project.urls]
+Documentation = "https://signal-bot.readthedocs.io/"
+Repository = "https://github.com/Sidneys1/signal-bot"
+"Bug Tracker" = "https://github.com/Sidneys1/signal-bot/issues"
+
+[tool.yapf]
+"COLUMN_LIMIT" = 120
+
+[tool.pydocstyle]
+ignore = "D107"
```

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework/__init__.py` & `signal_bot_framework-0.2/src/signal_bot_framework/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""
-`signal_bot_framework`: An async Signal messenger bot framework, utilizing `signal-cli`.
-
-Get started with :meth:`signal_bot_framework.create`.
-
-Looking for high-level interfaces? Check out :mod:`signal_bot_framework.protocol`.
-"""
-
-from urllib.parse import urlparse
-
-from .version import __version__
-from .types import Account
-from .protocol import SignalBot
-from .transport import JsonRpcTransport
-
-
-####################################################
-# Looking for documentation? Check out the README: #
-#      https://github.com/Sidneys1/signal-bot      #
-####################################################
-
-#################################################################
-# Looking for high-level interfaces? Check out `./protocol.py`. #
-#################################################################
-async def create(account: Account, connection: str = 'ipc://') -> SignalBot:
-    """
-    Create an instance of `SignalBot`.
-
-    :param account: The Signal account to use (e.g., `"+12345678901"`).
-    :type account: :data:`~signal_bot_framework.types.Account`
-
-    :param connection: The connection string used to communicate with `signal-cli`. See classes in
-                       :mod:`signal_bot_framework.transport` for supported forms.
-
-    :raises NotImplementedError: When the URI scheme in :paramref:`connection` is not supported by an existing
-                                 :class:`~signal_bot_framework.transport.JsonRpcTransport`.
-    """
-    parts = urlparse(connection)
-    try:
-        transport_class = JsonRpcTransport.PROTOS[parts.scheme]  # type: ignore
-    except KeyError as ex:
-        extra = ", ".join(JsonRpcTransport.PROTOS)  # type: ignore
-        raise NotImplementedError(f'Connection scheme {parts.scheme!r} has not been '
-                                  f'implemented (recognized: {extra}).') from ex
-    from ._signal_impl import SignalBotImpl
-    return SignalBotImpl(account, await transport_class.create(parts))  # type: ignore
+"""
+`signal_bot_framework`: An async Signal messenger bot framework, utilizing `signal-cli`.
+
+Get started with :meth:`signal_bot_framework.create`.
+
+Looking for high-level interfaces? Check out :mod:`signal_bot_framework.protocol`.
+"""
+
+from urllib.parse import urlparse
+
+from .version import __version__
+from .types import AccountNumber
+from .protocol import SignalBot
+from .transport import JsonRpcTransport
+
+
+####################################################
+# Looking for documentation? Check out the README: #
+#      https://github.com/Sidneys1/signal-bot      #
+####################################################
+
+#################################################################
+# Looking for high-level interfaces? Check out `./protocol.py`. #
+#################################################################
+async def create(account: AccountNumber, connection: str = 'ipc://') -> SignalBot:
+    """
+    Create an instance of `SignalBot`.
+
+    :param account: The Signal account to use (e.g., `"+12345678901"`).
+    :type account: :data:`~signal_bot_framework.types.AccountNumber`
+
+    :param connection: The connection string used to communicate with `signal-cli`. See classes in
+                       :mod:`signal_bot_framework.transport` for supported forms.
+
+    :raises NotImplementedError: When the URI scheme in :paramref:`connection` is not supported by an existing
+                                 :class:`~signal_bot_framework.transport.JsonRpcTransport`.
+    """
+    parts = urlparse(connection)
+    try:
+        transport_class = JsonRpcTransport.PROTOS[parts.scheme]  # type: ignore
+    except KeyError as ex:
+        extra = ", ".join(JsonRpcTransport.PROTOS)  # type: ignore
+        raise NotImplementedError(f'Connection scheme {parts.scheme!r} has not been '
+                                  f'implemented (recognized: {extra}).') from ex
+    from ._signal_impl import SignalBotImpl
+    return SignalBotImpl(account, await transport_class.create(parts))  # type: ignore
```

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework/_signal_impl.py` & `signal_bot_framework-0.2/src/signal_bot_framework/_signal_impl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,240 +1,233 @@
-"""Signal-Bot implementation."""
-
-import asyncio
-from asyncio import Future
-from uuid import uuid4
-from logging import Logger, getLogger
-from datetime import datetime
-from inspect import isawaitable
-from typing import Dict, Hashable, Callable, cast
-
-from .types import Account, DataMessage, Response, GroupId, ResponseFrame, NotificationFrame, EnvelopeFrame
-from .aliases import GroupContext, AnyCb, IndividualContext
-from .args import SendMessageArgs
-from .exceptions import SignalRpcException
-from .personality import Personality
-from .protocol import SignalBot, PersonalityProto, RpcRet
-from .transport import JsonRpcTransport, JsonRpcHandler
-
-
-class SignalBotImpl(SignalBot, Personality, JsonRpcHandler):
-    """Concrete implementation of `SignalBot`."""
-
-    __account: Account
-    __transport: JsonRpcTransport
-    __log: Logger = getLogger(__module__ + '.Signal')  # type: ignore
-    __start_time: datetime
-    __personalities: list[Personality]
-    __stopping = asyncio.Event()
-    __cancelable: list[asyncio.Task | asyncio.Handle]
-
-    def __init__(self, account: Account, transport: JsonRpcTransport) -> None:
-        self.__account = account
-        self.__transport = transport
-        self.__start_time = datetime.now()
-        self.__personalities = []
-        self.__cancelable = []
-        Personality.__init__(self)
-
-    # `Signal`
-
-    @property
-    def account(self) -> Account:
-        return self.__account
-
-    async def run(self) -> None:
-        self.start_crons(self)
-        for personality in self.__personalities:
-            personality.start_crons(self)
-            asyncio.ensure_future(personality.started(self))
-        try:
-            await self.__transport.listen(self)
-        except asyncio.CancelledError:
-            self.__log.debug('Transport listen loop stopped.')
-            await self.stop()
-
-    async def stop(self) -> None:
-        if self.__stopping.is_set():
-            return
-        self.__log.info("Stop requested...")
-        self.__log.debug("Stopping Crons...")
-        self.__stopping.set()
-        self.stop_crons()
-        for personality in self.__personalities:
-            personality.stop_crons()
-        self.__log.debug("Disconnecting from signal-cli...")
-        await self.__transport.terminate()
-        self.__log.debug("Canceling anything in-flight...")
-        if self.__cancelable:
-            for cancelable in self.__cancelable:
-                cancelable.cancel()
-            self.__log.debug("Waiting for cancelables to finish...")
-            await asyncio.wait([x for x in self.__cancelable if isawaitable(x)])
-        self.__log.info("Stopped.")
-        self.__stopping.clear()
-
-    #######################
-    # `SignalRpc` Methods #
-    #######################
-
-    async def send_reaction(self, to: DataMessage, emoji: str) -> Future[Response]:
-        kwargs = {}
-        if to.group_info is None:
-            kwargs['recipient'] = to.sender
-        else:
-            kwargs['groupId'] = to.group_info['groupId']  # type: ignore
-
-        return asyncio.ensure_future(
-            Response.from_future_frame(await self.__json_rpc('sendReaction',
-                                                             emoji=emoji,
-                                                             targetAuthor=to.sender,
-                                                             targetTimestamp=to.unix_timestamp,
-                                                             **kwargs)))
-
-    async def send_typing(self, to: Account | GroupId, stop=False) -> Future[Response]:
-        kwargs: dict = {('groupId' if len(to) == 44 else 'recipient'): to}
-        if stop:
-            kwargs['stop'] = True
-        return asyncio.ensure_future(Response.from_future_frame(await self.__json_rpc('sendTyping', **kwargs)))
-
-    async def send_message(self,
-                           to: Account | GroupId,
-                           message: str | None = None,
-                           args: SendMessageArgs | None = None) -> Future[Response]:
-        if (not message) and args is not None and not args.attachment:
-            raise ValueError('message cannot be empty without attachment')
-        kwargs: dict = {('groupId' if len(to) == 44 else 'recipient'): to}
-        if args is not None:
-            kwargs.update(args.to_args())
-        return asyncio.ensure_future(
-            Response.from_future_frame(await self.__json_rpc('send', message=message, **kwargs)))
-
-    async def delete_message(self, to: Account | GroupId, target_timestamp: datetime) -> RpcRet:
-        kwargs: dict = {
-            ('groupId' if len(to) == 44 else 'recipient'): to,
-            'targetTimestamp': int(target_timestamp.timestamp() * 1000)
-        }
-        return asyncio.ensure_future(Response.from_future_frame(await self.__json_rpc('remoteDelete', **kwargs)))
-
-    def add_personality(self, personality: PersonalityProto) -> None:
-        assert isinstance(personality, Personality)
-        self.__personalities.append(personality)
-
-    def handle_callback_exception(self, exception: BaseException, cb: AnyCb) -> bool:
-        callback_type, *info = cb
-        post = "" if callback_type != 'cron' else " Cron will be rescheduled for the next occurance."
-        self.__log.exception("Uncaught exception while processing a registered %r callback (addt'l info: %r).%s",
-                             callback_type,
-                             info,
-                             post,
-                             exc_info=exception,
-                             stack_info=True)
-        return True
-
-    ############################
-    # `JsonRpcHandler` Methods #
-    ############################
-
-    async def handle_response(self, response: ResponseFrame) -> None:
-        remove = next((id for id, checker in self.__WAITERS.items() if checker(response)), None)
-        if remove is not None:
-            del self.__WAITERS[remove]
-
-    async def handle_notification(self, notification: NotificationFrame) -> None:
-        match notification['method']:
-            case 'receive':
-                await self.__receive(notification)
-            case _:
-                self.__log.warning('Received unexpected JsonRPC notification method: %r', notification['method'])
-
-    #############
-    # Internals #
-    #############
-
-    async def __receive(self, message: NotificationFrame) -> None:
-        # TODO: logging
-        envelope: EnvelopeFrame = message['params'].get('envelope', None)
-        if envelope is None:
-            # TODO: logging
-            return
-
-        # source = envelope['source']
-        # source_name = envelope['sourceName'] or source
-        timestamp = datetime.fromtimestamp(envelope['timestamp'] / 1000.0)
-        if timestamp <= self.__start_time:
-            # TODO: catchup mode?
-            return
-
-        match envelope:
-            case {'typingMessage': _}:
-                # TODO: self.__handle_typing_message(envelope)
-                pass
-            case {'dataMessage': _}:
-                asyncio.create_task(self.__handle_data_message(envelope))
-            case _:
-                # TODO: logging
-                pass
-
-    async def __handle_data_message(self, envelope: EnvelopeFrame) -> None:
-        if envelope['dataMessage']['message'] is None:
-            return
-
-        message = DataMessage(envelope)
-        context: GroupContext | IndividualContext
-        if message.group_info is not None:
-            context = ('group', GroupId(message.group_info['groupId']))
-        else:
-            context = ('individual', message.sender, envelope['sourceName'])
-
-        for personality in self.__personalities:
-            if personality.matches_context(context) and await personality.personality_handle_message(
-                    self, context, message):
-                return
-        await self.personality_handle_message(self, context, message)
-
-    __WAITERS: Dict[Hashable, Callable[[ResponseFrame], bool]] = {}
-
-    async def __json_rpc(self, method: str, **params) -> Future[ResponseFrame]:
-        request_id = params.pop("request_id", str(uuid4()))
-        if not params:
-            params = {}
-
-        params.update({"account": self.__account})
-        request: NotificationFrame = {
-            'jsonrpc': '2.0',
-            'id': request_id,
-            'method': method,
-            'params': params,
-        }
-
-        loop = asyncio.get_running_loop()
-        future: Future[ResponseFrame] = loop.create_future()
-        key = object()
-
-        def cancel_timer():
-            """Cancels our RPC after a timeout"""
-            if not future.done():
-                future.set_exception(TimeoutError(f"request id {request_id!r} timed out"))
-                self.__WAITERS.pop(key, None)
-
-        t_handle = loop.call_later(5.0, cancel_timer)
-        self.__cancelable.append(t_handle)
-
-        def check_return(ret: ResponseFrame) -> bool:
-            if ret['id'] != request_id:
-                return False
-            match ret:
-                case {'error': error}:
-                    self.__log.debug("Setting exception %r", error)
-                    future.set_exception(SignalRpcException(error['message'], cast(dict, ret)))
-                case _:
-                    self.__log.debug("Setting result %r", ret)
-                    future.set_result(ret)
-            t_handle.cancel()
-            self.__cancelable.remove(t_handle)
-            return True
-
-        self.__WAITERS[key] = check_return
-        self.__log.debug(request)
-        self.__cancelable.append(loop.create_task(self.__transport.write(request)))
-        return future
+"""Signal-Bot implementation."""
+
+import asyncio
+from asyncio import Future
+from uuid import uuid4
+from logging import Logger, getLogger
+from datetime import datetime
+from inspect import isawaitable
+from typing import Dict, Hashable, Callable, cast
+
+from .types import AccountNumber, AccountUUID, DataMessage, Response, GroupId, ResponseFrame, NotificationFrame, EnvelopeFrame
+from .aliases import GroupContext, AnyCb, IndividualContext
+from .args import SendMessageArgs
+from .exceptions import SignalRpcException
+from .personality import Personality
+from .protocol import SignalBot, PersonalityProto, RpcRet
+from .transport import JsonRpcTransport, JsonRpcHandler
+
+
+class SignalBotImpl(SignalBot, Personality, JsonRpcHandler):
+    """Concrete implementation of `SignalBot`."""
+
+    __account_number: AccountNumber
+    __transport: JsonRpcTransport
+    __log: Logger = getLogger(__module__ + '.Signal')  # type: ignore
+    __start_time: datetime
+    __personalities: list[Personality]
+    __stopping = asyncio.Event()
+    __cancelable: list[asyncio.Task | asyncio.Handle]
+
+    def __init__(self, account_number: AccountNumber, transport: JsonRpcTransport) -> None:
+        self.__account_number = account_number
+        self.__transport = transport
+        self.__start_time = datetime.now()
+        self.__personalities = []
+        self.__cancelable = []
+        Personality.__init__(self)
+
+    # `Signal`
+
+    @property
+    def account_number(self) -> AccountNumber:
+        return self.__account_number
+
+    async def run(self) -> None:
+        self.start_crons(self)
+        for personality in self.__personalities:
+            personality.start_crons(self)
+            asyncio.ensure_future(personality.started(self))
+        try:
+            await self.__transport.listen(self)
+        except asyncio.CancelledError:
+            self.__log.debug('Transport listen loop stopped.')
+            await self.stop()
+
+    async def stop(self) -> None:
+        if self.__stopping.is_set():
+            return
+        self.__log.info("Stop requested...")
+        self.__log.debug("Stopping Crons...")
+        self.__stopping.set()
+        self.stop_crons()
+        for personality in self.__personalities:
+            personality.stop_crons()
+        self.__log.debug("Disconnecting from signal-cli...")
+        await self.__transport.terminate()
+        self.__log.debug("Canceling anything in-flight...")
+        if self.__cancelable:
+            for cancelable in self.__cancelable:
+                cancelable.cancel()
+            self.__log.debug("Waiting for cancelables to finish...")
+            await asyncio.wait([x for x in self.__cancelable if isawaitable(x)])
+        self.__log.info("Stopped.")
+        self.__stopping.clear()
+
+    #######################
+    # `SignalRpc` Methods #
+    #######################
+
+    async def send_reaction(self, to: DataMessage, emoji: str) -> Future[Response]:
+        kwargs = {}
+        if to.group_info is None:
+            kwargs['recipient'] = to.sender_uuid
+        else:
+            kwargs['groupId'] = to.group_info['groupId']  # type: ignore
+
+        return asyncio.ensure_future(
+            Response.from_future_frame(await self.__json_rpc('sendReaction',
+                                                             emoji=emoji,
+                                                             targetAuthor=to.sender_uuid,
+                                                             targetTimestamp=to.unix_timestamp,
+                                                             **kwargs)))
+
+    async def send_typing(self, to: AccountNumber | AccountUUID | GroupId, stop=False) -> Future[Response]:
+        kwargs: dict = {('groupId' if len(to) == 44 else 'recipient'): to}
+        if stop:
+            kwargs['stop'] = True
+        return asyncio.ensure_future(Response.from_future_frame(await self.__json_rpc('sendTyping', **kwargs)))
+
+    async def send_message(self,
+                           to: AccountNumber | AccountUUID | GroupId,
+                           message: str | None = None,
+                           args: SendMessageArgs | None = None) -> Future[Response]:
+        if (not message) and args is not None and not args.attachment:
+            raise ValueError('message cannot be empty without attachment')
+        kwargs: dict = {('groupId' if len(to) == 44 else 'recipient'): to}
+        if args is not None:
+            kwargs.update(args.to_args())
+        return asyncio.ensure_future(
+            Response.from_future_frame(await self.__json_rpc('send', message=message, **kwargs)))
+
+    async def delete_message(self, to: AccountNumber | AccountUUID | GroupId, target_timestamp: datetime) -> RpcRet:
+        kwargs: dict = {
+            ('groupId' if len(to) == 44 else 'recipient'): to,
+            'targetTimestamp': int(target_timestamp.timestamp() * 1000)
+        }
+        return asyncio.ensure_future(Response.from_future_frame(await self.__json_rpc('remoteDelete', **kwargs)))
+
+    def add_personality(self, personality: PersonalityProto) -> None:
+        assert isinstance(personality, Personality)
+        self.__personalities.append(personality)
+
+    def handle_callback_exception(self, exception: BaseException, cb: AnyCb) -> bool:
+        callback_type, *info = cb
+        post = "" if callback_type != 'cron' else " Cron will be rescheduled for the next occurance."
+        self.__log.exception("Uncaught exception while processing a registered %r callback (addt'l info: %r).%s",
+                             callback_type,
+                             info,
+                             post,
+                             exc_info=exception,
+                             stack_info=True)
+        return True
+
+    ############################
+    # `JsonRpcHandler` Methods #
+    ############################
+
+    async def handle_response(self, response: ResponseFrame) -> None:
+        remove = next((id for id, checker in self.__WAITERS.items() if checker(response)), None)
+        if remove is not None:
+            del self.__WAITERS[remove]
+
+    async def handle_notification(self, notification: NotificationFrame) -> None:
+        match notification['method']:
+            case 'receive':
+                await self.__receive(notification)
+            case _:
+                self.__log.warning('Received unexpected JsonRPC notification method: %r', notification['method'])
+
+    #############
+    # Internals #
+    #############
+
+    async def __receive(self, message: NotificationFrame) -> None:
+        envelope: EnvelopeFrame = message['params'].get('envelope', None)
+        if envelope is None:
+            self.__log.warning("Received NotificationFrame with null Envelope: %r", message)
+            return
+
+        timestamp = datetime.fromtimestamp(envelope['timestamp'] / 1000.0)
+        if timestamp <= self.__start_time:
+            self.__log.warning("Received message from before signal_bot_framework started (%r).", timestamp)
+            return
+
+        match envelope:
+            case {'typingMessage': _}:
+                # TODO: self.__handle_typing_message(envelope)
+                pass
+            case {'dataMessage': _}:
+                asyncio.create_task(self.__handle_data_message(envelope))
+            case _:
+                self.__log.warning("Unknown message type: %r", set(envelope.keys()))
+
+    async def __handle_data_message(self, envelope: EnvelopeFrame) -> None:
+        message = DataMessage(envelope)
+        context: GroupContext | IndividualContext
+        if message.group_info is not None:
+            context = ('group', GroupId(message.group_info['groupId']))
+        else:
+            context = ('individual', message.sender, envelope['sourceName'])
+
+        for personality in self.__personalities:
+            if personality.matches_context(context) and await personality.personality_handle_message(
+                    self, context, message):
+                return
+        await self.personality_handle_message(self, context, message)
+
+    __WAITERS: Dict[Hashable, Callable[[ResponseFrame], bool]] = {}
+
+    async def __json_rpc(self, method: str, **params) -> Future[ResponseFrame]:
+        request_id = params.pop("request_id", str(uuid4()))
+        if not params:
+            params = {}
+
+        params.update({"account": self.__account_number})
+        request: NotificationFrame = {
+            'jsonrpc': '2.0',
+            'id': request_id,
+            'method': method,
+            'params': params,
+        }
+
+        loop = asyncio.get_running_loop()
+        future: Future[ResponseFrame] = loop.create_future()
+        key = object()
+
+        def cancel_timer():
+            """Cancels our RPC after a timeout"""
+            if not future.done():
+                future.set_exception(TimeoutError(f"request id {request_id!r} timed out"))
+                self.__WAITERS.pop(key, None)
+
+        t_handle = loop.call_later(5.0, cancel_timer)
+        self.__cancelable.append(t_handle)
+
+        def check_return(ret: ResponseFrame) -> bool:
+            if ret['id'] != request_id:
+                return False
+            match ret:
+                case {'error': error}:
+                    self.__log.debug("Setting exception %r", error)
+                    future.set_exception(SignalRpcException(error['message'], cast(dict, ret)))
+                case _:
+                    self.__log.debug("Setting result %r", ret)
+                    future.set_result(ret)
+            t_handle.cancel()
+            self.__cancelable.remove(t_handle)
+            return True
+
+        self.__WAITERS[key] = check_return
+        self.__log.debug(request)
+        self.__cancelable.append(loop.create_task(self.__transport.write(request)))
+        return future
```

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework/_util.py` & `signal_bot_framework-0.2/src/signal_bot_framework/_util.py`

 * *Files identical despite different names*

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework/args.py` & `signal_bot_framework-0.2/src/signal_bot_framework/args.py`

 * *Files identical despite different names*

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework/personality.py` & `signal_bot_framework-0.2/src/signal_bot_framework/personality.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-"""Personalities describe behavior for a subset of :data:`signal_bot_framework.aliases.Context`."""
-
-from __future__ import annotations
-
-from abc import abstractmethod, ABC
-from typing import Tuple, Sequence
-from datetime import datetime
-from logging import getLogger, Logger
-import asyncio
-import re
-
-import humanize
-from cron_converter import Cron
-from cron_converter.sub_modules.seeker import Seeker
-
-from .types import Account, DataMessage
-from .protocol import PersonalityProto, MessageCb, CronItem, GroupId, Context, AnyCb, SignalBot, CronCb
-
-
-class Personality(PersonalityProto, ABC):
-    """Specific behavior for a subset of :data:`signal_bot_framework.aliases.Context`."""
-
-    _message_hooks: list[MessageCb]
-    _prefix_hooks: dict[str, MessageCb]
-    _keyword_hooks: dict[Tuple[str, bool, bool], MessageCb]
-    _keyword_cache: dict[Tuple[str, bool, bool], re.Pattern]
-    _mention_hooks: dict[Account, MessageCb]
-    _cron_hooks: list[CronItem]
-    _crons: list[asyncio.TimerHandle]
-    _contexts: Sequence[Account | GroupId]
-    _logger: Logger
-
-    def __init__(self, contexts: Sequence[Account | GroupId] = tuple()):  # noqa: D107
-        self._message_hooks = []
-        self._prefix_hooks = {}
-        self._keyword_hooks = {}
-        self._keyword_cache = {}
-        self._mention_hooks = {}
-        self._cron_hooks = []
-        self._crons = []
-        self._contexts = contexts
-        self._logger = getLogger(f'{self.__class__.__module__}.{self.__class__.__qualname__}')
-
-    def matches_context(self, context: Context) -> bool:
-        """
-        Whether or not a given Context is valid for this Personality.
-
-        :param context: The Context in question.
-        :type context: :data:`~signal_bot_framework.aliases.Context`
-        """
-        return len(self._contexts) == 0 or context[1] in self._contexts
-
-    @abstractmethod
-    def handle_callback_exception(self, exception: BaseException, cb: AnyCb) -> bool:
-        """
-        Handle an exception that occured in a callback.
-
-        :param exception: The exception that occurred.
-        :param cb: The callback the exception occurred in.
-        :type cb: :data:`~signal_bot_framework.aliases.AnyCb`
-
-        :returns: If the callback is a Cron hook, the return value determines whether the Cron will be rescheduled.
-        """
-        raise NotImplementedError()
-
-    def _cron_repeat(self, signal: SignalBot, schedule: Seeker, item: CronItem):
-
-        def _reschedule(task: asyncio.Task[None]):
-            if (ex := task.exception()) is not None and not self.handle_callback_exception(ex, ('cron', *item)):
-                return
-
-            loop = asyncio.get_running_loop()
-            next_sched = schedule.next()
-            delay = (next_sched - datetime.now()).total_seconds()
-            self._logger.debug("Cron %r will re-fire %s (%s at %s)", item[0], humanize.naturaltime(next_sched),
-                               humanize.naturalday(next_sched), next_sched.strftime("%H:%M:%S"))
-            i = 0
-            while i < len(self._crons):
-                if self._crons[i].when() < loop.time():
-                    del self._crons[i]
-                    continue
-                i += 1
-            self._crons.append(loop.call_later(delay, self._cron_repeat, signal, schedule, item))
-
-        asyncio.ensure_future(item[1](signal)).add_done_callback(_reschedule)
-
-    def start_crons(self, signal: 'SignalBot'):
-        """
-        Start any registered Cron callbacks.
-
-        Called by :class:`~signal_bot_framework.protocol.SignalBot`.
-
-        :param signal: The current :class:`~signal_bot_framework.protocol.SignalBot` instance.
-        """
-        self._logger.debug("Starting crons...")
-        loop = asyncio.get_running_loop()
-        ref = datetime.now()
-        for item in self._cron_hooks:
-            cron_str, _ = item
-            cron = Cron(cron_str)
-            schedule = cron.schedule(ref)
-            next_schedule = schedule.next()
-            delay = (next_schedule - ref).total_seconds()
-            self._logger.debug("Cron %r will fire %s (%s at %s)", cron_str, humanize.naturaltime(next_schedule),
-                               humanize.naturalday(next_schedule), next_schedule.strftime("%H:%M:%S"))
-            self._crons.append(loop.call_later(delay, self._cron_repeat, signal, schedule, item))
-
-    def stop_crons(self) -> None:
-        """Stop any sleeping Cron callbacks."""
-        cron: asyncio.TimerHandle
-        for cron in self._crons:
-            cron.cancel()
-
-    async def personality_handle_message(self, signal: 'SignalBot', context: Context, message: DataMessage) -> bool:
-        """
-        Handle a single Signal message that has been approved for this Personality.
-
-        Determines if the message is handled by any of the existing hooks, and if so stops processing.
-
-        :param signal: The current `SignalBot` instance.
-        :param context: The context the message was received in.
-        :type context: :data:`~signal_bot_framework.aliases.Context`
-        :param message: The message that was received.
-
-        :returns: ``True`` if the message was handled by a hook - otherwise the message will be sent to the next
-                  Personality in line.
-        """
-        # First, prefixes
-        if message.message is not None:
-            for prefix, hook in self._prefix_hooks.items():
-                if message.message.startswith(prefix) and await hook(signal, context, message):
-                    return True
-
-        # Then mentions
-        for account, hook in self._mention_hooks.items():
-            if message.mentions and any(mention['number'] == account
-                                        for mention in message.mentions) and await hook(signal, context, message):
-                return True
-
-        # Then keywords
-        if message.message is not None:
-            for definition, hook in self._keyword_hooks.items():
-                keyword, case_sensitive, whole_word = definition
-                if definition in self._keyword_cache:
-                    pattern = self._keyword_cache[definition]
-                else:
-                    pattern = re.compile((r'\b{}\b' if whole_word else '{}').format(re.escape(keyword)),
-                                         re.NOFLAG if case_sensitive else re.IGNORECASE)
-                    self._keyword_cache[definition] = pattern
-
-                if pattern.search(message.message) and await hook(signal, context, message):
-                    return True
-
-        # Finally, global hooks
-        for hook in self._message_hooks:
-            if await hook(signal, context, message):
-                return True
-
-        return False
-
-    def on_message(self, cb: MessageCb):
-        self._message_hooks.append(cb)
-
-    # pylint: disable=missing-function-docstring
-    def remove_message_callback(self, callback: MessageCb):
-        self._message_hooks.remove(callback)
-
-    def on_prefix(self, prefix: str, cb: MessageCb):
-        self._prefix_hooks[prefix] = cb
-
-    # pylint: disable=missing-function-docstring
-    def remove_prefix(self, prefix: str):
-        self._prefix_hooks.pop(prefix, None)
-
-    def on_keyword(self, keyword: str, cb: MessageCb, case_sensitive=False, whole_word=True):
-        self._keyword_hooks[keyword, case_sensitive, whole_word] = cb
-
-    # pylint: disable=missing-function-docstring
-    def remove_keyword(self, key: str | Tuple[str, bool, bool]):
-        for elem in self._keyword_hooks:
-            if key == (elem[0] if isinstance(key, str) else elem):
-                self._keyword_hooks.pop(elem, None)
-                self._keyword_cache.pop(elem, None)
-                return
-
-    def on_mention(self, mention: Account, cb: MessageCb):
-        self._mention_hooks[mention] = cb
-
-    # pylint: disable=missing-function-docstring
-    def remove_mention(self, mention: Account):
-        self._mention_hooks.pop(mention, None)
-
-    def on_cron(self, schedule: str, cb: CronCb) -> CronItem:
-        ret = (schedule, cb)
-        self._cron_hooks.append(ret)
-        return ret
-
-    # pylint: disable=missing-function-docstring
-    def remove_cron(self, item: CronItem):
-        self._cron_hooks.remove(item)
+"""Personalities describe behavior for a subset of :data:`signal_bot_framework.aliases.Context`."""
+
+from __future__ import annotations
+
+from abc import abstractmethod, ABC
+from typing import Tuple, Sequence
+from datetime import datetime
+from logging import getLogger, Logger
+import asyncio
+import re
+
+import humanize
+from cron_converter import Cron
+from cron_converter.sub_modules.seeker import Seeker
+
+from .types import AccountNumber, AccountUUID, DataMessage
+from .protocol import PersonalityProto, MessageCb, CronItem, GroupId, Context, AnyCb, SignalBot, CronCb
+
+
+class Personality(PersonalityProto, ABC):
+    """Specific behavior for a subset of :data:`signal_bot_framework.aliases.Context`."""
+
+    _message_hooks: list[MessageCb]
+    _prefix_hooks: dict[str, MessageCb]
+    _keyword_hooks: dict[Tuple[str, bool, bool], MessageCb]
+    _keyword_cache: dict[Tuple[str, bool, bool], re.Pattern]
+    _mention_hooks: dict[AccountNumber|AccountUUID, MessageCb]
+    _cron_hooks: list[CronItem]
+    _crons: list[asyncio.TimerHandle]
+    _contexts: Sequence[AccountNumber | AccountUUID | GroupId]
+    _logger: Logger
+
+    def __init__(self, contexts: Sequence[AccountNumber | AccountUUID | GroupId] = tuple()):  # noqa: D107
+        self._message_hooks = []
+        self._prefix_hooks = {}
+        self._keyword_hooks = {}
+        self._keyword_cache = {}
+        self._mention_hooks = {}
+        self._cron_hooks = []
+        self._crons = []
+        self._contexts = contexts
+        self._logger = getLogger(f'{self.__class__.__module__}.{self.__class__.__qualname__}')
+
+    def matches_context(self, context: Context) -> bool:
+        """
+        Whether or not a given Context is valid for this Personality.
+
+        :param context: The Context in question.
+        :type context: :data:`~signal_bot_framework.aliases.Context`
+        """
+        return len(self._contexts) == 0 or context[1] in self._contexts
+
+    @abstractmethod
+    def handle_callback_exception(self, exception: BaseException, cb: AnyCb) -> bool:
+        """
+        Handle an exception that occured in a callback.
+
+        :param exception: The exception that occurred.
+        :param cb: The callback the exception occurred in.
+        :type cb: :data:`~signal_bot_framework.aliases.AnyCb`
+
+        :returns: If the callback is a Cron hook, the return value determines whether the Cron will be rescheduled.
+        """
+        raise NotImplementedError()
+
+    def _cron_repeat(self, signal: SignalBot, schedule: Seeker, item: CronItem):
+
+        def _reschedule(task: asyncio.Task[None]):
+            if (ex := task.exception()) is not None and not self.handle_callback_exception(ex, ('cron', *item)):
+                return
+
+            loop = asyncio.get_running_loop()
+            next_sched = schedule.next()
+            delay = (next_sched - datetime.now()).total_seconds()
+            self._logger.debug("Cron %r will re-fire %s (%s at %s)", item[0], humanize.naturaltime(next_sched),
+                               humanize.naturalday(next_sched), next_sched.strftime("%H:%M:%S"))
+            i = 0
+            while i < len(self._crons):
+                if self._crons[i].when() < loop.time():
+                    del self._crons[i]
+                    continue
+                i += 1
+            self._crons.append(loop.call_later(delay, self._cron_repeat, signal, schedule, item))
+
+        asyncio.ensure_future(item[1](signal)).add_done_callback(_reschedule)
+
+    def start_crons(self, signal: 'SignalBot'):
+        """
+        Start any registered Cron callbacks.
+
+        Called by :class:`~signal_bot_framework.protocol.SignalBot`.
+
+        :param signal: The current :class:`~signal_bot_framework.protocol.SignalBot` instance.
+        """
+        self._logger.debug("Starting crons...")
+        loop = asyncio.get_running_loop()
+        ref = datetime.now()
+        for item in self._cron_hooks:
+            cron_str, _ = item
+            cron = Cron(cron_str)
+            schedule = cron.schedule(ref)
+            next_schedule = schedule.next()
+            delay = (next_schedule - ref).total_seconds()
+            self._logger.debug("Cron %r will fire %s (%s at %s)", cron_str, humanize.naturaltime(next_schedule),
+                               humanize.naturalday(next_schedule), next_schedule.strftime("%H:%M:%S"))
+            self._crons.append(loop.call_later(delay, self._cron_repeat, signal, schedule, item))
+
+    def stop_crons(self) -> None:
+        """Stop any sleeping Cron callbacks."""
+        cron: asyncio.TimerHandle
+        for cron in self._crons:
+            cron.cancel()
+
+    async def personality_handle_message(self, signal: 'SignalBot', context: Context, message: DataMessage) -> bool:
+        """
+        Handle a single Signal message that has been approved for this Personality.
+
+        Determines if the message is handled by any of the existing hooks, and if so stops processing.
+
+        :param signal: The current `SignalBot` instance.
+        :param context: The context the message was received in.
+        :type context: :data:`~signal_bot_framework.aliases.Context`
+        :param message: The message that was received.
+
+        :returns: ``True`` if the message was handled by a hook - otherwise the message will be sent to the next
+                  Personality in line.
+        """
+        # First, prefixes
+        if message.message is not None:
+            for prefix, hook in self._prefix_hooks.items():
+                if message.message.startswith(prefix) and await hook(signal, context, message):
+                    return True
+
+        # Then mentions
+        for account, hook in self._mention_hooks.items():
+            if message.mentions and any(mention['number'] == account
+                                        for mention in message.mentions) and await hook(signal, context, message):
+                return True
+
+        # Then keywords
+        if message.message is not None:
+            for definition, hook in self._keyword_hooks.items():
+                keyword, case_sensitive, whole_word = definition
+                if definition in self._keyword_cache:
+                    pattern = self._keyword_cache[definition]
+                else:
+                    pattern = re.compile((r'\b{}\b' if whole_word else '{}').format(re.escape(keyword)),
+                                         re.NOFLAG if case_sensitive else re.IGNORECASE)
+                    self._keyword_cache[definition] = pattern
+
+                if pattern.search(message.message) and await hook(signal, context, message):
+                    return True
+
+        # Finally, global hooks
+        for hook in self._message_hooks:
+            if await hook(signal, context, message):
+                return True
+
+        return False
+
+    def on_message(self, cb: MessageCb):
+        self._message_hooks.append(cb)
+
+    # pylint: disable=missing-function-docstring
+    def remove_message_callback(self, callback: MessageCb):
+        self._message_hooks.remove(callback)
+
+    def on_prefix(self, prefix: str, cb: MessageCb):
+        self._prefix_hooks[prefix] = cb
+
+    # pylint: disable=missing-function-docstring
+    def remove_prefix(self, prefix: str):
+        self._prefix_hooks.pop(prefix, None)
+
+    def on_keyword(self, keyword: str, cb: MessageCb, case_sensitive=False, whole_word=True):
+        self._keyword_hooks[keyword, case_sensitive, whole_word] = cb
+
+    # pylint: disable=missing-function-docstring
+    def remove_keyword(self, key: str | Tuple[str, bool, bool]):
+        for elem in self._keyword_hooks:
+            if key == (elem[0] if isinstance(key, str) else elem):
+                self._keyword_hooks.pop(elem, None)
+                self._keyword_cache.pop(elem, None)
+                return
+
+    def on_mention(self, mention: AccountNumber | AccountUUID, cb: MessageCb):
+        self._mention_hooks[mention] = cb
+
+    # pylint: disable=missing-function-docstring
+    def remove_mention(self, mention: AccountNumber | AccountUUID):
+        self._mention_hooks.pop(mention, None)
+
+    def on_cron(self, schedule: str, cb: CronCb) -> CronItem:
+        ret = (schedule, cb)
+        self._cron_hooks.append(ret)
+        return ret
+
+    # pylint: disable=missing-function-docstring
+    def remove_cron(self, item: CronItem):
+        self._cron_hooks.remove(item)
```

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework/protocol.py` & `signal_bot_framework-0.2/src/signal_bot_framework/protocol.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,182 +1,185 @@
-"""High-level interface definitions."""
-
-from __future__ import annotations
-
-from typing import Protocol, runtime_checkable
-from abc import abstractmethod
-from datetime import datetime
-
-from .args import SendMessageArgs
-from .types import Account, GroupId, DataMessage
-from .aliases import Context, MessageCb, CronCb, CronItem, AnyCb, RpcRet
-
-########################
-# High Level Protocols #
-########################
-
-
-@runtime_checkable
-class PersonalityProto(Protocol):
-    """
-    Defines a "personality" that applies only to messages in specific contexts (e.g., in a specific group).
-
-    This ``Protocol`` contains shared functionality between a :class:`SignalBot` instance (a "root" personality) and
-    individual :class:`signal_bot_framework.personality.Personality` instances. When a message is received, it is checked against
-    any personalities' callbacks first, then the root peronality's callbacks.
-
-    To use, create an instance of (or subclass) :class:`~signal_bot_framework.personality.Personality` and register it with
-    :func:`SignalBot.add_personality`.
-
-    Not listed here are associated ``remove_xxx(...)`` methods (e.g.,
-    :func:`~signal_bot_framework.personality.Personality.remove_cron`).
-    """
-
-    def matches_context(self, context: Context) -> bool:
-        """
-        Whether this personality matches a given context.
-
-        :param context: The context to match against.
-        :type context: :data:`~signal_bot_framework.aliases.Context`
-        """
-
-    def on_message(self, cb: MessageCb) -> None:
-        """
-        Register a callback to be called on any DataMessage.
-
-        :param cb: The function to call.
-        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
-        """
-
-    def on_prefix(self, prefix: str, cb: MessageCb) -> None:
-        """
-        Register a callback to be called on any DataMessage matching a given prefix (exact match).
-
-        :param prefix: The exact-match prefix to trigger on.
-        :param cb: The function to call.
-        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
-        """
-
-    def on_cron(self, schedule: str, cb: CronCb) -> CronItem:
-        """
-        Register a callback to be called on a Cron schedule.
-
-        :param schedule: The Cron schedule to trigger on.
-        :param cb: The function to call.
-        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
-        :rtype: :data:`~signal_bot_framework.aliases.CronItem`
-        """
-
-    def on_mention(self, mention: Account, cb: MessageCb) -> None:
-        """
-        Register a callback to be called when a given Account is @-mentioned.
-
-        :param mention: The Signal account to trigger on mentions of.
-        :type mention: :data:`~signal_bot_framework.types.Account`
-        :param cb: The function to call.
-        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
-        """
-
-    def on_keyword(self, keyword: str, cb: MessageCb, case_sensitive=False, whole_word=True) -> None:
-        """
-        Register a callback to be called when DataMessage contains a keyword.
-
-        :param keyword: The keyword to trigger on.
-        :param cb: The function to call.
-        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
-        :param case_sensitive: Whether the match is case-sensitive.
-        :type case_sensitive: :data:`bool`
-        :param whole_word: Whether to match whole words only.
-        :type whole_word: :data:`bool`
-        """
-
-    async def started(self, signal: 'SignalBot') -> None:
-        """
-        Handle when ``SignalBot`` is first started.
-
-        :param signal: An instance of the current ``SignalBot``.
-        :type signal: :class:`~SignalBot`
-        """
-
-    @abstractmethod
-    def handle_callback_exception(self, exception: BaseException, cb: AnyCb) -> bool:
-        """
-        Personalities should implement this to handle when unhandled exceptions occur in a callback.
-
-        :param exception: The exception that occurred.
-        :param cb: The callback that raised the exception.
-        :type cb: :data:`~signal_bot_framework.aliases.AnyCb`
-        :returns: Whether Cron callbacks should be rescheduled.
-        """
-
-
-class SignalBot(PersonalityProto, Protocol):
-    """
-    The high-level abstraction of ``signal_bot_framework`` functionality.
-
-    Implementation can be found in ``signal_bot_framework._signal_impl``.
-    To create an instance, call :meth:`signal_bot_framework.create`.
-    """
-
-    def __init__(self) -> None:  # noqa: D107
-        # TODO: remove this limitation in future versions.
-        raise TypeError("Instances must be created with `signal_bot_framework.create(...)`.")
-
-    @property
-    def account(self) -> Account:
-        """The currently registered Signal account."""
-
-    async def send_reaction(self, to: DataMessage, emoji: str) -> RpcRet:
-        """
-        React to a previous message.
-
-        :param to: The message to react to.
-        :param emoji: The emoji to react with.
-        """
-
-    async def send_typing(self, to: Account | GroupId, stop=False) -> RpcRet:
-        """
-        Start (or stop) the "Typing..." indicator.
-
-        When started, will display for 15 seconds unless stopped.
-
-        :param to: The destination of the typing indicator (an individual or a group).
-        :param stop: Stop (rather than start) the typing indicator.
-        :type stop: :data:`bool`
-        """
-
-    async def send_message(self,
-                           to: Account | GroupId,
-                           message: str | None = None,
-                           args: SendMessageArgs | None = None) -> RpcRet:
-        """
-        Send a message.
-
-        :param to: The destination of the message (an individual or a group).
-        :param message: The textual message to send (if any).
-        :param args: Additional arguments to ``send_message``.
-        """
-
-    async def delete_message(self, to: Account | GroupId, target_timestamp: datetime) -> RpcRet:
-        """
-        Delete a sent message (by timestamp).
-
-        :param to: The destination (an individual or a group) in which to delete a message.
-        :param target_timestamp: The timestamp of the message to delete.
-        """
-
-    async def run(self) -> None:
-        """
-        Start Cron callbacks and the message pump loop.
-
-        Runs until the transport raises ``asyncio.CancelledError`` (e.g., :meth:`stop` is called).
-        """
-
-    async def stop(self) -> None:
-        """Stop the message pump loop (if running) and any scheduled Cron callbacks, in-flight requests, etc."""
-
-    def add_personality(self, personality: PersonalityProto) -> None:
-        """
-        Add a sub-personality.
-
-        :param personality: The :class:`~signal_bot_framework.personality.Personality` to add.
-        """
+"""High-level interface definitions."""
+
+from __future__ import annotations
+
+from typing import Protocol, runtime_checkable
+from abc import abstractmethod
+from datetime import datetime
+
+from .args import SendMessageArgs
+from .types import AccountNumber, AccountUUID, GroupId, DataMessage
+from .aliases import Context, MessageCb, CronCb, CronItem, AnyCb, RpcRet
+
+########################
+# High Level Protocols #
+########################
+
+
+@runtime_checkable
+class PersonalityProto(Protocol):
+    """
+    Defines a "personality" that applies only to messages in specific contexts (e.g., in a specific group).
+
+    This ``Protocol`` contains shared functionality between a :class:`SignalBot` instance (a "root" personality) and
+    individual :class:`signal_bot_framework.personality.Personality` instances. When a message is received, it is checked against
+    any personalities' callbacks first, then the root peronality's callbacks.
+
+    To use, create an instance of (or subclass) :class:`~signal_bot_framework.personality.Personality` and register it with
+    :func:`SignalBot.add_personality`.
+
+    Not listed here are associated ``remove_xxx(...)`` methods (e.g.,
+    :func:`~signal_bot_framework.personality.Personality.remove_cron`).
+    """
+
+    def matches_context(self, context: Context) -> bool:
+        """
+        Whether this personality matches a given context.
+
+        :param context: The context to match against.
+        :type context: :data:`~signal_bot_framework.aliases.Context`
+        """
+
+    def on_message(self, cb: MessageCb) -> None:
+        """
+        Register a callback to be called on any DataMessage.
+
+        :param cb: The function to call.
+        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
+        """
+
+    def on_prefix(self, prefix: str, cb: MessageCb) -> None:
+        """
+        Register a callback to be called on any DataMessage matching a given prefix (exact match).
+
+        :param prefix: The exact-match prefix to trigger on.
+        :param cb: The function to call.
+        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
+        """
+
+    def on_cron(self, schedule: str, cb: CronCb) -> CronItem:
+        """
+        Register a callback to be called on a Cron schedule.
+
+        :param schedule: The Cron schedule to trigger on.
+        :param cb: The function to call.
+        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
+        :rtype: :data:`~signal_bot_framework.aliases.CronItem`
+        """
+
+    def on_mention(self, mention: AccountNumber | AccountUUID, cb: MessageCb) -> None:
+        """
+        Register a callback to be called when a given :data:`~signal_bot_framework.types.AccountNumber`/:data:`~signal_bot_framework.types.AccountUUID` is @-mentioned.
+
+        :param mention: The Signal account to trigger on mentions of.
+        :type mention: Union[:data:`~signal_bot_framework.types.AccountNumber`, :data:`~signal_bot_framework.types.AccountUUID`]
+        :param cb: The function to call.
+        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
+        """
+
+    def on_keyword(self, keyword: str, cb: MessageCb, case_sensitive=False, whole_word=True) -> None:
+        """
+        Register a callback to be called when DataMessage contains a keyword.
+
+        :param keyword: The keyword to trigger on.
+        :param cb: The function to call.
+        :type cb: :data:`~signal_bot_framework.aliases.MessageCb`
+        :param case_sensitive: Whether the match is case-sensitive.
+        :type case_sensitive: :data:`bool`
+        :param whole_word: Whether to match whole words only.
+        :type whole_word: :data:`bool`
+        """
+
+    async def started(self, signal: 'SignalBot') -> None:
+        """
+        Handle when ``SignalBot`` is first started.
+
+        :param signal: An instance of the current ``SignalBot``.
+        :type signal: :class:`~SignalBot`
+        """
+
+    @abstractmethod
+    def handle_callback_exception(self, exception: BaseException, cb: AnyCb) -> bool:
+        """
+        Personalities should implement this to handle when unhandled exceptions occur in a callback.
+
+        :param exception: The exception that occurred.
+        :param cb: The callback that raised the exception.
+        :type cb: :data:`~signal_bot_framework.aliases.AnyCb`
+        :returns: Whether Cron callbacks should be rescheduled.
+        """
+
+
+class SignalBot(PersonalityProto, Protocol):
+    """
+    The high-level abstraction of ``signal_bot_framework`` functionality.
+
+    Implementation can be found in ``signal_bot_framework._signal_impl``.
+    To create an instance, call :meth:`signal_bot_framework.create`.
+    """
+
+    def __init__(self) -> None:  # noqa: D107
+        # TODO: remove this limitation in future versions.
+        raise TypeError("Instances must be created with `signal_bot_framework.create(...)`.")
+
+    @property
+    def account_number(self) -> AccountNumber:
+        """The currently registered Signal account."""
+
+    async def send_reaction(self, to: DataMessage, emoji: str) -> RpcRet:
+        """
+        React to a previous message.
+
+        :param to: The message to react to.
+        :param emoji: The emoji to react with.
+        """
+
+    async def send_typing(self, to: AccountNumber | AccountUUID | GroupId, stop=False) -> RpcRet:
+        """
+        Start (or stop) the "Typing..." indicator.
+
+        When started, will display for 15 seconds unless stopped.
+
+        :param to: The destination of the typing indicator (an individual or a group).
+        :type to: Union[:data:`~signal_bot_framework.types.AccountNumber`, :data:`~signal_bot_framework.types.AccountUUID`, :data:`~signal_bot_framework.types.GroupID`]
+        :param stop: Stop (rather than start) the typing indicator.
+        :type stop: :data:`bool`
+        """
+
+    async def send_message(self,
+                           to: AccountNumber | AccountUUID | GroupId,
+                           message: str | None = None,
+                           args: SendMessageArgs | None = None) -> RpcRet:
+        """
+        Send a message.
+
+        :param to: The destination of the message (an individual or a group).
+        :type to: Union[:data:`~signal_bot_framework.types.AccountNumber`, :data:`~signal_bot_framework.types.AccountUUID`, :data:`~signal_bot_framework.types.GroupID`]
+        :param message: The textual message to send (if any).
+        :param args: Additional arguments to ``send_message``.
+        """
+
+    async def delete_message(self, to: AccountNumber | AccountUUID | GroupId, target_timestamp: datetime) -> RpcRet:
+        """
+        Delete a sent message (by timestamp).
+
+        :param to: The destination (an individual or a group) in which to delete a message.
+        :type to: Union[:data:`~signal_bot_framework.types.AccountNumber`, :data:`~signal_bot_framework.types.AccountUUID`, :data:`~signal_bot_framework.types.GroupID`]
+        :param target_timestamp: The timestamp of the message to delete.
+        """
+
+    async def run(self) -> None:
+        """
+        Start Cron callbacks and the message pump loop.
+
+        Runs until the transport raises ``asyncio.CancelledError`` (e.g., :meth:`stop` is called).
+        """
+
+    async def stop(self) -> None:
+        """Stop the message pump loop (if running) and any scheduled Cron callbacks, in-flight requests, etc."""
+
+    def add_personality(self, personality: PersonalityProto) -> None:
+        """
+        Add a sub-personality.
+
+        :param personality: The :class:`~signal_bot_framework.personality.Personality` to add.
+        """
```

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework/transport.py` & `signal_bot_framework-0.2/src/signal_bot_framework/transport.py`

 * *Files identical despite different names*

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/PKG-INFO` & `signal_bot_framework-0.2/src/signal_bot_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: signal-bot-framework
-Version: 0.1.0
+Name: signal_bot_framework
+Version: 0.2.0
 Summary: A Python module for building Signal.org bots that interact with signal-cli.
 Author-email: Sidneys1 <sidneys1@proton.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,18 +686,31 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Communications :: Chat
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
 License-File: LICENSE
 License-File: COPYING
+Requires-Dist: cron-converter~=1.0.2
+Requires-Dist: humanize~=4.6.0
+Provides-Extra: dev
+Requires-Dist: pylint~=2.17.5; extra == "dev"
+Requires-Dist: yapf~=0.40.1; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Provides-Extra: docs
+Requires-Dist: sphinx~=7.2.6; extra == "docs"
+Requires-Dist: myst-parser~=2.0.0; extra == "docs"
+Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
+Requires-Dist: sphinx-paramlinks~=0.6.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints~=1.23.0; extra == "docs"
+Requires-Dist: setuptools; extra == "docs"
 
 # Signal-Bot
 
 An `asyncio` Python 3.11 module for building [Signal][signal] bots that interact with [AsamK/signal-cli][signal-cli].
 
 ## Features
 
@@ -720,29 +733,29 @@
 ## Usage
 
 For development: `python3.11 -m pip install signal_bot_framework`.
 
 ```py
 # test_bot.py
 import asyncio
-from signal_bot_framework import create, Account
+from signal_bot_framework import create, AccountNumber
 
 async def crabby_callback(signal: Signal, context: Context, message: DataMessage) -> bool:
         to = context[1]
         await signal.send_reaction(message, "🦀")
         await signal.send_message(to, f"Sorry, just feeling a little crabby, {message.sender_name}.",
                                   args=SendMessageArgs(mention=[f"37:{len(message.sender_name)}:{message.sender}"]))
         return True
 
 async def main():
     # The default, finds `signal-cli` on path and launches it as a subprocess
     connection = 'ipc://'
     # or, use TCP: connection = 'tcp://HOST:PORT'
 
-    signal = await create(Account('+12345678900'), connection)
+    signal = await create(AccountNumber('+12345678900'), connection)
     signal.on_keyword('ok?', crabby_callback)
     await signal.run()
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
```

### Comparing `signal_bot_framework-0.1.0/src/signal_bot_framework.egg-info/SOURCES.txt` & `signal_bot_framework-0.2/src/signal_bot_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

