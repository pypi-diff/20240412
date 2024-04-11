# Comparing `tmp/wring-0.0.4.tar.gz` & `tmp/wring-0.0.5.tar.gz`

## Comparing `wring-0.0.4.tar` & `wring-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 wring-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/_app.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/_version.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/csv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/py.typed
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 wring-0.0.4/src/wring/tar_zst.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 wring-0.0.4/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 wring-0.0.4/LICENSE
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 wring-0.0.4/README.md
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 wring-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 wring-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wring-0.0.5/mkdocs.yml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/_app.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/_version.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/csv.py
+-rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/omx.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/py.typed
+-rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 wring-0.0.5/src/wring/tar_zst.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 wring-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 wring-0.0.5/LICENSE
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 wring-0.0.5/README.md
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 wring-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 wring-0.0.5/PKG-INFO
```

### Comparing `wring-0.0.4/mkdocs.yml` & `wring-0.0.5/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 site_name: wring
 site_url: https://github.com/jpn--/wring
 site_author: Jeff Newman
-site_description: A tool to compress multiple CSV data files into parquet
+site_description: A tool to compress data files
 
 repo_name: jpn--/wring
 repo_url: https://github.com/jpn--/wring
 
 copyright: Copyright (c) 2023-present Jeff Newman <jeff@newman.me>
 
 theme:
```

### Comparing `wring-0.0.4/src/wring/csv.py` & `wring-0.0.5/src/wring/csv.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rich import print
 
 from ._app import app
 
 
 @app.command()
 def csv(
-    directory: Path,
+    directory: Path = ".",
     compression: str = typer.Option("zstd", help="compression algorithm"),
     compression_level: int = typer.Option(9, help="compression level"),
     clean: bool = typer.Option(
         False, help="remove uncompressed files after successful wringing"
     ),
 ):
     """Crawl a directory and compress csv files into parquet."""
```

### Comparing `wring-0.0.4/src/wring/tar_zst.py` & `wring-0.0.5/src/wring/tar_zst.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,14 +87,16 @@
     in_path: pathlib.Path or str
       directory to compress
     archive: pathlib.Path or str
       .tar.zst file to compress into
     """
     if zstandard is None:
         raise ImportError("pip install zstandard")
+    if not in_path.is_dir():
+        raise NotADirectoryError(in_path)
     dctx = zstandard.ZstdCompressor(level=9, threads=-1, write_checksum=True)
     with tempfile.TemporaryFile(suffix=".tar") as ofh:
         with tarfile.open(fileobj=ofh, mode="w") as z:
             for dirpath, dirnames, filenames in os.walk(in_path):
                 if os.path.basename(dirpath) == ".git":
                     continue
                 for n in range(len(dirnames) - 1, -1, -1):
@@ -174,18 +176,33 @@
                 with archive_part(n).open("wb") as ifh:
                     ifh.write(out_chunk)
                 n += 1
 
 
 @app.command()
 def tarzst(
-    directory: Path,
-    archive: Optional[Path] = None,
-    chunkgigs: Optional[float] = typer.Option(None, "-c", "--chunk-gigs"),
+    directory: Path = typer.Argument(..., help="the directory to compress"),
+    archive: Optional[Path] = typer.Option(
+        None,
+        help=(
+            "base file name for the resulting archive file(s), if not provided "
+            "a '.tar.zst' suffix is added to the original directory name"
+        ),
+    ),
+    chunkgigs: Optional[float] = typer.Option(
+        None,
+        "-c",
+        "--chunk-gigs",
+        help=(
+            "chunk the resulting archive into parts that are no larger than "
+            "this many gigabytes"
+        ),
+    ),
 ):
+    """Compress a directory using the .tar.zst format."""
     directory = Path(directory)
     name = directory.name
     if not archive:
         archive = directory.with_name(name + ".tar.zst")
     if directory.exists():
         if not archive.exists():
             print(f"compressing to tar.zst: {directory}")
@@ -197,17 +214,27 @@
             print(f"not compressing, existing tar.zst: {directory}")
     else:
         print(f"not compressing, does not exist: {directory}")
 
 
 @app.command()
 def untarzst(
-    archive: Path,
-    outdir: Optional[Path] = None,
+    archive: Path = typer.Argument(
+        ..., help="the archive file to decompress, or the first of multiple parts"
+    ),
+    outdir: Optional[Path] = typer.Option(
+        None,
+        help=(
+            "directory name for the resulting decompressed file(s), if not "
+            "provided any '.tar.zst' suffix is stripped from the archive file name "
+            "and the rest is used"
+        ),
+    ),
 ):
+    """Decompress a directory stored in .tar.zst format."""
     name = archive.name
     if not outdir and name.endswith(".tar.zst"):
         outdir = archive.with_name(name[:-8])
     if not outdir and name.endswith(".tar.zst.part000"):
         outdir = archive.with_name(name[:-16])
     if not outdir:
         raise ValueError("must specify output dir")
```

### Comparing `wring-0.0.4/.gitignore` & `wring-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `wring-0.0.4/LICENSE` & `wring-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wring-0.0.4/pyproject.toml` & `wring-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 quality = [
   "black~=22.10.0",
   "ruff",
   "pre-commit~=2.20.0",
 ]
 tests = [
   "pytest~=7.1.2",
+  "tables",
+]
+omx = [
+  "pytables",
 ]
 
 [tool.hatch.envs.quality]
 features = [
   "quality",
 ]
 
@@ -66,30 +70,30 @@
 ]
 format = [
   "ruff --fix src tests",
   "black --preview src tests",
   "check",
 ]
 
-[tool.ruff]
+[tool.ruff.lint]
 ignore = [
   "E501", # line too long, handled by black
   "B008", # do not perform function calls in argument defaults
   "C901", # too complex
 ]
 select = [
   "E", # pycodestyle errors
   "W", # pycodestyle warnings
   "F", # pyflakes
   "I", # isort
   "C", # flake8-comprehensions
   "B", # flake8-bugbear
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["wring"]
 
 [tool.hatch.envs.test]
 features = [
   "tests",
 ]
```

### Comparing `wring-0.0.4/PKG-INFO` & `wring-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wring
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to compress multiple CSV data files into parquet
 Project-URL: Documentation, https://jpn--.github.io/wring
 Project-URL: Issues, https://github.com/jpn--/wring/issues
 Project-URL: Source, https://github.com/jpn--/wring
 Author: Jeff Newman
 License-Expression: MIT
 License-File: LICENSE
@@ -21,20 +21,21 @@
 Provides-Extra: docs
 Requires-Dist: mkdocs-click; extra == 'docs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.1.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=8.5.4; extra == 'docs'
 Requires-Dist: mkdocs-typer; extra == 'docs'
 Requires-Dist: mkdocstrings[python]~=0.19.0; extra == 'docs'
 Requires-Dist: mkdocs~=1.4.0; extra == 'docs'
+Provides-Extra: omx
+Requires-Dist: pytables; extra == 'omx'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
 Requires-Dist: pre-commit~=2.20.0; extra == 'quality'
 Requires-Dist: ruff; extra == 'quality'
 Provides-Extra: tests
 Requires-Dist: pytest~=7.1.2; extra == 'tests'
+Requires-Dist: tables; extra == 'tests'
 Description-Content-Type: text/markdown
 
-# WRING
+# Wring
 
-A tool to compress multiple CSV files into parquet.
-
-The default uses zstd compression level 9, which is more than average.
+A tool to manage efficient compression of various data files.
```

