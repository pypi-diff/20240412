# Comparing `tmp/cypartagraphqlsubscriptionstools-1.1.0.tar.gz` & `tmp/cypartagraphqlsubscriptionstools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cypartagraphqlsubscriptionstools-1.1.0.tar", last modified: Sat Apr  6 22:34:04 2024, max compression
+gzip compressed data, was "cypartagraphqlsubscriptionstools-1.1.1.tar", last modified: Fri Apr 12 03:58:23 2024, max compression
```

## Comparing `cypartagraphqlsubscriptionstools-1.1.0.tar` & `cypartagraphqlsubscriptionstools-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.396942 cypartagraphqlsubscriptionstools-1.1.0/
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.390275 cypartagraphqlsubscriptionstools-1.1.0/.vscode/
--rw-r--r--   0 eslam     (1000) eslam     (1003)      791 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/.vscode/launch.json
--rw-r--r--   0 eslam     (1000) eslam     (1003)       69 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/.vscode/settings.json
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.386942 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.github/
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.github/workflows/
--rw-r--r--   0 eslam     (1000) eslam     (1003)      409 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.github/workflows/test.yml
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1121 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.gitignore
--rw-r--r--   0 eslam     (1000) eslam     (1003)       89 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/__init__.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)       86 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/admin.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      128 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/apps.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     7310 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/consumers.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      800 2024-03-14 22:41:03.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/events.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1046 2024-04-06 21:47:52.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/middleware.py
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/
--rw-r--r--   0 eslam     (1000) eslam     (1003)      711 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)        0 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/__init__.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1254 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/mixins.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      342 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/models.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      359 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/routing.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     3601 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/schema.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      925 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/serialize.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      320 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/urls.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      648 2024-03-14 22:24:44.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/utils.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)      709 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/views.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1079 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/LICENSE
--rw-r--r--   0 eslam     (1000) eslam     (1003)    14736 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/PKG-INFO
--rw-r--r--   0 eslam     (1000) eslam     (1003)    13819 2024-04-06 21:57:21.000000 cypartagraphqlsubscriptionstools-1.1.0/README.md
--rw-r--r--   0 eslam     (1000) eslam     (1003)    30445 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/cover.jpg
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/
--rw-r--r--   0 eslam     (1000) eslam     (1003)    14736 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1273 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)        1 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/dependency_links.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)       55 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/requires.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)       33 2024-04-06 22:34:04.000000 cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/top_level.txt
-drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-06 22:34:04.393608 cypartagraphqlsubscriptionstools-1.1.0/dist/
--rw-r--r--   0 eslam     (1000) eslam     (1003)   522166 2024-04-06 22:21:03.000000 cypartagraphqlsubscriptionstools-1.1.0/dist/cypartagraphqlsubscriptionstools-1.0.0.tar.gz
--rw-r--r--   0 eslam     (1000) eslam     (1003)   499268 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/graph.jpg
--rwxr-xr-x   0 eslam     (1000) eslam     (1003)      663 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/manage.py
--rw-r--r--   0 eslam     (1000) eslam     (1003)       77 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.0/requirements.txt
--rw-r--r--   0 eslam     (1000) eslam     (1003)       38 2024-04-06 22:34:04.396942 cypartagraphqlsubscriptionstools-1.1.0/setup.cfg
--rw-r--r--   0 eslam     (1000) eslam     (1003)     1243 2024-04-06 22:33:46.000000 cypartagraphqlsubscriptionstools-1.1.0/setup.py
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-12 03:58:23.156746 cypartagraphqlsubscriptionstools-1.1.1/
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-12 03:58:23.153413 cypartagraphqlsubscriptionstools-1.1.1/.vscode/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      791 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/.vscode/launch.json
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       69 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/.vscode/settings.json
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-12 03:58:23.156746 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-12 03:58:23.150080 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/.github/
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-12 03:58:23.156746 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/.github/workflows/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      409 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/.github/workflows/test.yml
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1121 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/.gitignore
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       89 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/__init__.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       86 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/admin.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      128 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/apps.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     7522 2024-04-12 03:52:04.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/consumers.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      800 2024-03-14 22:41:03.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/events.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1046 2024-04-06 21:47:52.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/middleware.py
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-12 03:58:23.156746 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/migrations/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      711 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)        0 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/migrations/__init__.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1254 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/mixins.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      342 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/models.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      359 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/routing.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     3601 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/schema.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      925 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/serialize.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      320 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/urls.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      648 2024-03-14 22:24:44.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/utils.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)      709 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/views.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1079 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/LICENSE
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    14736 2024-04-12 03:58:23.156746 cypartagraphqlsubscriptionstools-1.1.1/PKG-INFO
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    13819 2024-04-06 21:57:21.000000 cypartagraphqlsubscriptionstools-1.1.1/README.md
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    30445 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/cover.jpg
+drwxr-xr-x   0 eslam     (1000) eslam     (1003)        0 2024-04-12 03:58:23.156746 cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/
+-rw-r--r--   0 eslam     (1000) eslam     (1003)    14736 2024-04-12 03:58:22.000000 cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1222 2024-04-12 03:58:23.000000 cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)        1 2024-04-12 03:58:22.000000 cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/dependency_links.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       55 2024-04-12 03:58:22.000000 cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/requires.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       33 2024-04-12 03:58:22.000000 cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/top_level.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)   499268 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/graph.jpg
+-rwxr-xr-x   0 eslam     (1000) eslam     (1003)      663 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/manage.py
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       77 2024-03-12 16:56:38.000000 cypartagraphqlsubscriptionstools-1.1.1/requirements.txt
+-rw-r--r--   0 eslam     (1000) eslam     (1003)       38 2024-04-12 03:58:23.156746 cypartagraphqlsubscriptionstools-1.1.1/setup.cfg
+-rw-r--r--   0 eslam     (1000) eslam     (1003)     1243 2024-04-12 03:58:08.000000 cypartagraphqlsubscriptionstools-1.1.1/setup.py
```

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/.vscode/launch.json` & `cypartagraphqlsubscriptionstools-1.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/.gitignore` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/.gitignore`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/consumers.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/consumers.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,21 +60,25 @@
     async def send_ping(self):
         # Periodically send ping messages to keep the connection alive
         while True:
             await self.send_json({'type': self.ping_command})
             await asyncio.sleep(self.ping_interval)
 
     async def _send_result(self, id, result):
+        errors = result.errors
+        #xx=list(map(errors.formatted, errors))
+        formatted_errors = [error.formatted for error in errors] if errors else None
         # Send subscription results back to the client
         await self.send_json(
             {
                 "id": id,
                 "type": self.result_command,
                 "payload": {
                     "data": result.data,
+                    "errors": formatted_errors 
                 },
             }
         )
 
 class CypartaGraphqlSubscriptionsConsumer(DetectWebSocketType):
     # Dictionary to store WebSocket groups
     groups = {}
```

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/events.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/events.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/middleware.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/middleware.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/mixins.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/mixins.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/schema.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/schema.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/serialize.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/serialize.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/utils.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/utils.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/CypartaGraphqlSubscriptionsTools/views.py` & `cypartagraphqlsubscriptionstools-1.1.1/CypartaGraphqlSubscriptionsTools/views.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/LICENSE` & `cypartagraphqlsubscriptionstools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/PKG-INFO` & `cypartagraphqlsubscriptionstools-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cypartagraphqlsubscriptionstools
-Version: 1.1.0
+Version: 1.1.1
 Summary: A CypartaGraphqlSubscriptionsTools implementation for Graphene + Django built using Django Channels +reactive programming in python (RxPY) . Provides support for model creation, mutation and deletion,and get data with websocket or path list of events name for subscriptions .
 Home-page: https://cyparta.com/
 Author: Cyparta Software House
 Author-email: Support@cyparta.com
 License: LICENSE
 Project-URL: homepage, https://cyparta.com/
 Project-URL: Documentation, https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools
