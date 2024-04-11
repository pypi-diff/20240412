# Comparing `tmp/metasequoia-sql-0.1.1.tar.gz` & `tmp/metasequoia-sql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasequoia-sql-0.1.1.tar", last modified: Tue Apr  9 23:19:48 2024, max compression
+gzip compressed data, was "metasequoia-sql-0.2.0.tar", last modified: Thu Apr 11 23:37:26 2024, max compression
```

## Comparing `metasequoia-sql-0.1.1.tar` & `metasequoia-sql-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.397704 metasequoia-sql-0.1.1/
--rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6183 2024-04-09 23:19:48.396703 metasequoia-sql-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5514 2024-04-09 23:19:02.000000 metasequoia-sql-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.385703 metasequoia-sql-0.1.1/metasequoia_sql/
--rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.388703 metasequoia-sql-0.1.1/metasequoia_sql/analyzer/
--rw-rw-rw-   0        0        0        0 2024-04-09 23:10:25.000000 metasequoia-sql-0.1.1/metasequoia_sql/analyzer/__init__.py
--rw-rw-rw-   0        0        0     1523 2024-04-09 23:10:25.000000 metasequoia-sql-0.1.1/metasequoia_sql/analyzer/consanguinity.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.390704 metasequoia-sql-0.1.1/metasequoia_sql/ast/
--rw-rw-rw-   0        0        0       86 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/__init__.py
--rw-rw-rw-   0        0        0     8647 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/functions.py
--rw-rw-rw-   0        0        0    17093 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/nodes.py
--rw-rw-rw-   0        0        0     8463 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/ast/parser.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.392703 metasequoia-sql-0.1.1/metasequoia_sql/common/
--rw-rw-rw-   0        0        0        0 2024-04-09 23:06:06.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/__init__.py
--rw-rw-rw-   0        0        0     3617 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/base_scanner.py
--rw-rw-rw-   0        0        0      325 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/basic.py
--rw-rw-rw-   0        0        0      150 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/text_scanner.py
--rw-rw-rw-   0        0        0     5712 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/common/token_scanner.py
--rw-rw-rw-   0        0        0      665 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/errors.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.392703 metasequoia-sql-0.1.1/metasequoia_sql/objects/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/objects/__init__.py
--rw-rw-rw-   0        0        0    75855 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/objects/core.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.393704 metasequoia-sql-0.1.1/metasequoia_sql/parser/
--rw-rw-rw-   0        0        0        0 2024-03-11 00:28:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/parser/__init__.py
--rw-rw-rw-   0        0        0    83932 2024-04-09 23:15:51.000000 metasequoia-sql-0.1.1/metasequoia_sql/parser/common.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.395704 metasequoia-sql-0.1.1/metasequoia_sql/static/
--rw-rw-rw-   0        0        0      183 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/common.py
--rw-rw-rw-   0        0        0     2571 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/mysql.py
--rw-rw-rw-   0        0        0     3824 2024-04-07 00:08:43.000000 metasequoia-sql-0.1.1/metasequoia_sql/static/other.py
-drwxrwxrwx   0        0        0        0 2024-04-09 23:19:48.396703 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/
--rw-rw-rw-   0        0        0     6183 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      892 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-09 23:19:48.000000 metasequoia-sql-0.1.1/metasequoia_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 23:19:48.397704 metasequoia-sql-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-04-09 23:17:20.000000 metasequoia-sql-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.256211 metasequoia-sql-0.2.0/
+-rw-rw-rw-   0        0        0     1088 2024-03-11 00:28:43.000000 metasequoia-sql-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6477 2024-04-11 23:37:26.256211 metasequoia-sql-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5808 2024-04-11 23:36:28.000000 metasequoia-sql-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.246211 metasequoia-sql-0.2.0/metasequoia_sql/
+-rw-rw-rw-   0        0        0      150 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.248211 metasequoia-sql-0.2.0/metasequoia_sql/analyzer/
+-rw-rw-rw-   0        0        0        0 2024-04-09 23:10:25.000000 metasequoia-sql-0.2.0/metasequoia_sql/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-04-09 23:10:25.000000 metasequoia-sql-0.2.0/metasequoia_sql/analyzer/consanguinity.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.251211 metasequoia-sql-0.2.0/metasequoia_sql/ast/
+-rw-rw-rw-   0        0        0       86 2024-04-07 00:08:43.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/__init__.py
+-rw-rw-rw-   0        0        0     8647 2024-04-07 00:08:43.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/functions.py
+-rw-rw-rw-   0        0        0    17097 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/nodes.py
+-rw-rw-rw-   0        0        0     8463 2024-04-09 23:15:51.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/parser.py
+-rw-rw-rw-   0        0        0     5581 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/ast/static.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.253211 metasequoia-sql-0.2.0/metasequoia_sql/common/
+-rw-rw-rw-   0        0        0      145 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/__init__.py
+-rw-rw-rw-   0        0        0     3617 2024-04-09 23:15:51.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/base_scanner.py
+-rw-rw-rw-   0        0        0      325 2024-04-07 00:08:43.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/basic.py
+-rw-rw-rw-   0        0        0      150 2024-04-09 23:15:51.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/text_scanner.py
+-rw-rw-rw-   0        0        0     6279 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/common/token_scanner.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.255211 metasequoia-sql-0.2.0/metasequoia_sql/core/
+-rw-rw-rw-   0        0        0      144 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/__init__.py
+-rw-rw-rw-   0        0        0      341 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/data_source.py
+-rw-rw-rw-   0        0        0    85050 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/objects.py
+-rw-rw-rw-   0        0        0    80134 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/parser.py
+-rw-rw-rw-   0        0        0      271 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/core/static.py
+-rw-rw-rw-   0        0        0      592 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/errors.py
+-rw-rw-rw-   0        0        0     1041 2024-04-11 15:14:53.000000 metasequoia-sql-0.2.0/metasequoia_sql/static.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:37:26.255211 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/
+-rw-rw-rw-   0        0        0     6477 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      843 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-11 23:37:26.000000 metasequoia-sql-0.2.0/metasequoia_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 23:37:26.256211 metasequoia-sql-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1042 2024-04-11 23:36:52.000000 metasequoia-sql-0.2.0/setup.py
```

### Comparing `metasequoia-sql-0.1.1/LICENSE` & `metasequoia-sql-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.1/PKG-INFO` & `metasequoia-sql-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasequoia-sql
-Version: 0.1.1
+Version: 0.2.0
 Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
 Home-page: https://github.com/ChangxingJiang/metasequoia-sql
 Author: changxing
 Author-email: 1278729001@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
@@ -37,44 +37,47 @@
 ```
 
 ### 句法分析
 
 对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
 
 ```python
-from metasequoia_sql.parser.common import parse_create_table_statement
-from metasequoia_sql.common.token_scanner import build_token_scanner
+from metasequoia_sql import *
 
 statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ### 翻译工具
 
 将 MySQL 的 CREATE TABLE 语句转换为 Hive 的 CREATE TABLE 语句：
 
 ```python
-from metasequoia_sql.parser.common import parse_create_table_statement
-from metasequoia_sql.translate import *
-from metasequoia_sql.common.token_scanner import build_token_scanner
+from metasequoia_sql import *
 
 statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ## 实现原理
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
 FullStatement 转化为另一个 DataSource 的 SQl。通过这样的处理，可以避免开发网状结构的转换器，而只需要开发星星转换器即可。
 
+- `analyzer`：分析器
 - `ast`：词法分析（主要使用有限状态自动机实现）
 - `common`：遍历器工具
+- `core`：句法分析节点类
+  - `abc`：抽象类（节点中不包含解析方法）
+  - `element`：元素类节点（不会引用其他节点）
+  - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
 - `objects`：SQL语句对象
 - `parser`：SQL语句解析器
-- `translate`：翻译器
+
+（因为在 Python 中若标记类型时，不同文件之间不同循环引用，所以需要保证所有类的引用之间为严格的拓扑关系）
 
 ### 词法分析
 
 字面值类型：[参考文档](https://deepinout.com/mysql/mysql-top-articles-mysql/1694052463_j_mysql-literals.html)
 
 - `ASTLiteralString`：字符串字面值
 
@@ -128,27 +131,28 @@
 
 ## 已知的不兼容
 
 - DB2 的 `CURRENT DATE` 的语法
 
 ## 修改记录
 
-#### 0.1.0 > 0.1.1
+#### 0.1.0 > 0.2.0
 
 新增：
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
 - 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
-- 清理多余对象
-- TokenScanner 使用方法
+- 整理 objects 的节点和 parse 中的方法，清理多余对象，优化引用路径
+- 统一 TokenScanner 使用方法
 
 修复：
 - `WITH` 语句解析报错的 Bug 修复
+- Hive 建表语句的类型包含参数的 Bug 修复
 
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
 
 ##### 0.0.1
```

### Comparing `metasequoia-sql-0.1.1/README.md` & `metasequoia-sql-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,44 +19,47 @@
 ```
 
 ### 句法分析
 
 对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
 
 ```python
-from metasequoia_sql.parser.common import parse_create_table_statement
-from metasequoia_sql.common.token_scanner import build_token_scanner
+from metasequoia_sql import *
 
 statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ### 翻译工具
 
 将 MySQL 的 CREATE TABLE 语句转换为 Hive 的 CREATE TABLE 语句：
 
 ```python
-from metasequoia_sql.parser.common import parse_create_table_statement
-from metasequoia_sql.translate import *
-from metasequoia_sql.common.token_scanner import build_token_scanner
+from metasequoia_sql import *
 
 statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ## 实现原理
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
 FullStatement 转化为另一个 DataSource 的 SQl。通过这样的处理，可以避免开发网状结构的转换器，而只需要开发星星转换器即可。
 
+- `analyzer`：分析器
 - `ast`：词法分析（主要使用有限状态自动机实现）
 - `common`：遍历器工具
+- `core`：句法分析节点类
+  - `abc`：抽象类（节点中不包含解析方法）
+  - `element`：元素类节点（不会引用其他节点）
+  - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
 - `objects`：SQL语句对象
 - `parser`：SQL语句解析器
-- `translate`：翻译器
+
+（因为在 Python 中若标记类型时，不同文件之间不同循环引用，所以需要保证所有类的引用之间为严格的拓扑关系）
 
 ### 词法分析
 
 字面值类型：[参考文档](https://deepinout.com/mysql/mysql-top-articles-mysql/1694052463_j_mysql-literals.html)
 
 - `ASTLiteralString`：字符串字面值
 
@@ -110,27 +113,28 @@
 
 ## 已知的不兼容
 
 - DB2 的 `CURRENT DATE` 的语法
 
 ## 修改记录
 
-#### 0.1.0 > 0.1.1
+#### 0.1.0 > 0.2.0
 
 新增：
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
 - 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
-- 清理多余对象
-- TokenScanner 使用方法
+- 整理 objects 的节点和 parse 中的方法，清理多余对象，优化引用路径
+- 统一 TokenScanner 使用方法
 
 修复：
 - `WITH` 语句解析报错的 Bug 修复
+- Hive 建表语句的类型包含参数的 Bug 修复
 
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
 
 ##### 0.0.1
```

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/analyzer/consanguinity.py` & `metasequoia-sql-0.2.0/metasequoia_sql/analyzer/consanguinity.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/ast/functions.py` & `metasequoia-sql-0.2.0/metasequoia_sql/ast/functions.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/ast/nodes.py` & `metasequoia-sql-0.2.0/metasequoia_sql/ast/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - 中间节点（插入语节点）：包含子节点的节点
 """
 
 import abc
 from typing import List, Optional, Any
 
 from metasequoia_sql.errors import AstParseError
-from metasequoia_sql.static import HEXADECIMAL_CHARACTER_SET, BINARY_CHARACTER_SET
+from metasequoia_sql.ast.static import HEXADECIMAL_CHARACTER_SET, BINARY_CHARACTER_SET
 
 __all__ = [
     "AST",
     # 固定值节点类
     "ASTSpace", "ASTLineBreak", "ASTComma", "ASTSemicolon",
 
     "ASTCommon",
```

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/ast/parser.py` & `metasequoia-sql-0.2.0/metasequoia_sql/ast/parser.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/common/base_scanner.py` & `metasequoia-sql-0.2.0/metasequoia_sql/common/base_scanner.py`

 * *Files identical despite different names*

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/common/token_scanner.py` & `metasequoia-sql-0.2.0/metasequoia_sql/common/token_scanner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 """
 TODO 多语句解析支持
+TODO 支持匹配各种特殊要求，例如：
+    return not scanner.is_finish and (
+            scanner.now.is_maybe_name and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
+            scanner.next1 is not None and scanner.next1.is_parenthesis and
+            scanner.next2 is not None and scanner.next2.equals("OVER") and
+            scanner.next3 is not None and scanner.next3.is_parenthesis)
 """
 
 from typing import List
 
 from metasequoia_sql import ast
 from metasequoia_sql.common.base_scanner import BaseScanner
 from metasequoia_sql.errors import ScannerError
@@ -76,14 +82,18 @@
         - 如果匹配成功，则将指针移动到 tokens 后的下一个元素
         - 如果匹配失败，则抛出异常
         """
         for word in tokens:
             if not self.pop().equals(word):
                 raise ScannerError(f"没有解析到目标词语:{self._elements}, 目标词={tokens}")
 
+    def get_as_source(self) -> str:
+        """将指针向后移动 1 个元素并返回当前元素的 source"""
+        return self.now.source
+
     def pop_as_source(self) -> str:
         """将指针向后移动 1 个元素并返回当前元素的 source"""
         return self.pop().source
 
     def get_as_children_scanner(self, ignore_space: bool = True, ignore_comment: bool = True) -> "TokenScanner":
         """【不移动指针】返回当前指针位置的插入语节点的子节点的扫描器"""
         return TokenScanner(self.now.children, ignore_space=ignore_space, ignore_comment=ignore_comment)
