# Comparing `tmp/nowgg-1.0.7.tar.gz` & `tmp/nowgg-1.1.1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowgg-1.0.7.tar", last modified: Thu Mar 21 12:43:16 2024, max compression
+gzip compressed data, was "nowgg-1.1.1.0.8.tar", last modified: Fri Apr 12 10:12:50 2024, max compression
```

## Comparing `nowgg-1.0.7.tar` & `nowgg-1.1.1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-03-21 12:43:16.195672 nowgg-1.0.7/
--rw-r--r--   0 apple      (501) staff       (20)     1504 2024-03-21 12:43:16.195166 nowgg-1.0.7/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     1380 2024-03-21 09:52:15.000000 nowgg-1.0.7/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-03-21 12:43:16.194169 nowgg-1.0.7/nowgg.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     1504 2024-03-21 12:43:16.000000 nowgg-1.0.7/nowgg.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      203 2024-03-21 12:43:16.000000 nowgg-1.0.7/nowgg.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2024-03-21 12:43:16.000000 nowgg-1.0.7/nowgg.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       37 2024-03-21 12:43:16.000000 nowgg-1.0.7/nowgg.egg-info/entry_points.txt
--rw-r--r--   0 apple      (501) staff       (20)        9 2024-03-21 12:43:16.000000 nowgg-1.0.7/nowgg.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        6 2024-03-21 12:43:16.000000 nowgg-1.0.7/nowgg.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)     9663 2024-03-21 12:42:38.000000 nowgg-1.0.7/nowgg.py
--rw-r--r--   0 apple      (501) staff       (20)       38 2024-03-21 12:43:16.195837 nowgg-1.0.7/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      516 2024-03-21 12:42:49.000000 nowgg-1.0.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-12 10:12:50.776403 nowgg-1.1.1.0.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1580 2024-04-12 10:12:50.776403 nowgg-1.1.1.0.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1380 2024-04-12 10:12:43.000000 nowgg-1.1.1.0.8/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-12 10:12:50.776403 nowgg-1.1.1.0.8/nowgg.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1580 2024-04-12 10:12:50.000000 nowgg-1.1.1.0.8/nowgg.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      203 2024-04-12 10:12:50.000000 nowgg-1.1.1.0.8/nowgg.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-12 10:12:50.000000 nowgg-1.1.1.0.8/nowgg.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-12 10:12:50.000000 nowgg-1.1.1.0.8/nowgg.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-12 10:12:50.000000 nowgg-1.1.1.0.8/nowgg.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-12 10:12:50.000000 nowgg-1.1.1.0.8/nowgg.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10284 2024-04-12 10:12:43.000000 nowgg-1.1.1.0.8/nowgg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-12 10:12:50.776403 nowgg-1.1.1.0.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2024-04-12 10:12:50.000000 nowgg-1.1.1.0.8/setup.py
```

### Comparing `nowgg-1.0.7/PKG-INFO` & `nowgg-1.1.1.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Metadata-Version: 2.1
 Name: nowgg
-Version: 1.0.7
+Version: 1.1.1.0.8
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author-email: cloudmaster@now.gg
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # nowStudio App Upload - CLI
 
 nowgg CLI is a command-line tool that enables you to upload your app builds to nowStudio.
 
 
@@ -45,7 +49,8 @@
 
 **Note**: Your app will be uploaded to the App Library within nowStudio.
 
 ## Important Information
 
 + While running the nowgg command, If you receive a `‘command not recognized’` error, consider adding` <python directory>\<Scripts>  `to your PATH.
 + If you receive any  `'permission-related errors'`, you should run the commands as an Administrator.
+
```

### Comparing `nowgg-1.0.7/README.md` & `nowgg-1.1.1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nowgg-1.0.7/nowgg.egg-info/PKG-INFO` & `nowgg-1.1.1.0.8/nowgg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Metadata-Version: 2.1
 Name: nowgg
-Version: 1.0.7
+Version: 1.1.1.0.8
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author-email: cloudmaster@now.gg
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # nowStudio App Upload - CLI
 
 nowgg CLI is a command-line tool that enables you to upload your app builds to nowStudio.
 
 
@@ -45,7 +49,8 @@
 
 **Note**: Your app will be uploaded to the App Library within nowStudio.
 
 ## Important Information
 
 + While running the nowgg command, If you receive a `‘command not recognized’` error, consider adding` <python directory>\<Scripts>  `to your PATH.
 + If you receive any  `'permission-related errors'`, you should run the commands as an Administrator.
+
```

### Comparing `nowgg-1.0.7/nowgg.py` & `nowgg-1.1.1.0.8/nowgg.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,38 +74,39 @@
             future = executor.submit(
                 upload_part, file_path, current_chunk_start_byte, current_chunk_end_byte, presigned_url, current_part)
             futures.append(future)
         logger.info("Starting upload..")
         for completed_future in concurrent.futures.as_completed(futures):
             if event.is_set():
                 executor.shutdown(wait=False)
-                os.kill(process_id, signal.SIGKILL)
+                os.kill(process_id, signal.SIGINT)
             progress = (
                 len([f for f in futures if f.done()]) / chunks_count) * 100
             logger.info(f"Uploading... {progress:.2f}%")
 
             response = completed_future.result()
             if response:
                 promises_array.append(response)
             else:
                 event.set()
                 logger.error(
                     "Error occurred during part upload. Please retry after some time.")
                 executor.shutdown(wait=False)
