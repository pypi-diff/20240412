# Comparing `tmp/dungeonmaker-0.6.2.tar.gz` & `tmp/dungeonmaker-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dungeonmaker-0.6.2.tar", last modified: Sat Mar  9 11:36:09 2024, max compression
+gzip compressed data, was "dungeonmaker-0.6.3.tar", last modified: Fri Apr 12 17:50:07 2024, max compression
```

## Comparing `dungeonmaker-0.6.2.tar` & `dungeonmaker-0.6.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.678282 dungeonmaker-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-09 11:36:09.678282 dungeonmaker-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.674282 dungeonmaker-0.6.2/dungeonmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.674282 dungeonmaker-0.6.2/dungeonmaker/dm_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.674282 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.678282 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/dba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.678282 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/dba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/dmtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/dungeon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/room.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.678282 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/scratchcomms/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/scratchcomms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/scratchcomms/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/scratchcomms/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:36:09.678282 dungeonmaker-0.6.2/dungeonmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-09 11:36:09.000000 dungeonmaker-0.6.2/dungeonmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-09 11:36:09.000000 dungeonmaker-0.6.2/dungeonmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 11:36:09.000000 dungeonmaker-0.6.2/dungeonmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-09 11:36:09.000000 dungeonmaker-0.6.2/dungeonmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-09 11:36:09.000000 dungeonmaker-0.6.2/dungeonmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 11:36:09.678282 dungeonmaker-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-09 11:36:05.000000 dungeonmaker-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.958245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/dba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dmtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dungeon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/dungeonmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 17:50:07.000000 dungeonmaker-0.6.3/dungeonmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:50:07.962245 dungeonmaker-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-12 17:50:03.000000 dungeonmaker-0.6.3/setup.py
```

### Comparing `dungeonmaker-0.6.2/LICENSE` & `dungeonmaker-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/PKG-INFO` & `dungeonmaker-0.6.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.2
+Version: 0.6.3
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/backend.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/backend.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import pickle, hmac, json, secrets
 from hashlib import sha3_256
 from types import ModuleType
 from typing import Union, Any
 from dataclasses import dataclass, field
 from scratchcommunication.cloud_socket import CloudSocket
 from scratchcommunication.cloud import CloudConnection
+from scratchcommunication.cloudrequests import RequestHandler
 from scratchattach import get_project, Project
-from .modules.scratchcomms import RequestHandler
 from .modules.database import MongoDBDatabaseAbstraction, MongoDBAtlasSession
 from .modules.dm.session import DMSession
 from .modules.dm.selectors import DUNGEON, ROOM, USER
 from .modules.dm.user import User, s_vars
 
 @dataclass(slots=True)
 class DMBackend:
@@ -71,134 +71,135 @@
                 return "Username already exists."
             if len(password) < 3 or len(username) < 3:
                 return "Your username and password needs to be at least 3 characters long."
             self.current_client_data["logged_in"] = True
             self.current_client_data["username"] = username
             linked_user = linked_user.lower()
             if linked_user:
-                try:
-                    has_linked = self.dm_session.database_abstraction.select_user(fields={"linked_user": linked_user})
-                except KeyError:
-                    pass
-                else:
+                has_linked = user_has_linked(session=self.dm_session, user=linked_user)
+                if has_linked:
                     return f"You already have an account linked: {has_linked['username']}"
                 project = self.project
-                comments = project.comments()
-                for comment in comments:
-                    if comment["author"]["username"] != linked_user:
-                        continue
-                    if comment["content"] != f"My account: {username}":
-                        continue
-                    break
-                else:
-                    return f"Couldn't link your new account to your scratch username. Try commenting \"My account: {username}\" on the project again."
+                user = linked_user
+                comment = f"My account: {username}"
+                if not find_comment(project, content=comment, user=user):
+                    return f"Couldn't link your new account to your scratch username. Try commenting \"{comment}\" on the project again."
             else:
                 project = self.project