```

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/errors.py` & `metasequoia-sql-0.2.0/metasequoia_sql/errors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+"""
+在 metasequoia_sql 中年可能抛出的异常
+"""
+
+__all__ = ["SqlParseError", "AstParseError", "UnSupportDataSourceError", "ScannerError"]
+
+
 class SqlParseError(Exception):
     """SQL解析失败的异常"""
 
     def __init__(self, reason: str):
         self.reason = reason
 
 
 class AstParseError(SqlParseError):
     """AST 解析失败"""
 
 
-class TokenIdxOutOfRangeError(SqlParseError):
-    """尝试获取超过 Tokens 长度的抽象语法树节点的异常"""
-
-
-class FullStatementCalledSource(Exception):
-    """调用了 FullStatement 的 source 方法"""
-
-
 class UnSupportDataSourceError(Exception):
     """数据源不支持的语法异常"""
 
     def __init__(self, reason: str):
         self.reason = reason
 
 
 class ScannerError(Exception):
-    """文本扫描异常"""
+    """文本扫描异常"""
```

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/objects/core.py` & `metasequoia-sql-0.2.0/metasequoia_sql/core/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,415 +7,552 @@
 """
 
 import abc
 import enum
 from typing import Optional, List, Tuple, Union, Dict
 
 from metasequoia_sql.common.basic import ordered_distinct
-from metasequoia_sql.errors import SqlParseError
+from metasequoia_sql.core.data_source import DataSource
+from metasequoia_sql.errors import SqlParseError, UnSupportDataSourceError
 
+__all__ = [
+    # ------------------------------ 所有 SQL 语句对象节点的抽象基类 ------------------------------
+    "SQLBase",
 
-class DataSource(enum.Enum):
-    MYSQL = "MYSQL"
-    HIVE = "HIVE"
+    # ------------------------------ 基础元素（其中不引用其他元素） ------------------------------
+    # 插入类型
+    "EnumInsertType", "SQLInsertType",
 
+    # 关联类型
+    "EnumJoinType", "SQLJoinType",
 
-class SQLEnumJoinType(enum.Enum):
-    """关联类型"""
-    JOIN = "JOIN"  # 内连接
-    INNER_JOIN = "INNER JOIN"  # 内连接
-    LEFT_JOIN = "LEFT JOIN"  # 左外连接
-    LEFT_OUTER_JOIN = "LEFT OUTER JOIN"  # 左外连接
-    RIGHT_JOIN = "RIGHT JOIN"  # 右外连接
-    RIGHT_OUTER_JOIN = "RIGHT OUTER JOIN"  # 右外连接
-    FULL_JOIN = "FULL JOIN"  # 全外连接
-    FULL_OUTER_JOIN = "FULL OUTER JOIN"  # 全外连接
-    CROSS_JOIN = "CROSS JOIN"  # 交叉连接
+    # 排序类型
+    "EnumOrderType", "SQLOrderType",
 
+    # 组合类型
+    "EnumUnionType", "SQLUnionType",
 
-class SQLEnumOrderType(enum.Enum):
-    """排序类型"""
-    ASC = "ASC"  # 升序
-    DESC = "DESC"  # 降序
+    # 比较运算符
+    "EnumCompareOperator", "SQLCompareOperator",
 
+    # 计算运算符
+    "EnumComputeOperator", "SQLComputeOperator",
 
-class SQLEnumCastDataType(enum.Enum):
-    """CAST 函数的字段类型"""
-    CHAR = "CHAR"
-    ENUM = "ENUM"
-    LONGTEXT = "LONGTEXT"
-    MEDIUMTEXT = "MEDIUMTEXT"
-    SET = "SET"
-    TEXT = "TEXT"
-    TINYTEXT = "TINYTEXT"
-    VARCHAR = "VARCHAR"
-    BIT = "BIT"
-    BIGINT = "BIGINT"
-    BOOLEAN = "BOOLEAN"
-    BOOL = "BOOL"
-    DECIMAL = "DECIMAL"
-    DEC = "DEC"
-    DOUBLE = "DOUBLE"
-    INT = "INT"
-    INTEGER = "INTEGER"
-    MEDIUMINT = "MEDIUMINT"
-    REAL = "REAL"
-    SMALLINT = "SMALLINT"
-    TINYINT = "TINYINT"
-    DATE = "DATE"
-    DATETIME = "DATETIME"
-    TIMESTAMP = "TIMESTAMP"
-    TIME = "TIME"
-    YEAR = "YEAR"
-    BOLB = "BOLB"
-    MEDIUMBLOB = "MEDIUMBLOB"
-    LONGBLOB = "LONGBLOB"
-    TINYBLOB = "TINYBLOB"
+    # 逻辑运算符
+    "EnumLogicalOperator", "SQLLogicalOperator",
 
+    # ------------------------------ 一般表达式 ------------------------------
+    # 一般表达式的抽象基类
+    "SQLGeneralExpression",
 
-class SQLEnumUnionType(enum.Enum):
-    """关联类型"""
-    UNION_ALL = ["UNION", "ALL"]
-    UNION = ["UNION"]
-    EXCEPT = ["EXCEPT"]
-    INTERSECT = ["INTERSECT"]
-    MINUS = ["MINUS"]
+    # 一般表达式：字面值表达式
+    "SQLLiteralExpression", "SQLLiteralIntegerExpression", "SQLLiteralFloatExpression", "SQLLiteralStringExpression",
+    "SQLLiteralHexExpression", "SQLLiteralBitExpression", "SQLLiteralBoolExpression", "SQLLiteralNullExpression",
 
+    # 一般表达式：列名表达式
+    "SQLColumnNameExpression",
 
-class SQLInsertType(enum.Enum):
-    """插入类型"""
-    INSERT_INTO = ["INSERT", "INTO"]
-    INSERT_OVERWRITE = ["INSERT", "OVERWRITE"]
+    # 一般表达式：函数表达式
+    "EnumCastDataType", "SQLFunctionExpression", "SQLAggregationFunctionExpression", "SQLCastDataType",
+    "SQLCastFunctionExpression", "SQLExtractFunctionExpression",
+
+    # 一般表达式：布尔值表达式
+    "SQLBoolExpression", "SQLBoolCompareExpression", "SQLBoolIsExpression", "SQLBoolInExpression",
+    "SQLBoolLikeExpression", "SQLBoolExistsExpression", "SQLBoolBetweenExpression",
+
+    # 一般表达式：窗口表达式
+    "SQLWindowExpression",
+
+    # 一般表达式：通配符表达式
+    "SQLWildcardExpression",
+
+    # 一般表达式：条件表达式
+    "SQLConditionExpression",
+
+    # 一般表达式：CASE 表达式
+    "SQLCaseExpression", "SQLCaseValueExpression",
+
+    # 一般表达式：计算表达式
+    "SQLComputeExpression",
+
+    # 一般表达式：值表达式
+    "SQLValueExpression",
+
+    # 一般表达式：子查询表达式
+    "SQLSubQueryExpression",
+
+    # ------------------------------ 专有表达式 ------------------------------
+    # 专有表达式：表名表达式
+    "SQLTableNameExpression",
+
+    # 专有表达式：别名表达式
+    "SQLAlisaExpression",
+
+    # 专有表达式：关联表达式
+    "SQLJoinExpression", "SQLJoinOnExpression", "SQLJoinUsingExpression",
+
+    # 专有表达式：字段类型表达式
+    "SQLColumnTypeExpression",
+
+    # 专有表达式：表表达式
+    "SQLTableExpression",
+
+    # 专有表达式：列表达式
+    "SQLColumnExpression",
+
+    # 专有表达式：等式表达式
+    "SQLEqualExpression",
+
+    # 专有表达式：分区表达式
+    "SQLPartitionExpression",
+
+    # 专有表达式：声明外键表达式
+    "SQLForeignKeyExpression",
+
+    # 专有表达式：声明索引表达式
+    "SQLIndexExpression", "SQLPrimaryIndexExpression", "SQLUniqueIndexExpression", "SQLNormalIndexExpression",
+    "SQLFulltextIndexExpression",
+
+    # 专有表达式：声明字段表达式
+    "SQLDefineColumnExpression",
+
+    # ------------------------------ 子句节点 ------------------------------
+    # 子句节点：SELECT 子句
+    "SQLSelectClause",
+
+    # 子句节点：FROM 子句
+    "SQLFromClause",
+
+    # 子句节点；JOIN 子句
+    "SQLJoinClause",
+
+    # 子句节点：WHERE 子句
+    "SQLWhereClause",
+
+    # 子句节点：GROUP BY 子句
+    "SQLGroupByClause", "SQLNormalGroupByClause", "SQLGroupingSetsGroupByClause",
+
+    # 子句节点：HAVING 子句
+    "SQLHavingClause",
+
+    # 子句节点：ORDER BY 子句
+    "SQLOrderByClause",
+
+    # 子句节点：LIMIT 子句
+    "SQLLimitClause",
+
+    # 子句节点：WITH 子句
+    "SQLWithClause",
+
+    # ------------------------------ 语句节点 ------------------------------
+    # 语句的抽象基类
+    "SQLStatement",
+
+    # SELECT 语句
+    "SQLSelectStatement", "SQLSingleSelectStatement", "SQLUnionSelectStatement",
+
+    # INSERT 语句
+    "SQLInsertStatement", "SQLInsertSelectStatement", "SQLInsertValuesStatement",
+
+    # CREATE TABLE 语句
+    "SQLCreateTableStatement",
+]
+
+
+# ---------------------------------------- 所有 SQL 语句对象节点的抽象基类 ----------------------------------------
 
 
 class SQLBase(abc.ABC):
+    """所有 SQL 语句对象节点的抽象基类
+
+    TODO 待增加 parse 和 check 两个抽象静态方法
+    """
+
     @abc.abstractmethod
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+    def source(self, data_source: DataSource) -> str:
         """返回 SQL 源码
 
         TODO 待将 MySQL 修改为自动指定
         """
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} source={self.source()}>"
+        """
+        TODO 修改 source 生成规则
+        """
+        return f"<{self.__class__.__name__} source={self.source(DataSource.MYSQL)}>"
 
 
-# ------------------------------ 元素层级 ------------------------------
+# ---------------------------------------- 插入类型 ----------------------------------------
 
 
-class SQLComputeOperator(SQLBase, abc.ABC):
-    """计算运算符"""
+class EnumInsertType(enum.Enum):
+    """插入类型的枚举类"""
+    INSERT_INTO = ["INSERT", "INTO"]
+    INSERT_OVERWRITE = ["INSERT", "OVERWRITE"]
 
-    @staticmethod
-    def get_used_column_list() -> List[str]:
-        """获取使用的字段列表"""
-        return []
 
+class SQLInsertType(SQLBase):
+    """插入类型"""
 
-class SQLPlus(SQLComputeOperator):
-    """加法运算符"""
+    def __init__(self, insert_type: EnumInsertType):
+        self._insert_type = insert_type
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "+"
+    @property
+    def insert_type(self) -> EnumInsertType:
+        return self._insert_type
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
+    def source(self, data_source: DataSource) -> str:
+        return " ".join(self.insert_type.value)
 
 
-class SQLSubtract(SQLComputeOperator):
-    """减法运算符"""
+# ---------------------------------------- 关联类型 ----------------------------------------
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "-"
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
+class EnumJoinType(enum.Enum):
+    """关联类型的枚举类"""
+    JOIN = ["JOIN"]  # 内连接
+    INNER_JOIN = ["INNER", "JOIN"]  # 内连接
+    LEFT_JOIN = ["LEFT", "JOIN"]  # 左外连接
+    LEFT_OUTER_JOIN = ["LEFT", "OUTER", "JOIN"]  # 左外连接
+    RIGHT_JOIN = ["RIGHT", "JOIN"]  # 右外连接
+    RIGHT_OUTER_JOIN = ["RIGHT", "OUTER", "JOIN"]  # 右外连接
+    FULL_JOIN = ["FULL", "JOIN"]  # 全外连接
+    FULL_OUTER_JOIN = ["FULL", "OUTER", "JOIN"]  # 全外连接
+    CROSS_JOIN = ["CROSS", "JOIN"]  # 交叉连接
 
 
-class SQLMultiple(SQLComputeOperator):
-    """乘法运算符"""
+class SQLJoinType(SQLBase):
+    """关联类型"""
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "*"
+    def __init__(self, join_type: EnumJoinType):
+        self._join_type = join_type
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
+    @property
+    def join_type(self) -> EnumJoinType:
+        return self._join_type
 
+    def source(self, data_source: DataSource) -> str:
+        return " ".join(self.join_type.value)
 
-class SQLDivide(SQLComputeOperator):
-    """除法运算符"""
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "/"
+# ---------------------------------------- 排序类型 ----------------------------------------
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
 
+class EnumOrderType(enum.Enum):
+    """排序类型的枚举类"""
+    ASC = "ASC"  # 升序
+    DESC = "DESC"  # 降序
 
-class SQLConcat(SQLComputeOperator):
-    """字符串拼接运算符（仅 Oracle、DB2、PostgreSQL 中适用）"""
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "||"
+class SQLOrderType(SQLBase):
+    def __init__(self, order_type: EnumOrderType):
+        self._order_type = order_type
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
+    @property
+    def order_type(self) -> EnumOrderType:
+        return self._order_type
 
+    def source(self, data_source: DataSource) -> str:
+        return self.order_type.value
 
-class SQLCompareOperator(SQLBase, abc.ABC):
-    """比较运算符"""
 
+# ---------------------------------------- 组合类型 ----------------------------------------
 
-class SQLEqualTo(SQLCompareOperator):
-    """等于运算符"""
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "="
+class EnumUnionType(enum.Enum):
+    """组合类型的枚举类"""
+    UNION_ALL = ["UNION", "ALL"]
+    UNION = ["UNION"]
+    EXCEPT = ["EXCEPT"]
+    INTERSECT = ["INTERSECT"]
+    MINUS = ["MINUS"]
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
 
+class SQLUnionType(SQLBase):
+    """组合类型"""
 
-class SQLNotEqualTo(SQLCompareOperator):
-    """不等于运算符：包含 != 和 <> 两种类型"""
+    def __init__(self, union_type: EnumUnionType):
+        self._union_type = union_type
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "!="
+    @property
+    def union_type(self) -> EnumUnionType:
+        return self._union_type
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
+    def source(self, data_source: DataSource) -> str:
+        return " ".join(self.union_type.value)
 
 
-class SQLIs(SQLCompareOperator):
-    """不等于运算符：包含 != 和 <> 两种类型"""
+# ---------------------------------------- 比较运算符 ----------------------------------------
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "IS"
+class EnumCompareOperator(enum.Enum):
+    """比较运算符的枚举类"""
+    EQ = "="
+    EQUAL_TO = "="
+    NEQ = "!="
+    NOT_EQUAL_TO = "!="
+    LT = "<"
+    LESS_THAN = "<"
+    LTE = "<="
+    LESS_THAN_OR_EQUAL = "<="
+    GT = ">"
+    GREATER_THAN = ">"
+    GTE = ">="
+    GREATER_THAN_OR_EQUAL = ">="
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
 
+class SQLCompareOperator(SQLBase):
+    """比较运算符"""
 
-class SQLLessThan(SQLCompareOperator):
-    """小于运算符"""
+    def __init__(self, compare_operator: EnumCompareOperator):
+        self._compare_operator = compare_operator
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "<"
+    @property
+    def compare_operator(self) -> EnumCompareOperator:
+        return self._compare_operator
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
+    def source(self, data_source: DataSource) -> str:
+        return self.compare_operator.value
 
+    @staticmethod
+    def get_used_column_list() -> List[str]:
+        """获取使用的字段列表"""
+        return []
 
-class SQLLessThanOrEqual(SQLCompareOperator):
-    """小于等于运算符"""
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "<="
+# ---------------------------------------- 计算运算符 ----------------------------------------
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
 
+class EnumComputeOperator(enum.Enum):
+    """计算运算符的枚举类"""
+    PLUS = "+"  # 加法运算符
+    SUBTRACT = "-"  # 减法运算符
+    MULTIPLE = "*"  # 乘法运算符
+    DIVIDE = "/"  # 除法运算符
+    MOD = "%"  # 取模运算符
+    CONCAT = "||"  # 字符串拼接运算符（仅 Oracle、DB2、PostgreSQL 中适用）
 
-class SQLGreaterThan(SQLCompareOperator):
-    """大于运算符"""
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return ">"
+class SQLComputeOperator(SQLBase):
+    """计算运算符"""
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
+    def __init__(self, compute_operator: EnumComputeOperator):
+        self._compute_operator = compute_operator
 
+    @property
+    def compute_operator(self) -> EnumComputeOperator:
+        return self._compute_operator
 
-class SQLGreaterThanOrEqual(SQLCompareOperator):
-    """大于等于运算符"""
+    def source(self, data_source: DataSource) -> str:
+        if self.compute_operator == EnumComputeOperator.MOD and data_source != DataSource.SQL_SERVER:
+            raise UnSupportDataSourceError(f"{data_source} 不支持使用 % 运算符")
+        if (self.compute_operator == EnumComputeOperator.CONCAT
+                and data_source not in {DataSource.ORACLE, DataSource.DB2, DataSource.POSTGRE_SQL}):
+            raise UnSupportDataSourceError(f"{data_source} 不支持使用 || 运算符")
+        return self.compute_operator.value
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return ">="
+    @staticmethod
+    def get_used_column_list() -> List[str]:
+        """获取使用的字段列表"""
+        return []
+
+
+# ---------------------------------------- 逻辑运算符 ----------------------------------------
 
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
 
+class EnumLogicalOperator(enum.Enum):
+    """逻辑运算符的枚举类"""
+    AND = "AND"
+    OR = "OR"
+    NOT = "NOT"
 
-class SQLLiteral(SQLBase, abc.ABC):
-    """字面值"""
+
+class SQLLogicalOperator(SQLBase):
+    """逻辑运算符"""
+
+    def __init__(self, logical_operator: EnumLogicalOperator):
+        self._logical_operator = logical_operator
 
     @property
+    def logical_operator(self) -> EnumLogicalOperator:
+        return self._logical_operator
+
+    def source(self, data_source: DataSource) -> str:
+        return self.logical_operator.value
+
+    @staticmethod
+    def get_used_column_list() -> List[str]:
+        """获取使用的字段列表"""
+        return []
+
+
+# ---------------------------------------- 一般表达式的抽象基类 ----------------------------------------
+
+
+class SQLGeneralExpression(SQLBase, abc.ABC):
+    """一般表达式的抽象基类"""
+
     @abc.abstractmethod
-    def value(self):
-        """获取字面值"""
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        """TODO 待移除"""
+
+    @abc.abstractmethod
+    def get_used_column_list(self) -> List[str]:
+        """获取使用的字段列表"""
+
+
+# ---------------------------------------- 字面值表达式 ----------------------------------------
+
+
+class SQLLiteralExpression(SQLGeneralExpression, abc.ABC):
+    """字面值表达式"""
+
+    def as_int(self) -> Optional[int]:
+        """将字面值作为整形返回"""
+        return None
+
+    def as_string(self) -> str:
+        """将字面值作为字符串返回"""
+        return self.source()
+
+    def get_used_column_list(self) -> List[str]:
+        """获取使用的字段列表"""
+        return []
 
 
-class SQLLiteralInteger(SQLLiteral):
+class SQLLiteralIntegerExpression(SQLLiteralExpression):
     """整数字面值"""
 
     def __init__(self, value: int):
         self._value = value
 
     @property
     def value(self) -> int:
         return self._value
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"{self._value}"
+        return f"{self.value}"
+
+    def as_int(self) -> int:
+        return self.value
+
+    def as_string(self) -> str:
+        return f"{self.value}"
 
 
-class SQLLiteralFloat(SQLLiteral):
+class SQLLiteralFloatExpression(SQLLiteralExpression):
     """浮点数字面值"""
 
     def __init__(self, value: float):
         self._value = value
 
     @property
     def value(self) -> float:
         return self._value
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"{self._value}"
+        return f"{self.value}"
 
+    def as_string(self) -> str:
+        return f"{self.value}"
 
-class SQLLiteralString(SQLLiteral):
+
+class SQLLiteralStringExpression(SQLLiteralExpression):
     """字符串字面值"""
 
     def __init__(self, value: str):
         self._value = value
 
     @property
     def value(self) -> str:
         return self._value
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"'{self._value}'"
+        return f"'{self.value}'"
+
+    def as_int(self) -> Optional[int]:
+        if self.value.isdigit():
+            return int(self.value)
+        return None
+
+    def as_string(self) -> Optional[str]:
+        return self.value
 
 
-class SQLLiteralHex(SQLLiteral):
+class SQLLiteralHexExpression(SQLLiteralExpression):
     """十六进制字面值"""
 
     def __init__(self, value: str):
         self._value = value
 
     @property
     def value(self) -> str:
         return self._value
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return f"x'{self._value}'"
 
+    def as_string(self) -> str:
+        return f"{self._value}"
 
-class SQLLiteralBit(SQLLiteral):
+
+class SQLLiteralBitExpression(SQLLiteralExpression):
     """位值字面值"""
 
     def __init__(self, value: str):
         self._value = value
 
     @property
     def value(self) -> str:
         return self._value
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return f"b'{self._value}'"
 
+    def as_string(self) -> str:
+        return f"{self._value}"
+
 
-class SQLLiteralBool(SQLLiteral):
+class SQLLiteralBoolExpression(SQLLiteralExpression):
     """布尔值字面值"""
 
     def __init__(self, value: bool):
         self._value = value
 
     @property
     def value(self) -> bool:
         return self._value
 
+    def as_int(self) -> int:
+        return 1 if self.value is True else 0
+
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return "TRUE" if self._value is True else "FALSE"
 
 
-class SQLLiteralNull(SQLLiteral):
+class SQLLiteralNullExpression(SQLLiteralExpression):
     """空值字面值"""
 
     @property
     def value(self) -> None:
         return None
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return "NULL"
 
 
-class SQLLogicalOperator(SQLBase, abc.ABC):
-    """逻辑运算符"""
-
-    @staticmethod
-    def get_used_column_list() -> List[str]:
-        """获取使用的字段列表"""
-        return []
-
-
-class SQLAndOperator(SQLLogicalOperator):
-    """逻辑 AND 运算符"""
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "AND"
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
-
-
-class SQLOrOperator(SQLLogicalOperator):
-    """逻辑 OR 运算符"""
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "OR"
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
-
-
-class SQLNotOperator(SQLLogicalOperator):
-    """逻辑 NOT 运算符"""
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "OR"
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
-
-
-class SQLUnionKeyword(SQLBase):
-    """复合查询关键字"""
-
-    def __init__(self, union_type: SQLEnumUnionType):
-        self._union_type = union_type
-
-    @property
-    def union_type(self) -> SQLEnumUnionType:
-        return self._union_type
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return " ".join(self._union_type.value)
-
-
-# ------------------------------ 表达式层级（一般表达式） ------------------------------
-
-
-class SQLGeneralExpression(SQLBase, abc.ABC):
-    """一般表达式"""
-
-    @abc.abstractmethod
-    def get_used_column_list(self) -> List[str]:
-        """获取使用的字段列表"""
+# ---------------------------------------- 列名表达式 ----------------------------------------
 
 
 class SQLColumnNameExpression(SQLGeneralExpression):
     """列名表达式"""
 
-    def __init__(self,
-                 table: Optional[str],
-                 column: str):
+    def __init__(self, table: Optional[str], column: str):
         self._table = table
         self._column = column
 
     @property
     def table(self) -> Optional[str]:
         return self._table
 
@@ -430,14 +567,51 @@
             return f"{self.column}"
 
     def get_used_column_list(self) -> List[str]:
         """获取使用的字段列表"""
         return [self.source()]
 
 
+# ---------------------------------------- 函数表达式 ----------------------------------------
+
+
+class EnumCastDataType(enum.Enum):
+    """CAST 函数的字段类型"""
+    CHAR = "CHAR"
+    ENUM = "ENUM"
+    LONGTEXT = "LONGTEXT"
+    MEDIUMTEXT = "MEDIUMTEXT"
+    SET = "SET"
+    TEXT = "TEXT"
+    TINYTEXT = "TINYTEXT"
+    VARCHAR = "VARCHAR"
+    BIT = "BIT"
+    BIGINT = "BIGINT"
+    BOOLEAN = "BOOLEAN"
+    BOOL = "BOOL"
+    DECIMAL = "DECIMAL"
+    DEC = "DEC"
+    DOUBLE = "DOUBLE"
+    INT = "INT"
+    INTEGER = "INTEGER"
+    MEDIUMINT = "MEDIUMINT"
+    REAL = "REAL"
+    SMALLINT = "SMALLINT"
+    TINYINT = "TINYINT"
+    DATE = "DATE"
+    DATETIME = "DATETIME"
+    TIMESTAMP = "TIMESTAMP"
+    TIME = "TIME"
+    YEAR = "YEAR"
+    BOLB = "BOLB"
+    MEDIUMBLOB = "MEDIUMBLOB"
+    LONGBLOB = "LONGBLOB"
+    TINYBLOB = "TINYBLOB"
+
+
 class SQLFunctionExpression(SQLGeneralExpression):
     """函数表达式"""
 
     def __init__(self,
                  schema_name: Optional[str],
                  function_name: str,
                  function_params: List[SQLGeneralExpression]):
@@ -454,18 +628,18 @@
         return self._function_name
 
     @property
     def function_params(self) -> List[SQLGeneralExpression]:
         return self._function_params
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"{self._get_function_str()}({self._get_param_str()})"
+        return f"{self._get_function_str()}({self._get_param_str(data_source)})"
 
-    def _get_param_str(self) -> str:
-        return ", ".join(param.source() for param in self.function_params)
+    def _get_param_str(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        return ", ".join(param.source(data_source) for param in self.function_params)
 
     def _get_function_str(self) -> str:
         if self.schema_name is not None:
             return f"{self.schema_name}.{self.function_name}"
         else:
             return f"{self.function_name}"
 
@@ -489,38 +663,67 @@
 
     @property
     def is_distinct(self) -> bool:
         return self._is_distinct
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         is_distinct = "DISTINCT " if self.is_distinct is True else ""
-        return f"{self._get_function_str()}({is_distinct}{self._get_param_str()})"
+        return f"{self._get_function_str()}({is_distinct}{self._get_param_str(data_source)})"
+
+
+class SQLCastDataType(SQLBase):
+    def __init__(self, signed: bool, data_type: EnumCastDataType, params: Optional[List[SQLGeneralExpression]]):
+        self._signed = signed
+        self._data_type = data_type
+        self._params = params
+
+    @property
+    def signed(self) -> bool:
+        return self._signed
+
+    @property
+    def data_type(self) -> EnumCastDataType:
+        return self._data_type
+
+    @property
+    def params(self) -> Optional[List[SQLGeneralExpression]]:
+        return self._params
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        result = []
+        if self.signed is True:
+            result.append("SIGNED")
+        result.append(self.data_type.value)
+        if self.params is not None:
+            param_str = ", ".join(param.source() for param in self.params)
+            result.append(f"({param_str})")
+        return " ".join(result)
 
 
 class SQLCastFunctionExpression(SQLFunctionExpression):
     """Cast 函数表达式"""
 
     def __init__(self,
                  column_expression: SQLGeneralExpression,
-                 cast_type: "SQLCastDataType"):
+                 cast_type: SQLCastDataType):
         super().__init__(None, "CAST", [])
         self._column_expression = column_expression
         self._cast_type = cast_type
 
     @property
     def function_params(self) -> List[SQLGeneralExpression]:
         # TODO 修改父类继承关系
         raise SqlParseError("SQLCastFunctionExpression.function_params() 方法不允许调用")
 
     @property
     def column_expression(self) -> SQLGeneralExpression:
         return self._column_expression
 
     @property
-    def cast_type(self) -> "SQLCastDataType":
+    def cast_type(self) -> SQLCastDataType:
         return self._cast_type
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return f"{self._get_function_str()}({self.column_expression.source()} AS {self.cast_type.source()})"
 
     def get_used_column_list(self) -> List[str]:
         """获取使用的字段列表"""
@@ -554,299 +757,15 @@
         return f"{self._get_function_str()}({self.extract_name.source()} FROM {self.column_expression.source()})"
 
     def get_used_column_list(self) -> List[str]:
         """获取使用的字段列表"""
         return self.column_expression.get_used_column_list()
 
 
-class SQLCaseExpression(SQLGeneralExpression):
-    """第 1 种格式的 CASE 表达式
-
-    CASE
-        WHEN {条件表达式} THEN {一般表达式}
-        ELSE {一般表达式}
-    END
-    """
-
-    def __init__(self,
-                 cases: List[Tuple["SQLConditionExpression", SQLGeneralExpression]],
-                 else_value: Optional[SQLGeneralExpression]):
-        self._cases = cases
-        self._else_value = else_value
-
-    @property
-    def cases(self) -> List[Tuple["SQLConditionExpression", SQLGeneralExpression]]:
-        return self._cases
-
-    @property
-    def else_value(self) -> Optional[SQLGeneralExpression]:
-        return self._else_value
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        result = ["CASE"]
-        for when, then in self.cases:
-            result.append(f"    WHEN {when.source()} THEN {then.source()}")
-        if self.else_value is not None:
-            result.append(f"    ELSE {self.else_value.source()}")
-        result.append("END")
-        return "\n".join(result)
-
-    def get_used_column_list(self) -> List[str]:
-        """获取使用的字段列表"""
-        result = []
-        for when, _ in self.cases:
-            result.extend(when.get_used_column_list())
-        return result
-
-
-class SQLCaseValueExpression(SQLGeneralExpression):
-    """第 2 种格式的 CASE 表达式
-
-    CASE {一般表达式}
-        WHEN {一般表达式} THEN {一般表达式}
-        ELSE {一般表达式}
-    END
-    """
-
-    def __init__(self,
-                 case_value: SQLGeneralExpression,
-                 cases: List[Tuple[SQLGeneralExpression, SQLGeneralExpression]],
-                 else_value: Optional[SQLGeneralExpression]):
-        self._case_value = case_value
-        self._cases = cases
-        self._else_value = else_value
-
-    @property
-    def case_value(self) -> SQLGeneralExpression:
-        return self._case_value
-
-    @property
-    def cases(self) -> List[Tuple[SQLGeneralExpression, SQLGeneralExpression]]:
-        return self._cases
-
-    @property
-    def else_value(self) -> Optional[SQLGeneralExpression]:
-        return self._else_value
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        result = ["CASE", self.case_value.source()]
-        for when, then in self.cases:
-            result.append(f"    WHEN {when.source()} THEN {then.source()}")
-        if self.else_value is not None:
-            result.append(f"    ELSE {self.else_value.source()}")
-        result.append("END")
-        return "\n".join(result)
-
-    def get_used_column_list(self) -> List[str]:
-        """获取使用的字段列表"""
-        result = self.case_value.get_used_column_list()
-        for when, _ in self.cases:
-            result.extend(when.get_used_column_list())
-        return result
-
-
-class SQLWindowExpression(SQLGeneralExpression):
-    """窗口表达式"""
-
-    def __init__(self,
-                 window_function: SQLFunctionExpression,
-                 partition_by: Optional[SQLGeneralExpression],
-                 order_by: Optional[SQLGeneralExpression]):
-        self._window_function = window_function
-        self._partition_by = partition_by
-        self._order_by = order_by
-
-    @property
-    def window_function(self) -> SQLFunctionExpression:
-        return self._window_function
-
-    @property
-    def partition_by(self) -> Optional[SQLGeneralExpression]:
-        return self._partition_by
-
-    @property
-    def order_by(self) -> Optional[SQLGeneralExpression]:
-        return self._order_by
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        result = f"{self.window_function.source()} OVER ("
-        if self.partition_by is not None:
-            result += f"PARTITION BY {self.partition_by.source()}"
-        if self.order_by is not None:
-            result += f"ORDER BY {self.order_by.source()}"
-        result += ")"
-        return result
-
-    def get_used_column_list(self) -> List[str]:
-        """获取使用的字段列表"""
-        result = []
-        if self.partition_by is not None:
-            result.extend(self.partition_by.get_used_column_list())
-        if self.order_by is not None:
-            result.extend(self.order_by.get_used_column_list())
-        return result
-
-
-class SQLComputeExpression(SQLGeneralExpression):
-    """计算表达式"""
-
-    def __init__(self,
-                 elements: List[Union[SQLGeneralExpression, SQLComputeOperator]]):
-        self._elements = elements
-
-    @property
-    def elements(self) -> List[Union[SQLGeneralExpression, SQLComputeOperator]]:
-        return self._elements
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return " ".join(element.source() for element in self.elements)
-
-    def get_used_column_list(self) -> List[str]:
-        """获取使用的字段列表"""
-        result = []
-        for element in self.elements:
-            result.extend(element.get_used_column_list())
-        return result
-
-
-class SQLLiteralExpression(SQLGeneralExpression):
-    """字面值表达式"""
-
-    def __init__(self, literal: SQLLiteral):
-        self._literal = literal
-
-    def as_int(self) -> int:
-        return int(self.literal.value)
-
-    @property
-    def literal(self) -> SQLLiteral:
-        return self._literal
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return self.literal.source()
-
-    def get_used_column_list(self) -> List[str]:
-        """获取使用的字段列表"""
-        return []
-
-
-class SQLSubQueryExpression(SQLGeneralExpression):
-    """子查询表达式"""
-
-    def __init__(self, select_statement: "SQLSelectStatement"):
-        self._select_statement = select_statement
-
-    @property
-    def select_statement(self) -> "SQLSelectStatement":
-        return self._select_statement
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"({self.select_statement.source()})"
-
-    def get_used_column_list(self) -> List[str]:
-        return self.select_statement.get_select_used_column_list()
-
-    def get_used_table_list(self) -> List[str]:
-        return self.select_statement.get_used_table_list()
-
-
-class SQLWildcardExpression(SQLGeneralExpression):
-    """通配符表达式"""
-
-    def __init__(self, schema: Optional[str]):
-        self._schema = schema
-
-    @property
-    def schema(self) -> Optional[str]:
-        return self._schema
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        if self.schema is not None:
-            return f"{self.schema}.*"
-        else:
-            return "*"
-
-    def get_used_column_list(self) -> List[str]:
-        """获取语句结果中使用的字段"""
-        return [self.source()]
-
-
-class SQLValueExpression(SQLGeneralExpression):
-    """值表达式"""
-
-    def __init__(self, values: List[SQLGeneralExpression]):
-        self._values = values
-
-    @property
-    def values(self) -> List[SQLGeneralExpression]:
-        return self._values
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        values_str = ", ".join(value.source() for value in self.values)
-        return f"({values_str})"
-
-    def get_used_column_list(self) -> List[str]:
-        return []
-
-
-# ------------------------------ 表达式层级（专有表达式） ------------------------------
-
-
-class SQLCastDataType(SQLBase):
-    def __init__(self, signed: bool, data_type: SQLEnumCastDataType, params: Optional[List[SQLGeneralExpression]]):
-        self._signed = signed
-        self._data_type = data_type
-        self._params = params
-
-    @property
-    def signed(self) -> bool:
-        return self._signed
-
-    @property
-    def data_type(self) -> SQLEnumCastDataType:
-        return self._data_type
-
-    @property
-    def params(self) -> Optional[List[SQLGeneralExpression]]:
-        return self._params
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        result = []
-        if self.signed is True:
-            result.append("SIGNED")
-        result.append(self.data_type.value)
-        if self.params is not None:
-            param_str = ", ".join(param.source() for param in self.params)
-            result.append(f"({param_str})")
-        return " ".join(result)
-
-
-class SQLTableNameExpression(SQLBase):
-    """表名表达式"""
-
-    def __init__(self, schema: Optional[str], table: str):
-        self._schema = schema
-        self._table = table
-
-    @property
-    def schema(self) -> Optional[str]:
-        return self._schema
-
-    @property
-    def table(self) -> str:
-        return self._table
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        if self.schema is not None:
-            return f"{self.schema}.{self.table}"
-        else:
-            return f"{self.table}"
-
-    def get_used_table_list(self) -> List[str]:
-        return [self.source()]
+# ---------------------------------------- 布尔值表达式 ----------------------------------------
 
 
 class SQLBoolExpression(SQLBase, abc.ABC):
     """布尔值表达式
 
     TODO 整理子类继承关系
     """
@@ -876,15 +795,17 @@
         return self._before_value
 
     @property
     def after_value(self) -> SQLGeneralExpression:
         return self._after_value
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"{self.before_value.source()} {self.operator.source()} {self.after_value.source()}"
+        return (f"{self.before_value.source(data_source)}"
+                f" {self.operator.source(data_source)} "
+                f"{self.after_value.source(data_source)}")
 
     def get_used_column_list(self) -> List[str]:
         """获取使用的字段列表"""
         return self.before_value.get_used_column_list() + self.after_value.get_used_column_list()
 
 
 class SQLBoolIsExpression(SQLBoolExpression):
@@ -1044,54 +965,321 @@
         return f"{self.before_value.source()} BETWEEN {self.from_value.source()} TO {self.to_value.source()}"
 
     def get_used_column_list(self) -> List[str]:
         """获取使用的字段列表"""
         return self.before_value.get_used_column_list()
 
 
-class SQLAlisaExpression(SQLBase):
-    """别名表达式"""
+# ---------------------------------------- 窗口表达式 ----------------------------------------
 
-    def __init__(self, alias_name: str):
-        self._alias_name = alias_name
+
+class SQLWindowExpression(SQLGeneralExpression):
+    """窗口表达式"""
+
+    def __init__(self,
+                 window_function: SQLFunctionExpression,
+                 partition_by: Optional[SQLGeneralExpression],
+                 order_by: Optional[SQLGeneralExpression]):
+        self._window_function = window_function
+        self._partition_by = partition_by
+        self._order_by = order_by
 
     @property
-    def alias_name(self) -> str:
-        return self._alias_name
+    def window_function(self) -> SQLFunctionExpression:
+        return self._window_function
+
+    @property
+    def partition_by(self) -> Optional[SQLGeneralExpression]:
+        return self._partition_by
+
+    @property
+    def order_by(self) -> Optional[SQLGeneralExpression]:
+        return self._order_by
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"AS {self.alias_name}"
+        result = f"{self.window_function.source()} OVER ("
+        if self.partition_by is not None:
+            result += f"PARTITION BY {self.partition_by.source()}"
+        if self.order_by is not None:
+            result += f"ORDER BY {self.order_by.source()}"
+        result += ")"
+        return result
 
+    def get_used_column_list(self) -> List[str]:
+        """获取使用的字段列表"""
+        result = []
+        if self.partition_by is not None:
+            result.extend(self.partition_by.get_used_column_list())
+        if self.order_by is not None:
+            result.extend(self.order_by.get_used_column_list())
+        return result
+
+
+# ---------------------------------------- 通配符表达式 ----------------------------------------
+
+
+class SQLWildcardExpression(SQLGeneralExpression):
+    """通配符表达式"""
+
+    def __init__(self, schema: Optional[str]):
+        self._schema = schema
+
+    @property
+    def schema(self) -> Optional[str]:
+        return self._schema
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        if self.schema is not None:
+            return f"{self.schema}.*"
+        else:
+            return "*"
+
+    def get_used_column_list(self) -> List[str]:
+        """获取语句结果中使用的字段"""
+        return [self.source()]
+
+
+# ---------------------------------------- 条件表达式 ----------------------------------------
 
 class SQLConditionExpression(SQLGeneralExpression):
     """条件表达式"""
 
     def __init__(self,
                  elements: List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]]):
         self._elements = elements
 
     @property
     def elements(self) -> List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]]:
         return self._elements
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return " ".join(f"({element.source()})" if isinstance(element, SQLConditionExpression) else element.source()
+        return " ".join(f"({element.source(data_source)})"
+                        if isinstance(element, SQLConditionExpression) else element.source(data_source)
                         for element in self._elements)
 
     def get_used_column_list(self) -> List[str]:
         """获取使用的字段列表"""
         result = []
         for element in self.elements:
             result.extend(element.get_used_column_list())
         return result
 
 
+# ---------------------------------------- CASE 表达式 ----------------------------------------
+
+
+class SQLCaseExpression(SQLGeneralExpression):
+    """第 1 种格式的 CASE 表达式
+
+    CASE
+        WHEN {条件表达式} THEN {一般表达式}
+        ELSE {一般表达式}
+    END
+    """
+
+    def __init__(self,
+                 cases: List[Tuple[SQLConditionExpression, SQLGeneralExpression]],
+                 else_value: Optional[SQLGeneralExpression]):
+        self._cases = cases
+        self._else_value = else_value
+
+    @property
+    def cases(self) -> List[Tuple[SQLConditionExpression, SQLGeneralExpression]]:
+        return self._cases
+
+    @property
+    def else_value(self) -> Optional[SQLGeneralExpression]:
+        return self._else_value
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        result = ["CASE"]
+        for when, then in self.cases:
+            result.append(f"    WHEN {when.source(data_source)} THEN {then.source(data_source)}")
+        if self.else_value is not None:
+            result.append(f"    ELSE {self.else_value.source(data_source)}")
+        result.append("END")
+        return "\n".join(result)
+
+    def get_used_column_list(self) -> List[str]:
+        """获取使用的字段列表"""
+        result = []
+        for when, _ in self.cases:
+            result.extend(when.get_used_column_list())
+        return result
+
+
+class SQLCaseValueExpression(SQLGeneralExpression):
+    """第 2 种格式的 CASE 表达式
+
+    CASE {一般表达式}
+        WHEN {一般表达式} THEN {一般表达式}
+        ELSE {一般表达式}
+    END
+    """
+
+    def __init__(self,
+                 case_value: SQLGeneralExpression,
+                 cases: List[Tuple[SQLGeneralExpression, SQLGeneralExpression]],
+                 else_value: Optional[SQLGeneralExpression]):
+        self._case_value = case_value
+        self._cases = cases
+        self._else_value = else_value
+
+    @property
+    def case_value(self) -> SQLGeneralExpression:
+        return self._case_value
+
+    @property
+    def cases(self) -> List[Tuple[SQLGeneralExpression, SQLGeneralExpression]]:
+        return self._cases
+
+    @property
+    def else_value(self) -> Optional[SQLGeneralExpression]:
+        return self._else_value
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        result = ["CASE", self.case_value.source()]
+        for when, then in self.cases:
+            result.append(f"    WHEN {when.source(data_source)} THEN {then.source(data_source)}")
+        if self.else_value is not None:
+            result.append(f"    ELSE {self.else_value.source(data_source)}")
+        result.append("END")
+        return "\n".join(result)
+
+    def get_used_column_list(self) -> List[str]:
+        """获取使用的字段列表"""
+        result = self.case_value.get_used_column_list()
+        for when, _ in self.cases:
+            result.extend(when.get_used_column_list())
+        return result
+
+
+# ---------------------------------------- 计算表达式 ----------------------------------------
+
+class SQLComputeExpression(SQLGeneralExpression):
+    """计算表达式"""
+
+    def __init__(self,
+                 elements: List[Union[SQLGeneralExpression, SQLComputeOperator]]):
+        self._elements = elements
+
+    @property
+    def elements(self) -> List[Union[SQLGeneralExpression, SQLComputeOperator]]:
+        return self._elements
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        return " ".join(element.source(data_source) for element in self.elements)
+
+    def get_used_column_list(self) -> List[str]:
+        """获取使用的字段列表"""
+        result = []
+        for element in self.elements:
+            result.extend(element.get_used_column_list())
+        return result
+
+
+# ---------------------------------------- 值表达式 ----------------------------------------
+
+
+class SQLValueExpression(SQLGeneralExpression):
+    """值表达式"""
+
+    def __init__(self, values: List[SQLGeneralExpression]):
+        self._values = values
+
+    @property
+    def values(self) -> List[SQLGeneralExpression]:
+        return self._values
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        values_str = ", ".join(value.source() for value in self.values)
+        return f"({values_str})"
+
+    def get_used_column_list(self) -> List[str]:
+        return []
+
+
+# ---------------------------------------- 子查询表达式 ----------------------------------------
+
+
+class SQLSubQueryExpression(SQLGeneralExpression):
+    """子查询表达式"""
+
+    def __init__(self, select_statement: "SQLSelectStatement"):
+        self._select_statement = select_statement
+
+    @property
+    def select_statement(self) -> "SQLSelectStatement":
+        return self._select_statement
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        return f"({self.select_statement.source()})"
+
+    def get_used_column_list(self) -> List[str]:
+        return self.select_statement.get_select_used_column_list()
+
+    def get_used_table_list(self) -> List[str]:
+        return self.select_statement.get_used_table_list()
+
+
+# ---------------------------------------- 表名表达式 ----------------------------------------
+
+
+class SQLTableNameExpression(SQLBase):
+    """表名表达式"""
+
+    def __init__(self, schema: Optional[str], table: str):
+        self._schema = schema
+        self._table = table
+
+    @property
+    def schema(self) -> Optional[str]:
+        return self._schema
+
+    @property
+    def table(self) -> str:
+        return self._table
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        if self.schema is not None:
+            return f"{self.schema}.{self.table}"
+        else:
+            return f"{self.table}"
+
+    def get_used_table_list(self) -> List[str]:
+        return [self.source()]
+
+
+# ---------------------------------------- 别名表达式 ----------------------------------------
+
+
+class SQLAlisaExpression(SQLBase):
+    """别名表达式"""
+
+    def __init__(self, alias_name: str):
+        self._alias_name = alias_name
+
+    @property
+    def alias_name(self) -> str:
+        return self._alias_name
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        return f"AS {self.alias_name}"
+
+
+# ---------------------------------------- 关联表达式 ----------------------------------------
+
+
 class SQLJoinExpression(SQLBase, abc.ABC):
     """关联表达式"""
 
+    @abc.abstractmethod
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        pass  # TODO 待移除
+
 
 class SQLJoinOnExpression(SQLJoinExpression):
     """ON 关联表达式"""
 
     def __init__(self, condition: SQLConditionExpression):
         self._condition = condition
 
@@ -1113,14 +1301,42 @@
     def using_function(self) -> SQLFunctionExpression:
         return self._using_function
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return f"{self.using_function.source()}"
 
 
+# ---------------------------------------- 字段类型表达式 ----------------------------------------
+
+class SQLColumnTypeExpression(SQLBase):
+    """字段类型表达式"""
+
+    def __init__(self, name: str, params: List[SQLGeneralExpression]):
+        self._name = name  # 函数名称
+        self._params = params  # 函数参数
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def params(self) -> List[SQLGeneralExpression]:
+        return self._params
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        if len(self.params) == 0 or data_source == DataSource.HIVE:
+            return self.name
+        else:
+            type_params = "(" + ", ".join([param.source() for param in self.params]) + ")"
+            return f"{self.name}{type_params}"
+
+
+# ---------------------------------------- 表表达式 ----------------------------------------
+
+
 class SQLTableExpression(SQLBase):
     """表表达式"""
 
     def __init__(self,
                  table: Union[SQLTableNameExpression, SQLSubQueryExpression],
                  alias: Optional[SQLAlisaExpression]):
         self._table = table
@@ -1140,14 +1356,17 @@
         else:
             return f"{self.table.source()}"
 
     def get_used_table_list(self) -> List[str]:
         return self.table.get_used_table_list()
 
 
+# ---------------------------------------- 列表达式 ----------------------------------------
+
+
 class SQLColumnExpression(SQLBase):
     """列表达式"""
 
     def __init__(self,
                  column: SQLGeneralExpression,
                  alias: Optional[SQLAlisaExpression]):
         self._column = column
@@ -1159,29 +1378,32 @@
 
     @property
     def alias(self) -> Optional[SQLAlisaExpression]:
         return self._alias
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         if self.alias is not None:
-            return f"{self.column.source()} {self.alias.source()}"
+            return f"{self.column.source(data_source)} {self.alias.source()}"
         else:
-            return f"{self.column.source()}"
+            return f"{self.column.source(data_source)}"
 
     def get_alias_name(self) -> Optional[str]:
         """获取别名名称"""
         if self.alias is not None:
             return self.alias.alias_name
         return None
 
     def get_used_column_list(self) -> List[str]:
         """获取语句结果中使用的字段"""
         return self.column.get_used_column_list()
 
 
+# ---------------------------------------- 等式表达式 ----------------------------------------
+
+
 class SQLEqualExpression(SQLBase):
     """等式表达式"""
 
     def __init__(self, before_value: SQLGeneralExpression, after_value: SQLGeneralExpression):
         self._before_value = before_value
         self._after_value = after_value
 
@@ -1193,14 +1415,17 @@
     def after_value(self) -> SQLGeneralExpression:
         return self._after_value
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return f"{self.before_value.source()} = {self.after_value.source()}"
 
 
+# ---------------------------------------- 分区表达式 ----------------------------------------
+
+
 class SQLPartitionExpression(SQLBase):
     """分区表达式：PARTITION (<partition_expression>)"""
 
     def __init__(self, partition_list: List[SQLEqualExpression]):
         self._partition_list = partition_list
 
     @property
@@ -1208,15 +1433,206 @@
         return self._partition_list
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         partition_list_str = ", ".join(partition.source() for partition in self.partition_list)
         return f"PARTITION ({partition_list_str})"
 
 
-# ------------------------------ 子句层级 ------------------------------
+# ---------------------------------------- 声明外键表达式 ----------------------------------------
+
+
+class SQLForeignKeyExpression(SQLBase):
+    """声明外键表达式"""
+
+    def __init__(self, constraint_name: str, slave_columns: List[str], master_table_name: str,
+                 master_columns: List[str]):
+        """
+
+        Parameters
+        ----------
+        constraint_name : str
+            外键约束名称
+        slave_columns : List[str]
+            从表的字段
+        master_table_name : str
+            主表名称
+        master_columns : List[str]
+            主表的字段名
+        """
+        self.constraint_name = constraint_name
+        self.slave_columns = slave_columns
+        self.master_table_name = master_table_name
+        self.master_columns = master_columns
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        slave_columns_str = ", ".join([f"{column}" for column in self.slave_columns])
+        master_columns_str = ", ".join([f"{column}" for column in self.master_columns])
+        return (f"CONSTRAINT {self.constraint_name} FOREIGN KEY({slave_columns_str}) "
+                f"REFERENCES {self.master_table_name}({master_columns_str})")
+
+
+# ---------------------------------------- 声明索引表达式 ----------------------------------------
+
+
+class SQLIndexExpression(SQLBase, abc.ABC):
+    """声明索引表达式"""
+
+    def __init__(self, name: Optional[str], columns: List[str]):
+        self._name = name
+        self._columns = columns
+
+    @property
+    def name(self) -> Optional[str]:
+        return self._name
+
+    @property
+    def columns(self) -> List[str]:
+        return self._columns
+
+
+class SQLPrimaryIndexExpression(SQLIndexExpression):
+    """主键索引声明表达式"""
+
+    def __init__(self, columns: List[str]):
+        super().__init__(None, columns)
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        columns_str = ", ".join([f"{column}" for column in self.columns])
+        return f"PRIMARY KEY ({columns_str})" if self.columns is not None else ""
+
+
+class SQLUniqueIndexExpression(SQLIndexExpression):
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        columns_str = ", ".join([f"{column}" for column in self.columns])
+        return f"UNIQUE KEY {self.name} ({columns_str})"
+
+
+class SQLNormalIndexExpression(SQLIndexExpression):
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        columns_str = ", ".join([f"{column}" for column in self.columns])
+        return f"KEY {self.name} ({columns_str})"
+
+
+class SQLFulltextIndexExpression(SQLIndexExpression):
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        columns_str = ", ".join([f"{column}" for column in self.columns])
+        return f"FULLTEXT KEY {self.name} ({columns_str})"
+
+
+# ---------------------------------------- 声明字段表达式 ----------------------------------------
+
+
+class SQLDefineColumnExpression(SQLBase):
+    """声明字段表达式"""
+
+    def __init__(self,
+                 column_name: str,
+                 column_type: SQLColumnTypeExpression,
+                 comment: Optional[str] = None,
+                 is_unsigned: bool = False,
+                 is_zerofill: bool = False,
+                 character_set: Optional[str] = None,
+                 collate: Optional[str] = None,
+                 is_allow_null: bool = False,
+                 is_not_null: bool = False,
+                 is_auto_increment: bool = False,
+                 default: Optional[SQLGeneralExpression] = None,
+                 on_update: Optional[SQLGeneralExpression] = None
+                 ):
+        self._column_name = column_name.strip("`")
+        self._column_type = column_type
+        self._comment = comment
+        self._is_unsigned = is_unsigned
+        self._is_zerofill = is_zerofill
+        self._character_set = character_set
+        self._collate = collate
+        self._is_allow_null = is_allow_null  # 是否显式地允许 NULL 值
+        self._is_not_null = is_not_null
+        self._is_auto_increment = is_auto_increment
+        self._default = default
+        self._on_update = on_update
+
+    @property
+    def column_name(self) -> str:
+        return f"`{self._column_name}`"
+
+    @property
+    def column_name_without_quote(self) -> str:
+        return self._column_name
+
+    @property
+    def column_type(self) -> SQLColumnTypeExpression:
+        return self._column_type
+
+    @property
+    def comment(self) -> Optional[str]:
+        return self._comment
+
+    @property
+    def is_unsigned(self) -> bool:
+        return self._is_unsigned
+
+    @property
+    def is_zerofill(self) -> bool:
+        return self._is_zerofill
+
+    @property
+    def character_set(self) -> Optional[str]:
+        return self._character_set
+
+    @property
+    def collate(self) -> Optional[str]:
+        return self._collate
+
+    @property
+    def is_allow_null(self) -> bool:
+        return self._is_allow_null
+
+    @property
+    def is_not_null(self) -> bool:
+        return self._is_not_null
+
+    @property
+    def is_auto_increment(self) -> bool:
+        return self._is_auto_increment
+
+    @property
+    def default(self) -> Optional[SQLGeneralExpression]:
+        return self._default
+
+    @property
+    def on_update(self) -> Optional[SQLGeneralExpression]:
+        return self._on_update
+
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        res = f"{self._column_name} {self.column_type.source(data_source)}"
+        if self.is_unsigned is True and data_source == DataSource.MYSQL:
+            res += " UNSIGNED"
+        if self.is_zerofill is True and data_source == DataSource.MYSQL:
+            res += " ZEROFILL"
+        if self.character_set is not None and data_source == DataSource.MYSQL:
+            res += f" CHARACTER SET {self.character_set}"
+        if self.collate is not None and data_source == DataSource.MYSQL:
+            res += f" COLLATE {self.collate}"
+        if self.is_allow_null is True and data_source == DataSource.MYSQL:
+            res += " NULL"
+        if self.is_not_null is True and data_source == DataSource.MYSQL:
+            res += " NOT NULL"
+        if self.is_auto_increment is True and data_source == DataSource.MYSQL:
+            res += " AUTO_INCREMENT"
+        if self.default is not None and data_source == DataSource.MYSQL:
+            res += f" DEFAULT {self.default.source()}"
+        if self.on_update is not None and data_source == DataSource.MYSQL:
+            res += f" ON UPDATE {self.on_update.source()}"
+        if self.comment is not None:
+            res += f" COMMENT {self.comment}"
+        return res
+
+
+# ---------------------------------------- SELECT 子句 ----------------------------------------
 
 
 class SQLSelectClause(SQLBase):
     """SELECT 子句"""
 
     def __init__(self, distinct: bool, columns: List[SQLColumnExpression]):
         self._distinct = distinct
@@ -1230,15 +1646,15 @@
     def columns(self) -> List[SQLColumnExpression]:
         return self._columns
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         result = ["SELECT"]
         if self.distinct is True:
             result.append("DISTINCT")
-        result.append(",\n".join(column.source() for column in self.columns))
+        result.append(",\n".join(column.source(data_source) for column in self.columns))
         return " ".join(result)
 
     def get_used_column_list(self) -> List[str]:
         """获取语句结果中使用的字段的列表"""
         result = []
         for column in self.columns:
             result.extend(column.get_used_column_list())
@@ -1254,14 +1670,16 @@
     def get_index_to_used_column_hash(self) -> Dict[int, List[str]]:
         result = {}
         for idx, column in enumerate(self.columns):
             result[idx + 1] = column.get_used_column_list()  # 列编号从 1 开始
         return result
 
 
+# ---------------------------------------- FROM 子句 ----------------------------------------
+
 class SQLFromClause(SQLBase):
     """FROM 子句"""
 
     def __init__(self, tables: List[SQLTableExpression]):
         self._tables = tables
 
     @property
@@ -1275,47 +1693,52 @@
         """获取语句中查询的表名的列表"""
         result = []
         for table in self.tables:
             result.extend(table.get_used_table_list())
         return result
 
 
+# ---------------------------------------- JOIN 子句 ----------------------------------------
+
 class SQLJoinClause(SQLBase):
     """JOIN 子句"""
 
     def __init__(self,
-                 join_type: SQLEnumJoinType,
+                 join_type: SQLJoinType,
                  table: SQLTableExpression,
                  join_rule: Optional[SQLJoinExpression]):
         self._join_type = join_type
         self._table = table
         self._join_rule = join_rule
 
     @property
-    def join_type(self) -> SQLEnumJoinType:
+    def join_type(self) -> SQLJoinType:
         return self._join_type
 
     @property
     def table(self) -> SQLTableExpression:
         return self._table
 
     @property
     def join_rule(self) -> Optional[SQLJoinExpression]:
         return self._join_rule
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         if self.join_rule is not None:
-            return f"{self.join_type.value} {self.table.source()} {self.join_rule.source()}"
+            return f"{self.join_type.source(data_source)} {self.table.source()} {self.join_rule.source()}"
         else:
-            return f"{self.join_type.value} {self.table.source()}"
+            return f"{self.join_type.source(data_source)} {self.table.source()}"
 
     def get_used_table_list(self) -> List[str]:
         return self.table.get_used_table_list()
 
 
+# ---------------------------------------- WHERE 子句 ----------------------------------------
+
+
 class SQLWhereClause(SQLBase):
     """WHERE 子句"""
 
     def __init__(self, condition: SQLConditionExpression):
         self._condition = condition
 
     @property
@@ -1326,14 +1749,16 @@
         return f"WHERE {self.condition.source()}"
 
     def get_used_column_list(self) -> List[str]:
         """获取使用的字段名列表"""
         return self.condition.get_used_column_list()
 
 
+# ---------------------------------------- GROUP BY 子句 ----------------------------------------
+
 class SQLGroupByClause(SQLBase, abc.ABC):
     """GROUP BY 子句"""
 
     @abc.abstractmethod
     def get_used_column_list(self) -> List[Union[str, int]]:
         """返回字段名和列编号"""
 
@@ -1360,15 +1785,15 @@
             return "GROUP BY " + ", ".join(column.source() for column in self.columns)
 
     def get_used_column_list(self) -> List[Union[str, int]]:
         """返回字段名和列编号"""
         result = []
         for column in self.columns:
             if isinstance(column, SQLLiteralExpression):
-                result.append(column.literal.value)  # 列编号
+                result.append(column.as_int())  # 列编号
             else:
                 result.extend(column.get_used_column_list())
         return result
 
 
 class SQLGroupingSetsGroupByClause(SQLGroupByClause):
     """使用 GROUPING SETS 语法的 GROUP BY 子句"""
@@ -1391,20 +1816,23 @@
 
     def get_used_column_list(self) -> List[Union[str, int]]:
         """返回字段名和列编号"""
         result = []
         for grouping in self.grouping_list:
             for column in grouping:
                 if isinstance(column, SQLLiteralExpression):
-                    result.append(column.literal.value)  # 列编号
+                    result.append(column.as_int())  # 列编号
                 else:
                     result.extend(column.get_used_column_list())
         return result
 
 
+# ---------------------------------------- HAVING 子句 ----------------------------------------
+
+
 class SQLHavingClause(SQLBase):
     """HAVING 子句"""
 
     def __init__(self, condition: SQLConditionExpression):
         self._condition = condition
 
     @property
@@ -1414,44 +1842,50 @@
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return f"HAVING {self.condition.source()}"
 
     def get_used_column_list(self) -> List[str]:
         return self.condition.get_used_column_list()
 
 
+# ---------------------------------------- ORDER BY 子句 ----------------------------------------
+
+
 class SQLOrderByClause(SQLBase):
     """ORDER BY 子句"""
 
-    def __init__(self, columns: List[Tuple[SQLGeneralExpression, SQLEnumOrderType]]):
+    def __init__(self, columns: List[Tuple[SQLGeneralExpression, SQLOrderType]]):
         self._columns = columns
 
     @property
-    def columns(self) -> List[Tuple[SQLGeneralExpression, SQLEnumOrderType]]:
+    def columns(self) -> List[Tuple[SQLGeneralExpression, SQLOrderType]]:
         return self._columns
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         result = []
         for column, order_type in self.columns:
-            if order_type == SQLEnumOrderType.ASC:
+            if order_type.source == "ASC":
                 result.append(f"{column.source()}")
             else:
                 result.append(f"{column.source()} DESC")
         return "ORDER BY " + ", ".join(result)
 
     def get_used_column_list(self) -> List[Union[str, int]]:
         """返回字段名和列编号"""
         result = []
         for column, order_type in self.columns:
             if isinstance(column, SQLLiteralExpression):
-                result.append(column.literal.value)  # 列编号
+                result.append(column.as_int())  # 列编号
             else:
                 result.extend(column.get_used_column_list())
         return result
 
 
+# ---------------------------------------- LIMIT 子句 ----------------------------------------
+
+
 class SQLLimitClause(SQLBase):
     """LIMIT 子句"""
 
     def __init__(self, limit: int, offset: int):
         self._limit = limit
         self._offset = offset
 
@@ -1463,14 +1897,17 @@
     def offset(self) -> int:
         return self._offset
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         return f"LIMIT {self.offset}, {self.limit}"
 
 
+# ---------------------------------------- WITH 子句 ----------------------------------------
+
+
 class SQLWithClause(SQLBase):
     """WITH 子句"""
 
     def __init__(self, tables: List[Tuple[str, "SQLSelectStatement"]]):
         self._tables = tables
 
     @staticmethod
@@ -1490,30 +1927,38 @@
         else:
             return ""
 
     def is_empty(self):
         return len(self.tables) == 0
 
 
-# ------------------------------ 语句层级 ------------------------------
+# ---------------------------------------- 语句的抽象基类 ----------------------------------------
 
 
 class SQLStatement(SQLBase, abc.ABC):
-    """表达式的抽象基类"""
+    """语句的抽象基类"""
 
     def __init__(self, with_clause: Optional[SQLWithClause]):
         self._with_clause = with_clause
 
     @property
     def with_clause(self) -> Optional[SQLWithClause]:
         return self._with_clause
 
 
+# ---------------------------------------- SELECT 语句 ----------------------------------------
+
+
 class SQLSelectStatement(SQLStatement, abc.ABC):
-    """SELECT 表达式"""
+    """SELECT 语句"""
+
+    @abc.abstractmethod
+    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
+        """TODO 待移除"""
+        pass
 
     @abc.abstractmethod
     def get_from_used_table_list(self) -> List[str]:
         """获取 FROM 语句中使用的表名的列表"""
 
     @abc.abstractmethod
     def get_join_used_table_list(self) -> List[str]:
@@ -1603,15 +2048,15 @@
 
     @property
     def limit_clause(self) -> Optional[SQLLimitClause]:
         return self._limit_clause
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         with_clause_str = self.with_clause.source() + "\n" if not self.with_clause.is_empty() else ""
-        result = [self.select_clause.source()]
+        result = [self.select_clause.source(data_source)]
         for clause in [self.from_clause, *self.join_clauses, self.where_clause, self.group_by_clause,
                        self.having_clause,
                        self.order_by_clause, self.limit_clause]:
             if clause is not None:
                 result.append(clause.source())
         return with_clause_str + "\n".join(result)
 
@@ -1685,25 +2130,25 @@
     """复合查询语句，使用 UNION、EXCEPT、INTERSECT 进行组合
 
     TODO 移除表达式中直接引用枚举类的行为，外面必须套一层表达式
     """
 
     def __init__(self,
                  with_clause: Optional[SQLWithClause],
-                 elements: List[Union[SQLUnionKeyword, SQLSingleSelectStatement]]):
+                 elements: List[Union[SQLUnionType, SQLSingleSelectStatement]]):
         super().__init__(with_clause)
         self._elements = elements
 
     @property
-    def elements(self) -> List[Union[SQLUnionKeyword, SQLSingleSelectStatement]]:
+    def elements(self) -> List[Union[SQLUnionType, SQLSingleSelectStatement]]:
         return self._elements
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         with_clause_str = self.with_clause.source() + "\n" if not self.with_clause.is_empty() else ""
-        return with_clause_str + "\n".join(element.source() for element in self.elements)
+        return with_clause_str + "\n".join(element.source(data_source) for element in self.elements)
 
     def get_from_used_table_list(self) -> List[str]:
         """获取 FROM 语句中使用的表名的列表"""
         result = []
         for element in self.elements:
             if isinstance(element, SQLSingleSelectStatement):
                 result.extend(element.get_from_used_table_list())
@@ -1753,14 +2198,17 @@
         result = []
         for element in self.elements:
             if isinstance(element, SQLSingleSelectStatement):
                 result.extend(element.get_order_by_used_column_list())
         return ordered_distinct(result)
 
 
+# ---------------------------------------- INSERT 语句 ----------------------------------------
+
+
 class SQLInsertStatement(SQLStatement, abc.ABC):
     """INSERT 表达式
 
     两个子类包含 VALUES 和 SELECT 两种方式
 
     INSERT {INTO|OVERWRITE} [TABLE] <table_name_expression> [PARTITION (<partition_expression>)]
     [(<colum_name_expression [,<column_name_expression> ...]>)]
