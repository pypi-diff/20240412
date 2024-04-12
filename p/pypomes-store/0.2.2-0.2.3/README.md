# Comparing `tmp/pypomes_store-0.2.2.tar.gz` & `tmp/pypomes_store-0.2.3.tar.gz`

## Comparing `pypomes_store-0.2.2.tar` & `pypomes_store-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_store-0.2.2/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pypomes_store-0.2.2/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pypomes_store-0.2.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.2/README.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/PKG-INFO
```

### Comparing `pypomes_store-0.2.2/src/pypomes_store/__init__.py` & `pypomes_store-0.2.3/src/pypomes_store/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.2/src/pypomes_store/minio_pomes.py` & `pypomes_store-0.2.3/src/pypomes_store/minio_pomes.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,26 +27,25 @@
 
     :param errors: incidental error messages
     :return: True if service is fully functional
     """
     # initialize the return variable
     result: bool = False
 
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-    
-    # was the MinIO client obtained ?
-    if minio_client:
-        # yes, build the bucket, if needed
-        try:
+    # obtain the MinIO client and proceed
+    try:
+        with Minio(endpoint=MINIO_HOST,
+                   access_key=MINIO_ACCESS_KEY,
+                   secret_key=MINIO_SECRET_KEY,
+                   secure=MINIO_SECURE_ACCESS) as minio_client:
             if not minio_client.bucket_exists(bucket_name=MINIO_BUCKET):
                 minio_client.make_bucket(bucket_name=MINIO_BUCKET)
             result = True
-        except Exception as e:
-            errors.append(__minio_except_msg(e))
+    except Exception as e:
+        errors.append(__minio_except_msg(e))
 
     return result
 
 
 def minio_access(errors: list[str]) -> Minio:
     """
     Obtain and return the *MinIO* client object.
@@ -78,69 +77,68 @@
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path specifying where the file is
     :param mimetype: the file mimetype
     :param tags: optional metadata describing the file
     """
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-
-    # was the MinIO client obtained ?
-    if minio_client:
-        # yes, store the file
-        remotepath: Path = Path(basepath) / identifier
-        # have tags been defined ?
-        if tags is None or len(tags) == 0:
-            # no
-            doc_tags = None
-        else:
-            # sim, store them
-            doc_tags = Tags(for_object=True)
-            for key, value in tags.items():
-                # normalize text, by removing all diacritics
-                doc_tags[key] = unidecode(value)
-        try:
+    # obtain the MinIO client and proceed
+    try:
+        with Minio(endpoint=MINIO_HOST,
+                   access_key=MINIO_ACCESS_KEY,
+                   secret_key=MINIO_SECRET_KEY,
+                   secure=MINIO_SECURE_ACCESS) as minio_client:
+            remotepath: Path = Path(basepath) / identifier
+            # have tags been defined ?
+            if tags is None or len(tags) == 0:
+                # no
+                doc_tags = None
+            else:
+                # sim, store them
+                doc_tags = Tags(for_object=True)
+                for key, value in tags.items():
+                    # normalize text, by removing all diacritics
+                    doc_tags[key] = unidecode(value)
+            # store the file
             minio_client.fput_object(bucket_name=MINIO_BUCKET,
                                      object_name=f"{remotepath}",
                                      file_path=filepath,
                                      content_type=mimetype,
                                      tags=doc_tags)
-        except Exception as e:
-            errors.append(__minio_except_msg(e))
+    except Exception as e:
+        errors.append(__minio_except_msg(e))
 
 
 def minio_file_retrieve(errors: list[str], basepath: Path | str,
                         identifier: str, filepath: Path | str) -> any:
     """
     Retrieve a file from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path to save the retrieved file at
     :return: information about the file retrieved
     """
-    # initialize the return variable
-    result: any = None
-
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-
-    # was the MinIO client obtained ?
-    if minio_client:
-        # yes, retrieve the file
-        remotepath: Path = Path(basepath) / identifier
-        try:
-            result = minio_client.fget_object(bucket_name=MINIO_BUCKET,
-                                              object_name=f"{remotepath}",
-                                              file_path=filepath)
-        except Exception as e:
-            if not hasattr(e, "code") or e.code != "NoSuchKey":
-                errors.append(__minio_except_msg(e))
+    # obtain the MinIO client and proceed
+    try:
+        with Minio(endpoint=MINIO_HOST,
+                   access_key=MINIO_ACCESS_KEY,
+                   secret_key=MINIO_SECRET_KEY,
+                   secure=MINIO_SECURE_ACCESS) as minio_client:
+            remotepath: Path = Path(basepath) / identifier
+            try:
+                result = minio_client.fget_object(bucket_name=MINIO_BUCKET,
+                                                  object_name=f"{remotepath}",
+                                                  file_path=filepath)
+            except Exception as e:
+                if not hasattr(e, "code") or e.code != "NoSuchKey":
+                    errors.append(__minio_except_msg(e))
+    except Exception as e:
+        errors.append(__minio_except_msg(e))
 
     return result
 
 
 def minio_object_exists(errors: list[str], basepath: Path | str, identifier: str = None) -> bool:
     """
     Determine if a given object exists in the *MinIO* store.
