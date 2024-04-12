# Comparing `tmp/edwh_restic_plugin-0.7.2.tar.gz` & `tmp/edwh_restic_plugin-0.7.3.tar.gz`

## Comparing `edwh_restic_plugin-0.7.2.tar` & `edwh_restic_plugin-0.7.3.tar`

### file list

```diff
@@ -1,29 +1,27 @@
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/CHANGELOG.md
--rwxr-xr-x   0        0        0       61 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/captain-hooks/backup_files.sh
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/env.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/helpers.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/restictypes.py
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0    17839 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/b2.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/local.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/oracle.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/s3.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/sftp.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/swift.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/tests/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/tests/test_repository_detection.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/README.md
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7741 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/env.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/helpers.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/restictypes.py
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0    17838 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/b2.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/local.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/oracle.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/s3.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/sftp.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/swift.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/tests/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/tests/test_repository_detection.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/LICENSE.txt
+-rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/README.md
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     7741 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.7.3/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.7.2/CHANGELOG.md` & `edwh_restic_plugin-0.7.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.7.3 (2024-04-12)
+
+### Fix
+
+* Add `edwh.require_sudo` to improve sudo password prompting ([`bf77993`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/bf77993be0d13773e2aad97c6109410bf4a952c7))
+
 ## v0.7.2 (2024-03-15)
 ### Fix
 * **hooks:** Show exit code on file execution error ([`15fb3f6`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/15fb3f60b16cd0d2bb4cfd71e948e67dadbfb8a5))
 
 ## v0.7.1 (2024-03-15)
 ### Fix
 * Output stdout and stderr live (instead of afterwards) ([`476132f`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/476132fbb0ef2ea3ade3cc5cbc7cce1dfaa319a1))
```

### Comparing `edwh_restic_plugin-0.7.2/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.7.3/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.7.3/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/env.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/env.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/helpers.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import typing
 
 import invoke
+from edwh.tasks import require_sudo
 
 T = typing.TypeVar("T")
 
 
 def fix_tags(tags: typing.Iterable[T | None]) -> list[T]:
     """
     Removes all None type elements from the input list.
@@ -16,25 +17,28 @@
     return [tag for tag in tags if tag is not None]
 
 
 def camel_to_snake(s: str) -> str:
     return "".join([f"_{c.lower()}" if c.isupper() else c for c in s]).lstrip("_")
 
 
-def _require_restic(c: invoke.Context = None):
+def _require_restic(c: invoke.Context = None) -> bool:
     """
     Checks if 'restic' is installed in the system. If not, it installs 'restic' using the 'apt' package manager
     and updates it to the latest version. The function returns False if 'restic' is already installed,
     and True after successfully installing and updating 'restic'.
 
     :param c: An optional Invoke context. If not provided, a new context will be created.
     :return: False if 'restic' is already installed, True otherwise.
     """
     c = c or invoke.Context()  # type: invoke.Context
     if c.run("which restic", warn=True, hide=True).ok:
+        # restic already exists, do nothing
         return False
 
-    print("Restic missing from this system! Installing now...", file=sys.stderr)
-    c.sudo("sudo apt install -y restic", hide=True)
-    c.sudo("restic self-update", hide=True)
-    print("Restic installed and updated!", file=sys.stderr)
-    return True
+    if require_sudo(c):
+        # sudo available
+        print("Restic missing from this system! Installing now...", file=sys.stderr)
+        c.sudo("sudo apt install -y restic", hide=True)
+        c.sudo("restic self-update", hide=True)
+        print("Restic installed and updated!", file=sys.stderr)
+        return True
```

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/restictypes.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/restictypes.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/__init__.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
 
         print("\n\nfile status codes:")
 
         for filename, status_code in zip(files, file_codes):
             if status_code == 0:
                 print(filename, tag="success", tag_color="green")
             else:
-                print( filename, tag=f"failure ({status_code})", tag_color="red")
+                print(filename, tag=f"failure ({status_code})", tag_color="red")
 
         if worst_status_code := max(file_codes) > 0:
             exit(worst_status_code)
 
     def backup(self, c, verbose: bool, target: str, message: str | None):
         """
         Backs up the specified target.
```

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/b2.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/b2.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/local.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/local.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/oracle.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/oracle.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/s3.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/s3.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/sftp.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/sftp.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/src/edwh_restic_plugin/repositories/swift.py` & `edwh_restic_plugin-0.7.3/src/edwh_restic_plugin/repositories/swift.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/tests/test_repository_detection.py` & `edwh_restic_plugin-0.7.3/tests/test_repository_detection.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/LICENSE.txt` & `edwh_restic_plugin-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/README.md` & `edwh_restic_plugin-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/pyproject.toml` & `edwh_restic_plugin-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.7.2/PKG-INFO` & `edwh_restic_plugin-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: edwh-restic-plugin
-Version: 0.7.2
+Version: 0.7.3
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