@@ -1797,17 +2245,17 @@
     def partition(self) -> SQLPartitionExpression:
         return self._partition
 
     @property
     def columns(self) -> Optional[List[SQLColumnExpression]]:
         return self._columns
 
-    def _insert_str(self) -> str:
+    def _insert_str(self, data_source: DataSource) -> str:
         """INSERT语句的前半部分"""
-        insert_type_str = " ".join(self.insert_type.value)
+        insert_type_str = self.insert_type.source(data_source)
         table_keyword_str = "TABLE " if self.has_table_keyword else ""
         partition_str = self.partition.source() + " " if self.partition is not None else ""
         if self.columns is not None:
             columns_str = "(" + ", ".join(column.source() for column in self.columns) + ") "
         else:
             columns_str = ""
         return f"{insert_type_str} {table_keyword_str}{self.table_name.source()} {partition_str}{columns_str}"
@@ -1829,15 +2277,15 @@
 
     @property
     def values(self) -> List[SQLValueExpression]:
         return self._values
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
         values_str = ", ".join(value.source() for value in self.values)
-        return f"{self._insert_str()}VALUES {values_str}"
+        return f"{self._insert_str(data_source)}VALUES {values_str}"
 
 
 class SQLInsertSelectStatement(SQLInsertStatement):
     """INSERT ... SELECT ... 语句"""
 
     def __init__(self,
                  with_clause: Optional[SQLWithClause],
@@ -1851,257 +2299,41 @@
         self._select_statement = select_statement
 
     @property
     def select_statement(self) -> SQLSelectStatement:
         return self._select_statement
 
     def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return f"{self._insert_str()} {self.select_statement.source()}"
-
-
-# ---------- 仅在部分 SQL 语言中使用的节点 ----------
-
-class SQLMod(SQLComputeOperator):
-    """取模运算符（仅 SQL Server 中适用）"""
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        return "%"
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>"
-
-
-# ---------- DDL 中使用的节点 ----------
-
-class DDLColumnTypeExpression(SQLBase):
-    """字段类型表达式"""
-
-    def __init__(self, name: str, params: List[SQLGeneralExpression]):
-        self._name = name  # 函数名称
-        self._params = params  # 函数参数
-
-    @property
-    def name(self) -> str:
-        return self._name
+        return f"{self._insert_str(data_source)} {self.select_statement.source(data_source)}"
 
-    @property
-    def params(self) -> List[SQLGeneralExpression]:
-        return self._params
 
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        if len(self.params) > 0:
-            type_params = "(" + ", ".join([param.source() for param in self.params]) + ")"
-            return f"{self.name}{type_params}"
-        else:
-            return self.name
-
-
-class DDLForeignKeyExpression(SQLBase):
-    """外键表达式"""
-
-    def __init__(self, constraint_name: str, slave_columns: List[str], master_table_name: str,
-                 master_columns: List[str]):
-        """
-
-        Parameters
-        ----------
-        constraint_name : str
-            外键约束名称
-        slave_columns : List[str]
-            从表的字段
-        master_table_name : str
-            主表名称
-        master_columns : List[str]
-            主表的字段名
-        """
-        self.constraint_name = constraint_name
-        self.slave_columns = slave_columns
-        self.master_table_name = master_table_name
-        self.master_columns = master_columns
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        slave_columns_str = ", ".join([f"{column}" for column in self.slave_columns])
-        master_columns_str = ", ".join([f"{column}" for column in self.master_columns])
-        return (f"CONSTRAINT {self.constraint_name} FOREIGN KEY({slave_columns_str}) "
-                f"REFERENCES {self.master_table_name}({master_columns_str})")
-
-
-class DDLIndexExpression(SQLBase, abc.ABC):
-    """声明索引表达式"""
-
-    def __init__(self, name: Optional[str], columns: List[str]):
-        self._name = name
-        self._columns = columns
-
-    @property
-    def name(self) -> Optional[str]:
-        return self._name
-
-    @property
-    def columns(self) -> List[str]:
-        return self._columns
-
-
-class DDLPrimaryIndexExpression(DDLIndexExpression):
-    """主键索引声明表达式"""
-
-    def __init__(self, columns: List[str]):
-        super().__init__(None, columns)
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        columns_str = ", ".join([f"{column}" for column in self.columns])
-        return f"PRIMARY KEY ({columns_str})" if self.columns is not None else ""
-
-
-class DDLUniqueIndexExpression(DDLIndexExpression):
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        columns_str = ", ".join([f"{column}" for column in self.columns])
-        return f"UNIQUE KEY {self.name} ({columns_str})"
-
-
-class DDLNormalIndexExpression(DDLIndexExpression):
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        columns_str = ", ".join([f"{column}" for column in self.columns])
-        return f"KEY {self.name} ({columns_str})"
-
-
-class DDLFulltextIndexExpression(DDLIndexExpression):
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        columns_str = ", ".join([f"{column}" for column in self.columns])
-        return f"FULLTEXT KEY {self.name} ({columns_str})"
-
-
-class DDLColumnExpression(SQLBase):
-    """【DDL】建表语句中的字段信息"""
-
-    def __init__(self,
-                 column_name: str,
-                 column_type: DDLColumnTypeExpression,
-                 comment: Optional[str] = None,
-                 is_unsigned: bool = False,
-                 is_zerofill: bool = False,
-                 character_set: Optional[str] = None,
-                 collate: Optional[str] = None,
-                 is_allow_null: bool = False,
-                 is_not_null: bool = False,
-                 is_auto_increment: bool = False,
-                 default: Optional[SQLGeneralExpression] = None,
-                 on_update: Optional[SQLGeneralExpression] = None
-                 ):
-        self._column_name = column_name.strip("`")
-        self._column_type = column_type
-        self._comment = comment
-        self._is_unsigned = is_unsigned
-        self._is_zerofill = is_zerofill
-        self._character_set = character_set
-        self._collate = collate
-        self._is_allow_null = is_allow_null  # 是否显式地允许 NULL 值
-        self._is_not_null = is_not_null
-        self._is_auto_increment = is_auto_increment
-        self._default = default
-        self._on_update = on_update
-
-    @property
-    def column_name(self) -> str:
-        return f"`{self._column_name}`"
-
-    @property
-    def column_name_without_quote(self) -> str:
-        return self._column_name
-
-    @property
-    def column_type(self) -> DDLColumnTypeExpression:
-        return self._column_type
-
-    @property
-    def comment(self) -> Optional[str]:
-        return self._comment
-
-    @property
-    def is_unsigned(self) -> bool:
-        return self._is_unsigned
-
-    @property
-    def is_zerofill(self) -> bool:
-        return self._is_zerofill
-
-    @property
-    def character_set(self) -> Optional[str]:
-        return self._character_set
-
-    @property
-    def collate(self) -> Optional[str]:
-        return self._collate
-
-    @property
-    def is_allow_null(self) -> bool:
-        return self._is_allow_null
-
-    @property
-    def is_not_null(self) -> bool:
-        return self._is_not_null
-
-    @property
-    def is_auto_increment(self) -> bool:
-        return self._is_auto_increment
-
-    @property
-    def default(self) -> Optional[SQLGeneralExpression]:
-        return self._default
-
-    @property
-    def on_update(self) -> Optional[SQLGeneralExpression]:
-        return self._on_update
-
-    def source(self, data_source: DataSource = DataSource.MYSQL) -> str:
-        res = f"{self._column_name} {self.column_type.source()}"
-        if self.is_unsigned is True and data_source == DataSource.MYSQL:
-            res += " UNSIGNED"
-        if self.is_zerofill is True and data_source == DataSource.MYSQL:
-            res += " ZEROFILL"
-        if self.character_set is not None and data_source == DataSource.MYSQL:
-            res += f" CHARACTER SET {self.character_set}"
-        if self.collate is not None and data_source == DataSource.MYSQL:
-            res += f" COLLATE {self.collate}"
-        if self.is_allow_null is True and data_source == DataSource.MYSQL:
-            res += " NULL"
-        if self.is_not_null is True and data_source == DataSource.MYSQL:
-            res += " NOT NULL"
-        if self.is_auto_increment is True and data_source == DataSource.MYSQL:
-            res += " AUTO_INCREMENT"
-        if self.default is not None and data_source == DataSource.MYSQL:
-            res += f" DEFAULT {self.default.source()}"
-        if self.on_update is not None and data_source == DataSource.MYSQL:
-            res += f" ON UPDATE {self.on_update.source()}"
-        if self.comment is not None:
-            res += f" COMMENT {self.comment}"
-        return res
+# ---------------------------------------- CREATE TABLE 语句 ----------------------------------------
 
 
-class DDLCreateTableStatement(SQLBase):
+class SQLCreateTableStatement(SQLBase):
     """【DDL】CREATE TABLE 语句"""
 
     def __init__(self,
                  schema_name: Optional[str] = None,
                  table_name: Optional[str] = None,
                  comment: Optional[str] = None,
                  if_not_exists: bool = False,
-                 columns: Optional[List[DDLColumnExpression]] = None,
-                 primary_key: Optional[DDLPrimaryIndexExpression] = None,
-                 unique_key: Optional[List[DDLUniqueIndexExpression]] = None,
-                 key: Optional[List[DDLNormalIndexExpression]] = None,
-                 fulltext_key: Optional[List[DDLFulltextIndexExpression]] = None,
-                 foreign_key: List[DDLForeignKeyExpression] = None,
+                 columns: Optional[List[SQLDefineColumnExpression]] = None,
+                 primary_key: Optional[SQLPrimaryIndexExpression] = None,
+                 unique_key: Optional[List[SQLUniqueIndexExpression]] = None,
+                 key: Optional[List[SQLNormalIndexExpression]] = None,
+                 fulltext_key: Optional[List[SQLFulltextIndexExpression]] = None,
+                 foreign_key: List[SQLForeignKeyExpression] = None,
                  engine: Optional[str] = None,
                  auto_increment: Optional[int] = None,
                  default_charset: Optional[str] = None,
                  collate: Optional[str] = None,
                  row_format: Optional[str] = None,
                  states_persistent: Optional[str] = None,
-                 partition_by: List[DDLColumnExpression] = None
+                 partition_by: List[SQLDefineColumnExpression] = None
                  ):
         self._schema_name = schema_name
         self._table_name = table_name
         self._comment = comment
         self._if_not_exists = if_not_exists
         self._columns = columns
         self._primary_key = primary_key
@@ -2130,35 +2362,35 @@
         return self._comment
 
     @property
     def if_not_exists(self) -> bool:
         return self._if_not_exists
 
     @property
-    def columns(self) -> List[DDLColumnExpression]:
+    def columns(self) -> List[SQLDefineColumnExpression]:
         return self._columns
 
     @property
-    def primary_key(self) -> DDLPrimaryIndexExpression:
+    def primary_key(self) -> SQLPrimaryIndexExpression:
         return self._primary_key
 
     @property
-    def unique_key(self) -> List[DDLUniqueIndexExpression]:
+    def unique_key(self) -> List[SQLUniqueIndexExpression]:
         return self._unique_key
 
     @property
-    def key(self) -> List[DDLNormalIndexExpression]:
+    def key(self) -> List[SQLNormalIndexExpression]:
         return self._key
 
     @property
-    def fulltext_key(self) -> List[DDLFulltextIndexExpression]:
+    def fulltext_key(self) -> List[SQLFulltextIndexExpression]:
         return self._fulltext_key
 
     @property
-    def foreign_key(self) -> List[DDLForeignKeyExpression]:
+    def foreign_key(self) -> List[SQLForeignKeyExpression]:
         return self._foreign_key
 
     @property
     def engine(self) -> Optional[str]:
         return self._engine
 
     @property
@@ -2178,15 +2410,15 @@
         return self._row_format
 
     @property
     def states_persistent(self) -> Optional[str]:
         return self._states_persistent
 
     @property
-    def partition_by(self) -> List[DDLColumnExpression]:
+    def partition_by(self) -> List[SQLDefineColumnExpression]:
         return self._partition_by
 
     def set_schema_name(self, schema_name: str):
         self._schema_name = schema_name
 
     def set_table_name(self, table_name: str):
         self._table_name = table_name
@@ -2196,19 +2428,19 @@
         for column in self.columns:
             old_column_type = column.column_type.name
             new_column_type = hashmap[old_column_type.upper()]
             column.column_type._name = new_column_type
             if remove_param is True:
                 column.column_type._function_params = []
 
-    def append_column(self, column: DDLColumnExpression):
+    def append_column(self, column: SQLDefineColumnExpression):
         """添加字段"""
         self.columns.append(column)
 
-    def append_partition_by_column(self, column: DDLColumnExpression):
+    def append_partition_by_column(self, column: SQLDefineColumnExpression):
         """添加分区字段"""
 
     def source(self, data_source: DataSource = DataSource.MYSQL, n_indent: int = 4) -> str:
         if data_source == DataSource.MYSQL:
             indentation = " " * n_indent  # 缩进字符串
             result = "CREATE TABLE"
             if self.if_not_exists is True:
```

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql/parser/common.py` & `metasequoia-sql-0.2.0/metasequoia_sql/core/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,370 +1,447 @@
 """
 基础元素的解析逻辑
 
 TODO 使用 search 替代直接使用 now 判断
 TODO 整理各种函数的共同规律
+TODO 将 doctest 转化为单元测试
 """
 
+from typing import Optional, Tuple, List, Union
+
 from metasequoia_sql import ast
-from metasequoia_sql.common.token_scanner import TokenScanner, build_token_scanner
-from metasequoia_sql.objects.core import *
+from metasequoia_sql.common import TokenScanner, build_token_scanner
+from metasequoia_sql.core.objects import *
+from metasequoia_sql.core.static import *
+from metasequoia_sql.errors import SqlParseError
 
+__all__ = [
+    # ------------------------------ 基础元素解析 ------------------------------
+    # 判断、解析插入类型
+    "check_insert_type", "parse_insert_type",
 
-def maybe_compute_operator(scanner: TokenScanner) -> bool:
-    """检查是否可能为计算运算符
+    # 判断、解析关联类型
+    "check_join_type", "parse_join_type",
 
-    Examples
-    --------
-    >>> maybe_compute_operator(TokenScanner(ast.parse_as_tokens("+ 3"), ignore_space=True))
-    True
-    >>> maybe_compute_operator(TokenScanner(ast.parse_as_tokens("- 3"), ignore_space=True))
-    True
-    >>> maybe_compute_operator(TokenScanner(ast.parse_as_tokens("* 3"), ignore_space=True))
-    True
-    >>> maybe_compute_operator(TokenScanner(ast.parse_as_tokens("/ 3"), ignore_space=True))
-    True
-    >>> maybe_compute_operator(TokenScanner(ast.parse_as_tokens("3 + 3"), ignore_space=True))
-    False
-    """
-    return not scanner.is_finish and scanner.now.is_compute_operator
+    # 判断、解析排序类型
+    "check_order_type", "parse_order_type",
 
+    # 判断、解析组合类型
+    "check_union_type", "parse_union_type",
 
-def parse_compute_operator(scanner: TokenScanner) -> SQLComputeOperator:
-    """解析计算运算符
+    # 判断、解析比较运算符
+    "check_compare_operator", "parse_compare_operator",
 
-    Examples
-    --------
-    >>> parse_compute_operator(TokenScanner(ast.parse_as_tokens("+ 3"), ignore_space=True))
-    <SQLPlus>
-    >>> parse_compute_operator(TokenScanner(ast.parse_as_tokens("- 3"), ignore_space=True))
-    <SQLSubtract>
-    >>> parse_compute_operator(TokenScanner(ast.parse_as_tokens("* 3"), ignore_space=True))
-    <SQLMultiple>
-    >>> parse_compute_operator(TokenScanner(ast.parse_as_tokens("/ 3"), ignore_space=True))
-    <SQLDivide>
-    >>> parse_compute_operator(TokenScanner(ast.parse_as_tokens("3 + 3"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 未知的计算运算符: <ASTLiteralInteger source=3>
-    """
-    token: ast.AST = scanner.pop()
-    if token.source == "+":
-        return SQLPlus()
-    if token.source == "-":
-        return SQLSubtract()
-    if token.source == "*":
-        return SQLMultiple()
-    if token.source == "/":
-        return SQLDivide()
-    if token.source == "%":
-        return SQLMod()
-    if token.source == "||":
-        return SQLConcat()
-    raise SqlParseError(f"未知的计算运算符: {token}")
+    # 判断、解析计算运算符
+    "check_compute_operator", "parse_compute_operator",
 
+    # 判断、解析逻辑运算符
+    "check_logical_operator", "parse_logical_operator",
 
-def maybe_compare_operator(scanner: TokenScanner) -> bool:
-    """检查是否可能为比较运算符
+    # ------------------------------ 一般表达式解析 ------------------------------
+    # 判断、解析字面值表达式
+    "check_literal_expression", "parse_literal_expression",
 
-    Examples
-    --------
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens("= 3"), ignore_space=True))
-    True
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens("< 3"), ignore_space=True))
-    True
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens("<= 3"), ignore_space=True))
-    True
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens("> 3"), ignore_space=True))
-    True
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens(">= 3"), ignore_space=True))
-    True
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens("!= 3"), ignore_space=True))
-    True
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens("<> 3"), ignore_space=True))
-    True
-    >>> maybe_compare_operator(TokenScanner(ast.parse_as_tokens("3 + 3"), ignore_space=True))
-    False
-    """
-    return not scanner.is_finish and scanner.now.is_compare_operator
+    # 判断、解析列名表达式
+    "check_column_name_expression", "parse_column_name_expression",
+
+    # 判断、解析函数表达式
+    # TODO 将 CAST_DATA_TYPE 提出作为一个基础类型节点
+    # TODO 将 function_name 提出作为一个专有表达式
+    "check_function_expression", "parse_cast_data_type", "parse_cast_function_expression",
+    "parse_extract_function_expression", "parse_if_function_expression", "parse_function_name",
+    "parse_function_expression",
+
+    # 解析布尔值表达式
+    "parse_bool_expression",
+
+    # 判断、解析窗口表达式
+    "check_window_expression", "parse_window_expression",
+
+    # 判断、解析通配符表达式
+    "check_wildcard_expression", "parse_wildcard_expression",
+
+    # 解析条件表达式
+    "parse_condition_expression",
+
+    # 判断、解析 CASE 表达式
+    "check_case_expression", "parse_case_expression",
+
+    # 解析值表达式
+    "parse_value_expression",
+
+    # 判断、解析子查询表达式
+    "check_sub_query_parenthesis", "parse_sub_query_expression",
+
+    # 解析一般表达式
+    "parse_general_expression",
+
+    # ------------------------------ 专有表达式解析 ------------------------------
+    # 解析表名表达式
+    "parse_table_name_expression",
+
+    # 判断、解析表名表达式
+    "check_alias_expression", "parse_alias_expression",
+
+    # 判断、解析关联表达式
+    "check_join_expression", "parse_join_on_expression", "parse_join_using_expression", "parse_join_expression",
+
+    # 解析字段类型表达式
+    "parse_column_type_expression",
+
+    # 解析表表达式
+    "parse_table_expression",
+
+    # 解析列表达式
+    "parse_column_expression",
+
+    # 解析等式表达式
+    "parse_equal_expression",
+
+    # 判断、解析分区表达式
+    "check_partition_expression", "parse_partition_expression",
+
+    # 判断、解析声明外键表达式
+    "check_foreign_key_expression", "parse_foreign_key_expression",
+
+    # 判断、解析声明索引表达式
+    "check_primary_index_expression", "parse_primary_index_expression", "check_unique_index_expression",
+    "parse_unique_index_expression", "check_normal_index_expression", "parse_normal_index_expression",
+    "check_fulltext_expression", "parse_fulltext_expression",
+
+    # 解析声明字段表达式
+    "parse_define_column_expression",
+
+    # ------------------------------ 子句解析 ------------------------------
+    # 判断、解析 SELECT 子句
+    "check_select_clause", "parse_select_clause",
+
+    # 判断、解析 FROM 子句
+    "check_from_clause", "parse_from_clause",
+
+    # 判断、解析 JOIN 子句
+    "check_join_clause", "parse_join_clause",
+
+    # 判断、解析 WHERE 子句
+    "check_where_clause", "parse_where_clause",
+
+    # 判断、解析 GROUP BY 子句
+    "check_group_by_clause", "parse_group_by_clause",
+
+    # 判断、解析 HAVING 子句
+    "check_having_clause", "parse_having_clause",
+
+    # 判断、解析 ORDER BY 子句
+    "check_order_by_clause", "parse_order_by_clause",
+
+    # 判断、解析 LIMIT 子句
+    "check_limit_clause", "parse_limit_clause",
+
+    # 解析 WITH 子句
+    "parse_with_clause",
+
+    # ------------------------------ 语句解析 ------------------------------
+    # 判断、解析 SELECT 语句
+    "check_select_statement", "parse_single_select_statement", "parse_select_statement",
+
+    # 判断、解析 INSERT 语句
+    "check_insert_statement", "parse_insert_statement",
+
+    # 解析 CREATE TABLE 语句
+    "parse_create_table_statement",
+
+    # 通用表达式解析
+    "parse_statement"
+]
+
+
+def check_insert_type(scanner: TokenScanner) -> bool:
+    """判断是否为插入类型"""
+    return scanner.search_and_move("INSERT", "INTO") or scanner.search_and_move("INSERT", "OVERWRITE")
+
+
+def parse_insert_type(scanner: TokenScanner) -> SQLInsertType:
+    """解析插入类型"""
+    if scanner.search_and_move("INSERT", "INTO"):
+        return SQLInsertType(insert_type=EnumInsertType.INSERT_INTO)
+    if scanner.search_and_move("INSERT", "OVERWRITE"):
+        return SQLInsertType(insert_type=EnumInsertType.INSERT_OVERWRITE)
+    raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
+
+
+def check_join_type(scanner: TokenScanner) -> bool:
+    for join_type in EnumJoinType:
+        if scanner.search(*join_type.value):
+            return True
+    return False
+
+
+def parse_join_type(scanner: TokenScanner) -> SQLJoinType:
+    for join_type in EnumJoinType:
+        if scanner.search_and_move(*join_type.value):
+            return SQLJoinType(join_type=join_type)
+    raise SqlParseError(f"无法解析的关联类型: {scanner}")
+
+
+def check_order_type() -> bool:
+    """任何元素都可以是排序类型（省略升序），所以均返回 True"""
+    return True
+
+
+def parse_order_type(scanner: TokenScanner) -> SQLOrderType:
+    if scanner.search_and_move("DESC"):
+        return SQLOrderType(order_type=EnumOrderType.DESC)
+    return SQLOrderType(order_type=EnumOrderType.ASC)
+
+
+def check_union_type(scanner: TokenScanner) -> bool:
+    for union_type in EnumUnionType:
+        if scanner.search(*union_type.value):
+            return True
+    return False
+
+
+def parse_union_type(scanner: TokenScanner) -> SQLUnionType:
+    for union_type in EnumUnionType:
+        if scanner.search_and_move(*union_type.value):
+            return SQLUnionType(union_type=union_type)
+    raise SqlParseError(f"无法解析的组合类型: {scanner}")
+
+
+def check_compare_operator(scanner: TokenScanner) -> bool:
+    return scanner.get_as_source() in {"=", "!=", "<>", "<", "<=", ">", ">="}
 
 
 def parse_compare_operator(scanner: TokenScanner) -> SQLCompareOperator:
-    """解析比较运算符
+    compare_operator_hash = {
+        "=": EnumCompareOperator.EQUAL_TO,
+        "<": EnumCompareOperator.LESS_THAN,
+        "<=": EnumCompareOperator.LESS_THAN_OR_EQUAL,
+        ">": EnumCompareOperator.GREATER_THAN,
+        ">=": EnumCompareOperator.GREATER_THAN_OR_EQUAL,
+        "!=": EnumCompareOperator.NOT_EQUAL_TO,
+        "<>": EnumCompareOperator.NOT_EQUAL_TO
+    }
+    compare_operator = compare_operator_hash.get(scanner.pop_as_source())
+    if compare_operator is not None:
+        return SQLCompareOperator(compare_operator=compare_operator)
+    raise SqlParseError(f"无法解析的比较运算符: {scanner}")
+
+
+def check_compute_operator(scanner: TokenScanner) -> bool:
+    for compute_operator in EnumComputeOperator:
+        if scanner.search(compute_operator.value):
+            return True
+    return False
 
-    Examples
-    --------
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("= 3"), ignore_space=True))
-    <SQLEqualTo>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("< 3"), ignore_space=True))
-    <SQLLessThan>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("<= 3"), ignore_space=True))
-    <SQLLessThanOrEqual>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("> 3"), ignore_space=True))
-    <SQLGreaterThan>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens(">= 3"), ignore_space=True))
-    <SQLGreaterThanOrEqual>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("!= 3"), ignore_space=True))
-    <SQLNotEqualTo>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("<> 3"), ignore_space=True))
-    <SQLNotEqualTo>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("IS NULL"), ignore_space=True))
-    <SQLIs>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("IS NOT NULL"), ignore_space=True))
-    <SQLIs>
-    >>> parse_compare_operator(TokenScanner(ast.parse_as_tokens("3 + 3"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 未知的比较运算符: <ASTLiteralInteger source=3>
-    """
-    token: ast.AST = scanner.pop()
-    if token.source == "=":
-        return SQLEqualTo()
-    if token.source == "<":
-        return SQLLessThan()
-    if token.source == "<=":
-        return SQLLessThanOrEqual()
-    if token.source == ">":
-        return SQLGreaterThan()
-    if token.source == ">=":
-        return SQLGreaterThanOrEqual()
-    if token.source in {"!=", "<>"}:
-        return SQLNotEqualTo()
-    if token.source == "IS":
-        return SQLIs()
-    raise SqlParseError(f"未知的比较运算符: {token}")
 
+def parse_compute_operator(scanner: TokenScanner) -> SQLComputeOperator:
+    for compute_operator in EnumComputeOperator:
+        if scanner.search_and_move(compute_operator.value):
+            return SQLComputeOperator(compute_operator=compute_operator)
+    raise SqlParseError(f"无法解析的计算运算符: {scanner}")
 
-def maybe_logical_operator(scanner: TokenScanner) -> bool:
-    """判断逻辑运算符：包含 AND、OR、NOT
 
-    Examples
-    --------
-    >>> maybe_logical_operator(TokenScanner(ast.parse_as_tokens("AND a > 1"), ignore_space=True))
-    True
-    >>> maybe_logical_operator(TokenScanner(ast.parse_as_tokens("NOT a > 1"), ignore_space=True))
-    True
-    >>> maybe_logical_operator(TokenScanner(ast.parse_as_tokens("OR a > 1"), ignore_space=True))
-    True
-    >>> maybe_logical_operator(TokenScanner(ast.parse_as_tokens("a > 1"), ignore_space=True))
-    False
-    """
-    return not scanner.is_finish and scanner.now.is_logical_operator
+def check_logical_operator(scanner: TokenScanner) -> bool:
+    return scanner.get_as_source() in {"AND", "OR", "NOT"}
 
 
 def parse_logical_operator(scanner: TokenScanner) -> SQLLogicalOperator:
-    """解析逻辑运算符：包含 AND、OR、NOT
-
-    Examples
-    --------
-    >>> parse_logical_operator(TokenScanner(ast.parse_as_tokens("AND a > 1"), ignore_space=True))
-    <SQLAndOperator>
-    >>> parse_logical_operator(TokenScanner(ast.parse_as_tokens("OR a > 1"), ignore_space=True))
-    <SQLOrOperator>
-    >>> parse_logical_operator(TokenScanner(ast.parse_as_tokens("NOT a > 1"), ignore_space=True))
-    <SQLNotOperator>
-    >>> parse_logical_operator(TokenScanner(ast.parse_as_tokens("a > 1"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 未知的逻辑运算符: <ASTOther source=a>
-    """
-    token: ast.AST = scanner.pop()
-    if token.source == "AND":
-        return SQLAndOperator()
-    if token.source == "OR":
-        return SQLOrOperator()
-    if token.source == "NOT":
-        return SQLNotOperator()
-    raise SqlParseError(f"未知的逻辑运算符: {token}")
+    for logical_operator in EnumLogicalOperator:
+        if scanner.search_and_move(logical_operator.value):
+            return SQLLogicalOperator(logical_operator=logical_operator)
+    raise SqlParseError(f"无法解析的逻辑运算符: {scanner}")
 
 
-def maybe_literal(scanner: TokenScanner) -> bool:
+def check_literal_expression(scanner: TokenScanner) -> bool:
     """判断是否为字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值
 
     Examples
     --------
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
     True
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
     False
-    >>> maybe_literal(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
+    >>> check_literal_expression(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
     False
     """
     return not scanner.is_finish and scanner.now.is_literal
 
 
-def parse_literal(scanner: TokenScanner) -> SQLLiteral:
+def parse_literal_expression(scanner: TokenScanner) -> SQLLiteralExpression:
     """解析字面值：包含整型字面值、浮点型字面值、字符串型字面值、十六进制型字面值、布尔型字面值、位值型字面值、空值的字面值
 
     Examples
     --------
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
     <SQLLiteralInteger source=1>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
     <SQLLiteralFloat source=2.5>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
     <SQLLiteralString source='a'>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
     <SQLLiteralHex source=x'3F'>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
     <SQLLiteralBool source=TRUE>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
     <SQLLiteralBool source=TRUE>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
     <SQLLiteralBool source=FALSE>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
     <SQLLiteralBit source=b'1'>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
     <SQLLiteralNull source=NULL>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
     <SQLLiteralNull source=NULL>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
     Traceback (most recent call last):
     ...
     metasequoia_sql.errors.SqlParseError: 未知的字面值: <ASTOther source=cnt>
-    >>> parse_literal(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
+    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
     Traceback (most recent call last):
     ...
     metasequoia_sql.errors.SqlParseError: 未知的字面值: <ASTOther source=table_name>
     """
     token: ast.AST = scanner.pop()
     if isinstance(token, ast.ASTLiteralInteger):
-        return SQLLiteralInteger(token.literal_value)
+        return SQLLiteralIntegerExpression(token.literal_value)
     if isinstance(token, ast.ASTLiteralFloat):
-        return SQLLiteralFloat(token.literal_value)
+        return SQLLiteralFloatExpression(token.literal_value)
     if isinstance(token, ast.ASTLiteralString):
-        return SQLLiteralString(token.literal_value)
+        return SQLLiteralStringExpression(token.literal_value)
     if isinstance(token, ast.ASTLiteralHex):
-        return SQLLiteralHex(token.literal_value)
+        return SQLLiteralHexExpression(token.literal_value)
     if isinstance(token, ast.ASTLiteralBool):
-        return SQLLiteralBool(token.literal_value)
+        return SQLLiteralBoolExpression(token.literal_value)
     if isinstance(token, ast.ASTLiteralBit):
-        return SQLLiteralBit(token.literal_value)
+        return SQLLiteralBitExpression(token.literal_value)
     if isinstance(token, ast.ASTLiteralNull):
-        return SQLLiteralNull()
+        return SQLLiteralNullExpression()
     raise SqlParseError(f"未知的字面值: {token}")
 
 
-def maybe_literal_expression(scanner: TokenScanner) -> bool:
-    """判断是否为字面值表达式
+def check_column_name_expression(scanner: TokenScanner) -> bool:
+    """是否可能为列名表达式
 
     Examples
     --------
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
-    True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
+    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
+    False
+    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
+    False
+    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.column AND"), ignore_space=True))
     True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
+    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`column` AND"), ignore_space=True))
     True
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
+    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
     False
-    >>> maybe_literal_expression(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
+    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
     False
+    >>> check_column_name_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
+    True
     """
-    return maybe_literal(scanner)
+    return not scanner.is_finish and (
+            (scanner.now.is_maybe_name and
+             (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))) or
+            (scanner.now.is_maybe_name and
+             scanner.next1 is not None and scanner.next1.is_dot and
+             scanner.next2 is not None and scanner.next2.is_maybe_name and
+             (scanner.next3 is None or not scanner.next3.is_parenthesis))
+    )
 
 
-def parse_literal_expression(scanner: TokenScanner) -> SQLLiteralExpression:
-    """解析字面值表达式
+def parse_column_name_expression(scanner: TokenScanner) -> SQLColumnNameExpression:
+    """解析列名表达式
 
     Examples
     --------
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("1 WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=1>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=2.5>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("'a' WHERE"), ignore_space=True))
-    <SQLLiteralExpression source='a'>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("x'3f' WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=x'3F'>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("TRUE WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=TRUE>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("true WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=TRUE>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("False WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=FALSE>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("b'1' WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=b'1'>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("null WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=NULL>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("NULL WHERE"), ignore_space=True))
-    <SQLLiteralExpression source=NULL>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("cnt WHERE"), ignore_space=True))
+    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
     Traceback (most recent call last):
     ...
-    metasequoia_sql.errors.SqlParseError: 未知的字面值: <ASTOther source=cnt>
-    >>> parse_literal_expression(TokenScanner(ast.parse_as_tokens("table_name.column_name WHERE"), ignore_space=True))
+    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTOther source=schema>, <ASTCommon source=.>, <ASTOther source=function>, <ASTParenthesis children=[<ASTOther source=param>]>, <ASTCommon source=AND>], pos=0>
+    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
     Traceback (most recent call last):
     ...
-    metasequoia_sql.errors.SqlParseError: 未知的字面值: <ASTOther source=table_name>
+    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTIdentifier source=`schema`>, <ASTCommon source=.>, <ASTIdentifier source=`function`>, <ASTParenthesis children=[<ASTOther source=param>]>, <ASTCommon source=AND>], pos=0>
+    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.column AND"), ignore_space=True))
+    <SQLColumnNameExpression source=schema.column>
+    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`column` AND"), ignore_space=True))
+    <SQLColumnNameExpression source=`schema`.`column`>
+    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
+    Traceback (most recent call last):
+    ...
+    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTOther source=trim>, <ASTParenthesis children=[<ASTOther source=column_name>]>, <ASTCommon source=AND>], pos=0>
+    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
+    Traceback (most recent call last):
+    ...
+    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTLiteralFloat source=2.5>, <ASTOther source=WHERE>], pos=0>
+    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
+    <SQLColumnNameExpression source=coumn_name>
     """
-    return SQLLiteralExpression(literal=parse_literal(scanner))
+    if (scanner.now.is_maybe_name and
+            (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))):
+        return SQLColumnNameExpression(None, scanner.pop_as_source())
+    if (scanner.now.is_maybe_name and
+            scanner.next1 is not None and scanner.next1.is_dot and
+            scanner.next2 is not None and scanner.next2.is_maybe_name and
+            (scanner.next3 is None or not scanner.next3.is_parenthesis)):
+        table_name = scanner.pop_as_source()
+        scanner.pop()
+        column_name = scanner.pop_as_source()
+        return SQLColumnNameExpression(table_name, column_name)
+    raise SqlParseError(f"无法解析为表名表达式: {scanner}")
 
 
-def maybe_function_expression(scanner: TokenScanner) -> bool:
+def check_function_expression(scanner: TokenScanner) -> bool:
     """是否可能为函数表达式
 
     Examples
     --------
-    >>> maybe_function_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
+    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
     True
-    >>> maybe_function_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
+    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
     True
-    >>> maybe_function_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
+    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
     True
-    >>> maybe_function_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
+    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
     False
-    >>> maybe_function_expression(TokenScanner(ast.parse_as_tokens("coumn_name WHERE"), ignore_space=True))
+    >>> check_function_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
     False
     """
     return not scanner.is_finish and (
             (scanner.now.is_maybe_name and
              scanner.next1 is not None and scanner.next1.is_parenthesis) or
             (scanner.now.is_maybe_name and
              scanner.next1 is not None and scanner.next1.is_dot and
              scanner.next2 is not None and scanner.next2.is_maybe_name and
              scanner.next3 is not None and scanner.next3.is_parenthesis
              ))
 
 
-def parse_cast_data_type(scanner: TokenScanner) -> SQLEnumCastDataType:
+def parse_cast_data_type(scanner: TokenScanner) -> EnumCastDataType:
     """解析 CAST 函数表达式中的类型"""
-    for cast_type in SQLEnumCastDataType:
+    for cast_type in EnumCastDataType:
         if scanner.search_and_move(cast_type.value):
             return cast_type
     raise SqlParseError(f"无法解析的 CAST 函数表达式中的类型: {scanner}")
 
 
 def parse_cast_function_expression(scanner: TokenScanner) -> SQLCastFunctionExpression:
     """解析 CAST 函数表达式"""
@@ -408,15 +485,15 @@
         else:
             function_params.append(parse_general_expression(param_scanner))
         if not param_scanner.is_finish:
             raise SqlParseError(f"无法解析函数参数: {param_scanner}")
     return SQLFunctionExpression(schema_name=None, function_name="IF", function_params=function_params)
 
 
-def _parse_function_name(scanner: TokenScanner) -> Tuple[Optional[str], str]:
+def parse_function_name(scanner: TokenScanner) -> Tuple[Optional[str], str]:
     """解析函数表达式函数的 schema 名和 function 名"""
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_parenthesis):
         return None, scanner.pop_as_source()
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_dot and
             scanner.next2 is not None and scanner.next2.is_maybe_name and
@@ -438,20 +515,20 @@
     <SQLFunctionExpression source=`schema`.`function`(<SQLColumnNameExpression source=param>)>
     >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
     <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column_name>)>
     >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
     Traceback (most recent call last):
     ...
     metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTLiteralFloat source=2.5>, <ASTOther source=WHERE>], pos=0>
-    >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("coumn_name WHERE"), ignore_space=True))
+    >>> parse_function_expression(TokenScanner(ast.parse_as_tokens("column_name WHERE"), ignore_space=True))
     Traceback (most recent call last):
     ...
     metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTOther source=coumn_name>, <ASTOther source=WHERE>], pos=0>
     """
-    schema_name, function_name = _parse_function_name(scanner)
+    schema_name, function_name = parse_function_name(scanner)
 
     if function_name.upper() == "CAST":
         return parse_cast_function_expression(scanner.pop_as_children_scanner())
     if function_name.upper() == "EXTRACT":
         return parse_extract_function_expression(scanner.pop_as_children_scanner())
     if function_name.upper() == "IF":
         return parse_if_function_expression(scanner.pop_as_children_scanner())
@@ -480,94 +557,194 @@
                                                 is_distinct=is_distinct)
     else:
         return SQLFunctionExpression(schema_name=schema_name,
                                      function_name=function_name,
                                      function_params=function_params)
 
 
-def maybe_column_name_expression(scanner: TokenScanner) -> bool:
-    """是否可能为列名表达式
+def parse_bool_expression(scanner: TokenScanner) -> SQLBoolExpression:
+    """解析布尔值表达式
 
     Examples
     --------
-    >>> maybe_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
-    False
-    >>> maybe_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
-    False
-    >>> maybe_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.column AND"), ignore_space=True))
-    True
-    >>> maybe_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`column` AND"), ignore_space=True))
+    >>> parse_bool_expression(build_token_scanner("column1 > 3"))
+    <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
+    >>> parse_bool_expression(build_token_scanner("t2.column1 > 3"))
+    <SQLBoolCompareExpression source=<SQLColumnNameExpression source=t2.column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
+    >>> parse_bool_expression(build_token_scanner("t2.column1 + 3 > 3"))
+    <SQLBoolCompareExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=t2.column1> <SQLPlus> <SQLLiteralExpression source=3>> <SQLGreaterThan> <SQLLiteralExpression source=3>>
+    >>> parse_bool_expression(build_token_scanner("column1 BETWEEN 3 AND 4"))
+    <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column1> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
+    >>> parse_bool_expression(build_token_scanner("column1 + 3 BETWEEN 3 AND 4"))
+    <SQLBoolBetweenExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=column1> <SQLPlus> <SQLLiteralExpression source=3>> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
+    """
+    if scanner.search_and_move("EXISTS"):
+        after_value = parse_sub_query_expression(scanner)
+        return SQLBoolExistsExpression(is_not=False, after_value=after_value)
+    if scanner.search_and_move("NOT", "EXISTS"):
+        after_value = parse_sub_query_expression(scanner)
+        return SQLBoolExistsExpression(is_not=True, after_value=after_value)
+    before_value = parse_general_expression(scanner)
+    if scanner.search_and_move("BETWEEN"):
+        # "... BETWEEN ... AND ..."
+        from_value = parse_general_expression(scanner)
+        if not scanner.search_and_move("AND"):
+            raise SqlParseError(f"无法解析为 BETWEEN 布尔值表达式: {scanner}")
+        to_value = parse_general_expression(scanner)
+        return SQLBoolBetweenExpression(before_value=before_value, from_value=from_value, to_value=to_value)
+    if scanner.search_and_move("IS"):
+        # ".... IS ...." 或 "... IS NOT ..."
+        if scanner.search_and_move("NOT"):
+            is_not = True
+        else:
+            is_not = False
+        after_value = parse_general_expression(scanner)
+        return SQLBoolIsExpression(is_not=is_not, before_value=before_value, after_value=after_value)
+    if scanner.search_and_move("IN"):
+        # "... IN (1, 2, 3)" 或 "... IN (SELECT ... )"
+        after_value = _parse_in_parenthesis(scanner)
+        return SQLBoolInExpression(is_not=False, before_value=before_value, after_value=after_value)
+    if scanner.search_and_move("NOT", "IN"):
+        after_value = _parse_in_parenthesis(scanner)
+        return SQLBoolInExpression(is_not=True, before_value=before_value, after_value=after_value)
+    if scanner.search_and_move("LIKE"):
+        after_value = parse_general_expression(scanner)
+        return SQLBoolLikeExpression(is_not=False, before_value=before_value, after_value=after_value)
+    if scanner.search_and_move("NOT LIKE"):
+        after_value = parse_general_expression(scanner)
+        return SQLBoolLikeExpression(is_not=True, before_value=before_value, after_value=after_value)
+    if check_compare_operator(scanner):
+        # "... > ..."
+        compare_operator = parse_compare_operator(scanner)
+        after_value = parse_general_expression(scanner)
+        return SQLBoolCompareExpression(operator=compare_operator, before_value=before_value, after_value=after_value)
+    raise SqlParseError(f"无法解析为布尔值表达式: {scanner}")
+
+
+def check_window_expression(scanner: TokenScanner) -> bool:
+    """判断是否可能为窗口函数
+
+    Examples
+    --------
+    >>> check_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
     True
-    >>> maybe_column_name_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
+    >>> check_window_expression(build_token_scanner("3 + 5"))
     False
-    >>> maybe_column_name_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
-    False
-    >>> maybe_column_name_expression(TokenScanner(ast.parse_as_tokens("coumn_name WHERE"), ignore_space=True))
-    True
     """
     return not scanner.is_finish and (
-            (scanner.now.is_maybe_name and
-             (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))) or
-            (scanner.now.is_maybe_name and
-             scanner.next1 is not None and scanner.next1.is_dot and
-             scanner.next2 is not None and scanner.next2.is_maybe_name and
-             (scanner.next3 is None or not scanner.next3.is_parenthesis))
-    )
+            scanner.now.is_maybe_name and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
+            scanner.next1 is not None and scanner.next1.is_parenthesis and
+            scanner.next2 is not None and scanner.next2.equals("OVER") and
+            scanner.next3 is not None and scanner.next3.is_parenthesis)
 
 
-def parse_column_name_expression(scanner: TokenScanner) -> SQLColumnNameExpression:
-    """解析列名表达式
+def parse_window_expression(scanner: TokenScanner) -> SQLWindowExpression:
+    """解析窗口函数
+
+    TODO 支持 ROW BETWEEN 的语法
 
     Examples
     --------
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.function(param) AND"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTOther source=schema>, <ASTCommon source=.>, <ASTOther source=function>, <ASTParenthesis children=[<ASTOther source=param>]>, <ASTCommon source=AND>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`function`(param) AND"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTIdentifier source=`schema`>, <ASTCommon source=.>, <ASTIdentifier source=`function`>, <ASTParenthesis children=[<ASTOther source=param>]>, <ASTCommon source=AND>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("schema.column AND"), ignore_space=True))
-    <SQLColumnNameExpression source=schema.column>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("`schema`.`column` AND"), ignore_space=True))
-    <SQLColumnNameExpression source=`schema`.`column`>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("trim(column_name) AND"), ignore_space=True))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTOther source=trim>, <ASTParenthesis children=[<ASTOther source=column_name>]>, <ASTCommon source=AND>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("2.5 WHERE"), ignore_space=True))
+    >>> parse_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
+    <SQLWindowExpression source=<SQLFunctionExpression source=ROW_NUMBER()> OVER (PARTITION BY <SQLColumnNameExpression source=column1>ORDER BY <SQLColumnNameExpression source=column2>)>
+    >>> parse_window_expression(build_token_scanner("3 + 5"))
     Traceback (most recent call last):
     ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为表名表达式: <TokenScanner tokens=[<ASTLiteralFloat source=2.5>, <ASTOther source=WHERE>], pos=0>
-    >>> parse_column_name_expression(TokenScanner(ast.parse_as_tokens("coumn_name WHERE"), ignore_space=True))
-    <SQLColumnNameExpression source=coumn_name>
+    metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTLiteralInteger source=3>, <ASTCommon source=+>, <ASTLiteralInteger source=5>], pos=0>
     """
-    if (scanner.now.is_maybe_name and
-            (scanner.next1 is None or (not scanner.next1.is_dot and not scanner.next1.is_parenthesis))):
-        return SQLColumnNameExpression(None, scanner.pop_as_source())
+    window_function = parse_function_expression(scanner)
+    partition_by = None
+    order_by = None
+    if not scanner.pop().equals("OVER"):
+        raise SqlParseError(f"无法解析为窗口表达式: {scanner}")
+    parenthesis_scanner = scanner.pop_as_children_scanner()
+    if parenthesis_scanner.search_and_move("PARTITION", "BY"):
+        partition_by = parse_general_expression(parenthesis_scanner, maybe_window=False)
+    if parenthesis_scanner.search_and_move("ORDER", "BY"):
+        order_by = parse_general_expression(parenthesis_scanner, maybe_window=False)
+    return SQLWindowExpression(window_function=window_function, partition_by=partition_by, order_by=order_by)
+
+
+def check_wildcard_expression(scanner: TokenScanner) -> bool:
+    """判断是否可能为通配符表达式
+
+    Examples
+    --------
+    >>> check_wildcard_expression(build_token_scanner("*"))
+    True
+    >>> check_wildcard_expression(build_token_scanner("t1.*"))
+    True
+    """
+    return not scanner.is_finish and (scanner.now.is_maybe_wildcard or
+                                      (scanner.now.is_maybe_name and
+                                       scanner.next1 is not None and scanner.next1.is_dot and
+                                       scanner.next2 is not None and scanner.next2.is_maybe_wildcard))
+
+
+def parse_wildcard_expression(scanner: TokenScanner) -> SQLWildcardExpression:
+    """解析通配符表达式
+
+    Examples
+    --------
+    >>> parse_wildcard_expression(build_token_scanner("*"))
+    <SQLWildcardExpression source=*>
+    >>> parse_wildcard_expression(build_token_scanner("t1.*"))
+    <SQLWildcardExpression source=t1.*>
+    """
+    if scanner.now.is_maybe_wildcard:
+        scanner.pop()
+        return SQLWildcardExpression(schema=None)
     if (scanner.now.is_maybe_name and
             scanner.next1 is not None and scanner.next1.is_dot and
-            scanner.next2 is not None and scanner.next2.is_maybe_name and
-            (scanner.next3 is None or not scanner.next3.is_parenthesis)):
-        table_name = scanner.pop_as_source()
+            scanner.next2 is not None and scanner.next2.is_maybe_wildcard):
+        schema_name = scanner.pop_as_source()
         scanner.pop()
-        column_name = scanner.pop_as_source()
-        return SQLColumnNameExpression(table_name, column_name)
-    raise SqlParseError(f"无法解析为表名表达式: {scanner}")
+        scanner.pop()
+        return SQLWildcardExpression(schema=schema_name)
+    raise SqlParseError("无法解析为通配符表达式")
+
+
+def parse_condition_expression(scanner: TokenScanner) -> SQLConditionExpression:
+    """解析条件表达式
+
+    Examples
+    --------
+    >>> parse_condition_expression(build_token_scanner("column1 > 3 AND column2 > 2 WHERE"))
+    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
+    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 > 2 WHERE"))
+    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
+    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 BETWEEN 2 AND 4 WHERE"))
+    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>
+    """
+
+    def parse_single():
+        if scanner.search("NOT"):
+            elements.append(parse_logical_operator(scanner))
+        if scanner.now_is_parenthesis:
+            elements.append(parse_condition_expression(scanner.pop_as_children_scanner()))  # 插入语，子句也应该是一个条件表达式
+        else:
+            elements.append(parse_bool_expression(scanner))
+
+    elements: List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]] = []
+    parse_single()  # 解析第 1 个表达式元素
+    while not scanner.is_finish and scanner.now.source.upper() in {"AND", "OR"}:  # 如果是用 AND 和 OR 连接的多个表达式，则继续解析
+        elements.append(parse_logical_operator(scanner))
+        parse_single()
+
+    return SQLConditionExpression(elements=elements)
 
 
-def maybe_case_expression(scanner: TokenScanner) -> bool:
+def check_case_expression(scanner: TokenScanner) -> bool:
     """判断是否可能为 CASE 表达式
 
     Examples
     --------
-    >>> maybe_case_expression(TokenScanner(ast.parse_as_tokens("CASE WHEN 2 THEN 3 ELSE 4 END"), ignore_space=True))
+    >>> check_case_expression(TokenScanner(ast.parse_as_tokens("CASE WHEN 2 THEN 3 ELSE 4 END"), ignore_space=True))
     True
-    >>> maybe_case_expression(TokenScanner(ast.parse_as_tokens("3 + 5"), ignore_space=True))
+    >>> check_case_expression(TokenScanner(ast.parse_as_tokens("3 + 5"), ignore_space=True))
     False
     """
     return not scanner.is_finish and scanner.now.equals("CASE")
 
 
 def parse_case_expression(scanner: TokenScanner) -> Union[SQLCaseExpression, SQLCaseValueExpression]:
     """解析 CASE 表达式
@@ -610,86 +787,73 @@
             cases.append((when_expression, case_expression))
         if scanner.search_and_move("ELSE"):
             else_value = parse_general_expression(scanner)
         scanner.match("END")
         return SQLCaseValueExpression(case_value=case_value, cases=cases, else_value=else_value)
 
 
-# 窗口函数名称集合
-WINDOW_FUNCTION_NAME_SET = {"ROW_NUMBER", "RANK", "DENSE_RANK", "SUM", "MIN", "MAX", "AVG", "LAG", "LEAD",
-                            "FIRST_VALUE", "LAST_VALUE", "NTILE"}
+def parse_value_expression(scanner: TokenScanner) -> SQLValueExpression:
+    """解析值表达式"""
+    values = []
+    for value_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+        values.append(parse_general_expression(value_scanner))
+    return SQLValueExpression(values=values)
 
 
-def maybe_window_expression(scanner: TokenScanner) -> bool:
-    """判断是否可能为窗口函数
+def check_sub_query_parenthesis(scanner: TokenScanner) -> bool:
+    """判断是否为子查询的插入语"""
+    parenthesis_scanner: TokenScanner = scanner.get_as_children_scanner()
+    return check_select_statement(parenthesis_scanner)
 
-    Examples
-    --------
-    >>> maybe_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
-    True
-    >>> maybe_window_expression(build_token_scanner("3 + 5"))
-    False
-    """
-    return not scanner.is_finish and (
-            scanner.now.is_maybe_name and scanner.now.source.upper() in WINDOW_FUNCTION_NAME_SET and
-            scanner.next1 is not None and scanner.next1.is_parenthesis and
-            scanner.next2 is not None and scanner.next2.equals("OVER") and
-            scanner.next3 is not None and scanner.next3.is_parenthesis)
 
+def parse_sub_query_expression(scanner: TokenScanner) -> SQLSubQueryExpression:
+    """解析子查询表达式"""
+    return SQLSubQueryExpression(select_statement=parse_select_statement(scanner.pop_as_children_scanner()))
 
-def parse_window_expression(scanner: TokenScanner) -> SQLWindowExpression:
-    """解析窗口函数
 
-    TODO 支持 ROW BETWEEN 的语法
+def _parse_in_parenthesis(scanner: TokenScanner) -> SQLGeneralExpression:
+    """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
+    if check_sub_query_parenthesis(scanner):
+        return parse_sub_query_expression(scanner)
+    return parse_value_expression(scanner)
 
-    Examples
-    --------
-    >>> parse_window_expression(build_token_scanner("ROW_NUMBER() OVER (PARTITION BY column1 ORDER BY column2) AS column3"))
-    <SQLWindowExpression source=<SQLFunctionExpression source=ROW_NUMBER()> OVER (PARTITION BY <SQLColumnNameExpression source=column1>ORDER BY <SQLColumnNameExpression source=column2>)>
-    >>> parse_window_expression(build_token_scanner("3 + 5"))
-    Traceback (most recent call last):
-    ...
-    metasequoia_sql.errors.SqlParseError: 无法解析为函数表达式: <TokenScanner tokens=[<ASTLiteralInteger source=3>, <ASTCommon source=+>, <ASTLiteralInteger source=5>], pos=0>
-    """
-    window_function = parse_function_expression(scanner)
-    partition_by = None
-    order_by = None
-    if not scanner.pop().equals("OVER"):
-        raise SqlParseError(f"无法解析为窗口表达式: {scanner}")
-    parenthesis_scanner = scanner.pop_as_children_scanner()
-    if parenthesis_scanner.search_and_move("PARTITION", "BY"):
-        partition_by = parse_general_expression(parenthesis_scanner, maybe_window=False)
-    if parenthesis_scanner.search_and_move("ORDER", "BY"):
-        order_by = parse_general_expression(parenthesis_scanner, maybe_window=False)
-    return SQLWindowExpression(window_function=window_function, partition_by=partition_by, order_by=order_by)
+
+def _parse_general_parenthesis(scanner: TokenScanner) -> SQLGeneralExpression:
+    """解析一般表达式中的插入语：插入语可能为一般表达式或子查询"""
+    if check_sub_query_parenthesis(scanner):
+        return parse_sub_query_expression(scanner)
+    return parse_general_expression(scanner.pop_as_children_scanner())
 
 
 def _parse_general_expression_element(scanner: TokenScanner, maybe_window: bool) -> SQLGeneralExpression:
-    """解析一般表达式中的一个元素"""
-    if maybe_case_expression(scanner):
+    """解析一般表达式中的一个元素
+
+    # TODO 将非一般表达式的子类移出一般表达式
+    """
+    if check_case_expression(scanner):
         return parse_case_expression(scanner)
-    if maybe_window is True and maybe_window_expression(scanner):
+    if maybe_window is True and check_window_expression(scanner):
         return parse_window_expression(scanner)
-    if maybe_function_expression(scanner):
+    if check_function_expression(scanner):
         return parse_function_expression(scanner)
-    if maybe_literal_expression(scanner):
+    if check_literal_expression(scanner):
         return parse_literal_expression(scanner)
-    if maybe_column_name_expression(scanner):
+    if check_column_name_expression(scanner):
         return parse_column_name_expression(scanner)
     if scanner.now_is_parenthesis:
-        return parse_general_parenthesis(scanner)
-    if maybe_wildcard_expression(scanner):
+        return _parse_general_parenthesis(scanner)
+    if check_wildcard_expression(scanner):
         return parse_wildcard_expression(scanner)
     raise SqlParseError(f"未知的一般表达式元素: {scanner}")
 
 
 def parse_general_expression(scanner: TokenScanner, maybe_window: bool = True) -> SQLGeneralExpression:
     """解析一般表达式"""
     elements = [_parse_general_expression_element(scanner, maybe_window)]
-    while not scanner.is_finish and maybe_compute_operator(scanner):
+    while check_compute_operator(scanner):
         elements.append(parse_compute_operator(scanner))
         elements.append(_parse_general_expression_element(scanner, maybe_window))
     if len(elements) > 1:
         return SQLComputeExpression(elements=elements)  # 如果超过 1 个元素，则返回计算表达式（多项式）
     else:
         return elements[0]  # 如果只有 1 个元素，则返回该元素的表达式
 
@@ -709,88 +873,29 @@
             scanner.next1 is not None and scanner.next1.is_dot and
             scanner.next2 is not None and scanner.next2.is_maybe_name and
             (scanner.next3 is None or not scanner.next3.is_parenthesis)):
         schema_name = scanner.pop_as_source()
         scanner.pop()
         table_name = scanner.pop_as_source()
         return SQLTableNameExpression(schema_name, table_name)
-    if is_sub_query_parenthesis(scanner):
-        return parse_sub_query_parenthesis(scanner)
+    if check_sub_query_parenthesis(scanner):
+        return parse_sub_query_expression(scanner)
     raise SqlParseError(f"无法解析为表名表达式: {scanner}")
 
 
-def parse_bool_expression(scanner: TokenScanner) -> SQLBoolExpression:
-    """解析布尔值表达式
-
-    Examples
-    --------
-    >>> parse_bool_expression(build_token_scanner("column1 > 3"))
-    <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_token_scanner("t2.column1 > 3"))
-    <SQLBoolCompareExpression source=<SQLColumnNameExpression source=t2.column1> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_token_scanner("t2.column1 + 3 > 3"))
-    <SQLBoolCompareExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=t2.column1> <SQLPlus> <SQLLiteralExpression source=3>> <SQLGreaterThan> <SQLLiteralExpression source=3>>
-    >>> parse_bool_expression(build_token_scanner("column1 BETWEEN 3 AND 4"))
-    <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column1> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
-    >>> parse_bool_expression(build_token_scanner("column1 + 3 BETWEEN 3 AND 4"))
-    <SQLBoolBetweenExpression source=<SQLComputeExpression source=<SQLColumnNameExpression source=column1> <SQLPlus> <SQLLiteralExpression source=3>> BETWEEN <SQLLiteralExpression source=3> TO <SQLLiteralExpression source=4>>
-    """
-    if scanner.search_and_move("EXISTS"):
-        after_value = parse_sub_query_parenthesis(scanner)
-        return SQLBoolExistsExpression(is_not=False, after_value=after_value)
-    if scanner.search_and_move("NOT", "EXISTS"):
-        after_value = parse_sub_query_parenthesis(scanner)
-        return SQLBoolExistsExpression(is_not=True, after_value=after_value)
-    before_value = parse_general_expression(scanner)
-    if scanner.search_and_move("BETWEEN"):
-        # "... BETWEEN ... AND ..."
-        from_value = parse_general_expression(scanner)
-        if not scanner.search_and_move("AND"):
-            raise SqlParseError(f"无法解析为 BETWEEN 布尔值表达式: {scanner}")
-        to_value = parse_general_expression(scanner)
-        return SQLBoolBetweenExpression(before_value=before_value, from_value=from_value, to_value=to_value)
-    if scanner.search_and_move("IS"):
-        # ".... IS ...." 或 "... IS NOT ..."
-        if scanner.search_and_move("NOT"):
-            is_not = True
-        else:
-            is_not = False
-        after_value = parse_general_expression(scanner)
-        return SQLBoolIsExpression(is_not=is_not, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("IN"):
-        # "... IN (1, 2, 3)" 或 "... IN (SELECT ... )"
-        after_value = parse_in_parenthesis(scanner)
-        return SQLBoolInExpression(is_not=False, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("NOT", "IN"):
-        after_value = parse_in_parenthesis(scanner)
-        return SQLBoolInExpression(is_not=True, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("LIKE"):
-        after_value = parse_general_expression(scanner)
-        return SQLBoolLikeExpression(is_not=False, before_value=before_value, after_value=after_value)
-    if scanner.search_and_move("NOT LIKE"):
-        after_value = parse_general_expression(scanner)
-        return SQLBoolLikeExpression(is_not=True, before_value=before_value, after_value=after_value)
-    if maybe_compare_operator(scanner):
-        # "... > ..."
-        compare_operator = parse_compare_operator(scanner)
-        after_value = parse_general_expression(scanner)
-        return SQLBoolCompareExpression(operator=compare_operator, before_value=before_value, after_value=after_value)
-    raise SqlParseError(f"无法解析为布尔值表达式: {scanner}")
-
-
-def maybe_alias_expression(scanner: TokenScanner) -> bool:
+def check_alias_expression(scanner: TokenScanner) -> bool:
     """判断是否可能为别名表达式
 
     Examples
     --------
-    >>> maybe_alias_expression(build_token_scanner("t1"))
+    >>> check_alias_expression(build_token_scanner("t1"))
     True
-    >>> maybe_alias_expression(build_token_scanner("AS t1"))
+    >>> check_alias_expression(build_token_scanner("AS t1"))
     True
-    >>> maybe_alias_expression(build_token_scanner("WHERE"))
+    >>> check_alias_expression(build_token_scanner("WHERE"))
     False
     """
     return not scanner.is_finish and (scanner.now.equals("AS") or scanner.now.is_maybe_name)
 
 
 def parse_alias_expression(scanner: TokenScanner) -> SQLAlisaExpression:
     """解析别名表达式
@@ -808,42 +913,17 @@
     """
     scanner.search_and_move("AS")
     if not scanner.now.is_maybe_name:
         raise SqlParseError(f"无法解析为别名表达式: {scanner}")
     return SQLAlisaExpression(alias_name=scanner.pop_as_source())
 
 
-def parse_condition_expression(scanner: TokenScanner) -> SQLConditionExpression:
-    """解析条件表达式
-
-    Examples
-    --------
-    >>> parse_condition_expression(build_token_scanner("column1 > 3 AND column2 > 2 WHERE"))
-    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
-    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 > 2 WHERE"))
-    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>
-    >>> parse_condition_expression(build_token_scanner("column1 > 3 OR column2 BETWEEN 2 AND 4 WHERE"))
-    <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>
-    """
-
-    def parse_single():
-        if scanner.search("NOT"):
-            elements.append(parse_logical_operator(scanner))
-        if scanner.now_is_parenthesis:
-            elements.append(parse_condition_expression(scanner.pop_as_children_scanner()))  # 插入语，子句也应该是一个条件表达式
-        else:
-            elements.append(parse_bool_expression(scanner))
-
-    elements: List[Union["SQLConditionExpression", SQLBoolExpression, SQLLogicalOperator]] = []
-    parse_single()  # 解析第 1 个表达式元素
-    while not scanner.is_finish and scanner.now.source.upper() in {"AND", "OR"}:  # 如果是用 AND 和 OR 连接的多个表达式，则继续解析
-        elements.append(parse_logical_operator(scanner))
-        parse_single()
-
-    return SQLConditionExpression(elements=elements)
+def check_join_expression(scanner: TokenScanner) -> bool:
+    """判断是否为关联表达式"""
+    return scanner.search("ON") or scanner.search("USING")
 
 
 def parse_join_on_expression(scanner: TokenScanner) -> SQLJoinOnExpression:
     """解析 ON 关联表达式
 
     Examples
     --------
@@ -866,19 +946,14 @@
     <SQLJoinUsingExpression source=<SQLFunctionExpression source=using(<SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>)>>
     """
     if not scanner.now.equals("USING"):
         raise SqlParseError(f"无法解析为 USING 关联表达式: {scanner}")
     return SQLJoinUsingExpression(using_function=parse_function_expression(scanner))
 
 
-def is_join_expression(scanner: TokenScanner) -> bool:
-    """判断是否为关联表达式"""
-    return scanner.search("ON") or scanner.search("USING")
-
-
 def parse_join_expression(scanner: TokenScanner) -> SQLJoinExpression:
     """解析关联表达式
 
     Examples
     --------
     >>> parse_join_on_expression(build_token_scanner("ON t1.column1 = t2.column2"))
     <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column2>>>>
@@ -890,63 +965,39 @@
     if scanner.search("ON"):
         return parse_join_on_expression(scanner)
     if scanner.search("USING"):
         return parse_join_using_expression(scanner)
     raise SqlParseError(f"无法解析为关联表达式: {scanner}")
 
 
-def maybe_wildcard_expression(scanner: TokenScanner) -> bool:
-    """判断是否可能为通配符表达式
-
-    Examples
-    --------
-    >>> maybe_wildcard_expression(build_token_scanner("*"))
-    True
-    >>> maybe_wildcard_expression(build_token_scanner("t1.*"))
-    True
-    """
-    return not scanner.is_finish and (scanner.now.is_maybe_wildcard or
-                                      (scanner.now.is_maybe_name and
-                                       scanner.next1 is not None and scanner.next1.is_dot and
-                                       scanner.next2 is not None and scanner.next2.is_maybe_wildcard))
-
-
-def parse_wildcard_expression(scanner: TokenScanner) -> SQLWildcardExpression:
-    """解析通配符表达式
+def parse_column_type_expression(scanner: TokenScanner) -> SQLColumnTypeExpression:
+    """解析 DDL 的字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
+    # 解析字段类型名称
+    function_name: str = scanner.pop_as_source()
 
-    Examples
-    --------
-    >>> parse_wildcard_expression(build_token_scanner("*"))
-    <SQLWildcardExpression source=*>
-    >>> parse_wildcard_expression(build_token_scanner("t1.*"))
-    <SQLWildcardExpression source=t1.*>
-    """
-    if scanner.now.is_maybe_wildcard:
-        scanner.pop()
-        return SQLWildcardExpression(schema=None)
-    if (scanner.now.is_maybe_name and
-            scanner.next1 is not None and scanner.next1.is_dot and
-            scanner.next2 is not None and scanner.next2.is_maybe_wildcard):
-        schema_name = scanner.pop_as_source()
-        scanner.pop()
-        scanner.pop()
-        return SQLWildcardExpression(schema=schema_name)
-    raise SqlParseError("无法解析为通配符表达式")
+    # 解析字段类型参数
+    if not scanner.is_finish and scanner.now_is_parenthesis:
+        function_params: List[SQLGeneralExpression] = []
+        for param_scanner in scanner.pop_as_children_scanner_list_split_by(","):
+            function_params.append(parse_general_expression(param_scanner))
+        return SQLColumnTypeExpression(function_name, function_params)
+    else:
+        return SQLColumnTypeExpression(function_name, [])
 
 
 def parse_table_expression(scanner: TokenScanner) -> SQLTableExpression:
     """解析表名表达式
 
     Examples
     --------
     >>> parse_table_expression(build_token_scanner("schema1.table1 AS t1"))
     <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>
     """
     table_name_expression = parse_table_name_expression(scanner)
-    alias_expression = parse_alias_expression(scanner) if maybe_alias_expression(scanner) else None
+    alias_expression = parse_alias_expression(scanner) if check_alias_expression(scanner) else None
     return SQLTableExpression(table=table_name_expression, alias=alias_expression)
 
 
 def parse_column_expression(scanner: TokenScanner) -> SQLColumnExpression:
     """解析列名表达式
 
     Examples
@@ -955,182 +1006,325 @@
     <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column1>)> AS <SQLAlisaExpression source=AS t1>>
     >>> parse_column_expression(build_token_scanner("3 + 5 AS t1"))
     <SQLColumnExpression source=<SQLComputeExpression source=<SQLLiteralExpression source=3> <SQLPlus> <SQLLiteralExpression source=5>> AS <SQLAlisaExpression source=AS t1>>
     >>> parse_column_expression(build_token_scanner("TRIM(column1) AS t1"))
     <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column1>)> AS <SQLAlisaExpression source=AS t1>>
     """
     general_expression = parse_general_expression(scanner)
-    alias_expression = parse_alias_expression(scanner) if maybe_alias_expression(scanner) else None
+    alias_expression = parse_alias_expression(scanner) if check_alias_expression(scanner) else None
     return SQLColumnExpression(column=general_expression, alias=alias_expression)
 
 
-def parse_value_expression(scanner: TokenScanner) -> SQLValueExpression:
-    """解析值表达式"""
-    values = []
-    for value_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-        values.append(parse_general_expression(value_scanner))
-    return SQLValueExpression(values=values)
-
-
 def parse_equal_expression(scanner: TokenScanner) -> SQLEqualExpression:
     """解析等式表达式"""
     before_value = parse_general_expression(scanner)
     scanner.match("=")
     after_value = parse_general_expression(scanner)
     return SQLEqualExpression(before_value=before_value, after_value=after_value)
 
 
-def is_partition_expression(scanner: TokenScanner) -> bool:
+def check_partition_expression(scanner: TokenScanner) -> bool:
     """判断是否可能为分区表达式"""
     return scanner.search("PARTITION")
 
 
 def parse_partition_expression(scanner: TokenScanner) -> SQLPartitionExpression:
     """解析分区表达式"""
     scanner.match("PARTITION")
     partition_list = []
     for partition_scanner in scanner.pop_as_children_scanner_list_split_by(","):
         partition_list.append(parse_equal_expression(partition_scanner))
     return SQLPartitionExpression(partition_list=partition_list)
 
 
-def maybe_limit_clause(scanner: TokenScanner) -> bool:
-    """是否可能为 LIMIT 子句
+def check_foreign_key_expression(scanner: TokenScanner) -> bool:
+    """判断是否为外键表达式"""
+    return scanner.search("CONSTRAINT")
+
+
+def parse_foreign_key_expression(scanner: TokenScanner) -> SQLForeignKeyExpression:
+    """解析外键表达式"""
+    scanner.match("CONSTRAINT")
+    constraint_name = scanner.pop_as_source()
+    scanner.match("FOREIGN", "KEY")
+    slave_columns = [column_scanner.pop_as_source()
+                     for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    scanner.match("REFERENCES")
+    master_table_name = scanner.pop_as_source()
+    master_columns = [column_scanner.pop_as_source()
+                      for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return SQLForeignKeyExpression(
+        constraint_name=constraint_name,
+        slave_columns=slave_columns,
+        master_table_name=master_table_name,
+        master_columns=master_columns
+    )
+
+
+def check_primary_index_expression(scanner: TokenScanner) -> bool:
+    """判断是否为主键表达式"""
+    return scanner.search("PRIMARY", "KEY")
+
+
+def parse_primary_index_expression(scanner: TokenScanner) -> SQLPrimaryIndexExpression:
+    """解析主键表达式"""
+    scanner.match("PRIMARY", "KEY")
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return SQLPrimaryIndexExpression(columns=columns)
+
+
+def check_unique_index_expression(scanner: TokenScanner) -> bool:
+    """判断是否为唯一键表达式"""
+    return scanner.search("UNIQUE", "KEY")
+
+
+def parse_unique_index_expression(scanner: TokenScanner) -> SQLUniqueIndexExpression:
+    """解析唯一键表达式"""
+    scanner.match("UNIQUE", "KEY")
+    name = scanner.pop_as_source()
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return SQLUniqueIndexExpression(name=name, columns=columns)
+
+
+def check_normal_index_expression(scanner: TokenScanner) -> bool:
+    """判断是否为一般索引表达式"""
+    return scanner.search("KEY")
+
+
+def parse_normal_index_expression(scanner: TokenScanner) -> SQLNormalIndexExpression:
+    """解析一般索引表达式"""
+    scanner.match("KEY")
+    name = scanner.pop_as_source()
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return SQLNormalIndexExpression(name=name, columns=columns)
+
+
+def check_fulltext_expression(scanner: TokenScanner) -> bool:
+    """判断是否为全文索引表达式"""
+    return scanner.search("FULLTEXT", "KEY")
+
+
+def parse_fulltext_expression(scanner: TokenScanner) -> SQLFulltextIndexExpression:
+    """解析全文索引表达式"""
+    scanner.match("FULLTEXT", "KEY")
+    name = scanner.pop_as_source()
+    columns = [column_scanner.pop_as_source()
+               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
+    return SQLFulltextIndexExpression(name=name, columns=columns)
+
+
+def parse_define_column_expression(scanner: TokenScanner) -> SQLDefineColumnExpression:
+    """解析 DDL 的字段表达式"""
+    # 解析顺序固定的信息
+    column_name = scanner.pop_as_source()
+    column_type = parse_column_type_expression(scanner)
+
+    # 解析顺序可能不定的字段信息
+    comment: Optional[str] = None
+    is_unsigned: bool = False
+    is_zerofill: bool = False
+    character_set: Optional[str] = None
+    collate: Optional[str] = None
+    is_allow_null: bool = False
+    is_not_null: bool = False
+    is_auto_increment: bool = False
+    default: Optional[SQLGeneralExpression] = None
+    on_update: Optional[SQLGeneralExpression] = None
+    while not scanner.is_finish:
+        if scanner.search_and_move("NOT", "NULL"):
+            is_not_null = True
+        elif scanner.search_and_move("NULL"):
+            is_allow_null = True
+        elif scanner.search_and_move("CHARACTER", "SET"):
+            character_set = scanner.pop_as_source()
+        elif scanner.search_and_move("COLLATE"):
+            collate = scanner.pop_as_source()
+        elif scanner.search_and_move("DEFAULT"):
+            default = parse_general_expression(scanner)
+        elif scanner.search_and_move("COMMENT"):
+            comment = scanner.pop_as_source()
+        elif scanner.search_and_move("ON", "UPDATE"):  # ON UPDATE
+            on_update = parse_general_expression(scanner)
+        elif scanner.search_and_move("AUTO_INCREMENT"):
+            is_auto_increment = True
+        elif scanner.search_and_move("UNSIGNED"):
+            is_unsigned = True
+        elif scanner.search_and_move("ZEROFILL"):
+            is_zerofill = True
+        else:
+            raise SqlParseError(f"无法解析的 DDL 字段表达式的字段属性: {scanner}")
+
+    # 构造 DDL 字段表达式对象
+    return SQLDefineColumnExpression(
+        column_name=column_name,
+        column_type=column_type,
+        comment=comment,
+        is_unsigned=is_unsigned,
+        is_zerofill=is_zerofill,
+        character_set=character_set,
+        collate=collate,
+        is_allow_null=is_allow_null,
+        is_not_null=is_not_null,
+        is_auto_increment=is_auto_increment,
+        default=default,
+        on_update=on_update
+    )
+
+
+def check_select_clause(scanner: TokenScanner) -> bool:
+    """判断是否为 SELECT 子句
 
     Examples
     --------
-    >>> maybe_limit_clause(build_token_scanner("LIMIT 2, 5"))
+    >>> check_from_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
     True
-    >>> maybe_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
+    >>> check_from_clause(build_token_scanner("SELECT column1 AS c1"))
     True
-    >>> maybe_limit_clause(build_token_scanner("ORDER BY column1"))
+    >>> check_from_clause(build_token_scanner("FROM table1"))
     False
     """
-    return scanner.search("LIMIT")
+    return scanner.search("SELECT")
 
 
-def parse_limit_clause(scanner: TokenScanner) -> SQLLimitClause:
-    """解析 LIMIT 子句
+def parse_select_clause(scanner: TokenScanner) -> SQLSelectClause:
+    """解析 SELECT 子句
 
     Examples
     --------
-    >>> parse_limit_clause(build_token_scanner("LIMIT 2, 5"))
-    <SQLLimitClause source=LIMIT 2, 5>
-    >>> parse_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
-    <SQLLimitClause source=LIMIT 2, 5>
+    >>> parse_select_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
+    <SQLSelectClause source=SELECT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>,
+    <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column2>)> AS <SQLAlisaExpression source=AS c2>>>
+    >>> parse_select_clause(build_token_scanner("SELECT DISTINCT column1 AS c1"))
+    <SQLSelectClause source=SELECT DISTINCT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>>
     """
-    if not scanner.search_and_move("LIMIT"):
-        raise SqlParseError("无法解析为 LIMIT 子句")
-    cnt_1 = parse_literal_expression(scanner).as_int()
-    mark = scanner.pop()
-    if mark.is_comma:
-        offset_int = cnt_1
-        limit_int = parse_literal_expression(scanner).as_int()
-    elif mark.equals("OFFSET"):
-        offset_int = parse_literal_expression(scanner).as_int()
-        limit_int = cnt_1
-    else:
-        raise SqlParseError("无法解析为 LIMIT 子句")
 
-    return SQLLimitClause(limit=limit_int, offset=offset_int)
+    scanner.match("SELECT")
+    distinct = scanner.search_and_move("DISTINCT")
+    columns = [parse_column_expression(scanner)]
+    while not scanner.is_finish and scanner.now.is_comma:
+        scanner.pop()
+        columns.append(parse_column_expression(scanner))
+    return SQLSelectClause(distinct=distinct, columns=columns)
 
 
-def maybe_order_by_clause(scanner: TokenScanner) -> bool:
-    """是否可能为 ORDER BY 子句
+def check_from_clause(scanner: TokenScanner) -> bool:
+    """判断是否为 FROM 子句
 
     Examples
     --------
-    >>> maybe_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
-    True
-    >>> maybe_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
+    >>> check_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
     True
-    >>> maybe_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
+    >>> check_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
     True
-    >>> maybe_order_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
+    >>> check_from_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
     False
     """
-    return scanner.search("ORDER", "BY")
+    return scanner.search("FROM")
 
 
-def parse_order_by_clause(scanner: TokenScanner) -> SQLOrderByClause:
-    """解析 ORDER BY 子句
+def parse_from_clause(scanner: TokenScanner) -> SQLFromClause:
+    """解析 FROM 子句
 
     Examples
     --------
-    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
-    <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
-    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
-    <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2> DESC>
-    >>> parse_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
-    <SQLOrderByClause source=ORDER BY <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column1>)>>
+    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
+    <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>>
+    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
+    <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>, <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>>>
     """
-
-    def parse_single():
-        column = parse_general_expression(scanner)
-        if not scanner.is_finish and scanner.search_and_move("DESC"):
-            order = SQLEnumOrderType.DESC
-        else:
-            order = SQLEnumOrderType.ASC
-        columns.append((column, order))
-
-    scanner.match("ORDER", "BY")
-    columns = []
-    parse_single()
+    scanner.match("FROM")
+    tables = [parse_table_expression(scanner)]
     while not scanner.is_finish and scanner.now.is_comma:
         scanner.pop()
-        parse_single()
+        tables.append(parse_table_expression(scanner))
+    return SQLFromClause(tables=tables)
 
-    return SQLOrderByClause(columns=columns)
 
+def check_join_clause(scanner: TokenScanner) -> bool:
+    """判断是否为 JOIN 子句
+
+    Examples
+    --------
+    >>> check_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
+    True
+    >>> check_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
+    True
+    >>> check_join_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    False
+    """
+    return check_join_type(scanner)
 
-def maybe_having_clause(scanner: TokenScanner) -> bool:
-    """是否可能为 HAVING 子句
+
+def parse_join_clause(scanner: TokenScanner) -> SQLJoinClause:
+    """解析 JOIN 子句
+
+    Examples
+    --------
+    >>> parse_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
+    <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
+    >>> parse_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
+    <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
+    """
+    join_type = parse_join_type(scanner)
+    table_expression = parse_table_expression(scanner)
+    if check_join_expression(scanner):
+        join_rule = parse_join_expression(scanner)
+    else:
+        join_rule = None
+    return SQLJoinClause(join_type=join_type, table=table_expression, join_rule=join_rule)
+
+
+def check_where_clause(scanner: TokenScanner) -> bool:
+    """判断是否可能为 WHERE 子句
 
     Examples
     --------
-    >>> maybe_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
+    >>> check_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
     True
-    >>> maybe_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
+    >>> check_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
     True
-    >>> maybe_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> check_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
     True
-    >>> maybe_having_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> check_where_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
     False
     """
-    return scanner.search("HAVING")
+    return scanner.search("WHERE")
 
 
-def parse_having_clause(scanner: TokenScanner) -> SQLHavingClause:
-    """解析 HAVING 子句
+def parse_where_clause(scanner: TokenScanner) -> SQLWhereClause:
+    """解析 WHERE 子句
 
     Examples
     --------
-    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
-    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
-    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
+    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
+    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
+    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
+    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
+    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
     """
-    scanner.match("HAVING")
-    return SQLHavingClause(condition=parse_condition_expression(scanner))
+    scanner.match("WHERE")
+    return SQLWhereClause(condition=parse_condition_expression(scanner))
 
 
-def maybe_group_by_clause(scanner: TokenScanner) -> bool:
+def check_group_by_clause(scanner: TokenScanner) -> bool:
     """判断是否可能为 GROUP BY 子句
 
     Examples
     --------
-    >>> maybe_group_by_clause(build_token_scanner("GROUP BY column1, column2"))
+    >>> check_group_by_clause(build_token_scanner("GROUP BY column1, column2"))
     True
-    >>> maybe_group_by_clause(build_token_scanner("GROUP BY column1, column2 DESC"))
+    >>> check_group_by_clause(build_token_scanner("GROUP BY column1, column2 DESC"))
     True
-    >>> maybe_group_by_clause(build_token_scanner("GROUP BY trim(column1) ASC, column2"))
+    >>> check_group_by_clause(build_token_scanner("GROUP BY trim(column1) ASC, column2"))
     True
-    >>> maybe_group_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
+    >>> check_group_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
     False
     """
     return scanner.search("GROUP", "BY")
 
 
 def parse_group_by_clause(scanner: TokenScanner) -> SQLGroupByClause:
     """解析 GROUP BY 子句
@@ -1163,179 +1357,131 @@
             columns.append(parse_general_expression(scanner))
         with_rollup = False
         if scanner.search_and_move("WITH", "ROLLUP"):
             with_rollup = True
         return SQLNormalGroupByClause(columns=columns, with_rollup=with_rollup)
 
 
-def maybe_where_clause(scanner: TokenScanner) -> bool:
-    """判断是否可能为 WHERE 子句
+def check_having_clause(scanner: TokenScanner) -> bool:
+    """是否可能为 HAVING 子句
 
     Examples
     --------
-    >>> maybe_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
+    >>> check_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
     True
-    >>> maybe_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
+    >>> check_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
     True
-    >>> maybe_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> check_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
     True
-    >>> maybe_where_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> check_having_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
     False
     """
-    return scanner.search("WHERE")
+    return scanner.search("HAVING")
 
 
-def parse_where_clause(scanner: TokenScanner) -> SQLWhereClause:
-    """解析 WHERE 子句
+def parse_having_clause(scanner: TokenScanner) -> SQLHavingClause:
+    """解析 HAVING 子句
 
     Examples
     --------
-    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 AND column2 > 2"))
-    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 > 2"))
-    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
-    >>> parse_where_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
-    <SQLWhereClause source=WHERE <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
+    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 AND column2 > 2"))
+    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLAndOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
+    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 > 2"))
+    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolCompareExpression source=<SQLColumnNameExpression source=column2> <SQLGreaterThan> <SQLLiteralExpression source=2>>>>
+    >>> parse_having_clause(build_token_scanner("HAVING column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    <SQLHavingClause source=HAVING <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=column1> <SQLGreaterThan> <SQLLiteralExpression source=3>> <SQLOrOperator> <SQLBoolBetweenExpression source=<SQLColumnNameExpression source=column2> BETWEEN <SQLLiteralExpression source=2> TO <SQLLiteralExpression source=4>>>>
     """
-    scanner.match("WHERE")
-    return SQLWhereClause(condition=parse_condition_expression(scanner))
+    scanner.match("HAVING")
+    return SQLHavingClause(condition=parse_condition_expression(scanner))
 
 
-def maybe_join_clause(scanner: TokenScanner) -> bool:
-    """判断是否为 JOIN 子句
+def check_order_by_clause(scanner: TokenScanner) -> bool:
+    """是否可能为 ORDER BY 子句
 
     Examples
     --------
-    >>> maybe_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
+    >>> check_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
+    True
+    >>> check_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
     True
-    >>> maybe_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
+    >>> check_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
     True
-    >>> maybe_join_clause(build_token_scanner("WHERE column1 > 3 OR column2 BETWEEN 2 AND 4"))
+    >>> check_order_by_clause(build_token_scanner("WHERE trim(column1) IS NOT NULL"))
     False
     """
-    return (scanner.search("JOIN") or
-            scanner.search("INNER", "JOIN") or
-            scanner.search("LEFT", "JOIN") or
-            scanner.search("LEFT", "OUTER", "JOIN") or
-            scanner.search("RIGHT", "JOIN") or
-            scanner.search("RIGHT", "OUTER", "JOIN") or
-            scanner.search("FULL", "JOIN") or
-            scanner.search("FULL", "OUTER", "JOIN") or
-            scanner.search("CROSS", "JOIN"))
-
-
-def _parse_join_type(scanner: TokenScanner) -> SQLEnumJoinType:
-    """解析关联类型"""
-    if scanner.search_and_move("JOIN"):
-        return SQLEnumJoinType.JOIN
-    if scanner.search_and_move("INNER", "JOIN"):
-        return SQLEnumJoinType.INNER_JOIN
-    if scanner.search_and_move("LEFT", "JOIN"):
-        return SQLEnumJoinType.LEFT_JOIN
-    if scanner.search_and_move("LEFT", "OUTER", "JOIN"):
-        return SQLEnumJoinType.LEFT_OUTER_JOIN
-    if scanner.search_and_move("RIGHT", "JOIN"):
-        return SQLEnumJoinType.RIGHT_JOIN
-    if scanner.search_and_move("RIGHT", "OUTER", "JOIN"):
-        return SQLEnumJoinType.RIGHT_OUTER_JOIN
-    if scanner.search_and_move("FULL", "JOIN"):
-        return SQLEnumJoinType.FULL_JOIN
-    if scanner.search_and_move("FULL", "OUTER", "JOIN"):
-        return SQLEnumJoinType.FULL_OUTER_JOIN
-    if scanner.search_and_move("CROSS", "JOIN"):
-        return SQLEnumJoinType.CROSS_JOIN
-    raise SqlParseError(f"无法解析的关联类型: {scanner}")
-
-
-def parse_join_clause(scanner: TokenScanner) -> SQLJoinClause:
-    """解析 JOIN 子句
-
-    Examples
-    --------
-    >>> parse_join_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
-    <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
-    >>> parse_join_clause(build_token_scanner("LEFT JOIN schema2.table2 AS t2 ON t1.column1 = t2.column1"))
-    <SQLJoinClause source=LEFT JOIN <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>> <SQLJoinOnExpression source=ON <SQLConditionExpression source=<SQLBoolCompareExpression source=<SQLColumnNameExpression source=t1.column1> <SQLEqualTo> <SQLColumnNameExpression source=t2.column1>>>>>
-    """
-    join_type = _parse_join_type(scanner)
-    table_expression = parse_table_expression(scanner)
-    if is_join_expression(scanner):
-        join_rule = parse_join_expression(scanner)
-    else:
-        join_rule = None
-    return SQLJoinClause(join_type=join_type, table=table_expression, join_rule=join_rule)
+    return scanner.search("ORDER", "BY")
 
 
-def maybe_from_clause(scanner: TokenScanner) -> bool:
-    """判断是否为 FROM 子句
+def parse_order_by_clause(scanner: TokenScanner) -> SQLOrderByClause:
+    """解析 ORDER BY 子句
 
     Examples
     --------
-    >>> maybe_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
-    True
-    >>> maybe_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
-    True
-    >>> maybe_from_clause(build_token_scanner("LEFT JOIN table2 AS t2 ON t1.column1 = t2.column1"))
-    False
+    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2"))
+    <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2>>
+    >>> parse_order_by_clause(build_token_scanner("ORDER BY column1, column2 DESC"))
+    <SQLOrderByClause source=ORDER BY <SQLColumnNameExpression source=column1>, <SQLColumnNameExpression source=column2> DESC>
+    >>> parse_order_by_clause(build_token_scanner("ORDER BY trim(column1) ASC, column2"))
+    <SQLOrderByClause source=ORDER BY <SQLFunctionExpression source=trim(<SQLColumnNameExpression source=column1>)>>
     """
-    return scanner.search("FROM")
-
 
-def parse_from_clause(scanner: TokenScanner) -> SQLFromClause:
-    """解析 FROM 子句
+    def parse_single():
+        column = parse_general_expression(scanner)
+        order = parse_order_type(scanner)
+        columns.append((column, order))
 
-    Examples
-    --------
-    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1"))
-    <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>>
-    >>> parse_from_clause(build_token_scanner("FROM schema1.table1 AS t1, schema2.table2 AS t2"))
-    <SQLFromClause source=FROM <SQLTableExpression source=<SQLTableNameExpression source=schema1.table1> AS <SQLAlisaExpression source=AS t1>>, <SQLTableExpression source=<SQLTableNameExpression source=schema2.table2> AS <SQLAlisaExpression source=AS t2>>>
-    """
-    scanner.match("FROM")
-    tables = [parse_table_expression(scanner)]
+    scanner.match("ORDER", "BY")
+    columns = []
+    parse_single()
     while not scanner.is_finish and scanner.now.is_comma:
         scanner.pop()
-        tables.append(parse_table_expression(scanner))
-    return SQLFromClause(tables=tables)
+        parse_single()
 
+    return SQLOrderByClause(columns=columns)
 
-def maybe_select_clause(scanner: TokenScanner) -> bool:
-    """判断是否为 SELECT 子句
+
+def check_limit_clause(scanner: TokenScanner) -> bool:
+    """是否可能为 LIMIT 子句
 
     Examples
     --------
-    >>> maybe_from_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
+    >>> check_limit_clause(build_token_scanner("LIMIT 2, 5"))
     True
-    >>> maybe_from_clause(build_token_scanner("SELECT column1 AS c1"))
+    >>> check_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
     True
-    >>> maybe_from_clause(build_token_scanner("FROM table1"))
+    >>> check_limit_clause(build_token_scanner("ORDER BY column1"))
     False
     """
-    return scanner.search("SELECT")
+    return scanner.search("LIMIT")
 
 
-def parse_select_clause(scanner: TokenScanner) -> SQLSelectClause:
-    """解析 SELECT 子句
+def parse_limit_clause(scanner: TokenScanner) -> SQLLimitClause:
+    """解析 LIMIT 子句
 
     Examples
     --------
-    >>> parse_select_clause(build_token_scanner("SELECT column1 AS c1, TRIM(column2) AS c2 FROM table1"))
-    <SQLSelectClause source=SELECT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>,
-    <SQLColumnExpression source=<SQLFunctionExpression source=TRIM(<SQLColumnNameExpression source=column2>)> AS <SQLAlisaExpression source=AS c2>>>
-    >>> parse_select_clause(build_token_scanner("SELECT DISTINCT column1 AS c1"))
-    <SQLSelectClause source=SELECT DISTINCT <SQLColumnExpression source=<SQLColumnNameExpression source=column1> AS <SQLAlisaExpression source=AS c1>>>
+    >>> parse_limit_clause(build_token_scanner("LIMIT 2, 5"))
+    <SQLLimitClause source=LIMIT 2, 5>
+    >>> parse_limit_clause(build_token_scanner("LIMIT 5 OFFSET 2"))
+    <SQLLimitClause source=LIMIT 2, 5>
     """
+    if not scanner.search_and_move("LIMIT"):
+        raise SqlParseError("无法解析为 LIMIT 子句")
+    cnt_1 = parse_literal_expression(scanner).as_int()
+    mark = scanner.pop()
+    if mark.is_comma:
+        offset_int = cnt_1
+        limit_int = parse_literal_expression(scanner).as_int()
+    elif mark.equals("OFFSET"):
+        offset_int = parse_literal_expression(scanner).as_int()
+        limit_int = cnt_1
+    else:
+        raise SqlParseError("无法解析为 LIMIT 子句")
 
-    scanner.match("SELECT")
-    distinct = scanner.search_and_move("DISTINCT")
-    columns = [parse_column_expression(scanner)]
-    while not scanner.is_finish and scanner.now.is_comma:
-        scanner.pop()
-        columns.append(parse_column_expression(scanner))
-    return SQLSelectClause(distinct=distinct, columns=columns)
+    return SQLLimitClause(limit=limit_int, offset=offset_int)
 
 
 def _parse_single_with_table(scanner: TokenScanner) -> Tuple[str, SQLSelectStatement]:
     """解析一个 WITH 临时表"""
     table_name = scanner.pop_as_source()
     scanner.match("AS")
     table_statement = parse_select_statement(scanner.pop_as_children_scanner(), with_clause=SQLWithClause.empty())
@@ -1350,15 +1496,15 @@
             table_statement = _parse_single_with_table(scanner)
             tables.append(table_statement)  # 将前置的 WITH 作为当前解析临时表的 WITH 子句
         return SQLWithClause(tables=tables)
     else:
         return SQLWithClause.empty()
 
 
-def maybe_select_statement(scanner: TokenScanner) -> bool:
+def check_select_statement(scanner: TokenScanner) -> bool:
     """判断是否可能为 SELECT 语句"""
     return scanner.search("SELECT")
 
 
 def parse_single_select_statement(scanner: TokenScanner,
                                   with_clause: Optional[SQLWithClause] = None
                                   ) -> SQLSingleSelectStatement:
@@ -1374,90 +1520,72 @@
     Returns
     -------
 
     """
     if with_clause is None:
         with_clause = parse_with_clause(scanner)
     select_clause = parse_select_clause(scanner)
-    from_clause = parse_from_clause(scanner) if maybe_from_clause(scanner) else None
+    from_clause = parse_from_clause(scanner) if check_from_clause(scanner) else None
     join_clause = []
-    while maybe_join_clause(scanner):
+    while check_join_clause(scanner):
         join_clause.append(parse_join_clause(scanner))
-    where_clause = parse_where_clause(scanner) if maybe_where_clause(scanner) else None
-    group_by_clause = parse_group_by_clause(scanner) if maybe_group_by_clause(scanner) else None
-    having_clause = parse_having_clause(scanner) if maybe_having_clause(scanner) else None
-    order_by_clause = parse_order_by_clause(scanner) if maybe_order_by_clause(scanner) else None
-    limit_clause = parse_limit_clause(scanner) if maybe_limit_clause(scanner) else None
+    where_clause = parse_where_clause(scanner) if check_where_clause(scanner) else None
+    group_by_clause = parse_group_by_clause(scanner) if check_group_by_clause(scanner) else None
+    having_clause = parse_having_clause(scanner) if check_having_clause(scanner) else None
+    order_by_clause = parse_order_by_clause(scanner) if check_order_by_clause(scanner) else None
+    limit_clause = parse_limit_clause(scanner) if check_limit_clause(scanner) else None
     return SQLSingleSelectStatement(
         with_clause=with_clause,
         select_clause=select_clause,
         from_clause=from_clause,
         join_clauses=join_clause,
         where_clause=where_clause,
         group_by_clause=group_by_clause,
         having_clause=having_clause,
         order_by_clause=order_by_clause,
         limit_clause=limit_clause
     )
 
 
-def is_select_statement(scanner: TokenScanner) -> bool:
-    """判断是否为 SELECT 语句（已匹配过 WITH 语句后才可以调用）"""
-    return scanner.search("SELECT")
-
-
 def parse_select_statement(scanner: TokenScanner,
                            with_clause: Optional[SQLWithClause] = None) -> SQLSelectStatement:
     """解析 SELECT 语句"""
     if with_clause is None:
         with_clause = parse_with_clause(scanner)
     result = [parse_single_select_statement(scanner, with_clause=with_clause)]
-    while not scanner.is_finish:
-        for union_type in SQLEnumUnionType:
-            if scanner.search_and_move(*union_type.value):
-                result.append(SQLUnionKeyword(union_type=union_type))
-                result.append(parse_single_select_statement(scanner, with_clause=with_clause))
-                break
-        else:
-            break
+    while not scanner.is_finish and check_union_type(scanner):
+        result.append(parse_union_type(scanner))
+        result.append(parse_single_select_statement(scanner, with_clause=with_clause))
     scanner.search_and_move(";")
     if not scanner.is_finish:
         raise SqlParseError(f"没有解析完成: {scanner}")
 
     if len(result) > 1:
         return SQLUnionSelectStatement(with_clause=with_clause, elements=result)
     else:
         return result[0]
 
 
-def is_insert_statement(scanner: TokenScanner) -> bool:
+def check_insert_statement(scanner: TokenScanner) -> bool:
     """判断是否为 INSERT 语句（已匹配过 WITH 语句才可以调用）"""
     return scanner.search("INSERT")
 
 
 def parse_insert_statement(scanner: TokenScanner, with_clause: SQLWithClause) -> SQLInsertStatement:
     """解析 INSERT 表达式"""
-    scanner.match("INSERT")
-
-    # 解析 INSERT 类型
-    if scanner.search_and_move("INTO"):
-        insert_type = SQLInsertType.INSERT_INTO
-    elif scanner.search_and_move("OVERWRITE"):
-        insert_type = SQLInsertType.INSERT_OVERWRITE
-    else:
-        raise SqlParseError(f"未知的 INSERT 类型: {scanner}")
+    insert_type = parse_insert_type(scanner)
 
     # 匹配可能包含的 TABLE 关键字
     has_table_keyword = scanner.search_and_move("TABLE")
 
     # 匹配表名
     table_name = parse_table_name_expression(scanner)
 
     # 匹配分区表达式
-    if is_partition_expression(scanner):
+    if check_partition_expression(scanner):
         partition = parse_partition_expression(scanner)
     else:
         partition = None
 
     # 匹配列名列表
     if scanner.now_is_parenthesis:
         columns = []
@@ -1494,240 +1622,40 @@
             table_name=table_name,
             partition=partition,
             columns=columns,
             select_statement=select_statement
         )
 
 
-def is_sub_query_parenthesis(scanner: TokenScanner) -> bool:
-    """判断是否为子查询的插入语"""
-    parenthesis_scanner: TokenScanner = scanner.get_as_children_scanner()
-    return maybe_select_statement(parenthesis_scanner)
-
-
-def parse_sub_query_parenthesis(scanner: TokenScanner) -> SQLSubQueryExpression:
-    """解析子查询的插入语"""
-    return SQLSubQueryExpression(select_statement=parse_select_statement(scanner.pop_as_children_scanner()))
-
-
-def parse_general_parenthesis(scanner: TokenScanner) -> SQLGeneralExpression:
-    """解析一般表达式中的插入语：插入语可能为一般表达式或子查询"""
-    if is_sub_query_parenthesis(scanner):
-        return parse_sub_query_parenthesis(scanner)
-    return parse_general_expression(scanner.pop_as_children_scanner())
-
-
-def parse_in_parenthesis(scanner: TokenScanner) -> SQLGeneralExpression:
-    """解析 IN 关键字后的插入语：插入语可能为子查询或值表达式"""
-    if is_sub_query_parenthesis(scanner):
-        return parse_sub_query_parenthesis(scanner)
-    return parse_value_expression(scanner)
-
-
-def parse_ddl_column_type_expression(scanner: TokenScanner) -> DDLColumnTypeExpression:
-    """解析 DDL 的字段类型：要求当前指针位置节点为函数名，下一个节点可能为函数参数也可能不是，解析为 SQLColumnType 对象"""
-    # 解析字段类型名称
-    function_name: str = scanner.pop_as_source()
-
-    # 解析字段类型参数
-    if not scanner.is_finish and scanner.now_is_parenthesis:
-        function_params: List[SQLGeneralExpression] = []
-        for param_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-            function_params.append(parse_general_expression(param_scanner))
-        return DDLColumnTypeExpression(function_name, function_params)
-    else:
-        return DDLColumnTypeExpression(function_name, [])
-
-
-def parse_ddl_column_expression(scanner: TokenScanner) -> DDLColumnExpression:
-    """解析 DDL 的字段表达式"""
-    # 解析顺序固定的信息
-    column_name = scanner.pop_as_source()
-    column_type = parse_ddl_column_type_expression(scanner)
-
-    # 解析顺序可能不定的字段信息
-    comment: Optional[str] = None
-    is_unsigned: bool = False
-    is_zerofill: bool = False
-    character_set: Optional[str] = None
-    collate: Optional[str] = None
-    is_allow_null: bool = False
-    is_not_null: bool = False
-    is_auto_increment: bool = False
-    default: Optional[SQLGeneralExpression] = None
-    on_update: Optional[SQLGeneralExpression] = None
-    while not scanner.is_finish:
-        if scanner.search_and_move("NOT", "NULL"):
-            is_not_null = True
-        elif scanner.search_and_move("NULL"):
-            is_allow_null = True
-        elif scanner.search_and_move("CHARACTER", "SET"):
-            character_set = scanner.pop_as_source()
-        elif scanner.search_and_move("COLLATE"):
-            collate = scanner.pop_as_source()
-        elif scanner.search_and_move("DEFAULT"):
-            default = parse_general_expression(scanner)
-        elif scanner.search_and_move("COMMENT"):
-            comment = scanner.pop_as_source()
-        elif scanner.search_and_move("ON", "UPDATE"):  # ON UPDATE
-            on_update = parse_general_expression(scanner)
-        elif scanner.search_and_move("AUTO_INCREMENT"):
-            is_auto_increment = True
-        elif scanner.search_and_move("UNSIGNED"):
-            is_unsigned = True
-        elif scanner.search_and_move("ZEROFILL"):
-            is_zerofill = True
-        else:
-            raise SqlParseError(f"无法解析的 DDL 字段表达式的字段属性: {scanner}")
-
-    # 构造 DDL 字段表达式对象
-    return DDLColumnExpression(
-        column_name=column_name,
-        column_type=column_type,
-        comment=comment,
-        is_unsigned=is_unsigned,
-        is_zerofill=is_zerofill,
-        character_set=character_set,
-        collate=collate,
-        is_allow_null=is_allow_null,
-        is_not_null=is_not_null,
-        is_auto_increment=is_auto_increment,
-        default=default,
-        on_update=on_update
-    )
-
-
-def is_ddl_primary_index_expression(scanner: TokenScanner) -> bool:
-    """判断是否为主键表达式"""
-    return scanner.search("PRIMARY", "KEY")
-
-
-def parse_ddl_primary_index_expression(scanner: TokenScanner) -> DDLPrimaryIndexExpression:
-    """解析主键表达式"""
-    scanner.match("PRIMARY", "KEY")
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return DDLPrimaryIndexExpression(columns=columns)
-
-
-def is_ddl_unique_index_expression(scanner: TokenScanner) -> bool:
-    """判断是否为唯一键表达式"""
-    return scanner.search("UNIQUE", "KEY")
-
-
-def parse_ddl_unique_index_expression(scanner: TokenScanner) -> DDLUniqueIndexExpression:
-    """解析唯一键表达式"""
-    scanner.match("UNIQUE", "KEY")
-    name = scanner.pop_as_source()
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return DDLUniqueIndexExpression(name=name, columns=columns)
-
-
-def is_ddl_normal_index_expression(scanner: TokenScanner) -> bool:
-    """判断是否为一般索引表达式"""
-    return scanner.search("KEY")
-
-
-def parse_ddl_normal_index_expression(scanner: TokenScanner) -> DDLNormalIndexExpression:
-    """解析一般索引表达式"""
-    scanner.match("KEY")
-    name = scanner.pop_as_source()
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return DDLNormalIndexExpression(name=name, columns=columns)
-
-
-def is_ddl_fulltext_expression(scanner: TokenScanner) -> bool:
-    """判断是否为全文索引表达式"""
-    return scanner.search("FULLTEXT", "KEY")
-
-
-def parse_ddl_fulltext_expression(scanner: TokenScanner) -> DDLFulltextIndexExpression:
-    """解析全文索引表达式"""
-    scanner.match("FULLTEXT", "KEY")
-    name = scanner.pop_as_source()
-    columns = [column_scanner.pop_as_source()
-               for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return DDLFulltextIndexExpression(name=name, columns=columns)
-
-
-def is_ddl_foreign_key_expression(scanner: TokenScanner) -> bool:
-    """判断是否为外键表达式"""
-    return scanner.search("CONSTRAINT")
-
-
-def parse_dll_foreign_key_expression(scanner: TokenScanner) -> DDLForeignKeyExpression:
-    """解析外键表达式"""
-    scanner.match("CONSTRAINT")
-    constraint_name = scanner.pop_as_source()
-    scanner.match("FOREIGN", "KEY")
-    slave_columns = [column_scanner.pop_as_source()
-                     for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    scanner.match("REFERENCES")
-    master_table_name = scanner.pop_as_source()
-    master_columns = [column_scanner.pop_as_source()
-                      for column_scanner in scanner.pop_as_children_scanner_list_split_by(",")]
-    return DDLForeignKeyExpression(
-        constraint_name=constraint_name,
-        slave_columns=slave_columns,
-        master_table_name=master_table_name,
-        master_columns=master_columns
-    )
-
-
-def parse(scanner: TokenScanner) -> List[SQLStatement]:
-    """解析一段 SQL 语句，返回表达式的列表
-
-    Examples
-    --------
-    >>> parse(build_token_scanner("SELECT a FROM b; SELECT c FROM d"))
-    [<SQLSingleSelectStatement source=SELECT a
-    FROM b>, <SQLSingleSelectStatement source=SELECT c
-    FROM d>]
-    """
-    statement_list = []
-    for statement_scanner in scanner.split_by(";"):
-        # 先尝试解析 WITH 语句
-        with_clause = parse_with_clause(statement_scanner)
-
-        if is_select_statement(statement_scanner):
-            statement_list.append(parse_select_statement(statement_scanner, with_clause=with_clause))
-        else:
-            raise SqlParseError(f"未知语句类型: {statement_scanner}")
-
-    return statement_list
-
-
-def parse_create_table_statement(scanner: TokenScanner) -> DDLCreateTableStatement:
+def parse_create_table_statement(scanner: TokenScanner) -> SQLCreateTableStatement:
     # 解析字段、索引括号前的部分
     scanner.match("CREATE", "TABLE")
     if_not_exists = scanner.search_and_move("IF", "NOT", "EXISTS")
     table_name = scanner.pop_as_source().strip("`")  # TODO 待改为 TableNameExpression，并支持 schema_name
 
     # 解析字段和索引
-    columns: List[DDLColumnExpression] = []
-    primary_key: Optional[DDLPrimaryIndexExpression] = None
-    unique_key: List[DDLUniqueIndexExpression] = []
-    key: List[DDLNormalIndexExpression] = []
-    fulltext_key: List[DDLFulltextIndexExpression] = []
-    foreign_key: List[DDLForeignKeyExpression] = []
+    columns: List[SQLDefineColumnExpression] = []
+    primary_key: Optional[SQLPrimaryIndexExpression] = None
+    unique_key: List[SQLUniqueIndexExpression] = []
+    key: List[SQLNormalIndexExpression] = []
+    fulltext_key: List[SQLFulltextIndexExpression] = []
+    foreign_key: List[SQLForeignKeyExpression] = []
     for group_scanner in scanner.pop_as_children_scanner_list_split_by(","):
-        if is_ddl_primary_index_expression(group_scanner):
-            primary_key = parse_ddl_primary_index_expression(group_scanner)
-        elif is_ddl_unique_index_expression(group_scanner):
-            unique_key.append(parse_ddl_unique_index_expression(group_scanner))
-        elif is_ddl_normal_index_expression(group_scanner):
-            key.append(parse_ddl_normal_index_expression(group_scanner))
-        elif is_ddl_fulltext_expression(group_scanner):
-            fulltext_key.append(parse_ddl_fulltext_expression(group_scanner))
-        elif is_ddl_foreign_key_expression(group_scanner):
-            foreign_key.append(parse_dll_foreign_key_expression(group_scanner))
+        if check_primary_index_expression(group_scanner):
+            primary_key = parse_primary_index_expression(group_scanner)
+        elif check_unique_index_expression(group_scanner):
+            unique_key.append(parse_unique_index_expression(group_scanner))
+        elif check_normal_index_expression(group_scanner):
+            key.append(parse_normal_index_expression(group_scanner))
+        elif check_fulltext_expression(group_scanner):
+            fulltext_key.append(parse_fulltext_expression(group_scanner))
+        elif check_foreign_key_expression(group_scanner):
+            foreign_key.append(parse_foreign_key_expression(group_scanner))
         else:
-            columns.append(parse_ddl_column_expression(group_scanner))
+            columns.append(parse_define_column_expression(group_scanner))
 
     # 解析表属性
     comment: Optional[str] = None
     engine: Optional[str] = None
     auto_increment: Optional[int] = None
     default_charset: Optional[str] = None
     collate: Optional[str] = None
@@ -1755,15 +1683,15 @@
         elif scanner.search_and_move("STATS_PERSISTENT"):
             scanner.match("=")
             states_persistent = scanner.pop_as_source()
         else:
             raise SqlParseError(f"未知的 DDL 表属性: {scanner}")
     scanner.search_and_move(";")
 
-    return DDLCreateTableStatement(
+    return SQLCreateTableStatement(
         table_name=table_name,
         comment=comment,
         if_not_exists=if_not_exists,
         columns=columns,
         primary_key=primary_key,
         unique_key=unique_key,
         key=key,
@@ -1772,7 +1700,30 @@
         engine=engine,
         auto_increment=auto_increment,
         default_charset=default_charset,
         collate=collate,
         row_format=row_format,
         states_persistent=states_persistent
     )
+
+
+def parse_statement(scanner: TokenScanner) -> List[SQLStatement]:
+    """解析一段 SQL 语句，返回表达式的列表
+
+    Examples
+    --------
+    >>> parse_statement(build_token_scanner("SELECT a FROM b; SELECT c FROM d"))
+    [<SQLSingleSelectStatement source=SELECT a
+    FROM b>, <SQLSingleSelectStatement source=SELECT c
+    FROM d>]
+    """
+    statement_list = []
+    for statement_scanner in scanner.split_by(";"):
+        # 先尝试解析 WITH 语句
+        with_clause = parse_with_clause(statement_scanner)
+
+        if check_select_statement(statement_scanner):
+            statement_list.append(parse_select_statement(statement_scanner, with_clause=with_clause))
+        else:
+            raise SqlParseError(f"未知语句类型: {statement_scanner}")
+
+    return statement_list
```

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql.egg-info/PKG-INFO` & `metasequoia-sql-0.2.0/metasequoia_sql.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasequoia-sql
-Version: 0.1.1
+Version: 0.2.0
 Summary: SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能
 Home-page: https://github.com/ChangxingJiang/metasequoia-sql
 Author: changxing
 Author-email: 1278729001@qq.com
 License: MIT License
 Platform: all
 Classifier: Intended Audience :: Developers
@@ -37,44 +37,47 @@
 ```
 
 ### 句法分析
 
 对 SQL 语句进行语法分析，将 SQL 语句转化为对应可操作的对象（详见 demo_2）：
 
 ```python
-from metasequoia_sql.parser.common import parse_create_table_statement
-from metasequoia_sql.common.token_scanner import build_token_scanner
+from metasequoia_sql import *
 
 statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ### 翻译工具
 
 将 MySQL 的 CREATE TABLE 语句转换为 Hive 的 CREATE TABLE 语句：
 
 ```python
-from metasequoia_sql.parser.common import parse_create_table_statement
-from metasequoia_sql.translate import *
-from metasequoia_sql.common.token_scanner import build_token_scanner
+from metasequoia_sql import *
 
 statement = parse_create_table_statement(build_token_scanner("your sql"))
 ```
 
 ## 实现原理
 
 **SQL 解析原理**：将词法分析与句法分析分离，对所有 SQL 语句进行词法分析，然后对不同的 SQL 语句类型使用不同的句法分析方法。
 
 **不同 DataSource 的 SQL 语句转换方法**： 先从特定 DataSource 的 SQL 转化为包含所有数据库特性的 FullStatement，然后再从
 FullStatement 转化为另一个 DataSource 的 SQl。通过这样的处理，可以避免开发网状结构的转换器，而只需要开发星星转换器即可。
 
+- `analyzer`：分析器
 - `ast`：词法分析（主要使用有限状态自动机实现）
 - `common`：遍历器工具
+- `core`：句法分析节点类
+  - `abc`：抽象类（节点中不包含解析方法）
+  - `element`：元素类节点（不会引用其他节点）
+  - `general_expression`：一般表达式节点（可能引用元素类节点和其他一般表达式节点）
 - `objects`：SQL语句对象
 - `parser`：SQL语句解析器
-- `translate`：翻译器
+
+（因为在 Python 中若标记类型时，不同文件之间不同循环引用，所以需要保证所有类的引用之间为严格的拓扑关系）
 
 ### 词法分析
 
 字面值类型：[参考文档](https://deepinout.com/mysql/mysql-top-articles-mysql/1694052463_j_mysql-literals.html)
 
 - `ASTLiteralString`：字符串字面值
 
@@ -128,27 +131,28 @@
 
 ## 已知的不兼容
 
 - DB2 的 `CURRENT DATE` 的语法
 
 ## 修改记录
 
-#### 0.1.0 > 0.1.1
+#### 0.1.0 > 0.2.0
 
 新增：
 - `INSERT` 语句解析逻辑
 - 一次性解析多条 SQL 语句
 
 优化：
 - 统一 `CREATE TABLE` 解析逻辑（使用 `TokenScanner`，改造节点对象，改造解析逻辑，改造 Hive 源码生成逻辑）
-- 清理多余对象
-- TokenScanner 使用方法
+- 整理 objects 的节点和 parse 中的方法，清理多余对象，优化引用路径
+- 统一 TokenScanner 使用方法
 
 修复：
 - `WITH` 语句解析报错的 Bug 修复
+- Hive 建表语句的类型包含参数的 Bug 修复
 
 ##### 0.1.0
 
 - 新增 SELECT 语句解析逻辑
 - Bug 修复：移除在 Hive 建表语句末尾的分号
 
 ##### 0.0.1
```

### Comparing `metasequoia-sql-0.1.1/metasequoia_sql.egg-info/SOURCES.txt` & `metasequoia-sql-0.2.0/metasequoia_sql.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 LICENSE
 README.md
 setup.py
 metasequoia_sql/__init__.py
 metasequoia_sql/errors.py
+metasequoia_sql/static.py
 metasequoia_sql.egg-info/PKG-INFO
 metasequoia_sql.egg-info/SOURCES.txt
 metasequoia_sql.egg-info/dependency_links.txt
 metasequoia_sql.egg-info/top_level.txt
 metasequoia_sql/analyzer/__init__.py
 metasequoia_sql/analyzer/consanguinity.py
 metasequoia_sql/ast/__init__.py
 metasequoia_sql/ast/functions.py
 metasequoia_sql/ast/nodes.py
 metasequoia_sql/ast/parser.py
+metasequoia_sql/ast/static.py
 metasequoia_sql/common/__init__.py
 metasequoia_sql/common/base_scanner.py
 metasequoia_sql/common/basic.py
 metasequoia_sql/common/text_scanner.py
 metasequoia_sql/common/token_scanner.py
-metasequoia_sql/objects/__init__.py
-metasequoia_sql/objects/core.py
-metasequoia_sql/parser/__init__.py
-metasequoia_sql/parser/common.py
-metasequoia_sql/static/__init__.py
-metasequoia_sql/static/common.py
-metasequoia_sql/static/mysql.py
-metasequoia_sql/static/other.py
+metasequoia_sql/core/__init__.py
+metasequoia_sql/core/data_source.py
+metasequoia_sql/core/objects.py
+metasequoia_sql/core/parser.py
+metasequoia_sql/core/static.py
```

### Comparing `metasequoia-sql-0.1.1/setup.py` & `metasequoia-sql-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="metasequoia-sql",
-    version="0.1.1",
+    version="0.2.0",
     description="SQL解析器：提供词法解析、句法解析和不同SQL类型翻译的功能",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="changxing",
     author_email="1278729001@qq.com",
     url="https://github.com/ChangxingJiang/metasequoia-sql",
     install_requires=[],
```