@@ -175,27 +173,29 @@
     :param basepath: the path specifying where to locate the object
     :param identifier: the object identifier
     :return: metadata and information about the object
     """
     # initialize the return variable
     result: MinioObject | None = None
 
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-
-    # was the MinIO client obtained ?
-    if minio_client:
-        # yes, retrieve the object's information
-        remotepath: Path = Path(basepath) / identifier
-        try:
-            result = minio_client.stat_object(bucket_name=MINIO_BUCKET,
-                                              object_name=f"{remotepath}")
-        except Exception as e:
-            if not hasattr(e, "code") or e.code != "NoSuchKey":
-                errors.append(__minio_except_msg(e))
+    # obtain the MinIO client and proceed
+    try:
+        with Minio(endpoint=MINIO_HOST,
+                   access_key=MINIO_ACCESS_KEY,
+                   secret_key=MINIO_SECRET_KEY,
+                   secure=MINIO_SECURE_ACCESS) as minio_client:
+            remotepath: Path = Path(basepath) / identifier
+            try:
+                result = minio_client.stat_object(bucket_name=MINIO_BUCKET,
+                                                  object_name=f"{remotepath}")
+            except Exception as e:
+                if not hasattr(e, "code") or e.code != "NoSuchKey":
+                    errors.append(__minio_except_msg(e))
+    except Exception as e:
+        errors.append(__minio_except_msg(e))
 
     return result
 
 
 def minio_object_store(errors: list[str], basepath: Path | str,
                        identifier: str, obj: any, tags: dict = None) -> None:
     """
@@ -203,27 +203,25 @@
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
     :param obj: object to be stored
     :param tags: optional metadata describing the object
     """
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-
-    # proceed, if the MinIO client was obtained
-    if minio_client:
+    # serialize the object into a file
+    filepath: Path = Path(MINIO_TEMP_PATH) / f"{uuid.uuid4()}.pickle"
+    with Path.open(filepath, "wb") as f:
+        pickle.dump(obj, f)
 
-        # serialize the object into a file
-        filepath: Path = Path(MINIO_TEMP_PATH) / f"{uuid.uuid4()}.pickle"
-        with Path.open(filepath, "wb") as f:
-            pickle.dump(obj, f)
+    # store the file
+    minio_file_store(errors, basepath, identifier, filepath, "application/octet-stream", tags)
 
-        # store the file and remove it
-        minio_file_store(errors, basepath, identifier, filepath, "application/octet-stream", tags)
+    # was the file stored ?
+    if len(errors) == 0:
+        # yes, remove it from the file system
         Path.unlink(filepath)
 
 
 def minio_object_retrieve(errors: list[str], basepath: Path, identifier: str) -> any:
     """
     Retrieve an object from the *MinIO* store.
 
