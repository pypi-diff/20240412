# Comparing `tmp/neuropacs-1.6.5.tar.gz` & `tmp/neuropacs-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuropacs-1.6.5.tar", last modified: Wed Apr  3 00:07:53 2024, max compression
+gzip compressed data, was "neuropacs-1.6.6.tar", last modified: Fri Apr 12 21:19:38 2024, max compression
```

## Comparing `neuropacs-1.6.5.tar` & `neuropacs-1.6.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-03 00:07:53.708454 neuropacs-1.6.5/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.5/LICENSE
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-03 00:07:53.708232 neuropacs-1.6.5/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.5/README.md
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-03 00:07:53.705312 neuropacs-1.6.5/examples/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.5/examples/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      970 2024-03-28 21:09:19.000000 neuropacs-1.6.5/examples/example1.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-03 00:07:53.706246 neuropacs-1.6.5/neuropacs/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-04-03 00:07:19.000000 neuropacs-1.6.5/neuropacs/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1072 2024-04-02 21:51:52.000000 neuropacs-1.6.5/neuropacs/ex.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    19764 2024-04-03 00:05:02.000000 neuropacs-1.6.5/neuropacs/sdk.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-03 00:07:53.707935 neuropacs-1.6.5/neuropacs.egg-info/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-03 00:07:53.000000 neuropacs-1.6.5/neuropacs.egg-info/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-04-03 00:07:53.000000 neuropacs-1.6.5/neuropacs.egg-info/SOURCES.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-04-03 00:07:53.000000 neuropacs-1.6.5/neuropacs.egg-info/dependency_links.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-04-03 00:07:53.000000 neuropacs-1.6.5/neuropacs.egg-info/requires.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-04-03 00:07:53.000000 neuropacs-1.6.5/neuropacs.egg-info/top_level.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-04-03 00:07:53.708503 neuropacs-1.6.5/setup.cfg
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-04-03 00:07:16.000000 neuropacs-1.6.5/setup.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-03 00:07:53.707489 neuropacs-1.6.5/tests/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.5/tests/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.5/tests/tests_neuropacs.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.262622 neuropacs-1.6.6/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.6/LICENSE
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-12 21:19:38.262343 neuropacs-1.6.6/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.6/README.md
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.257437 neuropacs-1.6.6/examples/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.6/examples/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      970 2024-04-04 07:24:41.000000 neuropacs-1.6.6/examples/example1.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.258315 neuropacs-1.6.6/neuropacs/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-04-12 21:19:04.000000 neuropacs-1.6.6/neuropacs/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1556 2024-04-12 21:16:50.000000 neuropacs-1.6.6/neuropacs/ex.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    22249 2024-04-12 21:18:50.000000 neuropacs-1.6.6/neuropacs/sdk.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.262035 neuropacs-1.6.6/neuropacs.egg-info/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/SOURCES.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/dependency_links.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/requires.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/top_level.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-04-12 21:19:38.262667 neuropacs-1.6.6/setup.cfg
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-04-12 21:19:01.000000 neuropacs-1.6.6/setup.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.260778 neuropacs-1.6.6/tests/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.6/tests/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.6/tests/tests_neuropacs.py
```

### Comparing `neuropacs-1.6.5/LICENSE` & `neuropacs-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.5/PKG-INFO` & `neuropacs-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.5
+Version: 1.6.6
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.5/README.md` & `neuropacs-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.5/examples/example1.py` & `neuropacs-1.6.6/examples/example1.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     print(conn)
 
     # # # CREATE A NEW JOB
     order = npcs.new_job()
     # print(order)
 
     # # # UPLOAD A DATASET
-    # datasetID = npcs.upload_dataset("../dicom_examples/DICOM_small")
-    # print(datasetID)
+    datasetID = npcs.upload_dataset("../dicom_examples/DICOM_small")
+    print(datasetID)
 
     # # START A JOB
-    job = npcs.run_job(product_id)
-    print(job)
+    # job = npcs.run_job(product_id)
+    # print(job)
 
     # # CHECK STATUS
     # status = npcs.check_status("TEST")
     # print(status)
 
     # # # GET RESULTS
     # results = npcs.get_results(result_format, "TEST")
```

### Comparing `neuropacs-1.6.5/neuropacs/sdk.py` & `neuropacs-1.6.6/neuropacs/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,20 +257,21 @@
             if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
                 raise Exception(e.args[0]['neuropacsError']) 
             else:
                 raise Exception("Connection failed.")
             
 
 
-    def upload_dataset(self, directory, order_id=None, connection_id=None):
+    def upload_dataset(self, directory, order_id=None, connection_id=None, callback=None):
         """Upload a dataset to the server
 
         :param str directory: Path to dataset folder to be uploaded.
         :param str order_id: Base64 order_id
         :param str connection_id: Base64 connection_id
+        :param str callback: Function to be called after every upload
 
         :return: Upload status code.
         """
         if order_id is None:
             order_id = self.order_id
 
         if connection_id is None:
