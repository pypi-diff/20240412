# Comparing `tmp/pgspot-0.7.0.tar.gz` & `tmp/pgspot-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgspot-0.7.0.tar", last modified: Wed Jan 31 19:15:58 2024, max compression
+gzip compressed data, was "pgspot-0.7.1.tar", last modified: Fri Apr 12 06:49:23 2024, max compression
```

## Comparing `pgspot-0.7.0.tar` & `pgspot-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:15:58.001866 pgspot-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-31 19:15:50.000000 pgspot-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-01-31 19:15:58.001866 pgspot-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-01-31 19:15:50.000000 pgspot-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-31 19:15:50.000000 pgspot-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-31 19:15:58.001866 pgspot-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 19:15:50.000000 pgspot-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:15:57.997866 pgspot-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:15:58.001866 pgspot-0.7.0/src/pgspot/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 19:15:50.000000 pgspot-0.7.0/src/pgspot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-31 19:15:50.000000 pgspot-0.7.0/src/pgspot/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3491 2024-01-31 19:15:50.000000 pgspot-0.7.0/src/pgspot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-01-31 19:15:50.000000 pgspot-0.7.0/src/pgspot/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-31 19:15:50.000000 pgspot-0.7.0/src/pgspot/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-01-31 19:15:50.000000 pgspot-0.7.0/src/pgspot/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-01-31 19:15:50.000000 pgspot-0.7.0/src/pgspot/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 19:15:58.001866 pgspot-0.7.0/src/pgspot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-01-31 19:15:57.000000 pgspot-0.7.0/src/pgspot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-31 19:15:57.000000 pgspot-0.7.0/src/pgspot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 19:15:57.000000 pgspot-0.7.0/src/pgspot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-31 19:15:57.000000 pgspot-0.7.0/src/pgspot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-31 19:15:57.000000 pgspot-0.7.0/src/pgspot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-31 19:15:57.000000 pgspot-0.7.0/src/pgspot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:49:23.255189 pgspot-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-12 06:49:19.000000 pgspot-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-12 06:49:23.255189 pgspot-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-12 06:49:19.000000 pgspot-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 06:49:19.000000 pgspot-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 06:49:23.255189 pgspot-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:49:19.000000 pgspot-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:49:23.251189 pgspot-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:49:23.255189 pgspot-0.7.1/src/pgspot/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 06:49:19.000000 pgspot-0.7.1/src/pgspot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 06:49:19.000000 pgspot-0.7.1/src/pgspot/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3491 2024-04-12 06:49:19.000000 pgspot-0.7.1/src/pgspot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-04-12 06:49:19.000000 pgspot-0.7.1/src/pgspot/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-12 06:49:19.000000 pgspot-0.7.1/src/pgspot/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-12 06:49:19.000000 pgspot-0.7.1/src/pgspot/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17779 2024-04-12 06:49:19.000000 pgspot-0.7.1/src/pgspot/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:49:23.255189 pgspot-0.7.1/src/pgspot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-12 06:49:23.000000 pgspot-0.7.1/src/pgspot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-12 06:49:23.000000 pgspot-0.7.1/src/pgspot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:49:23.000000 pgspot-0.7.1/src/pgspot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 06:49:23.000000 pgspot-0.7.1/src/pgspot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 06:49:23.000000 pgspot-0.7.1/src/pgspot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 06:49:23.000000 pgspot-0.7.1/src/pgspot.egg-info/top_level.txt
```

### Comparing `pgspot-0.7.0/LICENSE` & `pgspot-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgspot-0.7.0/PKG-INFO` & `pgspot-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgspot
-Version: 0.7.0
+Version: 0.7.1
 Summary: Spot vulnerabilities in postgres extension scripts
 Home-page: https://github.com/timescale/pgspot
 Author: Timescale, Inc.
 License: The PostgreSQL License
 Project-URL: Bug Tracker, https://github.com/timescale/pgspot/issues
 Keywords: postgresql
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pglast==5.0
+Requires-Dist: pglast==6.2
 
 ## pgspot
 <p align="center">
   <a href="https://github.com/timescale/pgspot/actions"><img alt="Actions Status" src="https://github.com/timescale/pgspot/workflows/Test/badge.svg"></a>
   <a href="https://github.com/timescale/pgspot/blob/main/LICENSE"><img alt="License: PostgreSQL" src="https://img.shields.io/github/license/timescale/pgspot"></a>
   <a href="https://pypi.org/project/pgspot/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pgspot"></a>
   <a href="https://pepy.tech/project/pgspot"><img alt="Downloads" src="https://pepy.tech/badge/pgspot"></a>
