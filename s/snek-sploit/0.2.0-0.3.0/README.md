# Comparing `tmp/snek_sploit-0.2.0.tar.gz` & `tmp/snek_sploit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek_sploit-0.2.0.tar", max compression
+gzip compressed data, was "snek_sploit-0.3.0.tar", max compression
```

## Comparing `snek_sploit-0.2.0.tar` & `snek_sploit-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-10-06 17:59:31.968076 snek_sploit-0.2.0/LICENSE
--rw-r--r--   0        0        0     1601 2023-11-22 14:26:28.235084 snek_sploit-0.2.0/README.md
--rw-r--r--   0        0        0      603 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       76 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/__init__.py
--rw-r--r--   0        0        0        0 2023-10-06 15:26:11.900129 snek_sploit-0.2.0/snek_sploit/lib/__init__.py
--rw-r--r--   0        0        0     1082 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/base.py
--rw-r--r--   0        0        0     2594 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/client.py
--rw-r--r--   0        0        0     3581 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/context.py
--rw-r--r--   0        0        0      423 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/__init__.py
--rw-r--r--   0        0        0      390 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/auth.py
--rw-r--r--   0        0        0      241 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/console.py
--rw-r--r--   0        0        0      219 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/core.py
--rw-r--r--   0        0        0      213 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/db.py
--rw-r--r--   0        0        0      225 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/health.py
--rw-r--r--   0        0        0      216 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/job.py
--rw-r--r--   0        0        0      225 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/module.py
--rw-r--r--   0        0        0      225 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/plugin.py
--rw-r--r--   0        0        0      228 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/groups/session.py
--rw-r--r--   0        0        0      747 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/__init__.py
--rw-r--r--   0        0        0     2749 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/auth.py
--rw-r--r--   0        0        0     7319 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/console.py
--rw-r--r--   0        0        0     7722 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/core.py
--rw-r--r--   0        0        0    12181 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/db.py
--rw-r--r--   0        0        0      558 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/health.py
--rw-r--r--   0        0        0     2475 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/job.py
--rw-r--r--   0        0        0    19695 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/module.py
--rw-r--r--   0        0        0     1456 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/plugin.py
--rw-r--r--   0        0        0    15493 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/lib/rpc/session.py
--rw-r--r--   0        0        0        0 2023-10-06 15:26:11.900129 snek_sploit-0.2.0/snek_sploit/util/__init__.py
--rw-r--r--   0        0        0     1887 2023-11-22 14:26:28.239084 snek_sploit-0.2.0/snek_sploit/util/constants.py
--rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 snek_sploit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-12 09:29:23.618328 snek_sploit-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1420 2024-04-12 09:29:23.618328 snek_sploit-0.3.0/README.md
+-rw-r--r--   0        0        0      603 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1178 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/__init__.py
+-rw-r--r--   0        0        0     4600 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/context.py
+-rw-r--r--   0        0        0     3010 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/metasploit.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/__init__.py
+-rw-r--r--   0        0        0     3085 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/auth.py
+-rw-r--r--   0        0        0     9243 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/consoles.py
+-rw-r--r--   0        0        0     7887 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/core.py
+-rw-r--r--   0        0        0    12329 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/db.py
+-rw-r--r--   0        0        0      727 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/health.py
+-rw-r--r--   0        0        0     2641 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/jobs.py
+-rw-r--r--   0        0        0    19857 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/modules.py
+-rw-r--r--   0        0        0     1628 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/plugins.py
+-rw-r--r--   0        0        0    23772 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/sessions.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/util/__init__.py
+-rw-r--r--   0        0        0     1887 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/util/constants.py
+-rw-r--r--   0        0        0      446 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/util/enums.py
+-rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 snek_sploit-0.3.0/PKG-INFO
```

### Comparing `snek_sploit-0.2.0/LICENSE` & `snek_sploit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.2.0/README.md` & `snek_sploit-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 # snek-sploit
 Python typed RPC client for Metasploit Framework.
 
 ![](logo.png)
 
+## Installation
+
+```shell
+pip install snek-sploit
+```
+
+## Usage
+
 ```python
-from snek_sploit import Client
+from snek_sploit import MetasploitClient
+
 
 if __name__ == '__main__':
-    client = Client("msf", "root")
+    client = MetasploitClient("msf", "root")
     print(client.core.rpc.version())
 
 ```
 