-                os.kill(process_id, signal.SIGKILL)
+                os.kill(process_id, signal.SIGINT)
     if event.is_set():
         return []
     return promises_array
 
 
-def upload_file(file_path, game_id, token, app_version, app_version_code):
+def upload_file(file_path, game_id, token, app_version, app_version_code, no_code):
     if not (file_path.endswith(".zip") or file_path.endswith(".apk")):
         logging.error(
             "Invalid file type. Only .zip or .apk files are allowed.")
         return
+    
     try:
         file_name = os.path.basename(file_path)
         upload_type = "upload_file_zip" if file_name.endswith(
             ".zip") else "upload_file"
         headers = {"publisher_token": token}
 
         file_size = os.path.getsize(file_path)
@@ -143,67 +144,76 @@
         response = requests.post(f"{get_host()}/v2/publisher/asset/mutipart_upload/end", json={
             "upload_id": upload_id, "parts_info": sorted_upload_parts_array,
                                     "s3_file_path": s3_file_path}, headers=headers)
         response.raise_for_status
         if response.status_code in OK_STATUS:
             logger.info("Upload completed.")
             file_url = f"https://cdn.now.gg/{s3_file_path}"
-            response = requests.post(
-                f"{get_host()}/v2/publisher/apk-library",
-                json={"upload_url": file_url,
+            json_to_send = {"upload_url": file_url,
                       "app_version": app_version,
                       "app_version_code": app_version_code,
                       "game_id": game_id,
-                      "upload_type": upload_type}, headers=headers)
+                      "upload_type": upload_type,
+                      "is_no_code_payment": True if no_code else False}
+            
+            response = requests.post(
+                f"{get_host()}/v2/publisher/apk-library",
+                json=json_to_send, headers=headers)
             if response.status_code in OK_STATUS:
                 logger.info("Successfully uploaded to your Apk Library!")
             else:
                 logger.error(response.json().get('message', response.reason))
         else:
             logger.error(response.json().get('message', response.reason))
 
     except Exception as e:
         logger.error(f"Error: {e}")
 
 
 class Nowgg:
 
     def config(self, hostname=""):
-
+        
         if hostname:
             old_host = get_host()
             cache["host"] = hostname
             logger.info(f"changed host from {old_host} to {hostname}")
-
-        else:
-            logger.debug(f"TOKEN: {cache.get('token')}")
-            logger.debug(f"HOST: {get_host()}")
+        logger.debug(f"TOKEN: {cache.get('token')}")
+        logger.debug(f"HOST: {get_host()}")
 
     def init(self, token):
         """Init
         Args:
             token (str): required parameter token
         """
-
+        headers = {"publisher_token": token}
+        response = requests.post(
+                f"{get_host()}/v2/publisher/verify-token",
+                json={}, headers=headers)
+        
+        if response.status_code not in OK_STATUS:
+            logger.error(response.json().get('message', response.reason))
+            return
+        
         cache['token'] = token
         logger.info("init successful!")
 
-    def upload(self, app_id, app_file_path, app_version, app_version_code):
+    def upload(self, app_id, app_file_path, app_version, app_version_code, no_code=0):
         """Upload utility
 
         Args:
             app_id (str): required parameter app_id
             app_file_path (str): required parameter app_file_path
             app_version (str): required parameter app_version
             app_version_code (int): required parameter app_version_code
 
         """
         token = cache.get('token')
         if token:
-            return upload_file(app_file_path, app_id, token, app_version, app_version_code)
+            return upload_file(app_file_path, app_id, token, app_version, app_version_code, no_code)
         else:
             logger.error(
                 "Please init first with token. nowgg init -t <your-token>")
 
 
 set_log_level()
 
@@ -231,28 +241,30 @@
         '-a', '--app_id', type=str, help='App Id', required=True)
     upload_parser.add_argument(
         '-f', '--file_path', type=str, help='File Path', required=True)
     upload_parser.add_argument(
         '-av', '--apk_version', type=str, help='apk version name', required=True)
     upload_parser.add_argument(
         '-vc', '--version_code', type=int, help='apk version code', required=True)
+    upload_parser.add_argument(
+        '-nc', '--no_code', action="store_true", help=argparse.SUPPRESS, required=False)
 
     config_parser = subparsers.add_parser('config')
     config_parser.add_argument(
         '-hn', '--host_name', help=argparse.SUPPRESS, required=False)
-
+    
     args = parser.parse_args()
     if args.verbose:
         set_log_level(logging.DEBUG)
 
     if args.command == 'init':
         nowgg.init(args.token)
     elif args.command == 'upload':
         nowgg.upload(args.app_id, args.file_path,
-                     args.apk_version, args.version_code)
+                     args.apk_version, args.version_code, args.no_code)
     elif args.command == 'config':
         nowgg.config(args.host_name)
     else:
         parser.print_help()
 
 
 class CustomHelpFormatter(argparse.HelpFormatter):
```

### Comparing `nowgg-1.0.7/setup.py` & `nowgg-1.1.1.0.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 import os
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
     name='nowgg',
-    version="1.0.7",
+    version='1.1.1.0.8',
     scripts=['nowgg.py'],
     author_email='cloudmaster@now.gg',
     install_requires=[
         'requests'
     ],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