-                comments = project.comments()
-                for comment in comments:
-                    if comment["content"] != f"My account: {username}":
-                        continue
-                    break
-                else:
-                    return "Couldn't verify your username."
+                comment = f"My account: {username}"
+                if not find_comment(project=project, content=comment):
+                    return f"Couldn't verify your username. Try commenting \"{comment}\" on the project again."
             user = self.dm_session.create(USER, kwargs={"username": username, "passdata": passdata, "linked_user": linked_user})
             self.current_client_data["user_id"] = user.user_id
             user.write()
             return "Success!"
         
         @self.request_handler.request(name="load_private_profile", allow_python_syntax=True, auto_convert=True)
-        def load_private_profile() -> str:
+        def load_private_profile() -> json.dumps:
             if not self.current_client_data["logged_in"]:
-                return "You are not logged in."
-            return json.dumps(s_vars(self.find_current_client_user()))
+                return {"success": False, "result": None, "reason": "You are not logged in."}
+            user_data = s_vars(self.find_current_client_user())
+            user_data = include_data(user_data, include=
+                [
+                    "username", 
+                    "user_id",
+                    "admin_level",
+                    "linked_user",
+                    "recent_dungeons",
+                    "owned_dungeons",
+                    "permitted_dungeons",
+                    "passdata"
+                ]
+            )
+            user_data["passdata"] = "maybe not"
+            return {"success": True, "result": user_data, "reason": "success"}
                 
         @self.request_handler.request(name="load_profile", allow_python_syntax=True, auto_convert=True)
-        def load_profile(username : str = None, *, user_id : str = None) -> str:
+        def load_profile(username : str = None, *, user_id : str = None) -> json.dumps:
             try:
                 user = self.dm_session.find(USER, id=user_id, name=username)
             except KeyError:
-                return "That profile doesn't seem to exist."
+                return {"success": False, "result": None, "reason": "That profile doesn't seem to exist."}
             user_data = s_vars(user)
-            user_data.pop("passdata")
-            return json.dumps(user_data)
+            user_data = include_data(user_data, include=
+                [
+                    "username", 
+                    "user_id",
+                    "admin_level",
+                    "linked_user",
+                    "recent_dungeons",
+                    "owned_dungeons",
+                    "permitted_dungeons"
+                ]
+            )
+            return {"success": True, "result": user_data, "reason": "success"}
         
         @self.request_handler.request(name="link_user", allow_python_syntax=True, auto_convert=True)
         def link_user(linked_user : str, password : str) -> str:
             if not self.current_client_data["logged_in"]:
                 return "You are not logged in."
             linked_user = linked_user.lower()
-            try:
-                has_linked = self.dm_session.database_abstraction.select_user(fields={"linked_user": linked_user})
-            except KeyError:
-                pass
-            else:
+            has_linked = user_has_linked(session=self.dm_session, user=linked_user)
+            if has_linked:
                 return f"You already have an account linked: {has_linked['username']}"
             user = self.find_current_client_user()
             passdata = gen_passdata(username=self.current_client_data["username"], password=password)
             if passdata != user.passdata:
                 return "Wrong password."
             project = self.project
-            comments = project.comments()
             username = self.current_client_data["username"]
-            for comment in comments:
-                if comment["author"]["username"] != linked_user:
-                    continue
-                if comment["content"] != f"My account: {username}":
-                    continue
-                break
-            else:
-                return f"Couldn't link your new account to your scratch username. Try commenting \"My account: {username}\" on the project again."
+            comment = f"My account: {username}"
+            user = linked_user
+            if not find_comment(project=project, user=user):
+                return f"Couldn't link your new account to your scratch username. Try commenting \"{comment}\" on the project again."
             user.linked_user = linked_user
             user.write()
             return "Success!"
         
         @self.request_handler.request(name="unlink_user", allow_python_syntax=True, auto_convert=True)
         def unlink_user(password : str) -> str:
             if not self.current_client_data["logged_in"]:
                 return "You are not logged in."
             user = self.find_current_client_user()
             passdata = gen_passdata(username=self.current_client_data["username"], password=password)
             if passdata != user.passdata:
                 return "Wrong password."
-            project = self.project
             user.linked_user = None
             user.write()
             return "Success!"
         
         @self.request_handler.request(name="reset_password", allow_python_syntax=True, auto_convert=True)