@@ -253,32 +251,35 @@
     """
     Remove an object from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     """
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-
-    # proceed, if the MinIO client was obtained
-    if minio_client:
-        # was the identifier provided ?
-        if identifier is None:
-            # no, remove the folder
-            __minio_folder_delete(errors, minio_client, basepath)
-        else:
-            # yes, remove the object
-            remotepath: str = os.path.join(basepath, identifier)
-            try:
-                minio_client.remove_object(bucket_name=MINIO_BUCKET,
-                                           object_name=remotepath)
-            except Exception as e:
-                if not hasattr(e, "code") or e.code != "NoSuchKey":
-                    errors.append(__minio_except_msg(e))
+    # obtain the MinIO client and proceed
+    try:
+        with Minio(endpoint=MINIO_HOST,
+                   access_key=MINIO_ACCESS_KEY,
+                   secret_key=MINIO_SECRET_KEY,
+                   secure=MINIO_SECURE_ACCESS) as minio_client:
+            # was the identifier provided ?
+            if identifier is None:
+                # no, remove the folder
+                __minio_folder_delete(errors, minio_client, basepath)
+            else:
+                # yes, remove the object
+                remotepath: str = os.path.join(basepath, identifier)
+                try:
+                    minio_client.remove_object(bucket_name=MINIO_BUCKET,
+                                               object_name=remotepath)
+                except Exception as e:
+                    if not hasattr(e, "code") or e.code != "NoSuchKey":
+                        errors.append(__minio_except_msg(e))
+    except Exception as e:
+        errors.append(__minio_except_msg(e))
 
 
 # recupera as tags do objeto
 def minio_object_tags_retrieve(errors: list[str], basepath: str, identifier: str) -> dict:
     """
     Retrieve and return the metadata information for an object in the *MinIO* store.
 
@@ -318,53 +319,53 @@
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to iterate from
     :param recursive: whether the location is iterated recursively
     :return: the iterator into the list of objects
     """
     # initialize the return variable
-    result: any = None
+    result: Iterator | None = None
 
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-
-    # was the MinIO client obtained ?
-    if minio_client:
-        # yes, retrieve the iterator into the list of objects
-        try:
+    # obtain the MinIO client and proceed
+    try:
+        with Minio(endpoint=MINIO_HOST,
+                   access_key=MINIO_ACCESS_KEY,
+                   secret_key=MINIO_SECRET_KEY,
+                   secure=MINIO_SECURE_ACCESS) as minio_client:
             result = minio_client.list_objects(bucket_name=MINIO_BUCKET,
                                                prefix=basepath,
                                                recursive=recursive)
-        except Exception as e:
-            errors.append(__minio_except_msg(e))
+    except Exception as e:
+        errors.append(__minio_except_msg(e))
 
     return result
 
 
 def __minio_folder_delete(errors: list[str],  minio_client: Minio, basepath: str) -> None:
     """
     Traverse the folders recursively, removing its objects.
 
     :param errors: incidental error messages
     :param minio_client: the MinIO client object
     :param basepath: the path specifying the location to delete the objects at.
     """
-    #
-    try:
-        objs: Iterator = minio_objects_list(errors, basepath, True)
+    # obtain the list of entries in the given folder
+    objs: Iterator = minio_objects_list(errors, basepath, True)
+
+    # was the list obtained ?
+    if objs:
+        # yes, proceed
         for obj in objs:
             try:
                 minio_client.remove_object(bucket_name=MINIO_BUCKET,
                                            object_name=obj.object_name)
-            except Exception as e:  # noqa: PERF203
+            except Exception as e:
                 # SANITY CHECK: in case of concurrent exclusion
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
                     errors.append(__minio_except_msg(e))
-    except Exception as e:
-        errors.append(__minio_except_msg(e))
 
 
 def __minio_except_msg(exception: Exception) -> str:
     """
     Format and return an error message from *exception*.
 
     :param exception: the reference exception
```

### Comparing `pypomes_store-0.2.2/LICENSE` & `pypomes_store-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.2/pyproject.toml` & `pypomes_store-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_store-0.2.2/PKG-INFO` & `pypomes_store-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_store
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