@@ -285,21 +286,42 @@
             else:
                 raise Exception({"neuropacsError": "Path must be a string!"}) 
 
             dataset_id = self.__generate_filename()
 
             total_files = sum(len(filenames) for _, _, filenames in os.walk(directory))
 
+            files_uploaded = 0
+
             with tqdm(total=total_files, desc="Uploading", unit="file") as prog_bar:
                 for dirpath, _, filenames in os.walk(directory):
                     for filename in filenames:
                         file_path = os.path.join(dirpath, filename)
                         status = self.upload(file_path, dataset_id, order_id, connection_id)
                         if status != 201:
+                            if callback is not None:
+                               callback({
+                                'datasetId': dataset_id,
+                                'progress': -1,
+                                }) 
                             raise Exception({"neuropacsError": "Upload failed!"})
+                        files_uploaded += 1
+                        if callback is not None:
+                            # Calculate progress and round to two decimal places
+                            progress = (files_uploaded / total_files) * 100
+                            progress = round(progress, 2)
+
+                            # Ensure progress is exactly 100 if it's effectively 100
+                            progress = 100 if progress == 100.0 else progress
+                            callback({
+                                'datasetId': dataset_id,
+                                'progress': progress,
+                                'filesUploaded': files_uploaded
+                            })
+                        
                         prog_bar.update(1)  # Update the outer progress bar for each file
             
             return dataset_id
 
         except Exception as e:
             if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
                 raise Exception(e.args[0]['neuropacsError']) 
@@ -375,36 +397,75 @@
             header += DELIM
         header += CRLF
         header += CONTENT_TYPE
         header += CRLF + CRLF
 
         header_bytes = header.encode("utf-8")
 
+        footer_bytes = END.encode("utf-8")
+
         encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
 
         payload_data = None
 
         if isinstance(data, bytes):
             # encrypted_binary_data = self.__encrypt_aes_ctr(data, "bytes","bytes")
-            payload_data = header_bytes + data + END.encode("utf-8")
+            payload_data = header_bytes + data + footer_bytes
         
         elif isinstance(data,str):
             with open(data, 'rb') as f:
                 binary_data = f.read()
                 # encrypted_binary_data = self.__encrypt_aes_ctr(binary_data, "bytes","bytes")
-                payload_data = header_bytes + binary_data + END.encode("utf-8")
+                payload_data = header_bytes + binary_data + footer_bytes
 
 
         res = requests.put(presigned_url, data=payload_data)
 
         if not res.ok:
             raise Exception({"neuropacsError": f"{res.text}"})
 
         return 201
 
+    def validate_upload(self, file_array, dataset_id, order_id=None, connection_id=None):
+        """
+        Validate dataset upload
+        """
+        if connection_id is None:
+            connection_id = self.connection_id
+        if order_id is None:
+            order_id = self.order_id
+        try:
+            encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
+        
+            headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'dataset-id': dataset_id,'order-id': encrypted_order_id, 'client': self.client}
+
+            body = {
+                'fileArray': file_array,
+            }
+
+            encrypted_body = self.__encrypt_aes_ctr(body, "json", "string")
+
+            res = requests.post(f"{self.server_url}/api/verifyUpload/", data=encrypted_body, headers=headers)
+            
+            if not res.ok:
+                raise Exception({"neuropacsError": f"{res.text}"})
+
+            text = res.text
+            decrypted_dataset_validation = self.__decrypt_aes_ctr(text, "string")
+            return decrypted_dataset_validation
+
+        except Exception as e:
+            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
+                raise Exception(e.args[0]['neuropacsError'])
+            else:
+                raise Exception(f"Result retrieval failed!")
+        
+
+
+
     def new_job (self, connection_id=None):
         """Create a new order
 
         :param str connection_id: Base64 connection_id
 
         :return: Base64 string order_id.
         """
```

### Comparing `neuropacs-1.6.5/neuropacs.egg-info/PKG-INFO` & `neuropacs-1.6.6/neuropacs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.5
+Version: 1.6.6
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.5/setup.py` & `neuropacs-1.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuropacs',
-    version='1.6.5',
+    version='1.6.6',
     description='NeuroPACS Python SDK',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kerrick Cavanaugh',
     author_email='kerrick@neuropacs.com',
     url='https://github.com/neuropacs/neuropacs-py-sdk',
     packages=find_packages(),
```

### Comparing `neuropacs-1.6.5/tests/tests_neuropacs.py` & `neuropacs-1.6.6/tests/tests_neuropacs.py`

 * *Files identical despite different names*