-        def reset_password(username : str, password : str = None, linked_user : str = None, code : int = None):
+        def reset_password(username : str, password : str = None, linked_user : str = None, code : int = None) -> str:
             if code is None:
                 code = secrets.randbits(24)
                 self.current_client_data["password_reset_code"] = code
                 return f"Your password reset code is \"{code}\". Try commenting \"Password reset code: {code}\" using your linked account."
             if code != self.current_client_data["password_reset_code"]:
                 return "Wrong code."
             user = self.dm_session.find(USER, name=username)
             if linked_user != user.linked_user:
                 if user.linked_user is None:
                     return "You do not have a user linked, so you cannot reset your password like this. Try commenting on the project for help."
                 return "That is not your linked user."
             project = self.project
-            comments = project.comments()
-            for comment in comments:
-                if comment["author"]["username"] != linked_user:
-                    continue
-                if comment["content"] != f"Password reset code: {code}":
-                    continue
-                break
-            else:
-                return f"Couldn't verify your password reset request. Try commenting \"Password reset code: {code}\" on the project again."
+            comment = f"Password reset code: {code}"
+            user = linked_user
+            if not find_comment(project, content=comment, user=user):
+                return f"Couldn't verify your password reset request. Try commenting \"{comment}\" on the project again."
             passdata = gen_passdata(username=username, password=password)
             user.passdata = passdata
             user.write()
             return "Success!"
         
         self.request_handler.start(thread=thread)
         
     def stop(self):
+        """
+        Stop the dungeon maker backend.
+        """
         self.request_handler.stop()
         
     @property
     def current_client_data(self) -> dict:
         """
         Client data of the current user
         """
@@ -219,23 +220,52 @@
         return self.dm_session.find(USER, self.current_client_data["user_id"])
 
 
 
 
 
 def gen_passdata(*, username : str, password : str) -> bytes:
+    """
+    Generate passdata for an account
+    """
     passdata = sha3_256(pickle.dumps((username, password, "Dungeon Maker: Reinvented - Login System Salt"))).digest()
     return passdata
 
+def find_comment(project : Project, *, content : str = None, user : str = None) -> bool:
+    """
+    Find a comment.
+    """
+    comments = project.comments()
+    for comment in comments:
+        if user and comment["author"]["username"] != user:
+            continue
+        if content and comment["content"] != content:
+            continue
+        return True
+    return False
 
+def user_has_linked(*, session : DMSession, user : str) -> Union[None, dict]:
+    """
+    Find out if a user has linked an account to his name.
+    """
+    try:
+        has_linked = session.database_abstraction.select_user(fields={"linked_user": user})
+    except KeyError:
+        return None
+    else:
+        return has_linked
 
-
-
-
-
+def include_data(data : dict, *, include : list[str] = ()) -> dict:
+    """
+    Remove all elements from a dict except those specified
+    """
+    new = {}
+    for i in include:
+        new[i] = data.get(i)
+    return new
```

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/basetypes.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/basetypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/connection.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/connection.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/database/dba.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/database/dba.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/dba.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dba.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/dmtypes.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dmtypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/dungeon.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/dungeon.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/room.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/room.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/session.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/session.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/dm/user.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/dm/user.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/scratchcomms/basetypes.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/basetypes.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker/dm_backend/modules/scratchcomms/requests.py` & `dungeonmaker-0.6.3/dungeonmaker/dm_backend/modules/scratchcomms/requests.py`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/dungeonmaker.egg-info/PKG-INFO` & `dungeonmaker-0.6.3/dungeonmaker.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dungeonmaker
-Version: 0.6.2
+Version: 0.6.3
 Summary: Dungeon maker backend and other things
 Home-page: https://github.com/thecommcraft/dungeon-maker-reinvented
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dungeonmaker-0.6.2/dungeonmaker.egg-info/SOURCES.txt` & `dungeonmaker-0.6.3/dungeonmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dungeonmaker-0.6.2/setup.py` & `dungeonmaker-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='dungeonmaker',
-    version='0.6.2',
+    version='0.6.3',
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='Dungeon maker backend and other things',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/thecommcraft/dungeon-maker-reinvented',
     packages=find_packages(),
```

