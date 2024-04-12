# Comparing `tmp/dbt-impala-1.4.3.tar.gz` & `tmp/dbt-impala-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-impala-1.4.3.tar", last modified: Fri Feb  9 06:11:32 2024, max compression
+gzip compressed data, was "dbt-impala-1.6.0.tar", last modified: Fri Apr 12 16:22:19 2024, max compression
```

## Comparing `dbt-impala-1.4.3.tar` & `dbt-impala-1.6.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.478304 dbt-impala-1.4.3/
--rw-r--r--   0 jenkins   (1001) users      (100)    10837 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/LICENSE
--rw-r--r--   0 jenkins   (1001) users      (100)       83 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) users      (100)     3196 2024-02-09 06:11:32.478304 dbt-impala-1.4.3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     2433 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/README.md
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.470304 dbt-impala-1.4.3/dbt/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.470304 dbt-impala-1.4.3/dbt/adapters/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.470304 dbt-impala-1.4.3/dbt/adapters/impala/
--rw-------   0 jenkins   (1001) users      (100)      227 2024-02-09 06:11:32.000000 dbt-impala-1.4.3/dbt/adapters/impala/.env
--rw-r--r--   0 jenkins   (1001) users      (100)     1062 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/adapters/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      596 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/adapters/impala/__version__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     8443 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/adapters/impala/cloudera_tracking.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2771 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/adapters/impala/column.py
--rw-r--r--   0 jenkins   (1001) users      (100)    15338 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/adapters/impala/connections.py
--rw-r--r--   0 jenkins   (1001) users      (100)    15711 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/adapters/impala/impl.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2431 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/adapters/impala/relation.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.470304 dbt-impala-1.4.3/dbt/include/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.470304 dbt-impala-1.4.3/dbt/include/impala/
--rw-r--r--   0 jenkins   (1001) users      (100)      630 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      651 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/dbt_project.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.474305 dbt-impala-1.4.3/dbt/include/impala/macros/
--rw-r--r--   0 jenkins   (1001) users      (100)    15594 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/adapters.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1591 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/apply_grants.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      676 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/catalog.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     6325 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/incremental.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1899 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/insertoverwrite.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1877 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/seed.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.478304 dbt-impala-1.4.3/dbt/include/impala/macros/utils/
--rw-r--r--   0 jenkins   (1001) users      (100)      721 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/any_value.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      157 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/array_append.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      155 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/array_concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      159 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/array_construct.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      751 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/bool_or.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      672 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      750 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/dateadd.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     5905 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/datediff.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      696 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      825 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/hash.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1208 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/last_day.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1106 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/listagg.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      727 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/position.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      863 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/split_part.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      665 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/macros/utils/timestamps.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      779 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/dbt/include/impala/sample_profiles.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-02-09 06:11:32.478304 dbt-impala-1.4.3/dbt_impala.egg-info/
--rw-r--r--   0 jenkins   (1001) users      (100)     3196 2024-02-09 06:11:32.000000 dbt-impala-1.4.3/dbt_impala.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1544 2024-02-09 06:11:32.000000 dbt-impala-1.4.3/dbt_impala.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-02-09 06:11:32.000000 dbt-impala-1.4.3/dbt_impala.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-02-09 06:11:32.000000 dbt-impala-1.4.3/dbt_impala.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) users      (100)       50 2024-02-09 06:11:32.000000 dbt-impala-1.4.3/dbt_impala.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        4 2024-02-09 06:11:32.000000 dbt-impala-1.4.3/dbt_impala.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) users      (100)       38 2024-02-09 06:11:32.478304 dbt-impala-1.4.3/setup.cfg
--rw-r--r--   0 jenkins   (1001) users      (100)     3118 2024-02-09 06:11:04.000000 dbt-impala-1.4.3/setup.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/
+-rw-r--r--   0 jenkins   (1001) users      (100)    10837 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/LICENSE
+-rw-r--r--   0 jenkins   (1001) users      (100)       83 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) users      (100)     3196 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     2433 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/README.md
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.527736 dbt-impala-1.6.0/dbt/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.527736 dbt-impala-1.6.0/dbt/adapters/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.531736 dbt-impala-1.6.0/dbt/adapters/impala/
+-rw-------   0 jenkins   (1001) users      (100)      227 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt/adapters/impala/.env
+-rw-r--r--   0 jenkins   (1001) users      (100)     1062 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      596 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/__version__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     8443 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/cloudera_tracking.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2771 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/column.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15338 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/connections.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15711 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/impl.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2431 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/relation.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.527736 dbt-impala-1.6.0/dbt/include/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.531736 dbt-impala-1.6.0/dbt/include/impala/
+-rw-r--r--   0 jenkins   (1001) users      (100)      630 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      651 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/dbt_project.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.531736 dbt-impala-1.6.0/dbt/include/impala/macros/
+-rw-r--r--   0 jenkins   (1001) users      (100)    15594 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/adapters.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1591 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/apply_grants.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      676 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/catalog.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     6325 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/incremental.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1899 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/insertoverwrite.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1877 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/seed.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/dbt/include/impala/macros/utils/
+-rw-r--r--   0 jenkins   (1001) users      (100)      721 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/any_value.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      157 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/array_append.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      155 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/array_concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      159 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/array_construct.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      751 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/bool_or.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      672 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      750 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/dateadd.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     5180 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/datediff.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      696 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      825 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/hash.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1208 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/last_day.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1106 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/listagg.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      727 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/position.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      863 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/split_part.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      665 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/timestamps.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      779 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/sample_profiles.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/dbt_impala.egg-info/
+-rw-r--r--   0 jenkins   (1001) users      (100)     3196 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     1544 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) users      (100)       50 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        4 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)       38 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/setup.cfg
+-rw-r--r--   0 jenkins   (1001) users      (100)     3118 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/setup.py
```

### Comparing `dbt-impala-1.4.3/LICENSE` & `dbt-impala-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/PKG-INFO` & `dbt-impala-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-impala
-Version: 1.4.3
+Version: 1.6.0
 Summary: Impala adapter for DBT
 Home-page: https://github.com/cloudera/dbt-impala
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.4.0
+Requires-Dist: dbt-core~=1.6.0
 Requires-Dist: impyla==0.18
 Requires-Dist: python-decouple>=3.6
 
 # dbt-impala
 
 The `dbt-impala` adapter allows you to use [dbt](https://www.getdbt.com/) along with [Apache Impala](https://impala.apache.org/) and [Cloudera Data Platform](https://cloudera.com)
```

### Comparing `dbt-impala-1.4.3/README.md` & `dbt-impala-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/adapters/impala/__init__.py` & `dbt-impala-1.6.0/dbt/adapters/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/adapters/impala/__version__.py` & `dbt-impala-1.6.0/dbt/adapters/impala/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "1.4.3"
+version = "1.6.0"
```

### Comparing `dbt-impala-1.4.3/dbt/adapters/impala/cloudera_tracking.py` & `dbt-impala-1.6.0/dbt/adapters/impala/cloudera_tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/adapters/impala/column.py` & `dbt-impala-1.6.0/dbt/adapters/impala/column.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/adapters/impala/connections.py` & `dbt-impala-1.6.0/dbt/adapters/impala/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/adapters/impala/impl.py` & `dbt-impala-1.6.0/dbt/adapters/impala/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/adapters/impala/relation.py` & `dbt-impala-1.6.0/dbt/adapters/impala/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/__init__.py` & `dbt-impala-1.6.0/dbt/include/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/dbt_project.yml` & `dbt-impala-1.6.0/dbt/include/impala/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/adapters.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/apply_grants.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/catalog.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/incremental.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/insertoverwrite.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/insertoverwrite.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/seed.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/any_value.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/any_value.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/bool_or.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/bool_or.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/concat.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/dateadd.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/datediff.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/datediff.sql`

 * *Files 3% similar despite different names*

```diff
@@ -104,25 +104,14 @@
             ) / {{divisor}})
             end
 
             {% if datepart == 'millisecond' %}
                 + millisecond({{org_second_date}})
                 - millisecond({{org_first_date}})
             {% endif %}
