# Comparing `tmp/dbservice-2.1.2.tar.gz` & `tmp/dbservice-2.1.3.tar.gz`

## Comparing `dbservice-2.1.2.tar` & `dbservice-2.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.2/.DS_Store
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dbservice-2.1.2/PKG-INFO
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/.DS_Store
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/DBService/__init__.py
--rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/DBService/dbcore.py
--rw-r--r--   0        0        0    26116 2020-02-02 00:00:00.000000 dbservice-2.1.2/src/DBService/dbcore_old.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dbservice-2.1.2/test/__init__.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 dbservice-2.1.2/test/test.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbservice-2.1.2/test/testMysql_gone_away.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dbservice-2.1.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dbservice-2.1.2/LICENSE
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 dbservice-2.1.2/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbservice-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dbservice-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.3/.DS_Store
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dbservice-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 dbservice-2.1.3/src/.DS_Store
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbservice-2.1.3/src/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dbservice-2.1.3/src/DBService/__init__.py
+-rw-r--r--   0        0        0    18078 2020-02-02 00:00:00.000000 dbservice-2.1.3/src/DBService/dbcore.py
+-rw-r--r--   0        0        0    26116 2020-02-02 00:00:00.000000 dbservice-2.1.3/src/DBService/dbcore_old.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 dbservice-2.1.3/test/__init__.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 dbservice-2.1.3/test/test.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 dbservice-2.1.3/test/testMysql_gone_away.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dbservice-2.1.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dbservice-2.1.3/LICENSE
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 dbservice-2.1.3/README.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dbservice-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 dbservice-2.1.3/PKG-INFO
```

### Comparing `dbservice-2.1.2/.DS_Store` & `dbservice-2.1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.2/PKG-INFO` & `dbservice-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBService
-Version: 2.1.2
+Version: 2.1.3
 Summary: a Database Wrapper for Redis and MySQL
 Project-URL: Homepage, https://pypi.org/project/DBService/
 Author-email: "hang.zhang" <hhczy1003@163.com>, "Marrin.Hu" <himarrin@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `dbservice-2.1.2/src/.DS_Store` & `dbservice-2.1.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.2/src/DBService/dbcore.py` & `dbservice-2.1.3/src/DBService/dbcore.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,15 @@
         # 创建连接池
         self.pool = await aiomysql.create_pool(
             host=self.host,
             port=self.port,
             user=self.user,
             password=self.password,
             db=self.db,
+            autocommit=True,
             minsize=self.minsize,
             maxsize=self.maxsize
         )
 
     async def close_pool(self):
         # 关闭连接池
         self.pool.close()
@@ -416,15 +417,16 @@
 
     async def execute(self, query, params=None):
         return await self.query(query, params, fetch_all=False)
 
     async def transaction(self, queries):
         async with self.pool.acquire() as conn:
             async with conn.cursor() as cur:
+                await conn.begin()
                 try:
-                    await conn.begin()
                     for query in queries:
                         await cur.execute(query)
                     await conn.commit()
+                    return True  # 如果所有操作都成功，返回True
                 except Exception as e:
-                    await cur.execute("ROLLBACK")
-                    raise e
+                    await conn.rollback()
+                    return False  # 如果发生异常，回滚事务并返回False
```

### Comparing `dbservice-2.1.2/src/DBService/dbcore_old.py` & `dbservice-2.1.3/src/DBService/dbcore_old.py`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.2/test/test.py` & `dbservice-2.1.3/test/test.py`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.2/test/testMysql_gone_away.py` & `dbservice-2.1.3/test/testMysql_gone_away.py`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.2/LICENSE` & `dbservice-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.2/README.md` & `dbservice-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dbservice-2.1.2/pyproject.toml` & `dbservice-2.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DBService"
-version = "2.1.2"
+version = "2.1.3"
 authors = [
   { name="hang.zhang", email="hhczy1003@163.com"},
   { name="Marrin.Hu", email="himarrin@gmail.com"},
 ]
 description = "a Database Wrapper for Redis and MySQL"
 readme = "README.md"
 requires-python = ">=3.8"
```

