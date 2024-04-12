# Comparing `tmp/eezo-0.1.8.tar.gz` & `tmp/eezo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eezo-0.1.8.tar", last modified: Wed Apr 10 19:48:11 2024, max compression
+gzip compressed data, was "eezo-0.2.0.tar", last modified: Fri Apr 12 09:01:53 2024, max compression
```

## Comparing `eezo-0.1.8.tar` & `eezo-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.251496 eezo-0.1.8/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-10 19:48:11.251389 eezo-0.1.8/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.8/README.md
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.249508 eezo-0.1.8/eezo/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.8/eezo/async_client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-04-10 16:05:56.000000 eezo-0.1.8/eezo/client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    11720 2024-04-10 18:30:47.000000 eezo-0.1.8/eezo/connector.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.250472 eezo-0.1.8/eezo/interface/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      106 2024-04-10 17:54:01.000000 eezo-0.1.8/eezo/interface/__init__.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.251239 eezo-0.1.8/eezo/interface/components/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/chart.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/component.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/image.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/text.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/components/youtube_video.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     5824 2024-04-10 18:29:33.000000 eezo-0.1.8/eezo/interface/interface.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     5974 2024-04-10 19:39:16.000000 eezo-0.1.8/eezo/interface/interface_async.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.8/eezo/interface/message.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-10 19:48:11.250028 eezo-0.1.8/eezo.egg-info/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      567 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/SOURCES.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/dependency_links.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      367 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/requires.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-10 19:48:11.000000 eezo-0.1.8/eezo.egg-info/top_level.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-10 19:48:11.251532 eezo-0.1.8/setup.cfg
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1946 2024-04-10 19:45:26.000000 eezo-0.1.8/setup.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 09:01:53.394338 eezo-0.2.0/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-12 09:01:53.394214 eezo-0.2.0/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.2.0/README.md
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 09:01:53.390962 eezo-0.2.0/eezo/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.2.0/eezo/async_client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-04-10 16:05:56.000000 eezo-0.2.0/eezo/client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    12191 2024-04-12 08:54:26.000000 eezo-0.2.0/eezo/connector.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 09:01:53.392609 eezo-0.2.0/eezo/interface/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      106 2024-04-10 17:54:01.000000 eezo-0.2.0/eezo/interface/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 09:01:53.394030 eezo-0.2.0/eezo/interface/components/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/interface/components/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/interface/components/chart.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/interface/components/component.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/interface/components/image.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/interface/components/text.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/interface/components/youtube_video.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     5824 2024-04-10 18:29:33.000000 eezo-0.2.0/eezo/interface/interface.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     5974 2024-04-12 08:48:22.000000 eezo-0.2.0/eezo/interface/interface_async.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.2.0/eezo/interface/message.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-12 09:01:53.391766 eezo-0.2.0/eezo.egg-info/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-12 09:01:53.000000 eezo-0.2.0/eezo.egg-info/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      567 2024-04-12 09:01:53.000000 eezo-0.2.0/eezo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-12 09:01:53.000000 eezo-0.2.0/eezo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      367 2024-04-12 09:01:53.000000 eezo-0.2.0/eezo.egg-info/requires.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-12 09:01:53.000000 eezo-0.2.0/eezo.egg-info/top_level.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-12 09:01:53.394374 eezo-0.2.0/setup.cfg
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1946 2024-04-12 09:01:15.000000 eezo-0.2.0/setup.py
```

### Comparing `eezo-0.1.8/PKG-INFO` & `eezo-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.8
+Version: 0.2.0
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.8/README.md` & `eezo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/eezo/async_client.py` & `eezo-0.2.0/eezo/async_client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/eezo/client.py` & `eezo-0.2.0/eezo/client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/eezo/connector.py` & `eezo-0.2.0/eezo/connector.py`

 * *Files 25% similar despite different names*

```diff
@@ -128,60 +128,68 @@
                 success=False,
                 error=str(e),
                 traceback=traceback.format_exc(),
                 error_tag="Connector error",
             )
             await self.sio.emit("job_completed", job_completed.to_dict())
 
+    async def __handle_disconnect(self):
+        self.__log(f" ✖ Connector {self.connector_id} disconnected")
+        # Additional logic to determine if reconnect should be attempted
+        # For example, check if it was an expected disconnection or if a maximum number of retries has been reached
+        await self.__attempt_connect()
+
     async def connect(self):
         await self.__authenticate()
 
-        self.sio.on(
-            "disconnect",
-            lambda: self.__log(f" ✖ Connector {self.connector_id} disconnected"),
-        )
+        self.sio.on("disconnect", self.__handle_disconnect)
 
         def auth_error(message: str):
             self.__log(f" ✖ Authentication failed: {message}")
             self.run_loop = False
 
-        self.sio.on("job_request", lambda p: asyncio.create_task(self.__execute_job(p)))
-        self.sio.on("job_response", lambda p: self.job_responses.update({p["id"]: p}))
-        self.sio.on("token_expired", lambda: self.__authenticate())
+        async def job_response(response):
+            self.job_responses[response["id"]] = response
+
+        async def on_job_request(p):
+            await self.__execute_job(p)
+
+        async def on_token_expired():
+            await self.__authenticate()
+
+        self.sio.on("job_request", on_job_request)
+        self.sio.on("job_response", job_response)
+        self.sio.on("token_expired", on_token_expired)
         self.sio.on("auth_error", auth_error)
 
