# Comparing `tmp/llama_index_readers_s3-0.1.5.tar.gz` & `tmp/llama_index_readers_s3-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_s3-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_readers_s3-0.1.6.tar", max compression
```

## Comparing `llama_index_readers_s3-0.1.5.tar` & `llama_index_readers_s3-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1552 2024-03-28 15:33:59.619766 llama_index_readers_s3-0.1.5/README.md
--rw-r--r--   0        0        0       73 2024-03-14 20:48:34.890068 llama_index_readers_s3-0.1.5/llama_index/readers/s3/__init__.py
--rw-r--r--   0        0        0     4342 2024-03-26 15:59:59.482239 llama_index_readers_s3-0.1.5/llama_index/readers/s3/base.py
--rw-r--r--   0        0        0     1646 2024-03-28 15:33:59.620046 llama_index_readers_s3-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 llama_index_readers_s3-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1552 2024-03-28 20:25:46.514060 llama_index_readers_s3-0.1.6/README.md
+-rw-r--r--   0        0        0       73 2024-03-13 22:17:44.756075 llama_index_readers_s3-0.1.6/llama_index/readers/s3/__init__.py
+-rw-r--r--   0        0        0     4320 2024-04-12 00:53:45.633864 llama_index_readers_s3-0.1.6/llama_index/readers/s3/base.py
+-rw-r--r--   0        0        0     1646 2024-04-12 16:24:05.461050 llama_index_readers_s3-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 llama_index_readers_s3-0.1.6/PKG-INFO
```

### Comparing `llama_index_readers_s3-0.1.5/README.md` & `llama_index_readers_s3-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_s3-0.1.5/llama_index/readers/s3/base.py` & `llama_index_readers_s3-0.1.6/llama_index/readers/s3/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     required_exts: Optional[List[str]] = None
     filename_as_id: bool = True
     num_files_limit: Optional[int] = None
     file_metadata: Optional[Callable[[str], Dict]] = Field(default=None, exclude=True)
     aws_access_id: Optional[str] = None
     aws_access_secret: Optional[str] = None
     aws_session_token: Optional[str] = None
-    s3_endpoint_url: Optional[str] = "https://s3.amazonaws.com"
+    s3_endpoint_url: Optional[str] = None
     custom_reader_path: Optional[str] = None
 
     @classmethod
     def class_name(cls) -> str:
         return "S3Reader"
 
     def load_s3_files_as_docs(self, temp_dir=None) -> List[Document]:
```

### Comparing `llama_index_readers_s3-0.1.5/pyproject.toml` & `llama_index_readers_s3-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 description = "llama-index readers s3 integration"
 exclude = ["**/BUILD"]
 keywords = ["amazon web services", "aws s3", "bucket"]
 license = "MIT"
 maintainers = ["thejessezhang"]
 name = "llama-index-readers-s3"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-readers-file = "^0.1.12"
-s3fs = "^2024.3.0"
+s3fs = "^2024.3.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_readers_s3-0.1.5/PKG-INFO` & `llama_index_readers_s3-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-s3
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index readers s3 integration
 License: MIT
 Keywords: amazon web services,aws s3,bucket
 Author: Your Name
 Author-email: you@example.com
 Maintainer: thejessezhang
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: llama-index-readers-file (>=0.1.12,<0.2.0)
-Requires-Dist: s3fs (>=2024.3.0,<2025.0.0)
+Requires-Dist: s3fs (>=2024.3.1,<2025.0.0)
 Description-Content-Type: text/markdown
 
 # S3 File or Directory Loader
 
 This loader parses any file stored on S3, or the entire Bucket (with an optional prefix filter) if no particular file is specified. When initializing `S3Reader`, you may pass in your [AWS Access Key](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html). If none are found, the loader assumes they are stored in `~/.aws/credentials`.
 
 All files are parsed with `SimpleDirectoryReader`. Hence, you may also specify a custom `file_extractor`, relying on any of the loaders in this library (or your own)!
```