@@ -52,15 +52,15 @@
 ## Installation
 
 pip install pgspot
 
 ## Requirements
 
 - python >= 3.10
-- [pglast == 5.0](https://github.com/lelit/pglast)
+- [pglast](https://github.com/lelit/pglast)
 - [libpg_query](https://github.com/pganalyze/libpg_query) (through pglast)
 
 To install the runtime requirements, use `pip -r requirements.txt`.
 
 
 ### Usage
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: pgspot Version: 0.7.0 Summary: Spot vulnerabilities
+Metadata-Version: 2.1 Name: pgspot Version: 0.7.1 Summary: Spot vulnerabilities
 in postgres extension scripts Home-page: https://github.com/timescale/pgspot
 Author: Timescale, Inc. License: The PostgreSQL License Project-URL: Bug
 Tracker, https://github.com/timescale/pgspot/issues Keywords: postgresql
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: PostgreSQL License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.10 Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Classifier: Topic ::
 Software Development :: Quality Assurance Requires-Python: >=3.10 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: pglast==5.0 ##
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: pglast==6.2 ##
 pgspot
    _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _P_o_s_t_g_r_e_S_Q_L_]_[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
               _[_h_t_t_p_s_:_/_/_w_w_w_._b_e_s_t_p_r_a_c_t_i_c_e_s_._d_e_v_/_p_r_o_j_e_c_t_s_/_8_0_0_9_/_b_a_d_g_e_]
 Spot vulnerabilities in PostgreSQL extension scripts. pgspot checks extension
 scripts for following PostgreSQL security best practices. In addition to
 checking extension scripts it can also be used to check security definer
 functions or any other PostgreSQL SQL code. pgspot checks for the following
@@ -20,24 +20,24 @@
 the [reference] for detailed documentation of the vulnerabilities which pgspot
 detects, and their potential mitigations. [reference]: https://github.com/
 timescale/pgspot/blob/main/REFERENCE.md ## Useful links - [PostgreSQL security
 recommendations for extensions](https://www.postgresql.org/docs/current/extend-
 extensions.html#EXTEND-EXTENSIONS-SECURITY) - [PostgreSQL security
 recommendations for SECURITY DEFINER functions](https://www.postgresql.org/
 docs/current/sql-createfunction.html#SQL-CREATEFUNCTION-SECURITY) ##
-Installation pip install pgspot ## Requirements - python >= 3.10 - [pglast ==
-5.0](https://github.com/lelit/pglast) - [libpg_query](https://github.com/
-pganalyze/libpg_query) (through pglast) To install the runtime requirements,
-use `pip -r requirements.txt`. ### Usage ``` > pgspot -h usage: pgspot [-h] [-
-a] [--proc-without-search-path PROC] [--summary-only] [--plpgsql | --no-
-plpgsql] [--explain EXPLAIN] [--ignore IGNORE] [--sql-accepting SQL_FN] [FILE
-...] Spot vulnerabilities in PostgreSQL SQL scripts positional arguments: FILE
-file to check for vulnerabilities options: -h, --help show this help message
-and exit -a, --append append files before checking --proc-without-search-path
-PROC whitelist functions without explicit search_path --summary-only only print
+Installation pip install pgspot ## Requirements - python >= 3.10 - [pglast]
+(https://github.com/lelit/pglast) - [libpg_query](https://github.com/pganalyze/
+libpg_query) (through pglast) To install the runtime requirements, use `pip -
+r requirements.txt`. ### Usage ``` > pgspot -h usage: pgspot [-h] [-a] [--proc-
+without-search-path PROC] [--summary-only] [--plpgsql | --no-plpgsql] [--
+explain EXPLAIN] [--ignore IGNORE] [--sql-accepting SQL_FN] [FILE ...] Spot
+vulnerabilities in PostgreSQL SQL scripts positional arguments: FILE file to
+check for vulnerabilities options: -h, --help show this help message and exit -
+a, --append append files before checking --proc-without-search-path PROC
+whitelist functions without explicit search_path --summary-only only print
 number of errors, warnings and unknowns --plpgsql, --no-plpgsql Analyze PLpgSQL
 code (default: True) --explain EXPLAIN Describe an error/warning code --ignore
 IGNORE Ignore error or warning code --sql-accepting SQL_FN Specify one or more
 sql-accepting functions ``` ``` > pgspot --ignore PS017 <<<"CREATE TABLE IF NOT
 EXISTS foo();" PS012: Unsafe table creation: foo Errors: 1 Warnings: 0 Unknown:
 0 ``` #### SQL-accepting functions It is a common pattern that SQL-accepting
 functions exist, which take a string-like argument which will be executed as
```