-
-            {% if datepart == 'microsecond' %}
-                {% set capture_str = '[0-9]{4}-[0-9]{2}-[0-9]{2}.[0-9]{2}:[0-9]{2}:[0-9]{2}.([0-9]{6})' %}
-                -- Impala doesn't really support microseconds extration from timestamp, eventhough there is microsecond_add/sub
-                -- So this is a massive hack!
-                -- It will only work if the timestamp-string is of the format
-                -- 'yyyy-MM-dd-HH mm.ss.SSSSSS'
-                + cast(regexp_extract(cast(cast({{second_date}} as timestamp) as string), '{{capture_str}}', 1) as bigint)
-                - cast(regexp_extract(cast(cast({{first_date}} as timestamp) as string), '{{capture_str}}', 1) as bigint)
-            {% endif %}
-
     {%- else -%}
 
         {{ exceptions.raise_compiler_error("macro datediff not implemented for datepart ~ '" ~ datepart ~ "' ~ on Impala") }}
 
     {%- endif -%}
 
 {% endmacro %}
```

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/escape_single_quotes.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/escape_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/hash.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/last_day.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/listagg.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/position.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/split_part.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/macros/utils/timestamps.sql` & `dbt-impala-1.6.0/dbt/include/impala/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt/include/impala/sample_profiles.yml` & `dbt-impala-1.6.0/dbt/include/impala/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/dbt_impala.egg-info/PKG-INFO` & `dbt-impala-1.6.0/dbt_impala.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-impala
-Version: 1.4.3
+Version: 1.6.0
 Summary: Impala adapter for DBT
 Home-page: https://github.com/cloudera/dbt-impala
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.4.0
+Requires-Dist: dbt-core~=1.6.0
 Requires-Dist: impyla==0.18
 Requires-Dist: python-decouple>=3.6
 
 # dbt-impala
 
 The `dbt-impala` adapter allows you to use [dbt](https://www.getdbt.com/) along with [Apache Impala](https://impala.apache.org/) and [Cloudera Data Platform](https://cloudera.com)
```

### Comparing `dbt-impala-1.4.3/dbt_impala.egg-info/SOURCES.txt` & `dbt-impala-1.6.0/dbt_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.4.3/setup.py` & `dbt-impala-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-impala"
 # make sure this always matches dbt/adapters/dbt_impala/__version__.py
-package_version = "1.4.3"
+package_version = "1.6.0"
 description = """The Impala adapter plugin for dbt"""
 
 dbt_core_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
```