-## Installation
-
-```shell
-pip install snek-sploit
-```
-
 ## Starting MSF RPC server
-In console
+In Metasploit console:
 ```shell
 load msgrpc ServerHost=127.0.0.1 ServerPort=55553 User=msf Pass='root' SSL=true
 ```
 
-In the background
+In shell:
 ```shell
 msfrpcd -U msf -P root
 ```
 
-More information can be found in the [MSF official documentation](https://docs.rapid7.com/metasploit/rpc-api/).
-
-### Using the MSF's certificate
-Certificate is by default taken from `/root/.msf4/msf-ws-cert.pem` (use the `-c` flag to choose a different location). If it's not, generate it as mentioned [here](https://github.com/rapid7/metasploit-framework/issues/15569#issuecomment-901158008).
-
-## Running MSF with RPC using Docker Compose
-Make sure you've installed [Docker Compose](https://docs.docker.com/compose/install/).
+With [Docker](https://docs.docker.com/engine/install/):
+```shell
+docker run --tty --network host --detach sadparad1se/metasploit-framework:rpc
+```
 
-In case you don't want to set up MSF RPC on your own, here is a convenient Compose config with MSF RPC and database:
+With [Docker Compose](https://docs.docker.com/compose/install/):
 ```shell
+git clone https://github.com/SadParad1se/snek-sploit.git
+cd snek-sploit
 docker compose up -d
 ```
 
-[Link to the MSF image documentation](https://cryton.gitlab-pages.ics.muni.cz/cryton-documentation/latest/docker-settings/#metasploit-framework).
+You can find more information in the [Metasploit Framework documentation](https://docs.rapid7.com/metasploit/rpc-api/).
 
-## TODO list
-- Typing and parameter support for the DB RPC class
-- async vs sync version?
-- Add custom exceptions
-- Wrapper classes for easier [workflows](https://docs.metasploit.com/docs/using-metasploit/advanced/RPC/how-to-use-metasploit-messagepack-rpc.html#example-workflows) (session, console, etc.)
+### Using the MSF RPC certificate
+MSF RPC loads the SSL certificate by default from `/root/.msf4/msf-ws-cert.pem` (use the `-c` flag to choose a different location). If not, generate it as mentioned [here](https://github.com/rapid7/metasploit-framework/issues/15569#issuecomment-901158008).
+
+To use it in the client, save it locally and pass the path:
+```python
+from snek_sploit import MetasploitClient
+
+
+MetasploitClient("msf", "root", certificate="/path/to/cert.pem")
+
+```
```

### Comparing `snek_sploit-0.2.0/pyproject.toml` & `snek_sploit-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snek-sploit"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python RPC client for Metasploit Framework"
 authors = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
 maintainers = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
@@ -15,13 +15,13 @@
     "metasploit", "msf", "rpc", "client"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
-msgpack = "^1.0.7"
+msgpack = "^1.0.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/__init__.py` & `snek_sploit-0.3.0/snek_sploit/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,35 @@
-from snek_sploit.lib.rpc.auth import RPCAuth
-from snek_sploit.lib.rpc.console import RPCConsole, ConsoleInfo, ConsoleData, ConsoleOptions
-from snek_sploit.lib.rpc.core import RPCCore, ModuleStatistics, VersionInformation, FrameworkThread
-from snek_sploit.lib.rpc.db import RPCDB  # TODO: add missing
-from snek_sploit.lib.rpc.health import RPCHealth
-from snek_sploit.lib.rpc.job import RPCJob, JobInformation
-from snek_sploit.lib.rpc.module import (RPCModule, ModuleType, EncodingOptions, ModuleShortInfo, ModuleExecutionInfo,
-                                        ModuleRunningStatistics)
-from snek_sploit.lib.rpc.plugin import RPCPlugin
-from snek_sploit.lib.rpc.session import RPCSession, SessionInformation, MeterpreterSessionTransportOptions
+__all__ = [
+    "MetasploitClient",
+    "ConsoleInfo",
+    "ConsoleData",
+    "ConsoleOptions",
+    "ModuleStatistics",
+    "VersionInformation",
+    "FrameworkThread",
+    "JobInformation",
+    "ModuleType",
+    "EncodingOptions",
+    "ModuleShortInfo",
+    "ModuleExecutionInfo",
+    "ModuleRunningStatistics",
+    "SessionInformation",
+    "MeterpreterSessionTransportOptions",
+    "SessionShell",
+    "SessionMeterpreter",
+    "SessionRing"
+]
+
+from snek_sploit.lib.metasploit import MetasploitClient
+# from snek_sploit.lib.rpc.auth import
+from snek_sploit.lib.rpc.consoles import ConsoleInfo, ConsoleData, ConsoleOptions
+from snek_sploit.lib.rpc.core import ModuleStatistics, VersionInformation, FrameworkThread
+# from snek_sploit.lib.rpc.db import
+# from snek_sploit.lib.rpc.health import
+from snek_sploit.lib.rpc.jobs import JobInformation
+from snek_sploit.lib.rpc.modules import (
+    ModuleType, EncodingOptions, ModuleShortInfo, ModuleExecutionInfo, ModuleRunningStatistics
+)
+# from snek_sploit.lib.rpc.plugins import
+from snek_sploit.lib.rpc.sessions import (
+    SessionInformation, MeterpreterSessionTransportOptions, SessionShell, SessionMeterpreter, SessionRing
+)
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/auth.py` & `snek_sploit-0.3.0/snek_sploit/lib/rpc/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from snek_sploit.lib.base import Base
+from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants
 
 
-class RPCAuth(Base):
+class RPCAuth(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Auth.html
     """
     LOGIN = "auth.login"
     LOGOUT = "auth.logout"
     TOKEN_ADD = "auth.token_add"
     TOKEN_REMOVE = "auth.token_remove"
@@ -75,7 +75,18 @@
         Generate a new token and save it to the Database.
         :return: New token
         :full response example: {b'result': b'success', b'token': b'TEMP6120290898789284108532566914'}
         """
         response = self._context.call(self.TOKEN_GENERATE)
 
         return response[constants.B_TOKEN].decode()
+
+
+class Auth(ContextBase):
+    def __init__(self, context: Context):
+        super().__init__(context)
+        self.rpc = RPCAuth(context)
+
+    def login(self):
+        token = self.rpc.login(self._context.username, self._context.password)
+        self._context.token = token
+        self.rpc.token_add(token)
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/console.py` & `snek_sploit-0.3.0/snek_sploit/lib/rpc/consoles.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass, asdict
 from typing import List
+import time
 
-from snek_sploit.lib.base import Base
+from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants
 
 
 @dataclass
 class ConsoleInfo:
     """
     Information about the console.
@@ -18,15 +19,15 @@
 @dataclass
 class ConsoleData:
     """
     Information about the console, including returned data.
     """
     prompt: str
     busy: bool
-    data: List[str]
+    data: str
 
 
 @dataclass
 class ConsoleOptions:
     """
     Options used to initialize the console.
     Only the relevant options are mentioned here, since some are always modified by the MSF.
@@ -41,15 +42,15 @@
     Config: str = None  # Path to the config file
     ConfirmExit: bool = None  # Whether to confirm before exiting
     XCommands: List[str] = None  # Additional startup commands
     DisableBanner: bool = None  # Whether to disable the banner on startup
     Plugins: List[str] = None  # Plugins to load
 
 
-class RPCConsole(Base):
+class RPCConsoles(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Console.html
     """
     CREATE = "console.create"
     DESTROY = "console.destroy"
     LIST = "console.list"
     READ = "console.read"
@@ -77,15 +78,15 @@
         Get console data from the response.
         :param response: API response containing the necessary data
         :return: Information about the console and its data
         """
         return ConsoleData(
             response[constants.B_PROMPT].decode(),
             response[constants.B_BUSY],
-            [data.decode() for data in response[constants.B_DATA]]
+            response[constants.B_DATA].decode()
         )
 
     def create(self, options: ConsoleOptions = None) -> ConsoleInfo:
         """
         Create a new framework console instance.
         :param options: Options used for creating the console
         :return: Information about the console
@@ -197,7 +198,72 @@
         """
         response = self._context.call(self.SESSION_DETACH, [console_id])
 
         if response[constants.B_RESULT] == constants.B_FAILURE:
             raise Exception("Invalid console ID")
 
         return response[constants.B_RESULT] == constants.B_SUCCESS
+
+
+class Console:
+    def __init__(self, rpc: RPCConsoles, console_id: int):
+        self._rpc = rpc
+        self.id = console_id
+
+    def read(self) -> ConsoleData:
+        return self._rpc.read(self.id)
+
+    def write(self, data: str, add_new_line: bool = True) -> None:
+        self._rpc.write(self.id, data, add_new_line)
+
+    def destroy(self) -> bool:
+        return self._rpc.destroy(self.id)
+
+    def tabs(self, line: str) -> List[str]:
+        return self._rpc.tabs(self.id, line)
+
+    def gather_output(self, timeout: float = None, reading_delay: float = 1) -> str:
+        """
+        Gather output from the console.
+        :param timeout: The maximum time to wait for the output
+        :param reading_delay: Delay between the readings
+        :return: Gathered output
+        """
+        if timeout is not None:
+            timeout = time.time() + timeout
+
+        output = ""
+        # TODO: shell wont be busy until the command is executed, check for the execution
+        while (console := self.read()).busy:
+            output += console.data
+
+            if timeout and time.time() >= timeout:
+                break
+            time.sleep(reading_delay)
+
+        return output
+
+    def clear_buffer(self) -> None:
+        """
+        Clear unread data from the console.
+        :return: None
+        """
+        self.read()
+
+    def execute(self, command: str, timeout: float = None, reading_delay: float = 1) -> str:
+        self.clear_buffer()
+        self.write(command)
+
+        return self.gather_output(timeout, reading_delay)
+
+
+class Consoles(ContextBase):
+    def __init__(self, context: Context):
+        super().__init__(context)
+        self.rpc = RPCConsoles(context)
+
+    def create(self, options: ConsoleOptions = None):
+        console_info = self.rpc.create(options)
+        return Console(self.rpc, console_info.id)
+
+    def all(self):
+        return self.rpc.list_consoles()
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/core.py` & `snek_sploit-0.3.0/snek_sploit/lib/rpc/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from requests import ReadTimeout
 from dataclasses import dataclass
 from typing import Union, Dict
 
-from snek_sploit.lib.base import Base
+from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants
 
 
 @dataclass
 class ModuleStatistics:
     """
     Number of installed modules.
@@ -37,15 +37,15 @@
     """
     status: str
     critical: bool
     name: str
     started: str
 
 
-class RPCCore(Base):
+class RPCCore(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Core.html
     """
     VERSION = "core.version"
     STOP = "core.stop"
     GETG = "core.getg"
     SETG = "core.setg"
@@ -236,7 +236,13 @@
         :param thread_id: ID of the thread
         :return: True in case of success
         :full response example: {b'result': b'success'}
         """
         response = self._context.call(self.THREAD_KILL, [thread_id])
 
         return response[constants.B_RESULT] == constants.B_SUCCESS
+
+
+class Core(ContextBase):
+    def __init__(self, context: Context):
+        super().__init__(context)
+        self.rpc = RPCCore(context)
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/db.py` & `snek_sploit-0.3.0/snek_sploit/lib/rpc/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, asdict
-from typing import List, Dict, Union
+from typing import Dict
 
-from snek_sploit.lib.base import Base
+from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants
 
 
 @dataclass
 class CrackedCredentialOptions:
     username: str
     password: str
@@ -40,15 +40,15 @@
 
 @dataclass
 class AnalyzeHost:
     pass
 
 
 # TODO unfinished, untested
-class RPCDB(Base):
+class RPCDB(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Db.html
     """
     CREATE_CRACKED_CREDENTIAL = "db.create_cracked_credential"
     CREATE_CREDENTIAL = "db.create_credential"
     INVALIDATE_LOGIN = "db.invalidate_login"
     CREDS = "db.creds"
@@ -513,7 +513,13 @@
 
         :return:
         :full response example:
         """
         response = self._context.call(self.STATUS, list(args))
 
         return response
+
+
+class DB(ContextBase):
+    def __init__(self, context: Context):
+        super().__init__(context)
+        self.rpc = RPCDB(context)
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/job.py` & `snek_sploit-0.3.0/snek_sploit/lib/rpc/jobs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Dict, Any
 from dataclasses import dataclass
 
-from snek_sploit.lib.base import Base
+from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants
 
 
 @dataclass
 class JobInformation:
     id: int
     name: str
     start_time: int
     datastore: Dict[str, Any]
 
 
-class RPCJob(Base):
+class RPCJobs(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Job.html
     """
     INFO = "job.info"
     LIST = "job.list"
     STOP = "job.stop"
 
@@ -64,7 +64,13 @@
         :param job_id: ID of the job
         :return: True in case of success
         :full response example: {b'result': b'success'}
         """
         response = self._context.call(self.STOP, [job_id])
 
         return response[constants.B_RESULT] == constants.B_SUCCESS
+
+
+class Jobs(ContextBase):
+    def __init__(self, context: Context):
+        super().__init__(context)
+        self.rpc = RPCJobs(context)
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/module.py` & `snek_sploit-0.3.0/snek_sploit/lib/rpc/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from enum import StrEnum
 from typing import List, Dict, Union, Any
 from dataclasses import dataclass, asdict
 
-from snek_sploit.lib.base import Base
+from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants
+from snek_sploit.util.enums import ModuleType
 
 
 @dataclass
 class ModuleShortInfo:
     """
     Short module information.
     """
@@ -69,26 +69,15 @@
     ecount: int = None
     inject: bool = None
     template: str = None
     template_path: str = None
     addshellcode: str = None
 
 
-class ModuleType(StrEnum):
-    """
-    List of the existing module types.
-    """
-    exploit = "exploit"
-    auxiliary = "auxiliary"
-    post = "post"
-    nop = "nop"
-    payload = "payload"
-
-
-class RPCModule(Base):
+class RPCModules(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Module.html
     """
     EXPLOITS = "module.exploits"
     EVASION = "module.evasion"
     AUXILIARY = "module.auxiliary"
     PAYLOADS = "module.payloads"
@@ -368,15 +357,15 @@
         :full response example: {b'waiting': [], b'running': [b'RNEN1jKepDfcWLpvuPlmhktc'], b'results': []}
         """
         response = self._context.call(self.RUNNING_STATS)
 
         return ModuleRunningStatistics(
             [each.decode() for each in response[constants.B_WAITING]],
             [each.decode() for each in response[constants.B_RUNNING]],
-            [each.decode() for each in response[constants.B_RESULTS]]
+            response[constants.B_RESULTS]
         )
 
     def list_module_options(self, module_type: ModuleType, module_name: str) \
             -> Dict[str, Dict[str, Union[dict, list, str, bool, int]]]:
         """
         Get module's datastore options.
         :param module_type: Module type
@@ -508,7 +497,18 @@
         :full response example:
             {b'encoded': b'unsigned char buf[] = \n"\\xd9\\xcd\\xd9\\x74\\x24\\xf4\\xb8\\x0e\\xe8\\xda\\x15\\x5b
              \\x33\\xc9"\n"\\xb1\\x01\\x31\\x43\\x18\\x03\\x43\\x18\\x83\\xeb\\xf2\\x0a\\x2f\\x54";\n'}
         """
         response = self._context.call(self.ENCODE, [data, encoder, asdict(options)])
 
         return response[constants.B_ENCODED].decode()
+
+
+class Modules(ContextBase):
+    def __init__(self, context: Context):
+        super().__init__(context)
+        self.rpc = RPCModules(context)
+
+    # def execute(self, ):
+    #     self.rpc.execute()
+    # # TODO: use console for everything
+    # #  https://github.com/rapid7/metasploit-framework/issues/18241#issuecomment-1662496538
```

### Comparing `snek_sploit-0.2.0/snek_sploit/lib/rpc/plugin.py` & `snek_sploit-0.3.0/snek_sploit/lib/rpc/plugins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from snek_sploit.lib.base import Base
+from snek_sploit.lib.context import ContextBase, Context
 from snek_sploit.util import constants
 
 
-class RPCPlugin(Base):
+class RPCPlugins(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Plugin.html
     """
     LOAD = "plugin.load"
     UNLOAD = "plugin.unload"
     LOADED = "plugin.loaded"
 
@@ -43,7 +43,13 @@
         List loaded plugins.
         :return: List of loaded plugins
         :full response example: {'plugins': ['msgrpc']}
         """
         response = self._context.call(self.LOADED)
 
         return response[constants.PLUGINS]
+
+
+class Plugins(ContextBase):
+    def __init__(self, context: Context):
+        super().__init__(context)
+        self.rpc = RPCPlugins(context)
```

### Comparing `snek_sploit-0.2.0/snek_sploit/util/constants.py` & `snek_sploit-0.3.0/snek_sploit/util/constants.py`

 * *Files identical despite different names*