### Comparing `pgspot-0.7.0/README.md` & `pgspot-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ## Installation
 
 pip install pgspot
 
 ## Requirements
 
 - python >= 3.10
-- [pglast == 5.0](https://github.com/lelit/pglast)
+- [pglast](https://github.com/lelit/pglast)
 - [libpg_query](https://github.com/pganalyze/libpg_query) (through pglast)
 
 To install the runtime requirements, use `pip -r requirements.txt`.
 
 
 ### Usage
```

#### html2text {}

```diff
@@ -9,24 +9,24 @@
 the [reference] for detailed documentation of the vulnerabilities which pgspot
 detects, and their potential mitigations. [reference]: https://github.com/
 timescale/pgspot/blob/main/REFERENCE.md ## Useful links - [PostgreSQL security
 recommendations for extensions](https://www.postgresql.org/docs/current/extend-
 extensions.html#EXTEND-EXTENSIONS-SECURITY) - [PostgreSQL security
 recommendations for SECURITY DEFINER functions](https://www.postgresql.org/
 docs/current/sql-createfunction.html#SQL-CREATEFUNCTION-SECURITY) ##
-Installation pip install pgspot ## Requirements - python >= 3.10 - [pglast ==
-5.0](https://github.com/lelit/pglast) - [libpg_query](https://github.com/
-pganalyze/libpg_query) (through pglast) To install the runtime requirements,
-use `pip -r requirements.txt`. ### Usage ``` > pgspot -h usage: pgspot [-h] [-
-a] [--proc-without-search-path PROC] [--summary-only] [--plpgsql | --no-
-plpgsql] [--explain EXPLAIN] [--ignore IGNORE] [--sql-accepting SQL_FN] [FILE
-...] Spot vulnerabilities in PostgreSQL SQL scripts positional arguments: FILE
-file to check for vulnerabilities options: -h, --help show this help message
-and exit -a, --append append files before checking --proc-without-search-path
-PROC whitelist functions without explicit search_path --summary-only only print
+Installation pip install pgspot ## Requirements - python >= 3.10 - [pglast]
+(https://github.com/lelit/pglast) - [libpg_query](https://github.com/pganalyze/
+libpg_query) (through pglast) To install the runtime requirements, use `pip -
+r requirements.txt`. ### Usage ``` > pgspot -h usage: pgspot [-h] [-a] [--proc-
+without-search-path PROC] [--summary-only] [--plpgsql | --no-plpgsql] [--
+explain EXPLAIN] [--ignore IGNORE] [--sql-accepting SQL_FN] [FILE ...] Spot
+vulnerabilities in PostgreSQL SQL scripts positional arguments: FILE file to
+check for vulnerabilities options: -h, --help show this help message and exit -
+a, --append append files before checking --proc-without-search-path PROC
+whitelist functions without explicit search_path --summary-only only print
 number of errors, warnings and unknowns --plpgsql, --no-plpgsql Analyze PLpgSQL
 code (default: True) --explain EXPLAIN Describe an error/warning code --ignore
 IGNORE Ignore error or warning code --sql-accepting SQL_FN Specify one or more
 sql-accepting functions ``` ``` > pgspot --ignore PS017 <<<"CREATE TABLE IF NOT
 EXISTS foo();" PS012: Unsafe table creation: foo Errors: 1 Warnings: 0 Unknown:
 0 ``` #### SQL-accepting functions It is a common pattern that SQL-accepting
 functions exist, which take a string-like argument which will be executed as
```

