# Comparing `tmp/crm1-0.0.9.tar.gz` & `tmp/crm1-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.0.9.tar", max compression
+gzip compressed data, was "crm1-0.1.0.tar", max compression
```

## Comparing `crm1-0.0.9.tar` & `crm1-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rw-r--r--   0        0        0     1064 2024-04-03 18:22:52.030781 crm1-0.0.9/LICENSE
--rw-r--r--   0        0        0     4110 2024-04-03 18:22:52.030781 crm1-0.0.9/README.md
--rw-r--r--   0        0        0      152 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/__init__.py
--rw-r--r--   0        0        0      394 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/autorepotools.py
--rw-r--r--   0        0        0        0 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/helpers/__init__.py
--rw-r--r--   0        0        0     7088 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/helpers/versions.py
--rw-r--r--   0        0        0      176 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/__init__.py
--rw-r--r--   0        0        0     1954 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/common_modext.py
--rw-r--r--   0        0        0      437 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/dependency.py
--rw-r--r--   0        0        0      948 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/mod.py
--rw-r--r--   0        0        0      553 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/spec/repository.py
--rw-r--r--   0        0        0      153 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/__init__.py
--rw-r--r--   0        0        0     1043 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/dependency.py
--rw-r--r--   0        0        0     1068 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/mod.py
--rw-r--r--   0        0        0     1869 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/repository.py
--rw-r--r--   0        0        0     2818 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      574 2024-04-03 18:22:52.030781 crm1-0.0.9/crm1/utils.py
--rw-r--r--   0        0        0      476 2024-04-03 18:22:52.030781 crm1-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     4722 1970-01-01 00:00:00.000000 crm1-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-12 20:13:20.045375 crm1-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4110 2024-04-12 20:13:20.045375 crm1-0.1.0/README.md
+-rw-r--r--   0        0        0      139 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/autorepotools.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     7075 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      677 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/__init__.py
+-rw-r--r--   0        0        0     1972 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/common_modext.py
+-rw-r--r--   0        0        0      436 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/dependency.py
+-rw-r--r--   0        0        0      907 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/mod.py
+-rw-r--r--   0        0        0      557 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/repository.py
+-rw-r--r--   0        0        0      176 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/__init__.py
+-rw-r--r--   0        0        0     1973 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/common_modext.py
+-rw-r--r--   0        0        0      436 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/dependency.py
+-rw-r--r--   0        0        0      907 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/mod.py
+-rw-r--r--   0        0        0      680 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/repository.py
+-rw-r--r--   0        0        0      142 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/__init__.py
+-rw-r--r--   0        0        0     2156 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1093 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/mod.py
+-rw-r--r--   0        0        0     3750 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/repository.py
+-rw-r--r--   0        0        0     3125 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      824 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/utils.py
+-rw-r--r--   0        0        0      631 2024-04-12 20:13:20.049375 crm1-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 crm1-0.1.0/PKG-INFO
```

### Comparing `crm1-0.0.9/LICENSE` & `crm1-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crm1-0.0.9/README.md` & `crm1-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crm1-0.0.9/crm1/helpers/versions.py` & `crm1-0.1.0/crm1/helpers/versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,20 @@
         The string should be in the format of `[lower,upper]`. Examples: `[1.0,2.0.1)`, `(1.0,]`.
         """
         if range_.startswith("["):
             lower_mode = VersionEndMode.INCLUSIVE
         elif range_.startswith("("):
             lower_mode = VersionEndMode.EXCLUSIVE
         else:
-            return VersionRange(Version.from_string(range_), DONTCARE, Version.from_string(range_), DONTCARE)
+            return VersionRange(
+                Version.from_string(range_),
+                DONTCARE,
+                Version.from_string(range_),
+                DONTCARE,
+            )
         if range_.endswith("]"):
             upper_mode = VersionEndMode.INCLUSIVE
         elif range_.endswith(")"):
             upper_mode = VersionEndMode.EXCLUSIVE
         else:
             raise ValueError("Invalid range string")
         range_ = range_[1:-1]
@@ -159,27 +164,23 @@
                 else ")"
             )
         )
 
     def contains(self, version: Version) -> bool:
         """Check if the version is in the range."""
         if self.lower is not None:
-            if self.lower_mode == VersionEndMode.INCLUSIVE:
-                if version < self.lower:
-                    return False
-            else:
-                if version <= self.lower:
-                    return False
+            if version < self.lower:
+                return False
+            if self.lower_mode == VersionEndMode.EXCLUSIVE and version == self.lower:
+                return False
         if self.upper is not None:
-            if self.upper_mode == VersionEndMode.INCLUSIVE:
-                if version > self.upper:
-                    return False
-            else:
-                if version >= self.upper:
-                    return False
+            if version > self.upper:
+                return False
+            if self.upper_mode == VersionEndMode.EXCLUSIVE and version == self.upper:
+                return False
         return True
 
     def __contains__(self, version: Version) -> bool:
         return self.contains(version)
 
     def __str__(self) -> str:
         return self.to_string()
```

### Comparing `crm1-0.0.9/crm1/spec/common_modext.py` & `crm1-0.1.0/crm1/spec/v1/common_modext.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Don't import this module directly."""
 
 from dataclasses import dataclass, field
 from typing import Optional
 