-        while self.run_loop:
+        await self.__attempt_connect()
+
+    async def __attempt_connect(self, retry_delay=5, max_retries=10):
+        retries = 0
+        while self.run_loop and retries < max_retries:
             try:
                 await self.sio.connect(SERVER)
                 await self.sio.wait()
-            except socketio.exceptions.ConnectionError as e:
-                if self.run_loop:
-                    if self.logger:
-                        self.__log(
-                            f" ✖ Connector {self.connector_id} failed to connect"
-                        )
-                        self.__log("   Retrying to connect...")
-                    await asyncio.sleep(5)
-                else:
-                    break
+                break  # Exit loop if connect is successful
+            except (socketio.exceptions.ConnectionError, Exception) as e:
+                self.__log(
+                    f" ✖ Connector {self.connector_id} failed to connect with error: {e}"
+                )
+                await asyncio.sleep(retry_delay)
+                retries += 1
+                if retries >= max_retries:
+                    self.__log("Reached maximum retries, stopping.")
+                    self.run_loop = False
             except KeyboardInterrupt:
+                self.__log("Manual interrupt, stopping.")
                 self.run_loop = False
                 break
-            except Exception as e:
-                if self.run_loop:
-                    if self.logger:
-                        self.__log(
-                            f" ✖ Connector {self.connector_id} failed to connect with error: {e}"
-                        )
-                        self.__log("   Retrying to connect...")
-                    await asyncio.sleep(5)
-                else:
-                    break
 
-        await self.sio.disconnect()
+        if not self.run_loop:
+            await self.sio.disconnect()
 
 
 class Connector:
     def __init__(self, api_key, connector_id, connector_function, logger=False):
         self.api_key = api_key
         self.logger = logger
         self.func = connector_function
@@ -275,56 +283,55 @@
                 success=False,
                 error=str(e),
                 traceback=str(traceback.format_exc()),
                 error_tag="Connector error",
             )
             self.sio.emit("job_completed", job_completed.to_dict())
 
+    def __handle_disconnect(self):
+        self.__log(f" ✖ Connector {self.connector_id} disconnected")
+        # Additional logic to determine if reconnect should be attempted
+        # For example, check if it was an expected disconnection or if a maximum number of retries has been reached
+        self.__attempt_connect()
+
     def connect(self):
         self.__authenticate()
 
-        self.sio.on(
-            "disconnect",
-            lambda: self.__log(f" ✖ Connector {self.connector_id} disconnected"),
-        )
+        self.sio.on("disconnect", self.__handle_disconnect)
 
         def auth_error(message: str):
             self.__log(f" ✖ Authentication failed: {message}")
             self.run_loop = False
 
         def job_response(response):
             self.job_responses[response["id"]] = response
 
         self.sio.on("job_request", lambda p: self.__execute_job(p))
         self.sio.on("job_response", job_response)
         self.sio.on("token_expired", lambda: self.__authenticate())
         self.sio.on("auth_error", auth_error)
 
-        while self.run_loop:
+        self.__attempt_connect()
+
+    def __attempt_connect(self, retry_delay=5, max_retries=10):
+        retries = 0
+        while self.run_loop and retries < max_retries:
             try:
                 self.sio.connect(SERVER)
                 self.sio.wait()
-            except socketio.exceptions.ConnectionError as e:
-                if self.run_loop:
-                    if self.logger:
-                        self.__log(
-                            f" ✖ Connector {self.connector_id} failed to connect"
-                        )
-                        self.__log("   Retrying to connect...")
-                    time.sleep(5)
-                else:
-                    break
+                break  # Exit loop if connect is successful
+            except (socketio.exceptions.ConnectionError, Exception) as e:
+                self.__log(
+                    f" ✖ Connector {self.connector_id} failed to connect with error: {e}"
+                )
+                time.sleep(retry_delay)
+                retries += 1
+                if retries >= max_retries:
+                    self.__log("Reached maximum retries, stopping.")
+                    self.run_loop = False
             except KeyboardInterrupt:
+                self.__log("Manual interrupt, stopping.")
                 self.run_loop = False
                 break
-            except Exception as e:
-                if self.run_loop:
-                    if self.logger:
-                        self.__log(
-                            f" ✖ Connector {self.connector_id} failed to connect with error: {e}"
-                        )
-                        self.__log("   Retrying to connect...")
-                    time.sleep(5)
-                else:
-                    break
 
-        self.sio.disconnect()
+        if not self.run_loop:
+            self.sio.disconnect()
```

### Comparing `eezo-0.1.8/eezo/interface/components/chart.py` & `eezo-0.2.0/eezo/interface/components/chart.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/eezo/interface/interface.py` & `eezo-0.2.0/eezo/interface/interface.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/eezo/interface/interface_async.py` & `eezo-0.2.0/eezo/interface/interface_async.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/eezo/interface/message.py` & `eezo-0.2.0/eezo/interface/message.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/eezo.egg-info/PKG-INFO` & `eezo-0.2.0/eezo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.8
+Version: 0.2.0
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.8/eezo.egg-info/SOURCES.txt` & `eezo-0.2.0/eezo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eezo-0.1.8/setup.py` & `eezo-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eezo",
-    version="0.1.8",
+    version="0.2.0",
     description="Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.",
     author="Daniel Schoenbohm",
     author_email="daniel@eezo.ai",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.9.3",
         "aiosignal==1.3.1",
```