```

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/README.md` & `cypartagraphqlsubscriptionstools-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/cover.jpg` & `cypartagraphqlsubscriptionstools-1.1.1/cover.jpg`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO` & `cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cypartagraphqlsubscriptionstools
-Version: 1.1.0
+Version: 1.1.1
 Summary: A CypartaGraphqlSubscriptionsTools implementation for Graphene + Django built using Django Channels +reactive programming in python (RxPY) . Provides support for model creation, mutation and deletion,and get data with websocket or path list of events name for subscriptions .
 Home-page: https://cyparta.com/
 Author: Cyparta Software House
 Author-email: Support@cyparta.com
 License: LICENSE
 Project-URL: homepage, https://cyparta.com/
 Project-URL: Documentation, https://github.com/Cyparta/CypartaGraphqlSubscriptionsTools
```

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt` & `cypartagraphqlsubscriptionstools-1.1.1/cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,8 @@
 CypartaGraphqlSubscriptionsTools/.github/workflows/test.yml
 CypartaGraphqlSubscriptionsTools/migrations/0001_initial.py
 CypartaGraphqlSubscriptionsTools/migrations/__init__.py
 cypartagraphqlsubscriptionstools.egg-info/PKG-INFO
 cypartagraphqlsubscriptionstools.egg-info/SOURCES.txt
 cypartagraphqlsubscriptionstools.egg-info/dependency_links.txt
 cypartagraphqlsubscriptionstools.egg-info/requires.txt
-cypartagraphqlsubscriptionstools.egg-info/top_level.txt
-dist/cypartagraphqlsubscriptionstools-1.0.0.tar.gz
+cypartagraphqlsubscriptionstools.egg-info/top_level.txt
```

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/graph.jpg` & `cypartagraphqlsubscriptionstools-1.1.1/graph.jpg`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/manage.py` & `cypartagraphqlsubscriptionstools-1.1.1/manage.py`

 * *Files identical despite different names*

### Comparing `cypartagraphqlsubscriptionstools-1.1.0/setup.py` & `cypartagraphqlsubscriptionstools-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 import setuptools
 
 setuptools.setup(
     name="cypartagraphqlsubscriptionstools",
-    version="1.1.0",
+    version="1.1.1",
     description = "A CypartaGraphqlSubscriptionsTools implementation for Graphene + Django built using Django Channels +reactive programming in python (RxPY) . Provides support for model creation, mutation and deletion,and get data with websocket or path list of events name for subscriptions .",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://cyparta.com/",
     author="Cyparta Software House",
     author_email="Support@cyparta.com",
     license="LICENSE",
```