+from dataclasses_hjson import DataClassHjsonMixin
 from dataclasses_json import CatchAll, Undefined
 
-from .. import spec
-from dataclasses_hjson import DataClassHjsonMixin, using_config
+from .. import v1 as spec
 
 
-@using_config(
-    undefined=Undefined.EXCLUDE,
-)
 @dataclass
 class CommonModExt(DataClassHjsonMixin):
     """Some common mod.ext fields. Unknown fields are stored in `others`."""
 
+    dataclass_json_config = {
+        "undefined": Undefined.INCLUDE,
+    }
     icon: Optional[str] = None
     """A URL to the mod's icon."""
     modid: Optional[str] = None
     """The mod's ID. This is similar to mod.id, but does not include the group. Eg. `examplemod`."""
     loader: Optional[str] = None
     """Which mod loader the mod uses. Eg. `fabric`."""
     loader_version: Optional[str] = None
```

### Comparing `crm1-0.0.9/crm1/spec/mod.py` & `crm1-0.1.0/crm1/spec/v1/mod.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Don't import this module directly."""
 
 from dataclasses import dataclass
 
-from dataclasses_json import LetterCase
+from dataclasses_hjson import DataClassHjsonMixin
 
 from .common_modext import CommonModExt
 from .dependency import RDependency
 
-from dataclasses_hjson import DataClassHjsonMixin
-
 
 @dataclass
 class RMod(DataClassHjsonMixin):
     """Raw mod data. This is used for deserialization."""
 
     id: str
     """Mod ID. This is in the format of group.id, like `com.example.mod`."""
```

### Comparing `crm1-0.0.9/crm1/spec/repository.py` & `crm1-0.1.0/crm1/spec/v1/repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Don't import this module directly."""
 
 from dataclasses import dataclass
 
+from dataclasses_hjson import DataClassHjsonMixin
 
 from .mod import RMod
-from dataclasses_hjson import DataClassHjsonMixin
 
 
 @dataclass
 class RRepository(DataClassHjsonMixin):
     """Raw repository data. This is used for deserialization."""
 
-    spec_version: int
-    """The version of the repository specification."""
     last_updated: int
     """The timestamp of the last update of the repository."""
     root_id: str
     """The root ID of the repository."""
     mods: list[RMod]
     """A list of mods in the repository."""
+    spec_version: int = 1
+    """The version of the repository specification."""
```

### Comparing `crm1-0.0.9/crm1/types/mod.py` & `crm1-0.1.0/crm1/types/mod.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Don't import this module directly."""
 
 from .. import spec
 from .dependency import Dependency
 
 
 class Mod:
-    """This class represents a mod.
+    """
+    This class represents a mod.
 
     Raises:
         ValueError: If the data is not of type spec.RMod
     """
 
     meta: spec.RMod
     """The raw data of the mod."""
@@ -27,15 +28,15 @@
     @property
     def id(self) -> str:
         """The ID of the mod."""
         return self.meta.id
 
     @property
     def depends(self) -> list[Dependency]:
-        """The dependencies of the mod."""
+        """The required dependencies of the mod."""
         return [Dependency(dep) for dep in self.meta.deps]
 
     @property
     def suggests(self) -> list[Dependency]:
-        """The suggestions of the mod."""
+        """The suggested dependencies of the mod."""
         if self.meta.ext.suggests is not None:
             return [Dependency(dep) for dep in self.meta.ext.suggests]
```

### Comparing `crm1-0.0.9/PKG-INFO` & `crm1-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: crm1
-Version: 0.0.9
+Version: 0.1.0
 Summary: A CRM-1 repository exploration package
+Home-page: https://github.com/J0J0HA/py-crm1
 License: MIT
+Keywords: crm1,repository,exploration,python
 Author: JoJoJux
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dataclasses-hjson (>=0.0.3,<0.0.4)
 Requires-Dist: hjson (>=3.1.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/J0J0HA/py-crm1
 Description-Content-Type: text/markdown
 
 # ``crm1`` Python package
 
 This package is a Python implementation of the CRM-1 specification.
 
 You can find the specification [here](https://github.com/CRModders/CRM-1/).
```

