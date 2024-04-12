# Comparing `tmp/laorm-2.1.0.tar.gz` & `tmp/laorm-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laorm-2.1.0.tar", max compression
+gzip compressed data, was "laorm-2.2.0.tar", max compression
```

## Comparing `laorm-2.1.0.tar` & `laorm-2.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      208 2024-03-18 02:36:55.471518 laorm-2.1.0/laorm/__init__.py
--rw-r--r--   0        0        0     1425 2024-03-13 06:31:12.009572 laorm-2.1.0/laorm/PPA.py
--rw-r--r--   0        0        0    14123 2024-03-18 02:30:45.266747 laorm-2.1.0/laorm/stream.py
--rw-r--r--   0        0        0    11558 2024-03-13 06:31:12.008017 laorm-2.1.0/LICENSE
--rw-r--r--   0        0        0     1306 2024-03-18 02:36:55.356661 laorm-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 laorm-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      208 2024-04-12 16:23:38.155130 laorm-2.2.0/laorm/__init__.py
+-rw-r--r--   0        0        0     1425 2024-03-10 14:20:23.040591 laorm-2.2.0/laorm/PPA.py
+-rw-r--r--   0        0        0    14711 2024-04-12 16:21:34.004920 laorm-2.2.0/laorm/stream.py
+-rw-r--r--   0        0        0    11558 2024-01-12 14:31:32.745557 laorm-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1362 2024-04-12 16:23:37.972664 laorm-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 laorm-2.2.0/PKG-INFO
```

### Comparing `laorm-2.1.0/laorm/PPA.py` & `laorm-2.2.0/laorm/PPA.py`

 * *Files identical despite different names*

### Comparing `laorm-2.1.0/laorm/stream.py` & `laorm-2.2.0/laorm/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             "from": "",
             "where": [],
             "field": [],
             "value": [],
             "group_by": [],
             "having": [],
             "order_by": [],
+            "limit": [],
         }
 
     def process_keyword(self, keyword, value=None):
         # 异常返回
         if self.current_state == "select" and keyword not in ["by", "from"]:
             return
         if keyword == "select":
@@ -57,14 +58,16 @@
         elif keyword == "order_by":
             self.sql_parts["order_by"].append(value)
             self.current_state = "order_by"
         elif keyword == "by":
             self.current_state = "by"
         elif keyword == "insertField":
             self.sql_parts["field"].append(value)
+        elif keyword == "limit":
+            self.sql_parts["limit"].append(value)
         elif keyword == "insertValue":
             self.sql_parts["value"].append(value)
 
             pass  # 其他可能的状态处理
 
     def selectMode(self):
         if self.mode != "select":
@@ -76,14 +79,16 @@
             execute_sql += f"where {' AND '.join(self.sql_parts['where'])} "
         if self.sql_parts["group_by"]:
             execute_sql += f"GROUP by {' ,'.join(self.sql_parts['group_by'])} "
         if self.sql_parts["having"]:
             execute_sql += f"having {' AND '.join(self.sql_parts['having'])} "
         if self.sql_parts["order_by"]:
             execute_sql += f"ORDER by {' ,'.join(self.sql_parts['order_by'])} "
+        if len(self.sql_parts["limit"]):
+            execute_sql += f"{self.sql_parts['limit'][0]}"
         self.execute_sql = execute_sql
 
     def postMode(self):
         if self.mode != "post":
             return True
         values_str_list = [
             f"({', '.join(map(str, row))})" for row in self.sql_parts["value"]
@@ -119,14 +124,15 @@
             "from": self.sql_parts["from"],
             "where": [],
             "group_by": [],
             "having": [],
             "field": [],
             "value": [],
             "order_by": [],
+            "limit": []
         }
 
     def finalize(self):
         self.selectMode() and self.postMode() and self.updateMode() and self.deleteMode()
         self.current_state = "final"
         return self.execute_sql
 
@@ -274,14 +280,25 @@
             cls.state_machine.process_keyword(
                 "where", f"{cls.primaryKey} in {({', '.join(map(str, primaryIdList))})}"
             )
         res, _ = await cls.exec()
         return res
 
     @classmethod
+    async def page(cls: type[T], page: dict) -> T:
+        pageIndex = page.get("page")
+        size = page.get("size")
+        pageIndex = (pageIndex - 1) * size
+        cls.state_machine.process_keyword("limit", f"limit {pageIndex},{size}")
+        res, _ = await cls.exec()
+        # 封装新page
+
+        return res
+
+    @classmethod
     async def post(cls: type[T], data: T | list[T] = None):
         cls.state_machine.mode = "post"
         if data and not isinstance(data, (list, tuple)):
             data = [data]
 
         for key, _ in cls.dictMap.items():
             cls.state_machine.process_keyword("insertField", key)
```

### Comparing `laorm-2.1.0/LICENSE` & `laorm-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laorm-2.1.0/pyproject.toml` & `laorm-2.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "laorm"
-version = "2.1.0"
+version = "2.2.0"
 description = "A python async orm tool"
 authors = ["larry <176286171@qq.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/mryzhou/laorm"
 
 repository = "https://github.com/mryzhou/laorm.git"  # 可选，指定项目仓库地址
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiomysql = "*"
-
+cryptography = "^42.0.5" # aiomysql 密码认证依赖
 [tool.poetry.dev-dependencies]
 fastapi = "^0.110.0"  # 更改为最新稳定版的FastAPI
 uvicorn = {extras = ["standard"], version = "^0.27.1"}  # 或者使用最新稳定版Uvicorn
 
+
 [tool.poetry.extras]
 fastapi = ["fastapi"]
 flask = ["flask"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `laorm-2.1.0/PKG-INFO` & `laorm-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: laorm
-Version: 2.1.0
+Version: 2.2.0
 Summary: A python async orm tool
 Home-page: https://github.com/mryzhou/laorm
 License: Apache-2.0
 Author: larry
 Author-email: 176286171@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fastapi
 Provides-Extra: flask
 Requires-Dist: aiomysql
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Project-URL: Repository, https://github.com/mryzhou/laorm.git
```

