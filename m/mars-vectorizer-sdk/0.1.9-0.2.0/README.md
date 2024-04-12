# Comparing `tmp/mars_vectorizer_sdk-0.1.9.tar.gz` & `tmp/mars_vectorizer_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mars_vectorizer_sdk-0.1.9.tar", max compression
+gzip compressed data, was "mars_vectorizer_sdk-0.2.0.tar", max compression
```

## Comparing `mars_vectorizer_sdk-0.1.9.tar` & `mars_vectorizer_sdk-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2580 2024-03-04 14:41:00.938965 mars_vectorizer_sdk-0.1.9/README.md
--rw-r--r--   0        0        0     8801 2024-03-13 14:53:06.832774 mars_vectorizer_sdk-0.1.9/mars_vectorizer_sdk/__init__.py
--rw-r--r--   0        0        0      292 2024-03-13 14:53:24.613828 mars_vectorizer_sdk-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 mars_vectorizer_sdk-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2580 2024-03-04 14:41:00.938965 mars_vectorizer_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0    10183 2024-04-12 14:47:59.587292 mars_vectorizer_sdk-0.2.0/mars_vectorizer_sdk/__init__.py
+-rw-r--r--   0        0        0      292 2024-04-12 14:51:59.662116 mars_vectorizer_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 mars_vectorizer_sdk-0.2.0/PKG-INFO
```

### Comparing `mars_vectorizer_sdk-0.1.9/README.md` & `mars_vectorizer_sdk-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mars_vectorizer_sdk-0.1.9/mars_vectorizer_sdk/__init__.py` & `mars_vectorizer_sdk-0.2.0/mars_vectorizer_sdk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,21 @@
                 value=self.dtype(reduce(lambda x,y: x[y], self.path, data))
             )
         except:
             return None
         
     def sha256(self) -> str:
         return sha256((self.name + str(self.dtype) + "".join(self.path)).encode()).hexdigest()
+    
+    def to_json(self) -> dict:
+        return {
+            "name": self.name,
+            "dtype": self.dtype.__name__,
+            "path": self.path
+        }
         
 @dataclass
 class ListPropertyParser:
 
     name: str
     parser: Union["GroupParser", "PropertyParser"]
     path: List[str]
@@ -89,19 +96,26 @@
                 )
             )
         )
     
     def sha256(self) -> str:
         return sha256((self.name + self.parser.sha256() + "".join(self.path)).encode()).hexdigest()
     
+    def to_json(self) -> dict:
+        return {
+            "name": self.name,
+            "parser": self.parser.to_json(),
+            "path": self.path
+        }
+    
 @dataclass
 class GroupParser:
 
     name: str
-    children: List[Union["GroupParser", "PropertyParser"]]
+    children: List[Union["GroupParser", PropertyParser, ListPropertyParser]]
 
     def __call__(self, data: dict) -> Group:
         return Group(
             name=self.name,
             values=list(
                 filter(
                     lambda x: x is not None, 
@@ -111,14 +125,48 @@
                     )
                 )
             )
         )
     
     def sha256(self) -> str:
         return sha256((self.name + "".join(map(lambda x: x.sha256(), self.children))).encode()).hexdigest()
+    
+    @staticmethod
+    def from_json(json: dict) -> "GroupParser":
+
+        def parse_child(child):
+            if "children" in child:
+                return GroupParser.from_json(child)
+            elif "dtype" in child:
+                return PropertyParser(name=child["name"], dtype=eval(child["dtype"]), path=child["path"])
+            elif "parser" in child:
+                return ListPropertyParser(name=child["name"], parser=parse_child(child["parser"]), path=child["path"])
+            else:
+                raise ValueError("Invalid JSON")
+
+        return GroupParser(
+            name=json["name"],
+            children=list(
+                map(
+                    parse_child,
+                    json["children"]
+                )
+            )
+        )
+    
+    def to_json(self) -> dict:
+        return {
+            "name": self.name,
+            "children": list(
+                map(
+                    lambda x: x.to_json(),
+                    self.children
+                )
+            )
+        }
         
 @dataclass
 class VectorProperty:
 
     name: str
     vector: np.ndarray = field(repr=False)
     value: Union[str, float] = field(repr=False)
```

### Comparing `mars_vectorizer_sdk-0.1.9/PKG-INFO` & `mars_vectorizer_sdk-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mars-vectorizer-sdk
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