### Comparing `pgspot-0.7.0/setup.cfg` & `pgspot-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >= 3.10
 install_requires = 
-	pglast==5.0
+	pglast==6.2
 tests_require = 
 	pytest>=7.2.0
 	pytest-snapshot
 
 [options.packages.find]
 where = src
```

### Comparing `pgspot-0.7.0/src/pgspot/cli.py` & `pgspot-0.7.1/src/pgspot/cli.py`

 * *Files identical despite different names*

### Comparing `pgspot-0.7.0/src/pgspot/codes.py` & `pgspot-0.7.1/src/pgspot/codes.py`

 * *Files identical despite different names*

### Comparing `pgspot-0.7.0/src/pgspot/formatters.py` & `pgspot-0.7.1/src/pgspot/formatters.py`

 * *Files identical despite different names*

### Comparing `pgspot-0.7.0/src/pgspot/state.py` & `pgspot-0.7.1/src/pgspot/state.py`

 * *Files identical despite different names*

### Comparing `pgspot-0.7.0/src/pgspot/visitors.py` & `pgspot-0.7.1/src/pgspot/visitors.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,22 @@
                         if "upper" in value:
                             visit_sql(
                                 self.state,
                                 "SELECT " + value["upper"]["PLpgSQL_expr"]["query"],
                             )
                         if "body" in value:
                             self.visit(value["body"])
+                    case "PLpgSQL_stmt_foreach_a":
+                        if "expr" in value:
+                            visit_sql(
+                                self.state,
+                                "SELECT " + value["expr"]["PLpgSQL_expr"]["query"],
+                            )
+                        if "body" in value:
+                            self.visit(value["body"])
                     case "PLpgSQL_stmt_raise":
                         if "params" in value:
                             for item in value["params"]:
                                 visit_sql(
                                     self.state,
                                     "SELECT " + item["PLpgSQL_expr"]["query"],
                                 )
```

### Comparing `pgspot-0.7.0/src/pgspot.egg-info/PKG-INFO` & `pgspot-0.7.1/src/pgspot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgspot
-Version: 0.7.0
+Version: 0.7.1
 Summary: Spot vulnerabilities in postgres extension scripts
 Home-page: https://github.com/timescale/pgspot
 Author: Timescale, Inc.
 License: The PostgreSQL License
 Project-URL: Bug Tracker, https://github.com/timescale/pgspot/issues
 Keywords: postgresql
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pglast==5.0
+Requires-Dist: pglast==6.2
 
 ## pgspot
 <p align="center">
   <a href="https://github.com/timescale/pgspot/actions"><img alt="Actions Status" src="https://github.com/timescale/pgspot/workflows/Test/badge.svg"></a>
   <a href="https://github.com/timescale/pgspot/blob/main/LICENSE"><img alt="License: PostgreSQL" src="https://img.shields.io/github/license/timescale/pgspot"></a>
   <a href="https://pypi.org/project/pgspot/"><img alt="PyPI" src="https://img.shields.io/pypi/v/pgspot"></a>
   <a href="https://pepy.tech/project/pgspot"><img alt="Downloads" src="https://pepy.tech/badge/pgspot"></a>
@@ -52,15 +52,15 @@
 ## Installation
 
 pip install pgspot
 
 ## Requirements
 
 - python >= 3.10
