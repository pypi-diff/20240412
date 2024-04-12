# Comparing `tmp/hda-2.12.tar.gz` & `tmp/hda-2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hda-2.12.tar", last modified: Thu Mar 14 16:03:18 2024, max compression
+gzip compressed data, was "hda-2.13.tar", last modified: Fri Apr 12 17:32:43 2024, max compression
```

## Comparing `hda-2.12.tar` & `hda-2.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:03:18.056176 hda-2.12/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-03-14 16:03:06.000000 hda-2.12/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-14 16:03:18.056176 hda-2.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-14 16:03:06.000000 hda-2.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:03:18.056176 hda-2.12/hda/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-14 16:03:06.000000 hda-2.12/hda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25801 2024-03-14 16:03:06.000000 hda-2.12/hda/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-14 16:03:06.000000 hda-2.12/hda/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 16:03:18.056176 hda-2.12/hda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-14 16:03:17.000000 hda-2.12/hda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-14 16:03:18.000000 hda-2.12/hda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 16:03:17.000000 hda-2.12/hda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-14 16:03:17.000000 hda-2.12/hda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-14 16:03:17.000000 hda-2.12/hda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 16:03:17.000000 hda-2.12/hda.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 16:03:18.056176 hda-2.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-14 16:03:06.000000 hda-2.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:32:43.737866 hda-2.13/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-12 17:32:29.000000 hda-2.13/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-12 17:32:43.737866 hda-2.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-12 17:32:29.000000 hda-2.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:32:43.737866 hda-2.13/hda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 17:32:29.000000 hda-2.13/hda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-04-12 17:32:29.000000 hda-2.13/hda/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-12 17:32:29.000000 hda-2.13/hda/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:32:43.737866 hda-2.13/hda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:32:43.000000 hda-2.13/hda.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:32:43.737866 hda-2.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-12 17:32:29.000000 hda-2.13/setup.py
```

### Comparing `hda-2.12/LICENSE.txt` & `hda-2.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hda-2.12/PKG-INFO` & `hda-2.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hda
-Version: 2.12
+Version: 2.13
 Summary: API to harmonised data access for DIAS/WEkEO
 Home-page: https://github.com/ecmwf/hda
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `hda-2.12/README.md` & `hda-2.13/README.md`

 * *Files identical despite different names*

### Comparing `hda-2.12/hda/__init__.py` & `hda-2.13/hda/__init__.py`

 * *Files identical despite different names*

### Comparing `hda-2.12/hda/api.py` & `hda-2.13/hda/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,52 +313,44 @@
     """
 
     def __init__(
         self,
         url=os.environ.get("HDA_URL"),
         user=os.environ.get("HDA_USER"),
         password=os.environ.get("HDA_PASSWORD"),
-        verify=None,
+        verify=True,
         path=None,
     ):
         credentials = {
-            "url": url or BROKER_URL,
             "user": None,
-            "password": None,
-            "verify": True,
+            "password": None
         }
 
         dotrc = path or os.environ.get("HDA_RC", os.path.expanduser("~/.hdarc"))
 
         if os.path.isfile(dotrc):
             config = read_config(dotrc)
 
             for key in credentials.keys():
                 if config.get(key):
                     credentials[key] = config.get(key)
 
-        if url is not None:
-            credentials["url"] = url
-
         if user is not None:
             credentials["user"] = user
 
         if password is not None:
             credentials["password"] = password
 
-        if verify is not None:
-            credentials["verify"] = verify
-
         if credentials["user"] is None or credentials["password"] is None:
             raise ConfigurationError("Missing or incomplete configuration")
 
-        self.url = credentials["url"]
+        self.url = url or BROKER_URL
         self.user = credentials["user"]
         self.password = credentials["password"]
-        self.verify = credentials["verify"]
+        self.verify = verify
 
 
 class Client(object):
     """HTTP client to request data from the WEkEO HDA API.
 
     :param config: A :class:`hda.api.Configuration` instance.
         By default `None` is passed, which means that a `$HOME/.hdarc`
@@ -771,15 +763,15 @@
                     with open(os.path.join(download_dir, filename), mode) as f:
                         for chunk in r.iter_content(chunk_size=1024):
                             if chunk:
                                 f.write(chunk)
                                 total += len(chunk)
                                 pbar.update(len(chunk))
 
-            except requests.exceptions.ConnectionError as e:
+            except requests.exceptions.RequestException as e:
                 logger.error("Download interrupted: %s" % (e,))
             finally:
                 r.close()
 
             if size is None or total >= size:
                 size = os.path.getsize(filename)
                 break
```

### Comparing `hda-2.12/hda/utils.py` & `hda-2.13/hda/utils.py`

 * *Files identical despite different names*

### Comparing `hda-2.12/hda.egg-info/PKG-INFO` & `hda-2.13/hda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hda
-Version: 2.12
+Version: 2.13
 Summary: API to harmonised data access for DIAS/WEkEO
 Home-page: https://github.com/ecmwf/hda
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `hda-2.12/setup.py` & `hda-2.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return io.open(file_path, encoding="utf-8").read()
 
 
-version = "2.12"
+version = "2.13"
 
 setuptools.setup(
     name="hda",
     version=version,
     author="ECMWF",
     author_email="software.support@ecmwf.int",
     license="Apache 2.0",
```