-- [pglast == 5.0](https://github.com/lelit/pglast)
+- [pglast](https://github.com/lelit/pglast)
 - [libpg_query](https://github.com/pganalyze/libpg_query) (through pglast)
 
 To install the runtime requirements, use `pip -r requirements.txt`.
 
 
 ### Usage
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: pgspot Version: 0.7.0 Summary: Spot vulnerabilities
+Metadata-Version: 2.1 Name: pgspot Version: 0.7.1 Summary: Spot vulnerabilities
 in postgres extension scripts Home-page: https://github.com/timescale/pgspot
 Author: Timescale, Inc. License: The PostgreSQL License Project-URL: Bug
 Tracker, https://github.com/timescale/pgspot/issues Keywords: postgresql
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: PostgreSQL License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.10 Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Classifier: Topic ::
 Software Development :: Quality Assurance Requires-Python: >=3.10 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: pglast==5.0 ##
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: pglast==6.2 ##
 pgspot
    _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_:_ _P_o_s_t_g_r_e_S_Q_L_]_[_P_y_P_I_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
               _[_h_t_t_p_s_:_/_/_w_w_w_._b_e_s_t_p_r_a_c_t_i_c_e_s_._d_e_v_/_p_r_o_j_e_c_t_s_/_8_0_0_9_/_b_a_d_g_e_]
 Spot vulnerabilities in PostgreSQL extension scripts. pgspot checks extension
 scripts for following PostgreSQL security best practices. In addition to
 checking extension scripts it can also be used to check security definer
 functions or any other PostgreSQL SQL code. pgspot checks for the following
@@ -20,24 +20,24 @@
 the [reference] for detailed documentation of the vulnerabilities which pgspot
 detects, and their potential mitigations. [reference]: https://github.com/
 timescale/pgspot/blob/main/REFERENCE.md ## Useful links - [PostgreSQL security
 recommendations for extensions](https://www.postgresql.org/docs/current/extend-
 extensions.html#EXTEND-EXTENSIONS-SECURITY) - [PostgreSQL security
 recommendations for SECURITY DEFINER functions](https://www.postgresql.org/
 docs/current/sql-createfunction.html#SQL-CREATEFUNCTION-SECURITY) ##
-Installation pip install pgspot ## Requirements - python >= 3.10 - [pglast ==
-5.0](https://github.com/lelit/pglast) - [libpg_query](https://github.com/
-pganalyze/libpg_query) (through pglast) To install the runtime requirements,
-use `pip -r requirements.txt`. ### Usage ``` > pgspot -h usage: pgspot [-h] [-
-a] [--proc-without-search-path PROC] [--summary-only] [--plpgsql | --no-
-plpgsql] [--explain EXPLAIN] [--ignore IGNORE] [--sql-accepting SQL_FN] [FILE
-...] Spot vulnerabilities in PostgreSQL SQL scripts positional arguments: FILE
-file to check for vulnerabilities options: -h, --help show this help message
-and exit -a, --append append files before checking --proc-without-search-path
-PROC whitelist functions without explicit search_path --summary-only only print
+Installation pip install pgspot ## Requirements - python >= 3.10 - [pglast]
+(https://github.com/lelit/pglast) - [libpg_query](https://github.com/pganalyze/
+libpg_query) (through pglast) To install the runtime requirements, use `pip -
+r requirements.txt`. ### Usage ``` > pgspot -h usage: pgspot [-h] [-a] [--proc-
+without-search-path PROC] [--summary-only] [--plpgsql | --no-plpgsql] [--
+explain EXPLAIN] [--ignore IGNORE] [--sql-accepting SQL_FN] [FILE ...] Spot
+vulnerabilities in PostgreSQL SQL scripts positional arguments: FILE file to
+check for vulnerabilities options: -h, --help show this help message and exit -
+a, --append append files before checking --proc-without-search-path PROC
+whitelist functions without explicit search_path --summary-only only print
 number of errors, warnings and unknowns --plpgsql, --no-plpgsql Analyze PLpgSQL
 code (default: True) --explain EXPLAIN Describe an error/warning code --ignore
 IGNORE Ignore error or warning code --sql-accepting SQL_FN Specify one or more
 sql-accepting functions ``` ``` > pgspot --ignore PS017 <<<"CREATE TABLE IF NOT
 EXISTS foo();" PS012: Unsafe table creation: foo Errors: 1 Warnings: 0 Unknown:
 0 ``` #### SQL-accepting functions It is a common pattern that SQL-accepting
 functions exist, which take a string-like argument which will be executed as
```

