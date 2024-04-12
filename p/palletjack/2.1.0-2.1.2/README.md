# Comparing `tmp/palletjack-2.1.0.tar.gz` & `tmp/palletjack-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palletjack-2.1.0.tar", last modified: Fri Mar 22 12:34:43 2024, max compression
+gzip compressed data, was "palletjack-2.1.2.tar", last modified: Fri Apr 12 11:45:15 2024, max compression
```

## Comparing `palletjack-2.1.0.tar` & `palletjack-2.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:34:43.153363 palletjack-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 12:34:00.000000 palletjack-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-22 12:34:43.153363 palletjack-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-03-22 12:34:00.000000 palletjack-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:34:43.153363 palletjack-2.1.0/palletjack/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/cpalletjack.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    27771 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/palletjack.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/palletjack.h
--rw-r--r--   0 runner    (1001) docker     (127)  1744316 2024-03-22 12:34:41.000000 palletjack-2.1.0/palletjack/palletjack_cython.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/palletjack_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   216223 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/parquet_types_palletjack.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    86184 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/parquet_types_palletjack.h
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-22 12:34:00.000000 palletjack-2.1.0/palletjack/windows_fixup.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:34:43.153363 palletjack-2.1.0/palletjack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-22 12:34:43.000000 palletjack-2.1.0/palletjack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-22 12:34:43.000000 palletjack-2.1.0/palletjack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 12:34:43.000000 palletjack-2.1.0/palletjack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 12:34:41.000000 palletjack-2.1.0/palletjack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-22 12:34:43.000000 palletjack-2.1.0/palletjack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 12:34:43.000000 palletjack-2.1.0/palletjack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-22 12:34:00.000000 palletjack-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 12:34:43.153363 palletjack-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-22 12:34:00.000000 palletjack-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 12:34:43.153363 palletjack-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-03-22 12:34:00.000000 palletjack-2.1.0/test/test_palletjack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-22 12:34:00.000000 palletjack-2.1.0/test/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.346387 palletjack-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 11:44:46.000000 palletjack-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-12 11:45:15.346387 palletjack-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-12 11:44:46.000000 palletjack-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.342388 palletjack-2.1.2/palletjack/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/cpalletjack.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    28644 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/palletjack.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/palletjack.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1745720 2024-04-12 11:45:14.000000 palletjack-2.1.2/palletjack/palletjack_cython.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/palletjack_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   216223 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/parquet_types_palletjack.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    86184 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/parquet_types_palletjack.h
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/windows_fixup.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.346387 palletjack-2.1.2/palletjack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:45:14.000000 palletjack-2.1.2/palletjack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-12 11:44:46.000000 palletjack-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:45:15.346387 palletjack-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-12 11:44:46.000000 palletjack-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.346387 palletjack-2.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-04-12 11:44:46.000000 palletjack-2.1.2/test/test_palletjack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-12 11:44:46.000000 palletjack-2.1.2/test/test_readme.py
```

### Comparing `palletjack-2.1.0/LICENSE` & `palletjack-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.0/PKG-INFO` & `palletjack-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palletjack
-Version: 2.1.0
+Version: 2.1.2
 Summary: Faster parquet metadata reading
 Author-email: Marcin Krystianc <marcin.krystianc@gmail.com>
 Project-URL: Homepage, https://github.com/marcin-krystianc/PalletJack
 Project-URL: Issues, https://github.com/marcin-krystianc/PalletJack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -76,47 +76,47 @@
 ```
 
 ### Reading the in-memory metadata index from a file using pyarrow's fs:
 ```
 index_data = fs.LocalFileSystem().open_input_stream(index_path).readall()
 ```
 
-### Reading data with help of index file:
+### Reading data with help of the index file:
 ```
 metadata = pj.read_metadata(index_path, row_groups = [5, 7])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading data with help of in-memory index:
+### Reading data with help of the in-memory index:
 ```
 metadata = pj.read_metadata(index_data = index_data, row_groups = [5, 7])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of columns using column indices:
+### Reading a subset of columns using column indices:
 ```
 metadata = pj.read_metadata(index_path, column_indices = [1, 3])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of columns using column names:
+### Reading a subset of columns using column names:
 ```
 metadata = pj.read_metadata(index_path, column_names = ['column_1', 'column_3'])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of row groups and columns:
+### Reading a subset of row groups and columns:
 ```
 metadata = pj.read_metadata(index_path, row_groups = [5, 7], column_indices = [1, 3])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 
 data = pr.read_all()
 ```
```

### Comparing `palletjack-2.1.0/README.md` & `palletjack-2.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,47 +61,47 @@
 ```
 
 ### Reading the in-memory metadata index from a file using pyarrow's fs:
 ```
 index_data = fs.LocalFileSystem().open_input_stream(index_path).readall()
 ```
 
-### Reading data with help of index file:
+### Reading data with help of the index file:
 ```
 metadata = pj.read_metadata(index_path, row_groups = [5, 7])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading data with help of in-memory index:
+### Reading data with help of the in-memory index:
 ```
 metadata = pj.read_metadata(index_data = index_data, row_groups = [5, 7])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of columns using column indices:
+### Reading a subset of columns using column indices:
 ```
 metadata = pj.read_metadata(index_path, column_indices = [1, 3])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of columns using column names:
+### Reading a subset of columns using column names:
 ```
 metadata = pj.read_metadata(index_path, column_names = ['column_1', 'column_3'])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of row groups and columns:
+### Reading a subset of row groups and columns:
 ```
 metadata = pj.read_metadata(index_path, row_groups = [5, 7], column_indices = [1, 3])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 
 data = pr.read_all()
 ```
```

### Comparing `palletjack-2.1.0/palletjack/cpalletjack.pxd` & `palletjack-2.1.2/palletjack/palletjack.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-from libcpp.vector cimport vector
-from libcpp.string cimport string
-from libcpp.memory cimport shared_ptr
-from libc.stdint cimport uint32_t
-from pyarrow._parquet cimport *
+#include "parquet/arrow/reader.h"
+#include "parquet/arrow/writer.h"
+#include "parquet/arrow/schema.h"
 
-cdef extern from "palletjack.h":
-    cdef vector[char] GenerateMetadataIndex(const char *parquet_path) nogil except +
-    cdef void GenerateMetadataIndex(const char *parquet_path, const char *index_file_path) nogil except +
-    cdef shared_ptr[CFileMetaData] ReadMetadata(const char *index_file_path, const vector[uint32_t] row_groups, const vector[uint32_t] column_indices, const vector[string] column_names) nogil except +
-    cdef shared_ptr[CFileMetaData] ReadMetadata(const unsigned char *index_data, size_t index_data_length, const vector[uint32_t] row_groups, const vector[uint32_t] column_indices, const vector[string] column_names) nogil except +
+std::vector<char> GenerateMetadataIndex(const char *parquet_path);
+void GenerateMetadataIndex(const char *parquet_path, const char *index_file_path);
+std::shared_ptr<parquet::FileMetaData> ReadMetadata(const char *index_file_path,
+                                                    const std::vector<uint32_t> &row_groups,
+                                                    const std::vector<uint32_t> &column_indices,
+                                                    const std::vector<std::string> &column_names);
+
+std::shared_ptr<parquet::FileMetaData> ReadMetadata(const unsigned char *index_data,
+                                                    size_t index_data_length,
+                                                    const std::vector<uint32_t> &row_groups,
+                                                    const std::vector<uint32_t> &column_indices,
+                                                    const std::vector<std::string> &column_names);
```

### Comparing `palletjack-2.1.0/palletjack/palletjack.cc` & `palletjack-2.1.2/palletjack/palletjack.cc`

 * *Files 4% similar despite different names*

```diff
@@ -58,31 +58,29 @@
                column_names_length +
                metadata_length;
     }
 };
 
 /* File format: (Thrift-encoded metadata stored separately for each row group)
 -----------------------------
-| 0 - 3 | PJ_2              | (char[4]) - File header in ASCI
+| 0 ... | DataHeader        |
 |---------------------------|
-| 4 - 7 | Row groups        | (uint32) - Number of row groups
+|       | 'PJ_2'            | (char[4]) - File header in ASCI
+|       --------------------|
+|       | row groups        | (uint32) - Number of row groups
+|       --------------------|
+|       | columns           | (uint32) - Number of columns
+|       --------------------|
+|       | col. names length | (uint32) - Length of column names section
+|       --------------------|
+|       | metadata length   | (uint32) - Length of metadata section
 |---------------------------|
-| 8 - 11| Columns           | (uint32) - Number of columns
+| . . . | column names      | ['col_0', '\0', 'col_1', '\0', ....] - Section with column names
 |---------------------------|
-|12 - 15| Metadata length   | (uint32) - Metadata length
-|---------------------------|
-|16 -   | Row numbers       | (uint32*) - number of rows per row group
-|---------------------------|
-| . . . | Schema offsets    | (uint32*) - offsets of schema element (1 + 1 + c + 1)
-|---------------------------|
-| . . . | Row group offsets | (uint32*) - offsets of row grpups (1 + rg + 1)
-|---------------------------|
-| . . . | Chunks offsets    | (uint32*) - offsets of column chunks rg * (1 + c + 1)
-|---------------------------|
-| . . . | Metadata          | (uint8*) - Original metadata (thrift compact protocol)
+| . . . | metadata          | [bytes] - Section with original metadata (thrift compact protocol)
 -----------------------------
 */
 
 constexpr int32_t kDefaultThriftStringSizeLimit = 100 * 1000 * 1000;
 constexpr int32_t kDefaultThriftContainerSizeLimit = 1000 * 1000;
 
 using ThriftBuffer = apache::thrift::transport::TMemoryBuffer;
@@ -301,14 +299,20 @@
         if (data_header.get_row_groups_offsets_size() != metadata.row_groups_offsets.size())
         {
             auto msg = std::string("Row group offsets information is invalid, columns=") + std::to_string(data_header.row_groups) + ", row_groups_offsets=" + std::to_string(metadata.row_groups_offsets.size()) + " !";
 
             throw std::logic_error(msg);
         }
 
+        // column_orders is optional
+        if (metadata.column_orders_offsets.size() == 0)
+        {
+            metadata.column_orders_offsets.resize(data_header.get_column_orders_offsets_size());
+        }
+
         if (data_header.get_column_orders_offsets_size() != metadata.column_orders_offsets.size())
         {
             auto msg = std::string("Column orders offsets information is invalid, columns=") + std::to_string(data_header.columns) + ", column_orders_offsets=" + std::to_string(metadata.column_orders_offsets.size()) + " !";
 
             throw std::logic_error(msg);
         }
 
@@ -351,21 +355,25 @@
         auto to_write = name.length() + 1;
         fs.write((const char *)cname, to_write);
         written_column_names_length += to_write;
     }
 
     if (data_header.column_names_length != written_column_names_length)
     {
-        throw std::logic_error("Error when writign the index file,  data_header.column_names_length != written_column_names_length !");
+        throw std::logic_error("Error when writign the index file, data_header.column_names_length != written_column_names_length !");
     }
 
-    uint32_t offset = fs.tellp();
-
     fs.write((const char *)thrift_buffer.get()->data(), thrift_buffer.get()->size());
     auto s = fs.str();
+    if (sizeof(data_header) + data_header.get_body_size() != s.size())
+    {
+        auto msg = std::string("Error when writign the index file, exexted size=") + std::to_string(sizeof(data_header) + data_header.get_body_size()) + ", actual size=" + std::to_string(s.size()) + " !";
+        throw std::logic_error(msg);
+    }
+
     std::vector<char> v(s.size());
     memcpy(&v[0], s.data(), s.size());
     return v;
 }
 
 void GenerateMetadataIndex(const char *parquet_path, const char *index_file_path)
 {
@@ -433,14 +441,16 @@
 
     uint32_t index_src = 0;
     size_t toCopy = 0;
 
     std::vector<uint32_t> columns = column_indices;
     if (column_names.size() > 0)
     {
+        columns.reserve(column_names.size());
+
         std::unordered_map<std::string, uint32_t> columns_map;
         for (uint32_t c = 0; c < dataHeader.columns; c++)
         {
             std::string s = (const char *)column_names_ptr;
             column_names_ptr += s.length() + 1;
             columns_map[s] = c;
         }
@@ -456,36 +466,37 @@
             auto kvp = columns_map.find(column_name);
             if (kvp == columns_map.end())
             {
                 auto msg = std::string("Couldn't find a column with a name '") + column_name + "'!";
                 throw std::logic_error(msg);
             }
 
-            columns.push_back(kvp->second);
+            columns.emplace_back(kvp->second);
         }
     }
 
     if (columns.size() > 0)
     {
+        //> 2:required list<SchemaElement> schema;
         auto schema_list = &schema_offsets[0];
         toCopy = schema_list[0] - index_src;
         thriftCopier.CopyFrom(index_src, toCopy);
         index_src += toCopy;
 
-        thriftCopier.WriteListBegin(::apache::thrift::protocol::T_STRUCT, columns.size() + 1); // one extra element for root
-        index_src = schema_list[1];
+        thriftCopier.WriteListBegin(::apache::thrift::protocol::T_STRUCT, columns.size() + 1); // one extra schema element for root
+        index_src = schema_list[1]; // skip the list header and jump to the first schema element (which is the root element)
 
         auto root_schema_element = &schema_list[1];
         toCopy = root_schema_element[0] + schema_num_children_offsets[0] - index_src;
         thriftCopier.CopyFrom(index_src, toCopy);
-        index_src = root_schema_element[0] + schema_num_children_offsets[1];
 
-        // Update the num children in the schema
+        // Write updated num children in the root element
+        //> 5: optional i32 num_children; 
         thriftCopier.WriteI32(columns.size());
-
+        index_src = root_schema_element[0] + schema_num_children_offsets[1];
         toCopy = root_schema_element[1] - index_src;
         thriftCopier.CopyFrom(index_src, toCopy);
         index_src += toCopy;
 
         auto schema_elements = &schema_offsets[2];
         for (auto column : columns)
         {
@@ -494,14 +505,15 @@
         }
 
         index_src = schema_elements[dataHeader.columns];
     }
 
     if (row_groups.size() > 0)
     {
+        //> 3: required i64 num_rows
         int64_t num_rows = 0;
         for (auto row_group : row_groups)
         {
             num_rows += row_numbers[row_group];
         }
 
         toCopy = num_row_offsets[0] - index_src;
@@ -511,32 +523,33 @@
         thriftCopier.WriteI64(num_rows);
         index_src = num_row_offsets[1];
     }
 
     auto row_group_filtering = row_groups.size() > 0;
     if (row_group_filtering)
     {
+        //> 4: required list<RowGroup> row_groups
         auto row_groups_list = &row_groups_offsets[0];
         toCopy = row_groups_list[0] - index_src;
         thriftCopier.CopyFrom(index_src, toCopy);
         index_src += toCopy;
 
         thriftCopier.WriteListBegin(::apache::thrift::protocol::T_STRUCT, row_groups.size());
         index_src = row_groups_list[1];
     }
     else
     {
-        // copy, including the list
+        // Copy to here, including the list header
         auto row_groups_list = &row_groups_offsets[0];
         toCopy = row_groups_list[1] - index_src;
         thriftCopier.CopyFrom(index_src, toCopy);
         index_src += toCopy;
     }
 
-    for (auto idx = 0;; idx++)
+    for (auto idx = 0u;; idx++)
     {
         size_t row_group_idx = 0;
 
         if (row_group_filtering)
         {
             if (idx >= row_groups.size())
                 break;
@@ -551,22 +564,20 @@
             row_group_idx = idx;
         }
 
         auto row_group_offset = row_groups_offsets[1 + row_group_idx];
         index_src = row_groups_offsets[1 + row_group_idx];
         if (columns.size() > 0)
         {
+            //> 1: required list<ColumnChunk> columns
             auto chunks_list = &column_chunks_offsets[(1 + dataHeader.columns + 1) * row_group_idx];
             auto chunks = &chunks_list[1];
-
-            // START HERE
             toCopy = row_group_offset + chunks_list[0] - index_src;
             thriftCopier.CopyFrom(index_src, toCopy);
-
-            thriftCopier.WriteListBegin(::apache::thrift::protocol::T_STRUCT, columns.size()); // one extra element for root);
+            thriftCopier.WriteListBegin(::apache::thrift::protocol::T_STRUCT, columns.size());
 
             for (auto column_to_copy : columns)
             {
                 toCopy = chunks[column_to_copy + 1] - chunks[column_to_copy];
                 thriftCopier.CopyFrom(row_group_offset + chunks[column_to_copy], toCopy);
             }
 
@@ -579,33 +590,37 @@
         {
             toCopy = row_groups_offsets[1 + row_group_idx + 1] - index_src;
             thriftCopier.CopyFrom(index_src, toCopy);
             index_src += toCopy;
         }
     }
 
-    index_src = row_groups_offsets[dataHeader.get_row_groups_offsets_size() - 1];
+    index_src = row_groups_offsets[1 + dataHeader.row_groups];
 
     if (columns.size() > 0)
     {
-        auto column_orders_list = &column_orders_offsets[0];
-        toCopy = column_orders_list[0] - index_src;
-        thriftCopier.CopyFrom(index_src, toCopy);
-        index_src += toCopy;
+        //> 7: optional list<ColumnOrder> column_orders;
+        if (column_orders_offsets[0] != 0)
+        {
+            auto column_orders_list = &column_orders_offsets[0];
+            toCopy = column_orders_list[0] - index_src;
+            thriftCopier.CopyFrom(index_src, toCopy);
+            index_src += toCopy;
 
-        thriftCopier.WriteListBegin(::apache::thrift::protocol::T_STRUCT, columns.size()); // one extra element for root
-        index_src = column_orders_list[1];
+            thriftCopier.WriteListBegin(::apache::thrift::protocol::T_STRUCT, columns.size()); // one extra element for root
+            index_src = column_orders_list[1];
 
-        auto column_orders = &column_orders_offsets[1];
-        for (auto column : columns)
-        {
-            toCopy = column_orders[column + 1] - column_orders[column];
-            thriftCopier.CopyFrom(column_orders[column], toCopy);
+            auto column_orders = &column_orders_offsets[1];
+            for (auto column : columns)
+            {
+                toCopy = column_orders[column + 1] - column_orders[column];
+                thriftCopier.CopyFrom(column_orders[column], toCopy);
+            }
+            index_src = column_orders[dataHeader.columns];
         }
-        index_src = column_orders[dataHeader.columns];
     }
 
     // Copy leftovers
     toCopy = dataHeader.metadata_length - index_src;
     thriftCopier.CopyFrom(index_src, toCopy);
 
 #ifdef DEBUG
```

### Comparing `palletjack-2.1.0/palletjack/palletjack_cython.cpp` & `palletjack-2.1.2/palletjack/palletjack_cython.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/numpy/core/include/numpy/halffloat.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/api.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/array/concatenate.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/builder.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/c/abi.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/c/bridge.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack_abi.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/compute/api.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/compute/expression.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/config.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/csv/api.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/extension/fixed_shape_tensor.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/extension_type.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/io/api.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/ipc/api.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/json/options.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/json/reader.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/api.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/arrow_to_pandas.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/async.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/benchmark.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/common.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/csv.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/extension_type.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/gdb.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/inference.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/init.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/ipc.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/platform.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/pyarrow.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/python/udf.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/result.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/byte_size.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/cancel.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/compression.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/decimal.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/future.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/io_util.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/iterator.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/key_value_metadata.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/thread_pool.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/arrow/util/value_parsing.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/api/reader.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/api/schema.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/api/writer.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/reader.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/schema.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/writer.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/encryption/encryption.h",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include/parquet/properties.h"
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/numpy/core/include/numpy/halffloat.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/api.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/array/concatenate.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/builder.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/abi.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/bridge.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack_abi.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/compute/api.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/compute/expression.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/config.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/csv/api.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/extension/fixed_shape_tensor.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/extension_type.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/io/api.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/ipc/api.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/json/options.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/json/reader.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/api.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/arrow_to_pandas.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/async.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/benchmark.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/common.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/csv.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/extension_type.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/gdb.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/inference.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/init.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/ipc.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/platform.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/pyarrow.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/udf.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/result.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/byte_size.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/cancel.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/compression.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/decimal.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/future.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/io_util.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/iterator.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/key_value_metadata.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/thread_pool.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/value_parsing.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/api/reader.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/api/schema.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/api/writer.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/reader.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/schema.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/writer.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/encryption/encryption.h",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/properties.h"
         ],
         "extra_compile_args": [
             "-std=c++17"
         ],
         "include_dirs": [
             ".",
             "/home/runner/work/PalletJack/PalletJack/python/vcpkg_installed/include",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow/include",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include",
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "libraries": [
             "arrow",
             "parquet",
             "thrift"
         ],
         "library_dirs": [
             "/home/runner/work/PalletJack/PalletJack/python/vcpkg_installed/lib",
-            "/tmp/build-env-_en912p1/lib/python3.10/site-packages/pyarrow"
+            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow"
         ],
         "name": "palletjack.palletjack_cython",
         "sources": [
             "palletjack/palletjack_cython.pyx",
             "palletjack/palletjack.cc",
             "palletjack/parquet_types_palletjack.cpp"
         ]
@@ -123,18 +123,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -218,14 +218,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -279,14 +281,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -340,60 +344,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -476,14 +503,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2303,64 +2333,64 @@
 
 #line 599 "pyarrow/_parquet.pxd"
 struct __pyx_opt_args_10palletjack_17palletjack_cython_generate_metadata_index;
 
 #line 599 "pyarrow/_parquet.pxd"
 struct __pyx_opt_args_10palletjack_17palletjack_cython_read_metadata;
 
-/* "palletjack/palletjack_cython.pyx":12
+/* "palletjack/palletjack_cython.pyx":13
  * from pyarrow._parquet cimport *
  * 
  * cpdef generate_metadata_index(parquet_path, index_file_path = None):             # <<<<<<<<<<<<<<
  *     cdef string encoded_parquet_path = parquet_path.encode('utf8')
  *     cdef string encoded_index_file_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  */
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 struct __pyx_opt_args_10palletjack_17palletjack_cython_generate_metadata_index {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_n;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *index_file_path;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 };
 
-/* "palletjack/palletjack_cython.pyx":28
+/* "palletjack/palletjack_cython.pyx":29
  *     return None
  * 
  * cpdef read_metadata(index_file_path = None, row_groups = [], column_indices = [], column_names = [], index_data = None):             # <<<<<<<<<<<<<<
  * 
  *     cdef shared_ptr[CFileMetaData] c_metadata
  */
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 struct __pyx_opt_args_10palletjack_17palletjack_cython_read_metadata {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_n;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *index_file_path;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *row_groups;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *column_indices;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *column_names;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *index_data;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
 /* "pyarrow/lib.pxd":71
  * 
  * 
  * cdef class _Weakrefable:             # <<<<<<<<<<<<<<
  *     cdef object __weakref__
@@ -7582,20 +7612,14 @@
 #if CYTHON_USE_CPP_STD_MOVE
   #include <utility>
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
 #else
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
 #endif
 
-/* BufferIndexError.proto */
-static void __Pyx_RaiseBufferIndexError(int axis);
-
-/* BufferIndexErrorNogil.proto */
-static void __Pyx_RaiseBufferIndexErrorNogil(int axis);
-
 /* tp_new.proto */
 #define __Pyx_tp_new(type_obj, args) __Pyx_tp_new_kwargs(type_obj, args, NULL)
 static CYTHON_INLINE PyObject* __Pyx_tp_new_kwargs(PyObject* type_obj, PyObject* args, PyObject* kwargs) {
     return (PyObject*) (((PyTypeObject*)type_obj)->tp_new((PyTypeObject*)type_obj, args, kwargs));
 }
 
 /* PyObject_GenericGetAttrNoDict.proto */
@@ -7644,30 +7668,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -8068,14 +8092,21 @@
 static CYTHON_INLINE std::shared_ptr< parquet::FileEncryptionProperties>  __pyx_f_7pyarrow_8_parquet_24FileEncryptionProperties_unwrap(struct __pyx_obj_7pyarrow_8_parquet_FileEncryptionProperties *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_7pyarrow_8_parquet_12FileMetaData_init(struct __pyx_obj_7pyarrow_8_parquet_FileMetaData *__pyx_v_self, std::shared_ptr< parquet::FileMetaData>  const &__pyx_v_metadata); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_7pyarrow_8_parquet_19ColumnChunkMetaData_init(struct __pyx_obj_7pyarrow_8_parquet_ColumnChunkMetaData *__pyx_v_self, struct __pyx_obj_7pyarrow_8_parquet_RowGroupMetaData *__pyx_v_parent, int __pyx_v_i); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_7pyarrow_8_parquet_10Statistics_init(struct __pyx_obj_7pyarrow_8_parquet_Statistics *__pyx_v_self, std::shared_ptr< parquet::Statistics>  const &__pyx_v_statistics, struct __pyx_obj_7pyarrow_8_parquet_ColumnChunkMetaData *__pyx_v_parent); /* proto*/
 static CYTHON_INLINE struct __pyx_obj_7pyarrow_8_parquet_FileDecryptionProperties *__pyx_f_7pyarrow_8_parquet_24FileDecryptionProperties_wrap(std::shared_ptr< parquet::FileDecryptionProperties>  __pyx_v_properties); /* proto*/
 static CYTHON_INLINE std::shared_ptr< parquet::FileDecryptionProperties>  __pyx_f_7pyarrow_8_parquet_24FileDecryptionProperties_unwrap(struct __pyx_obj_7pyarrow_8_parquet_FileDecryptionProperties *__pyx_v_self); /* proto*/
 
+/* Module declarations from "cython.view" */
+static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
+
+/* Module declarations from "cython.dataclasses" */
+
+/* Module declarations from "cython" */
+
 /* Module declarations from "palletjack" */
 
 /* Module declarations from "libcpp.vector" */
 
 /* Module declarations from "libc.string" */
 
 /* Module declarations from "libcpp.string" */
@@ -8536,14 +8567,20 @@
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
   PyTypeObject *__pyx_ptype_7cpython_4type_type;
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
@@ -9595,14 +9632,20 @@
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
 #define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
@@ -37331,15 +37374,15 @@
 
 #line 1450 "BufferFormatFromTypeInfo"
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 #line 19 "cpython/complex.pxd"
 
 
@@ -37347,30 +37390,30 @@
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
 
 #line 19 "cpython/complex.pxd"
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 20 "cpython/complex.pxd"
   __pyx_r = __pyx_v_self->cval.real;
 
 #line 20 "cpython/complex.pxd"
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 #line 19 "cpython/complex.pxd"
 
 
@@ -37385,15 +37428,15 @@
 
 #line 19 "cpython/complex.pxd"
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 #line 23 "cpython/complex.pxd"
 
 
@@ -37401,30 +37444,30 @@
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
 
 #line 23 "cpython/complex.pxd"
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
 
 #line 24 "cpython/complex.pxd"
   __pyx_r = __pyx_v_self->cval.imag;
 
 #line 24 "cpython/complex.pxd"
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 #line 23 "cpython/complex.pxd"
 
 
@@ -37848,15 +37891,15 @@
 
 #line 129 "cpython/contextvars.pxd"
 }
 
 /* "cpython/datetime.pxd":72
  *     ctypedef extern class datetime.date[object PyDateTime_Date]:
  *         @property
- *         cdef inline int year(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int year(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
 #line 72 "cpython/datetime.pxd"
 
 
@@ -37864,30 +37907,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_4year_year(PyDateTime_Date *__pyx_v_self) {
 
 #line 72 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":73
  *         @property
- *         cdef inline int year(self):
+ *         cdef inline int year(self) noexcept:
  *             return PyDateTime_GET_YEAR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 73 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_YEAR(((PyObject *)__pyx_v_self));
 
 #line 73 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":72
  *     ctypedef extern class datetime.date[object PyDateTime_Date]:
  *         @property
- *         cdef inline int year(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int year(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
 #line 72 "cpython/datetime.pxd"
 
 
@@ -37902,15 +37945,15 @@
 
 #line 72 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":76
  * 
  *         @property
- *         cdef inline int month(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int month(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
 #line 76 "cpython/datetime.pxd"
 
 
@@ -37918,30 +37961,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_5month_month(PyDateTime_Date *__pyx_v_self) {
 
 #line 76 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":77
  *         @property
- *         cdef inline int month(self):
+ *         cdef inline int month(self) noexcept:
  *             return PyDateTime_GET_MONTH(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 77 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_MONTH(((PyObject *)__pyx_v_self));
 
 #line 77 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":76
  * 
  *         @property
- *         cdef inline int month(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int month(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
 #line 76 "cpython/datetime.pxd"
 
 
@@ -37956,15 +37999,15 @@
 
 #line 76 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":80
  * 
  *         @property
- *         cdef inline int day(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int day(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
 #line 80 "cpython/datetime.pxd"
 
 
@@ -37972,30 +38015,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4date_3day_day(PyDateTime_Date *__pyx_v_self) {
 
 #line 80 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":81
  *         @property
- *         cdef inline int day(self):
+ *         cdef inline int day(self) noexcept:
  *             return PyDateTime_GET_DAY(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.time[object PyDateTime_Time]:
  */
 
 #line 81 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_DAY(((PyObject *)__pyx_v_self));
 
 #line 81 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":80
  * 
  *         @property
- *         cdef inline int day(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int day(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
 #line 80 "cpython/datetime.pxd"
 
 
@@ -38010,15 +38053,15 @@
 
 #line 80 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":85
  *     ctypedef extern class datetime.time[object PyDateTime_Time]:
  *         @property
- *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int hour(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_HOUR(self)
  * 
  */
 
 #line 85 "cpython/datetime.pxd"
 
 
@@ -38026,30 +38069,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_4hour_hour(PyDateTime_Time *__pyx_v_self) {
 
 #line 85 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":86
  *         @property
- *         cdef inline int hour(self):
+ *         cdef inline int hour(self) noexcept:
  *             return PyDateTime_TIME_GET_HOUR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 86 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_HOUR(((PyObject *)__pyx_v_self));
 
 #line 86 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":85
  *     ctypedef extern class datetime.time[object PyDateTime_Time]:
  *         @property
- *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int hour(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_HOUR(self)
  * 
  */
 
 #line 85 "cpython/datetime.pxd"
 
 
@@ -38064,15 +38107,15 @@
 
 #line 85 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":89
  * 
  *         @property
- *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int minute(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MINUTE(self)
  * 
  */
 
 #line 89 "cpython/datetime.pxd"
 
 
@@ -38080,30 +38123,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_6minute_minute(PyDateTime_Time *__pyx_v_self) {
 
 #line 89 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":90
  *         @property
- *         cdef inline int minute(self):
+ *         cdef inline int minute(self) noexcept:
  *             return PyDateTime_TIME_GET_MINUTE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 90 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_MINUTE(((PyObject *)__pyx_v_self));
 
 #line 90 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":89
  * 
  *         @property
- *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int minute(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MINUTE(self)
  * 
  */
 
 #line 89 "cpython/datetime.pxd"
 
 
@@ -38118,15 +38161,15 @@
 
 #line 89 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":93
  * 
  *         @property
- *         cdef inline int second(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int second(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_SECOND(self)
  * 
  */
 
 #line 93 "cpython/datetime.pxd"
 
 
@@ -38134,30 +38177,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_6second_second(PyDateTime_Time *__pyx_v_self) {
 
 #line 93 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":94
  *         @property
- *         cdef inline int second(self):
+ *         cdef inline int second(self) noexcept:
  *             return PyDateTime_TIME_GET_SECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 94 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_SECOND(((PyObject *)__pyx_v_self));
 
 #line 94 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":93
  * 
  *         @property
- *         cdef inline int second(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int second(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_SECOND(self)
  * 
  */
 
 #line 93 "cpython/datetime.pxd"
 
 
@@ -38172,15 +38215,15 @@
 
 #line 93 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":97
  * 
  *         @property
- *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int microsecond(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MICROSECOND(self)
  * 
  */
 
 #line 97 "cpython/datetime.pxd"
 
 
@@ -38188,30 +38231,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_11microsecond_microsecond(PyDateTime_Time *__pyx_v_self) {
 
 #line 97 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":98
  *         @property
- *         cdef inline int microsecond(self):
+ *         cdef inline int microsecond(self) noexcept:
  *             return PyDateTime_TIME_GET_MICROSECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 98 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_MICROSECOND(((PyObject *)__pyx_v_self));
 
 #line 98 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":97
  * 
  *         @property
- *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int microsecond(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_TIME_GET_MICROSECOND(self)
  * 
  */
 
 #line 97 "cpython/datetime.pxd"
 
 
@@ -38304,30 +38347,30 @@
 
 #line 101 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":105
  * 
  *         @property
- *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int fold(self) noexcept:             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_TIME_GET_FOLD(self)
  */
 
 #line 105 "cpython/datetime.pxd"
 
 
 #line 105 "cpython/datetime.pxd"
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_4time_4fold_fold(PyDateTime_Time *__pyx_v_self) {
 
 #line 105 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":107
- *         cdef inline int fold(self):
+ *         cdef inline int fold(self) noexcept:
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_TIME_GET_FOLD(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.datetime[object PyDateTime_DateTime]:
  */
 
 #line 107 "cpython/datetime.pxd"
@@ -38335,15 +38378,15 @@
 
 #line 107 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":105
  * 
  *         @property
- *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int fold(self) noexcept:             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_TIME_GET_FOLD(self)
  */
 
 #line 105 "cpython/datetime.pxd"
 
 
@@ -38358,15 +38401,15 @@
 
 #line 105 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":111
  *     ctypedef extern class datetime.datetime[object PyDateTime_DateTime]:
  *         @property
- *         cdef inline int year(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int year(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
 #line 111 "cpython/datetime.pxd"
 
 
@@ -38374,30 +38417,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_4year_year(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 111 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":112
  *         @property
- *         cdef inline int year(self):
+ *         cdef inline int year(self) noexcept:
  *             return PyDateTime_GET_YEAR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 112 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_YEAR(((PyObject *)__pyx_v_self));
 
 #line 112 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":111
  *     ctypedef extern class datetime.datetime[object PyDateTime_DateTime]:
  *         @property
- *         cdef inline int year(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int year(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_YEAR(self)
  * 
  */
 
 #line 111 "cpython/datetime.pxd"
 
 
@@ -38412,15 +38455,15 @@
 
 #line 111 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":115
  * 
  *         @property
- *         cdef inline int month(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int month(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
 #line 115 "cpython/datetime.pxd"
 
 
@@ -38428,30 +38471,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_5month_month(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 115 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":116
  *         @property
- *         cdef inline int month(self):
+ *         cdef inline int month(self) noexcept:
  *             return PyDateTime_GET_MONTH(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 116 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_MONTH(((PyObject *)__pyx_v_self));
 
 #line 116 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":115
  * 
  *         @property
- *         cdef inline int month(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int month(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_MONTH(self)
  * 
  */
 
 #line 115 "cpython/datetime.pxd"
 
 
@@ -38466,15 +38509,15 @@
 
 #line 115 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":119
  * 
  *         @property
- *         cdef inline int day(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int day(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
 #line 119 "cpython/datetime.pxd"
 
 
@@ -38482,30 +38525,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_3day_day(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 119 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":120
  *         @property
- *         cdef inline int day(self):
+ *         cdef inline int day(self) noexcept:
  *             return PyDateTime_GET_DAY(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 120 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_DAY(((PyObject *)__pyx_v_self));
 
 #line 120 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":119
  * 
  *         @property
- *         cdef inline int day(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int day(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_GET_DAY(self)
  * 
  */
 
 #line 119 "cpython/datetime.pxd"
 
 
@@ -38520,15 +38563,15 @@
 
 #line 119 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":123
  * 
  *         @property
- *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int hour(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_HOUR(self)
  * 
  */
 
 #line 123 "cpython/datetime.pxd"
 
 
@@ -38536,30 +38579,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_4hour_hour(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 123 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":124
  *         @property
- *         cdef inline int hour(self):
+ *         cdef inline int hour(self) noexcept:
  *             return PyDateTime_DATE_GET_HOUR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 124 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_HOUR(((PyObject *)__pyx_v_self));
 
 #line 124 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":123
  * 
  *         @property
- *         cdef inline int hour(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int hour(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_HOUR(self)
  * 
  */
 
 #line 123 "cpython/datetime.pxd"
 
 
@@ -38574,15 +38617,15 @@
 
 #line 123 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":127
  * 
  *         @property
- *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int minute(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MINUTE(self)
  * 
  */
 
 #line 127 "cpython/datetime.pxd"
 
 
@@ -38590,30 +38633,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_6minute_minute(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 127 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":128
  *         @property
- *         cdef inline int minute(self):
+ *         cdef inline int minute(self) noexcept:
  *             return PyDateTime_DATE_GET_MINUTE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 128 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_MINUTE(((PyObject *)__pyx_v_self));
 
 #line 128 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":127
  * 
  *         @property
- *         cdef inline int minute(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int minute(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MINUTE(self)
  * 
  */
 
 #line 127 "cpython/datetime.pxd"
 
 
@@ -38628,15 +38671,15 @@
 
 #line 127 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":131
  * 
  *         @property
- *         cdef inline int second(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int second(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_SECOND(self)
  * 
  */
 
 #line 131 "cpython/datetime.pxd"
 
 
@@ -38644,30 +38687,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_6second_second(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 131 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":132
  *         @property
- *         cdef inline int second(self):
+ *         cdef inline int second(self) noexcept:
  *             return PyDateTime_DATE_GET_SECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 132 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_SECOND(((PyObject *)__pyx_v_self));
 
 #line 132 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":131
  * 
  *         @property
- *         cdef inline int second(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int second(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_SECOND(self)
  * 
  */
 
 #line 131 "cpython/datetime.pxd"
 
 
@@ -38682,15 +38725,15 @@
 
 #line 131 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":135
  * 
  *         @property
- *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int microsecond(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MICROSECOND(self)
  * 
  */
 
 #line 135 "cpython/datetime.pxd"
 
 
@@ -38698,30 +38741,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_11microsecond_microsecond(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 135 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":136
  *         @property
- *         cdef inline int microsecond(self):
+ *         cdef inline int microsecond(self) noexcept:
  *             return PyDateTime_DATE_GET_MICROSECOND(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 136 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_MICROSECOND(((PyObject *)__pyx_v_self));
 
 #line 136 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":135
  * 
  *         @property
- *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int microsecond(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DATE_GET_MICROSECOND(self)
  * 
  */
 
 #line 135 "cpython/datetime.pxd"
 
 
@@ -38814,30 +38857,30 @@
 
 #line 139 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":143
  * 
  *         @property
- *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int fold(self) noexcept:             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_DATE_GET_FOLD(self)
  */
 
 #line 143 "cpython/datetime.pxd"
 
 
 #line 143 "cpython/datetime.pxd"
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_8datetime_4fold_fold(PyDateTime_DateTime *__pyx_v_self) {
 
 #line 143 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":145
- *         cdef inline int fold(self):
+ *         cdef inline int fold(self) noexcept:
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_DATE_GET_FOLD(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.timedelta[object PyDateTime_Delta]:
  */
 
 #line 145 "cpython/datetime.pxd"
@@ -38845,15 +38888,15 @@
 
 #line 145 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":143
  * 
  *         @property
- *         cdef inline int fold(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int fold(self) noexcept:             # <<<<<<<<<<<<<<
  *             # For Python < 3.6 this returns 0 no matter what
  *             return PyDateTime_DATE_GET_FOLD(self)
  */
 
 #line 143 "cpython/datetime.pxd"
 
 
@@ -38868,15 +38911,15 @@
 
 #line 143 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":149
  *     ctypedef extern class datetime.timedelta[object PyDateTime_Delta]:
  *         @property
- *         cdef inline int day(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int day(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_DAYS(self)
  * 
  */
 
 #line 149 "cpython/datetime.pxd"
 
 
@@ -38884,30 +38927,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_3day_day(PyDateTime_Delta *__pyx_v_self) {
 
 #line 149 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":150
  *         @property
- *         cdef inline int day(self):
+ *         cdef inline int day(self) noexcept:
  *             return PyDateTime_DELTA_GET_DAYS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 150 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DELTA_GET_DAYS(((PyObject *)__pyx_v_self));
 
 #line 150 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":149
  *     ctypedef extern class datetime.timedelta[object PyDateTime_Delta]:
  *         @property
- *         cdef inline int day(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int day(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_DAYS(self)
  * 
  */
 
 #line 149 "cpython/datetime.pxd"
 
 
@@ -38922,15 +38965,15 @@
 
 #line 149 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":153
  * 
  *         @property
- *         cdef inline int second(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int second(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_SECONDS(self)
  * 
  */
 
 #line 153 "cpython/datetime.pxd"
 
 
@@ -38938,30 +38981,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_6second_second(PyDateTime_Delta *__pyx_v_self) {
 
 #line 153 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":154
  *         @property
- *         cdef inline int second(self):
+ *         cdef inline int second(self) noexcept:
  *             return PyDateTime_DELTA_GET_SECONDS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
 
 #line 154 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DELTA_GET_SECONDS(((PyObject *)__pyx_v_self));
 
 #line 154 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":153
  * 
  *         @property
- *         cdef inline int second(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int second(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_SECONDS(self)
  * 
  */
 
 #line 153 "cpython/datetime.pxd"
 
 
@@ -38976,15 +39019,15 @@
 
 #line 153 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":157
  * 
  *         @property
- *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int microsecond(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_MICROSECONDS(self)
  * 
  */
 
 #line 157 "cpython/datetime.pxd"
 
 
@@ -38992,30 +39035,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_11microsecond_microsecond(PyDateTime_Delta *__pyx_v_self) {
 
 #line 157 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":158
  *         @property
- *         cdef inline int microsecond(self):
+ *         cdef inline int microsecond(self) noexcept:
  *             return PyDateTime_DELTA_GET_MICROSECONDS(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef extern class datetime.tzinfo[object PyDateTime_TZInfo]:
  */
 
 #line 158 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DELTA_GET_MICROSECONDS(((PyObject *)__pyx_v_self));
 
 #line 158 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":157
  * 
  *         @property
- *         cdef inline int microsecond(self):             # <<<<<<<<<<<<<<
+ *         cdef inline int microsecond(self) noexcept:             # <<<<<<<<<<<<<<
  *             return PyDateTime_DELTA_GET_MICROSECONDS(self)
  * 
  */
 
 #line 157 "cpython/datetime.pxd"
 
 
@@ -39030,40 +39073,40 @@
 
 #line 157 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":282
  * # Datetime C API initialization function.
  * # You have to call it before any usage of DateTime CAPI functions.
- * cdef inline void import_datetime():             # <<<<<<<<<<<<<<
+ * cdef inline void import_datetime() noexcept:             # <<<<<<<<<<<<<<
  *     PyDateTime_IMPORT
  * 
  */
 
 #line 282 "cpython/datetime.pxd"
 
 
 #line 282 "cpython/datetime.pxd"
 static CYTHON_INLINE void __pyx_f_7cpython_8datetime_import_datetime(void) {
 
   /* "cpython/datetime.pxd":283
  * # You have to call it before any usage of DateTime CAPI functions.
- * cdef inline void import_datetime():
+ * cdef inline void import_datetime() noexcept:
  *     PyDateTime_IMPORT             # <<<<<<<<<<<<<<
  * 
  * # Create date object using DateTime CAPI factory function.
  */
 
 #line 283 "cpython/datetime.pxd"
   (void)(PyDateTime_IMPORT);
 
   /* "cpython/datetime.pxd":282
  * # Datetime C API initialization function.
  * # You have to call it before any usage of DateTime CAPI functions.
- * cdef inline void import_datetime():             # <<<<<<<<<<<<<<
+ * cdef inline void import_datetime() noexcept:             # <<<<<<<<<<<<<<
  *     PyDateTime_IMPORT
  * 
  */
 
 #line 282 "cpython/datetime.pxd"
 
 
@@ -40351,15 +40394,15 @@
 
 #line 336 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":340
  * 
  * # Get year of date
- * cdef inline int date_year(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int date_year(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
 #line 340 "cpython/datetime.pxd"
 
 
@@ -40367,30 +40410,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_date_year(PyObject *__pyx_v_o) {
 
 #line 340 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":341
  * # Get year of date
- * cdef inline int date_year(object o):
+ * cdef inline int date_year(object o) noexcept:
  *     return PyDateTime_GET_YEAR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get month of date
  */
 
 #line 341 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_YEAR(__pyx_v_o);
 
 #line 341 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":340
  * 
  * # Get year of date
- * cdef inline int date_year(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int date_year(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
 #line 340 "cpython/datetime.pxd"
 
 
@@ -40405,15 +40448,15 @@
 
 #line 340 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":344
  * 
  * # Get month of date
- * cdef inline int date_month(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int date_month(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
 #line 344 "cpython/datetime.pxd"
 
 
@@ -40421,30 +40464,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_date_month(PyObject *__pyx_v_o) {
 
 #line 344 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":345
  * # Get month of date
- * cdef inline int date_month(object o):
+ * cdef inline int date_month(object o) noexcept:
  *     return PyDateTime_GET_MONTH(o)             # <<<<<<<<<<<<<<
  * 
  * # Get day of date
  */
 
 #line 345 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_MONTH(__pyx_v_o);
 
 #line 345 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":344
  * 
  * # Get month of date
- * cdef inline int date_month(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int date_month(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
 #line 344 "cpython/datetime.pxd"
 
 
@@ -40459,15 +40502,15 @@
 
 #line 344 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":348
  * 
  * # Get day of date
- * cdef inline int date_day(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int date_day(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
 #line 348 "cpython/datetime.pxd"
 
 
@@ -40475,30 +40518,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_date_day(PyObject *__pyx_v_o) {
 
 #line 348 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":349
  * # Get day of date
- * cdef inline int date_day(object o):
+ * cdef inline int date_day(object o) noexcept:
  *     return PyDateTime_GET_DAY(o)             # <<<<<<<<<<<<<<
  * 
  * # Get year of datetime
  */
 
 #line 349 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_DAY(__pyx_v_o);
 
 #line 349 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":348
  * 
  * # Get day of date
- * cdef inline int date_day(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int date_day(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
 #line 348 "cpython/datetime.pxd"
 
 
@@ -40513,15 +40556,15 @@
 
 #line 348 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":352
  * 
  * # Get year of datetime
- * cdef inline int datetime_year(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_year(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
 #line 352 "cpython/datetime.pxd"
 
 
@@ -40529,30 +40572,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_year(PyObject *__pyx_v_o) {
 
 #line 352 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":353
  * # Get year of datetime
- * cdef inline int datetime_year(object o):
+ * cdef inline int datetime_year(object o) noexcept:
  *     return PyDateTime_GET_YEAR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get month of datetime
  */
 
 #line 353 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_YEAR(__pyx_v_o);
 
 #line 353 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":352
  * 
  * # Get year of datetime
- * cdef inline int datetime_year(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_year(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_YEAR(o)
  * 
  */
 
 #line 352 "cpython/datetime.pxd"
 
 
@@ -40567,15 +40610,15 @@
 
 #line 352 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":356
  * 
  * # Get month of datetime
- * cdef inline int datetime_month(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_month(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
 #line 356 "cpython/datetime.pxd"
 
 
@@ -40583,30 +40626,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_month(PyObject *__pyx_v_o) {
 
 #line 356 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":357
  * # Get month of datetime
- * cdef inline int datetime_month(object o):
+ * cdef inline int datetime_month(object o) noexcept:
  *     return PyDateTime_GET_MONTH(o)             # <<<<<<<<<<<<<<
  * 
  * # Get day of datetime
  */
 
 #line 357 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_MONTH(__pyx_v_o);
 
 #line 357 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":356
  * 
  * # Get month of datetime
- * cdef inline int datetime_month(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_month(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_MONTH(o)
  * 
  */
 
 #line 356 "cpython/datetime.pxd"
 
 
@@ -40621,15 +40664,15 @@
 
 #line 356 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":360
  * 
  * # Get day of datetime
- * cdef inline int datetime_day(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_day(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
 #line 360 "cpython/datetime.pxd"
 
 
@@ -40637,30 +40680,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_day(PyObject *__pyx_v_o) {
 
 #line 360 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":361
  * # Get day of datetime
- * cdef inline int datetime_day(object o):
+ * cdef inline int datetime_day(object o) noexcept:
  *     return PyDateTime_GET_DAY(o)             # <<<<<<<<<<<<<<
  * 
  * # Get hour of time
  */
 
 #line 361 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_GET_DAY(__pyx_v_o);
 
 #line 361 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":360
  * 
  * # Get day of datetime
- * cdef inline int datetime_day(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_day(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_GET_DAY(o)
  * 
  */
 
 #line 360 "cpython/datetime.pxd"
 
 
@@ -40675,15 +40718,15 @@
 
 #line 360 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":364
  * 
  * # Get hour of time
- * cdef inline int time_hour(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_hour(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_HOUR(o)
  * 
  */
 
 #line 364 "cpython/datetime.pxd"
 
 
@@ -40691,30 +40734,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_hour(PyObject *__pyx_v_o) {
 
 #line 364 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":365
  * # Get hour of time
- * cdef inline int time_hour(object o):
+ * cdef inline int time_hour(object o) noexcept:
  *     return PyDateTime_TIME_GET_HOUR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get minute of time
  */
 
 #line 365 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_HOUR(__pyx_v_o);
 
 #line 365 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":364
  * 
  * # Get hour of time
- * cdef inline int time_hour(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_hour(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_HOUR(o)
  * 
  */
 
 #line 364 "cpython/datetime.pxd"
 
 
@@ -40729,15 +40772,15 @@
 
 #line 364 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":368
  * 
  * # Get minute of time
- * cdef inline int time_minute(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_minute(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MINUTE(o)
  * 
  */
 
 #line 368 "cpython/datetime.pxd"
 
 
@@ -40745,30 +40788,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_minute(PyObject *__pyx_v_o) {
 
 #line 368 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":369
  * # Get minute of time
- * cdef inline int time_minute(object o):
+ * cdef inline int time_minute(object o) noexcept:
  *     return PyDateTime_TIME_GET_MINUTE(o)             # <<<<<<<<<<<<<<
  * 
  * # Get second of time
  */
 
 #line 369 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_MINUTE(__pyx_v_o);
 
 #line 369 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":368
  * 
  * # Get minute of time
- * cdef inline int time_minute(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_minute(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MINUTE(o)
  * 
  */
 
 #line 368 "cpython/datetime.pxd"
 
 
@@ -40783,15 +40826,15 @@
 
 #line 368 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":372
  * 
  * # Get second of time
- * cdef inline int time_second(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_second(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_SECOND(o)
  * 
  */
 
 #line 372 "cpython/datetime.pxd"
 
 
@@ -40799,30 +40842,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_second(PyObject *__pyx_v_o) {
 
 #line 372 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":373
  * # Get second of time
- * cdef inline int time_second(object o):
+ * cdef inline int time_second(object o) noexcept:
  *     return PyDateTime_TIME_GET_SECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get microsecond of time
  */
 
 #line 373 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_SECOND(__pyx_v_o);
 
 #line 373 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":372
  * 
  * # Get second of time
- * cdef inline int time_second(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_second(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_SECOND(o)
  * 
  */
 
 #line 372 "cpython/datetime.pxd"
 
 
@@ -40837,15 +40880,15 @@
 
 #line 372 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":376
  * 
  * # Get microsecond of time
- * cdef inline int time_microsecond(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_microsecond(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MICROSECOND(o)
  * 
  */
 
 #line 376 "cpython/datetime.pxd"
 
 
@@ -40853,30 +40896,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_microsecond(PyObject *__pyx_v_o) {
 
 #line 376 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":377
  * # Get microsecond of time
- * cdef inline int time_microsecond(object o):
+ * cdef inline int time_microsecond(object o) noexcept:
  *     return PyDateTime_TIME_GET_MICROSECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get fold of time
  */
 
 #line 377 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_TIME_GET_MICROSECOND(__pyx_v_o);
 
 #line 377 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":376
  * 
  * # Get microsecond of time
- * cdef inline int time_microsecond(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_microsecond(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_TIME_GET_MICROSECOND(o)
  * 
  */
 
 #line 376 "cpython/datetime.pxd"
 
 
@@ -40891,30 +40934,30 @@
 
 #line 376 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":380
  * 
  * # Get fold of time
- * cdef inline int time_fold(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_fold(object o) noexcept:             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_TIME_GET_FOLD(o)
  */
 
 #line 380 "cpython/datetime.pxd"
 
 
 #line 380 "cpython/datetime.pxd"
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_time_fold(PyObject *__pyx_v_o) {
 
 #line 380 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":382
- * cdef inline int time_fold(object o):
+ * cdef inline int time_fold(object o) noexcept:
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_TIME_GET_FOLD(o)             # <<<<<<<<<<<<<<
  * 
  * # Get hour of datetime
  */
 
 #line 382 "cpython/datetime.pxd"
@@ -40922,15 +40965,15 @@
 
 #line 382 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":380
  * 
  * # Get fold of time
- * cdef inline int time_fold(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int time_fold(object o) noexcept:             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_TIME_GET_FOLD(o)
  */
 
 #line 380 "cpython/datetime.pxd"
 
 
@@ -40945,15 +40988,15 @@
 
 #line 380 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":385
  * 
  * # Get hour of datetime
- * cdef inline int datetime_hour(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_hour(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_HOUR(o)
  * 
  */
 
 #line 385 "cpython/datetime.pxd"
 
 
@@ -40961,30 +41004,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_hour(PyObject *__pyx_v_o) {
 
 #line 385 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":386
  * # Get hour of datetime
- * cdef inline int datetime_hour(object o):
+ * cdef inline int datetime_hour(object o) noexcept:
  *     return PyDateTime_DATE_GET_HOUR(o)             # <<<<<<<<<<<<<<
  * 
  * # Get minute of datetime
  */
 
 #line 386 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_HOUR(__pyx_v_o);
 
 #line 386 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":385
  * 
  * # Get hour of datetime
- * cdef inline int datetime_hour(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_hour(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_HOUR(o)
  * 
  */
 
 #line 385 "cpython/datetime.pxd"
 
 
@@ -40999,15 +41042,15 @@
 
 #line 385 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":389
  * 
  * # Get minute of datetime
- * cdef inline int datetime_minute(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_minute(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MINUTE(o)
  * 
  */
 
 #line 389 "cpython/datetime.pxd"
 
 
@@ -41015,30 +41058,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_minute(PyObject *__pyx_v_o) {
 
 #line 389 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":390
  * # Get minute of datetime
- * cdef inline int datetime_minute(object o):
+ * cdef inline int datetime_minute(object o) noexcept:
  *     return PyDateTime_DATE_GET_MINUTE(o)             # <<<<<<<<<<<<<<
  * 
  * # Get second of datetime
  */
 
 #line 390 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_MINUTE(__pyx_v_o);
 
 #line 390 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":389
  * 
  * # Get minute of datetime
- * cdef inline int datetime_minute(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_minute(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MINUTE(o)
  * 
  */
 
 #line 389 "cpython/datetime.pxd"
 
 
@@ -41053,15 +41096,15 @@
 
 #line 389 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":393
  * 
  * # Get second of datetime
- * cdef inline int datetime_second(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_second(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_SECOND(o)
  * 
  */
 
 #line 393 "cpython/datetime.pxd"
 
 
@@ -41069,30 +41112,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_second(PyObject *__pyx_v_o) {
 
 #line 393 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":394
  * # Get second of datetime
- * cdef inline int datetime_second(object o):
+ * cdef inline int datetime_second(object o) noexcept:
  *     return PyDateTime_DATE_GET_SECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get microsecond of datetime
  */
 
 #line 394 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_SECOND(__pyx_v_o);
 
 #line 394 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":393
  * 
  * # Get second of datetime
- * cdef inline int datetime_second(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_second(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_SECOND(o)
  * 
  */
 
 #line 393 "cpython/datetime.pxd"
 
 
@@ -41107,15 +41150,15 @@
 
 #line 393 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":397
  * 
  * # Get microsecond of datetime
- * cdef inline int datetime_microsecond(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_microsecond(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MICROSECOND(o)
  * 
  */
 
 #line 397 "cpython/datetime.pxd"
 
 
@@ -41123,30 +41166,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_microsecond(PyObject *__pyx_v_o) {
 
 #line 397 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":398
  * # Get microsecond of datetime
- * cdef inline int datetime_microsecond(object o):
+ * cdef inline int datetime_microsecond(object o) noexcept:
  *     return PyDateTime_DATE_GET_MICROSECOND(o)             # <<<<<<<<<<<<<<
  * 
  * # Get fold of datetime
  */
 
 #line 398 "cpython/datetime.pxd"
   __pyx_r = PyDateTime_DATE_GET_MICROSECOND(__pyx_v_o);
 
 #line 398 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":397
  * 
  * # Get microsecond of datetime
- * cdef inline int datetime_microsecond(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_microsecond(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return PyDateTime_DATE_GET_MICROSECOND(o)
  * 
  */
 
 #line 397 "cpython/datetime.pxd"
 
 
@@ -41161,30 +41204,30 @@
 
 #line 397 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":401
  * 
  * # Get fold of datetime
- * cdef inline int datetime_fold(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_fold(object o) noexcept:             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_DATE_GET_FOLD(o)
  */
 
 #line 401 "cpython/datetime.pxd"
 
 
 #line 401 "cpython/datetime.pxd"
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_datetime_fold(PyObject *__pyx_v_o) {
 
 #line 401 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":403
- * cdef inline int datetime_fold(object o):
+ * cdef inline int datetime_fold(object o) noexcept:
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_DATE_GET_FOLD(o)             # <<<<<<<<<<<<<<
  * 
  * # Get days of timedelta
  */
 
 #line 403 "cpython/datetime.pxd"
@@ -41192,15 +41235,15 @@
 
 #line 403 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":401
  * 
  * # Get fold of datetime
- * cdef inline int datetime_fold(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int datetime_fold(object o) noexcept:             # <<<<<<<<<<<<<<
  *     # For Python < 3.6 this returns 0 no matter what
  *     return PyDateTime_DATE_GET_FOLD(o)
  */
 
 #line 401 "cpython/datetime.pxd"
 
 
@@ -41215,15 +41258,15 @@
 
 #line 401 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":406
  * 
  * # Get days of timedelta
- * cdef inline int timedelta_days(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int timedelta_days(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).days
  * 
  */
 
 #line 406 "cpython/datetime.pxd"
 
 
@@ -41231,30 +41274,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_timedelta_days(PyObject *__pyx_v_o) {
 
 #line 406 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":407
  * # Get days of timedelta
- * cdef inline int timedelta_days(object o):
+ * cdef inline int timedelta_days(object o) noexcept:
  *     return (<PyDateTime_Delta*>o).days             # <<<<<<<<<<<<<<
  * 
  * # Get seconds of timedelta
  */
 
 #line 407 "cpython/datetime.pxd"
   __pyx_r = ((PyDateTime_Delta *)__pyx_v_o)->days;
 
 #line 407 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":406
  * 
  * # Get days of timedelta
- * cdef inline int timedelta_days(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int timedelta_days(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).days
  * 
  */
 
 #line 406 "cpython/datetime.pxd"
 
 
@@ -41269,15 +41312,15 @@
 
 #line 406 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":410
  * 
  * # Get seconds of timedelta
- * cdef inline int timedelta_seconds(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int timedelta_seconds(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).seconds
  * 
  */
 
 #line 410 "cpython/datetime.pxd"
 
 
@@ -41285,30 +41328,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_timedelta_seconds(PyObject *__pyx_v_o) {
 
 #line 410 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":411
  * # Get seconds of timedelta
- * cdef inline int timedelta_seconds(object o):
+ * cdef inline int timedelta_seconds(object o) noexcept:
  *     return (<PyDateTime_Delta*>o).seconds             # <<<<<<<<<<<<<<
  * 
  * # Get microseconds of timedelta
  */
 
 #line 411 "cpython/datetime.pxd"
   __pyx_r = ((PyDateTime_Delta *)__pyx_v_o)->seconds;
 
 #line 411 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":410
  * 
  * # Get seconds of timedelta
- * cdef inline int timedelta_seconds(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int timedelta_seconds(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).seconds
  * 
  */
 
 #line 410 "cpython/datetime.pxd"
 
 
@@ -41323,15 +41366,15 @@
 
 #line 410 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":414
  * 
  * # Get microseconds of timedelta
- * cdef inline int timedelta_microseconds(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int timedelta_microseconds(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).microseconds
  * 
  */
 
 #line 414 "cpython/datetime.pxd"
 
 
@@ -41339,30 +41382,30 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_timedelta_microseconds(PyObject *__pyx_v_o) {
 
 #line 414 "cpython/datetime.pxd"
   int __pyx_r;
 
   /* "cpython/datetime.pxd":415
  * # Get microseconds of timedelta
- * cdef inline int timedelta_microseconds(object o):
+ * cdef inline int timedelta_microseconds(object o) noexcept:
  *     return (<PyDateTime_Delta*>o).microseconds             # <<<<<<<<<<<<<<
  * 
- * cdef inline double total_seconds(timedelta obj):
+ * cdef inline double total_seconds(timedelta obj) noexcept:
  */
 
 #line 415 "cpython/datetime.pxd"
   __pyx_r = ((PyDateTime_Delta *)__pyx_v_o)->microseconds;
 
 #line 415 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":414
  * 
  * # Get microseconds of timedelta
- * cdef inline int timedelta_microseconds(object o):             # <<<<<<<<<<<<<<
+ * cdef inline int timedelta_microseconds(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return (<PyDateTime_Delta*>o).microseconds
  * 
  */
 
 #line 414 "cpython/datetime.pxd"
 
 
@@ -41377,15 +41420,15 @@
 
 #line 414 "cpython/datetime.pxd"
 }
 
 /* "cpython/datetime.pxd":417
  *     return (<PyDateTime_Delta*>o).microseconds
  * 
- * cdef inline double total_seconds(timedelta obj):             # <<<<<<<<<<<<<<
+ * cdef inline double total_seconds(timedelta obj) noexcept:             # <<<<<<<<<<<<<<
  *     # Mirrors the "timedelta.total_seconds()" method.
  *     # Note that this implementation is not guaranteed to give *exactly* the same
  */
 
 #line 417 "cpython/datetime.pxd"
 
 
@@ -41447,15 +41490,15 @@
 
 #line 426 "cpython/datetime.pxd"
   goto __pyx_L0;
 
   /* "cpython/datetime.pxd":417
  *     return (<PyDateTime_Delta*>o).microseconds
  * 
- * cdef inline double total_seconds(timedelta obj):             # <<<<<<<<<<<<<<
+ * cdef inline double total_seconds(timedelta obj) noexcept:             # <<<<<<<<<<<<<<
  *     # Mirrors the "timedelta.total_seconds()" method.
  *     # Note that this implementation is not guaranteed to give *exactly* the same
  */
 
 #line 417 "cpython/datetime.pxd"
 
 
@@ -42203,5715 +42246,5691 @@
 
 #line 673 "pyarrow/_parquet.pxd"
   return __pyx_r;
 
 #line 673 "pyarrow/_parquet.pxd"
 }
 
-/* "palletjack/palletjack_cython.pyx":12
+/* "palletjack/palletjack_cython.pyx":13
  * from pyarrow._parquet cimport *
  * 
  * cpdef generate_metadata_index(parquet_path, index_file_path = None):             # <<<<<<<<<<<<<<
  *     cdef string encoded_parquet_path = parquet_path.encode('utf8')
  *     cdef string encoded_index_file_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  */
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pw_10palletjack_17palletjack_cython_1generate_metadata_index(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_f_10palletjack_17palletjack_cython_generate_metadata_index(PyObject *__pyx_v_parquet_path, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_10palletjack_17palletjack_cython_generate_metadata_index *__pyx_optional_args) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_v_index_file_path = ((PyObject *)Py_None);
   std::string __pyx_v_encoded_parquet_path
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 ;
   std::string __pyx_v_encoded_index_file_path
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 ;
   std::vector<char>  __pyx_v_c_index_data
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 ;
   __Pyx_memviewslice __pyx_v_mv = { 0, 0, { 0 }, { 0 }, { 0 } }
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 ;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_r = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyDeclarations
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_1 = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_2 = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_3 = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_t_4;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   std::string __pyx_t_5;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_t_6;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   std::string __pyx_t_7;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   std::vector<char>  __pyx_t_8;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   char *__pyx_t_9;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   struct __pyx_array_obj *__pyx_t_10 = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_lineno = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   const char *__pyx_filename = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_clineno = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannySetupContext("generate_metadata_index", 1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   if (__pyx_optional_args) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     if (__pyx_optional_args->__pyx_n > 0) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       __pyx_v_index_file_path = __pyx_optional_args->index_file_path;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   }
 
-  /* "palletjack/palletjack_cython.pyx":13
+  /* "palletjack/palletjack_cython.pyx":14
  * 
  * cpdef generate_metadata_index(parquet_path, index_file_path = None):
  *     cdef string encoded_parquet_path = parquet_path.encode('utf8')             # <<<<<<<<<<<<<<
  *     cdef string encoded_index_file_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  *     cdef vector[char] c_index_data
  */
 
-#line 13 "palletjack/palletjack_cython.pyx"
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_parquet_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 13, __pyx_L1_error)
+#line 14 "palletjack/palletjack_cython.pyx"
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_parquet_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 14, __pyx_L1_error)
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_2);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   __pyx_t_3 = NULL;
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   __pyx_t_4 = 0;
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   #if CYTHON_UNPACK_METHODS
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   if (likely(PyMethod_Check(__pyx_t_2))) {
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     if (likely(__pyx_t_3)) {
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
       __Pyx_INCREF(__pyx_t_3);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
       __Pyx_INCREF(function);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
       __Pyx_DECREF_SET(__pyx_t_2, function);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
       __pyx_t_4 = 1;
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     }
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   }
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   {
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_n_u_utf8};
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-#line 13 "palletjack/palletjack_cython.pyx"
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+#line 14 "palletjack/palletjack_cython.pyx"
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_1);
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   }
 
-#line 13 "palletjack/palletjack_cython.pyx"
-  __pyx_t_5 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 13, __pyx_L1_error)
+#line 14 "palletjack/palletjack_cython.pyx"
+  __pyx_t_5 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 14, __pyx_L1_error)
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-#line 13 "palletjack/palletjack_cython.pyx"
+#line 14 "palletjack/palletjack_cython.pyx"
   __pyx_v_encoded_parquet_path = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_5);
 
-  /* "palletjack/palletjack_cython.pyx":14
+  /* "palletjack/palletjack_cython.pyx":15
  * cpdef generate_metadata_index(parquet_path, index_file_path = None):
  *     cdef string encoded_parquet_path = parquet_path.encode('utf8')
  *     cdef string encoded_index_file_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')             # <<<<<<<<<<<<<<
  *     cdef vector[char] c_index_data
  *     cdef char[::1] mv;
  */
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
   __pyx_t_6 = (__pyx_v_index_file_path != Py_None);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
   if (__pyx_t_6) {
 
-#line 14 "palletjack/palletjack_cython.pyx"
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_file_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 14, __pyx_L1_error)
+#line 15 "palletjack/palletjack_cython.pyx"
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_file_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 15, __pyx_L1_error)
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_2);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     __pyx_t_3 = NULL;
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     __pyx_t_4 = 0;
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     #if CYTHON_UNPACK_METHODS
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     if (likely(PyMethod_Check(__pyx_t_2))) {
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       if (likely(__pyx_t_3)) {
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
         __Pyx_INCREF(__pyx_t_3);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
         __Pyx_INCREF(function);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
         __Pyx_DECREF_SET(__pyx_t_2, function);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
         __pyx_t_4 = 1;
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       }
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     }
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     #endif
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     {
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_n_u_utf8};
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-#line 14 "palletjack/palletjack_cython.pyx"
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+#line 15 "palletjack/palletjack_cython.pyx"
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       __Pyx_GOTREF(__pyx_t_1);
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     }
 
-#line 14 "palletjack/palletjack_cython.pyx"
-    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 14, __pyx_L1_error)
+#line 15 "palletjack/palletjack_cython.pyx"
+    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 15, __pyx_L1_error)
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     __pyx_t_5 = __pyx_t_7;
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
   } else {
 
-#line 14 "palletjack/palletjack_cython.pyx"
-    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_kp_b__10); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 14, __pyx_L1_error)
+#line 15 "palletjack/palletjack_cython.pyx"
+    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_kp_b__10); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 15, __pyx_L1_error)
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
     __pyx_t_5 = __pyx_t_7;
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
   }
 
-#line 14 "palletjack/palletjack_cython.pyx"
+#line 15 "palletjack/palletjack_cython.pyx"
   __pyx_v_encoded_index_file_path = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_5);
 
-  /* "palletjack/palletjack_cython.pyx":17
+  /* "palletjack/palletjack_cython.pyx":18
  *     cdef vector[char] c_index_data
  *     cdef char[::1] mv;
  *     if index_file_path is None:             # <<<<<<<<<<<<<<
  *         with nogil:
  *             c_index_data = cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str())
  */
 
-#line 17 "palletjack/palletjack_cython.pyx"
+#line 18 "palletjack/palletjack_cython.pyx"
   __pyx_t_6 = (__pyx_v_index_file_path == Py_None);
 
-#line 17 "palletjack/palletjack_cython.pyx"
+#line 18 "palletjack/palletjack_cython.pyx"
   if (__pyx_t_6) {
 
-    /* "palletjack/palletjack_cython.pyx":18
+    /* "palletjack/palletjack_cython.pyx":19
  *     cdef char[::1] mv;
  *     if index_file_path is None:
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_index_data = cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str())
  *         mv = <char[:c_index_data.size()]>&c_index_data[0]
  */
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
     {
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         #ifdef WITH_THREAD
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         PyThreadState *_save;
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         _save = NULL;
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         Py_UNBLOCK_THREADS
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         __Pyx_FastGIL_Remember();
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         #endif
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         /*try:*/ {
 
-          /* "palletjack/palletjack_cython.pyx":19
+          /* "palletjack/palletjack_cython.pyx":20
  *     if index_file_path is None:
  *         with nogil:
  *             c_index_data = cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str())             # <<<<<<<<<<<<<<
  *         mv = <char[:c_index_data.size()]>&c_index_data[0]
  *         return bytearray(mv)
  */
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
           try {
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
             __pyx_t_8 = GenerateMetadataIndex(__pyx_v_encoded_parquet_path.c_str());
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
           } catch(...) {
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
             PyGILState_STATE 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
 __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
             __Pyx_CppExn2PyErr();
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
             __Pyx_PyGILState_Release(__pyx_gilstate_save);
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 19 "palletjack/palletjack_cython.pyx"
-            __PYX_ERR(1, 19, __pyx_L5_error)
+#line 20 "palletjack/palletjack_cython.pyx"
+            __PYX_ERR(1, 20, __pyx_L5_error)
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
           }
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
           __pyx_v_c_index_data = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_8);
 
-#line 19 "palletjack/palletjack_cython.pyx"
+#line 20 "palletjack/palletjack_cython.pyx"
         }
 
-        /* "palletjack/palletjack_cython.pyx":18
+        /* "palletjack/palletjack_cython.pyx":19
  *     cdef char[::1] mv;
  *     if index_file_path is None:
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_index_data = cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str())
  *         mv = <char[:c_index_data.size()]>&c_index_data[0]
  */
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         /*finally:*/ {
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
           /*normal exit:*/{
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             goto __pyx_L6;
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
           }
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
           __pyx_L5_error: {
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
             goto __pyx_L1_error;
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
           }
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
           __pyx_L6:;
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
         }
 
-#line 18 "palletjack/palletjack_cython.pyx"
+#line 19 "palletjack/palletjack_cython.pyx"
     }
 
-    /* "palletjack/palletjack_cython.pyx":20
+    /* "palletjack/palletjack_cython.pyx":21
  *         with nogil:
  *             c_index_data = cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str())
  *         mv = <char[:c_index_data.size()]>&c_index_data[0]             # <<<<<<<<<<<<<<
  *         return bytearray(mv)
  *     else:
  */
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __pyx_t_9 = (&(__pyx_v_c_index_data[0]));
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     if (!__pyx_t_9) {
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
       PyErr_SetString(PyExc_ValueError,"Cannot create cython.array from NULL pointer");
 
-#line 20 "palletjack/palletjack_cython.pyx"
-      __PYX_ERR(1, 20, __pyx_L1_error)
+#line 21 "palletjack/palletjack_cython.pyx"
+      __PYX_ERR(1, 21, __pyx_L1_error)
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     }
 
-#line 20 "palletjack/palletjack_cython.pyx"
-    __pyx_t_2 = __pyx_format_from_typeinfo(&__Pyx_TypeInfo_char); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 20, __pyx_L1_error)
+#line 21 "palletjack/palletjack_cython.pyx"
+    __pyx_t_2 = __pyx_format_from_typeinfo(&__Pyx_TypeInfo_char); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 21, __pyx_L1_error)
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_2);
 
-#line 20 "palletjack/palletjack_cython.pyx"
-    __pyx_t_1 = Py_BuildValue((char*) "("  __PYX_BUILD_PY_SSIZE_T  ")", ((Py_ssize_t)__pyx_v_c_index_data.size())); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 20, __pyx_L1_error)
+#line 21 "palletjack/palletjack_cython.pyx"
+    __pyx_t_1 = Py_BuildValue((char*) "("  __PYX_BUILD_PY_SSIZE_T  ")", ((Py_ssize_t)__pyx_v_c_index_data.size())); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 21, __pyx_L1_error)
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_1);
 
-#line 20 "palletjack/palletjack_cython.pyx"
-    __pyx_t_10 = __pyx_array_new(__pyx_t_1, sizeof(char), PyBytes_AS_STRING(__pyx_t_2), (char *) "c", (char *) __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 20, __pyx_L1_error)
+#line 21 "palletjack/palletjack_cython.pyx"
+    __pyx_t_10 = __pyx_array_new(__pyx_t_1, sizeof(char), PyBytes_AS_STRING(__pyx_t_2), (char *) "c", (char *) __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 21, __pyx_L1_error)
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF((PyObject *)__pyx_t_10);
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 20 "palletjack/palletjack_cython.pyx"
-    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_char(((PyObject *)__pyx_t_10), PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(1, 20, __pyx_L1_error)
+#line 21 "palletjack/palletjack_cython.pyx"
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_dc_char(((PyObject *)__pyx_t_10), PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(1, 21, __pyx_L1_error)
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF((PyObject *)__pyx_t_10); __pyx_t_10 = 0;
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __pyx_v_mv = __pyx_t_11;
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __pyx_t_11.memview = NULL;
 
-#line 20 "palletjack/palletjack_cython.pyx"
+#line 21 "palletjack/palletjack_cython.pyx"
     __pyx_t_11.data = NULL;
 
-    /* "palletjack/palletjack_cython.pyx":21
+    /* "palletjack/palletjack_cython.pyx":22
  *             c_index_data = cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str())
  *         mv = <char[:c_index_data.size()]>&c_index_data[0]
  *         return bytearray(mv)             # <<<<<<<<<<<<<<
  *     else:
  *         with nogil:
  */
 
-#line 21 "palletjack/palletjack_cython.pyx"
+#line 22 "palletjack/palletjack_cython.pyx"
     __Pyx_XDECREF(__pyx_r);
 
-#line 21 "palletjack/palletjack_cython.pyx"
-    __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_mv, 1, (PyObject *(*)(char *)) __pyx_memview_get_char, (int (*)(char *, PyObject *)) __pyx_memview_set_char, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 21, __pyx_L1_error)
+#line 22 "palletjack/palletjack_cython.pyx"
+    __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_mv, 1, (PyObject *(*)(char *)) __pyx_memview_get_char, (int (*)(char *, PyObject *)) __pyx_memview_set_char, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 22, __pyx_L1_error)
 
-#line 21 "palletjack/palletjack_cython.pyx"
+#line 22 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_2);
 
-#line 21 "palletjack/palletjack_cython.pyx"
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 21, __pyx_L1_error)
+#line 22 "palletjack/palletjack_cython.pyx"
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 22, __pyx_L1_error)
 
-#line 21 "palletjack/palletjack_cython.pyx"
+#line 22 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_1);
 
-#line 21 "palletjack/palletjack_cython.pyx"
+#line 22 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-#line 21 "palletjack/palletjack_cython.pyx"
+#line 22 "palletjack/palletjack_cython.pyx"
     __pyx_r = __pyx_t_1;
 
-#line 21 "palletjack/palletjack_cython.pyx"
+#line 22 "palletjack/palletjack_cython.pyx"
     __pyx_t_1 = 0;
 
-#line 21 "palletjack/palletjack_cython.pyx"
+#line 22 "palletjack/palletjack_cython.pyx"
     goto __pyx_L0;
 
-    /* "palletjack/palletjack_cython.pyx":17
+    /* "palletjack/palletjack_cython.pyx":18
  *     cdef vector[char] c_index_data
  *     cdef char[::1] mv;
  *     if index_file_path is None:             # <<<<<<<<<<<<<<
  *         with nogil:
  *             c_index_data = cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str())
  */
 
-#line 17 "palletjack/palletjack_cython.pyx"
+#line 18 "palletjack/palletjack_cython.pyx"
   }
 
-  /* "palletjack/palletjack_cython.pyx":23
+  /* "palletjack/palletjack_cython.pyx":24
  *         return bytearray(mv)
  *     else:
  *         with nogil:             # <<<<<<<<<<<<<<
  *             cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str(), encoded_index_file_path.c_str())
  * 
  */
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
   /*else*/ {
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
     {
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         #ifdef WITH_THREAD
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         PyThreadState *_save;
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         _save = NULL;
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         Py_UNBLOCK_THREADS
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         __Pyx_FastGIL_Remember();
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         #endif
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         /*try:*/ {
 
-          /* "palletjack/palletjack_cython.pyx":24
+          /* "palletjack/palletjack_cython.pyx":25
  *     else:
  *         with nogil:
  *             cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str(), encoded_index_file_path.c_str())             # <<<<<<<<<<<<<<
  * 
  *     return None
  */
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
           try {
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
             GenerateMetadataIndex(__pyx_v_encoded_parquet_path.c_str(), __pyx_v_encoded_index_file_path.c_str());
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
           } catch(...) {
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
             PyGILState_STATE 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
 __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
             __Pyx_CppExn2PyErr();
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
             __Pyx_PyGILState_Release(__pyx_gilstate_save);
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 24 "palletjack/palletjack_cython.pyx"
-            __PYX_ERR(1, 24, __pyx_L8_error)
+#line 25 "palletjack/palletjack_cython.pyx"
+            __PYX_ERR(1, 25, __pyx_L8_error)
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
           }
 
-#line 24 "palletjack/palletjack_cython.pyx"
+#line 25 "palletjack/palletjack_cython.pyx"
         }
 
-        /* "palletjack/palletjack_cython.pyx":23
+        /* "palletjack/palletjack_cython.pyx":24
  *         return bytearray(mv)
  *     else:
  *         with nogil:             # <<<<<<<<<<<<<<
  *             cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str(), encoded_index_file_path.c_str())
  * 
  */
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         /*finally:*/ {
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
           /*normal exit:*/{
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             goto __pyx_L9;
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
           }
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
           __pyx_L8_error: {
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
             goto __pyx_L1_error;
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
           }
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
           __pyx_L9:;
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
         }
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
     }
 
-#line 23 "palletjack/palletjack_cython.pyx"
+#line 24 "palletjack/palletjack_cython.pyx"
   }
 
-  /* "palletjack/palletjack_cython.pyx":26
+  /* "palletjack/palletjack_cython.pyx":27
  *             cpalletjack.GenerateMetadataIndex(encoded_parquet_path.c_str(), encoded_index_file_path.c_str())
  * 
  *     return None             # <<<<<<<<<<<<<<
  * 
  * cpdef read_metadata(index_file_path = None, row_groups = [], column_indices = [], column_names = [], index_data = None):
  */
 
-#line 26 "palletjack/palletjack_cython.pyx"
+#line 27 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_r);
 
-#line 26 "palletjack/palletjack_cython.pyx"
+#line 27 "palletjack/palletjack_cython.pyx"
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
 
-#line 26 "palletjack/palletjack_cython.pyx"
+#line 27 "palletjack/palletjack_cython.pyx"
   goto __pyx_L0;
 
-  /* "palletjack/palletjack_cython.pyx":12
+  /* "palletjack/palletjack_cython.pyx":13
  * from pyarrow._parquet cimport *
  * 
  * cpdef generate_metadata_index(parquet_path, index_file_path = None):             # <<<<<<<<<<<<<<
  *     cdef string encoded_parquet_path = parquet_path.encode('utf8')
  *     cdef string encoded_index_file_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  */
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   /* function exit code */
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L1_error:;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_2);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_3);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF((PyObject *)__pyx_t_10);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __PYX_XCLEAR_MEMVIEW(&__pyx_t_11, 1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_AddTraceback("palletjack.palletjack_cython.generate_metadata_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_r = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L0:;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_mv, 1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XGIVEREF(__pyx_r);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   return __pyx_r;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 /* Python wrapper */
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pw_10palletjack_17palletjack_cython_1generate_metadata_index(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 PyDoc_STRVAR(__pyx_doc_10palletjack_17palletjack_cython_generate_metadata_index, "generate_metadata_index(parquet_path, index_file_path=None)");
 static PyMethodDef __pyx_mdef_10palletjack_17palletjack_cython_1generate_metadata_index = 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 {"generate_metadata_index", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10palletjack_17palletjack_cython_1generate_metadata_index, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10palletjack_17palletjack_cython_generate_metadata_index};
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pw_10palletjack_17palletjack_cython_1generate_metadata_index(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_parquet_path = 0
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 ;
   PyObject *__pyx_v_index_file_path = 0
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 ;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_METH_FASTCALL
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject* values[2] = {0,0};
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_lineno = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   const char *__pyx_filename = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_clineno = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_r = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyDeclarations
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannySetupContext("generate_metadata_index (wrapper)", 0);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_METH_FASTCALL
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   #if CYTHON_ASSUME_SAFE_MACROS
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_parquet_path,&__pyx_n_s_index_file_path,0};
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     values[1] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     if (__pyx_kwds) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       Py_ssize_t kw_args;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       switch (__pyx_nargs) {
         case  2: 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  1: 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  0: 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 break;
         default: 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 goto __pyx_L5_argtuple_error;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       switch (__pyx_nargs) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         case  0:
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_parquet_path)) != 0)) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
           kw_args--;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         }
 
-#line 12 "palletjack/palletjack_cython.pyx"
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L3_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 13, __pyx_L3_error)
         else 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 goto __pyx_L5_argtuple_error;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         case  1:
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         if (kw_args > 0) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index_file_path);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
 
-#line 12 "palletjack/palletjack_cython.pyx"
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 12, __pyx_L3_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 13, __pyx_L3_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       if (unlikely(kw_args > 0)) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
 
-#line 12 "palletjack/palletjack_cython.pyx"
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "generate_metadata_index") < 0)) __PYX_ERR(1, 12, __pyx_L3_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "generate_metadata_index") < 0)) __PYX_ERR(1, 13, __pyx_L3_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     } else {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       switch (__pyx_nargs) {
         case  2: 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  1: 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
         break;
         default: 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 goto __pyx_L5_argtuple_error;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     __pyx_v_parquet_path = values[0];
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     __pyx_v_index_file_path = values[1];
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   goto __pyx_L6_skip;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L5_argtuple_error:;
 
-#line 12 "palletjack/palletjack_cython.pyx"
-  __Pyx_RaiseArgtupleInvalid("generate_metadata_index", 0, 1, 2, __pyx_nargs); __PYX_ERR(1, 12, __pyx_L3_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+  __Pyx_RaiseArgtupleInvalid("generate_metadata_index", 0, 1, 2, __pyx_nargs); __PYX_ERR(1, 13, __pyx_L3_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L6_skip:;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   goto __pyx_L4_argument_unpacking_done;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L3_error:;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     Py_ssize_t __pyx_temp;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_AddTraceback("palletjack.palletjack_cython.generate_metadata_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   return NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 __pyx_pf_10palletjack_17palletjack_cython_generate_metadata_index(__pyx_self, __pyx_v_parquet_path, __pyx_v_index_file_path);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   /* function exit code */
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     Py_ssize_t __pyx_temp;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
     }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   return __pyx_r;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 }
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pf_10palletjack_17palletjack_cython_generate_metadata_index(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_parquet_path, PyObject *__pyx_v_index_file_path) {
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_r = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyDeclarations
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_1 = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   struct __pyx_opt_args_10palletjack_17palletjack_cython_generate_metadata_index __pyx_t_2;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_lineno = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   const char *__pyx_filename = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   int __pyx_clineno = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannySetupContext("generate_metadata_index", 1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_r);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.__pyx_n = 1;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.index_file_path = __pyx_v_index_file_path;
 
-#line 12 "palletjack/palletjack_cython.pyx"
-  __pyx_t_1 = __pyx_f_10palletjack_17palletjack_cython_generate_metadata_index(__pyx_v_parquet_path, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+  __pyx_t_1 = __pyx_f_10palletjack_17palletjack_cython_generate_metadata_index(__pyx_v_parquet_path, 0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_r = __pyx_t_1;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_t_1 = 0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   goto __pyx_L0;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   /* function exit code */
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L1_error:;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_1);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_AddTraceback("palletjack.palletjack_cython.generate_metadata_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_r = NULL;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __pyx_L0:;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_XGIVEREF(__pyx_r);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   return __pyx_r;
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
 }
 
-/* "palletjack/palletjack_cython.pyx":28
+/* "palletjack/palletjack_cython.pyx":29
  *     return None
  * 
  * cpdef read_metadata(index_file_path = None, row_groups = [], column_indices = [], column_names = [], index_data = None):             # <<<<<<<<<<<<<<
  * 
  *     cdef shared_ptr[CFileMetaData] c_metadata
  */
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pw_10palletjack_17palletjack_cython_3read_metadata(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_f_10palletjack_17palletjack_cython_read_metadata(CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_10palletjack_17palletjack_cython_read_metadata *__pyx_optional_args) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_v_index_file_path = ((PyObject *)Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_v_row_groups = __pyx_k__16;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_v_column_indices = __pyx_k__17;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_v_column_names = __pyx_k__18;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_v_index_data = ((PyObject *)Py_None);
   std::shared_ptr< parquet::FileMetaData>  __pyx_v_c_metadata
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   std::string __pyx_v_encoded_path
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   __Pyx_memviewslice __pyx_v_mv = { 0, 0, { 0 }, { 0 }, { 0 } }
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   std::vector<uint32_t>  __pyx_v_crow_groups
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   std::vector<uint32_t>  __pyx_v_ccolumn_indices
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   std::vector<std::string>  __pyx_v_ccolumn_names
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   struct __pyx_obj_7pyarrow_8_parquet_FileMetaData *__pyx_v_m = 0
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   PyObject *__pyx_7genexpr__pyx_v_c = NULL
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_r = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyDeclarations
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   std::string __pyx_t_1;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_t_2;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_3 = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_4 = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_5 = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_t_6;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   std::string __pyx_t_7;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_memviewslice __pyx_t_8 = { 0, 0, { 0 }, { 0 }, { 0 } };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   std::vector<uint32_t>  __pyx_t_9;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_ssize_t __pyx_t_10;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *(*__pyx_t_11)(PyObject *);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_12 = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_13 = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   std::vector<std::string>  __pyx_t_14;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_ssize_t __pyx_t_15;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   std::shared_ptr< parquet::FileMetaData>  __pyx_t_16;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_lineno = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   const char *__pyx_filename = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_clineno = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannySetupContext("read_metadata", 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (__pyx_optional_args) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (__pyx_optional_args->__pyx_n > 0) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       __pyx_v_index_file_path = __pyx_optional_args->index_file_path;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       if (__pyx_optional_args->__pyx_n > 1) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         __pyx_v_row_groups = __pyx_optional_args->row_groups;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         if (__pyx_optional_args->__pyx_n > 2) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           __pyx_v_column_indices = __pyx_optional_args->column_indices;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           if (__pyx_optional_args->__pyx_n > 3) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
             __pyx_v_column_names = __pyx_optional_args->column_names;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
             if (__pyx_optional_args->__pyx_n > 4) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
               __pyx_v_index_data = __pyx_optional_args->index_data;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
             }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-  /* "palletjack/palletjack_cython.pyx":31
+  /* "palletjack/palletjack_cython.pyx":32
  * 
  *     cdef shared_ptr[CFileMetaData] c_metadata
  *     cdef string encoded_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')             # <<<<<<<<<<<<<<
  *     cdef const unsigned char[::1] mv = index_data
  *     cdef vector[uint32_t] crow_groups = row_groups
  */
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
   __pyx_t_2 = (__pyx_v_index_file_path != Py_None);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
   if (__pyx_t_2) {
 
-#line 31 "palletjack/palletjack_cython.pyx"
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_file_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 31, __pyx_L1_error)
+#line 32 "palletjack/palletjack_cython.pyx"
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_file_path, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 32, __pyx_L1_error)
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_4);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     __pyx_t_5 = NULL;
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     __pyx_t_6 = 0;
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     #if CYTHON_UNPACK_METHODS
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     if (likely(PyMethod_Check(__pyx_t_4))) {
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       if (likely(__pyx_t_5)) {
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
         __Pyx_INCREF(__pyx_t_5);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
         __Pyx_INCREF(function);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
         __Pyx_DECREF_SET(__pyx_t_4, function);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
         __pyx_t_6 = 1;
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       }
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     }
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     #endif
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     {
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_n_u_utf8};
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-#line 31 "palletjack/palletjack_cython.pyx"
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 31, __pyx_L1_error)
+#line 32 "palletjack/palletjack_cython.pyx"
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 32, __pyx_L1_error)
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       __Pyx_GOTREF(__pyx_t_3);
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     }
 
-#line 31 "palletjack/palletjack_cython.pyx"
-    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 31, __pyx_L1_error)
+#line 32 "palletjack/palletjack_cython.pyx"
+    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 32, __pyx_L1_error)
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     __pyx_t_1 = __pyx_t_7;
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
   } else {
 
-#line 31 "palletjack/palletjack_cython.pyx"
-    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_kp_b__10); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 31, __pyx_L1_error)
+#line 32 "palletjack/palletjack_cython.pyx"
+    __pyx_t_7 = __pyx_convert_string_from_py_6libcpp_6string_std__in_string(__pyx_kp_b__10); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 32, __pyx_L1_error)
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
     __pyx_t_1 = __pyx_t_7;
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
   }
 
-#line 31 "palletjack/palletjack_cython.pyx"
+#line 32 "palletjack/palletjack_cython.pyx"
   __pyx_v_encoded_path = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1);
 
-  /* "palletjack/palletjack_cython.pyx":32
+  /* "palletjack/palletjack_cython.pyx":33
  *     cdef shared_ptr[CFileMetaData] c_metadata
  *     cdef string encoded_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  *     cdef const unsigned char[::1] mv = index_data             # <<<<<<<<<<<<<<
  *     cdef vector[uint32_t] crow_groups = row_groups
  *     cdef vector[uint32_t] ccolumn_indices = column_indices
  */
 
-#line 32 "palletjack/palletjack_cython.pyx"
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_char__const__(__pyx_v_index_data, 0); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(1, 32, __pyx_L1_error)
+#line 33 "palletjack/palletjack_cython.pyx"
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_char__const__(__pyx_v_index_data, 0); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(1, 33, __pyx_L1_error)
 
-#line 32 "palletjack/palletjack_cython.pyx"
+#line 33 "palletjack/palletjack_cython.pyx"
   __pyx_v_mv = __pyx_t_8;
 
-#line 32 "palletjack/palletjack_cython.pyx"
+#line 33 "palletjack/palletjack_cython.pyx"
   __pyx_t_8.memview = NULL;
 
-#line 32 "palletjack/palletjack_cython.pyx"
+#line 33 "palletjack/palletjack_cython.pyx"
   __pyx_t_8.data = NULL;
 
-  /* "palletjack/palletjack_cython.pyx":33
+  /* "palletjack/palletjack_cython.pyx":34
  *     cdef string encoded_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  *     cdef const unsigned char[::1] mv = index_data
  *     cdef vector[uint32_t] crow_groups = row_groups             # <<<<<<<<<<<<<<
  *     cdef vector[uint32_t] ccolumn_indices = column_indices
  *     cdef vector[string] ccolumn_names = [c.encode('utf8') for c in column_names]
  */
 
-#line 33 "palletjack/palletjack_cython.pyx"
-  __pyx_t_9 = __pyx_convert_vector_from_py_uint32_t(__pyx_v_row_groups); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 33, __pyx_L1_error)
+#line 34 "palletjack/palletjack_cython.pyx"
+  __pyx_t_9 = __pyx_convert_vector_from_py_uint32_t(__pyx_v_row_groups); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 34, __pyx_L1_error)
 
-#line 33 "palletjack/palletjack_cython.pyx"
+#line 34 "palletjack/palletjack_cython.pyx"
   __pyx_v_crow_groups = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_9);
 
-  /* "palletjack/palletjack_cython.pyx":34
+  /* "palletjack/palletjack_cython.pyx":35
  *     cdef const unsigned char[::1] mv = index_data
  *     cdef vector[uint32_t] crow_groups = row_groups
  *     cdef vector[uint32_t] ccolumn_indices = column_indices             # <<<<<<<<<<<<<<
  *     cdef vector[string] ccolumn_names = [c.encode('utf8') for c in column_names]
  * 
  */
 
-#line 34 "palletjack/palletjack_cython.pyx"
-  __pyx_t_9 = __pyx_convert_vector_from_py_uint32_t(__pyx_v_column_indices); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 34, __pyx_L1_error)
+#line 35 "palletjack/palletjack_cython.pyx"
+  __pyx_t_9 = __pyx_convert_vector_from_py_uint32_t(__pyx_v_column_indices); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 35, __pyx_L1_error)
 
-#line 34 "palletjack/palletjack_cython.pyx"
+#line 35 "palletjack/palletjack_cython.pyx"
   __pyx_v_ccolumn_indices = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_9);
 
-  /* "palletjack/palletjack_cython.pyx":35
+  /* "palletjack/palletjack_cython.pyx":36
  *     cdef vector[uint32_t] crow_groups = row_groups
  *     cdef vector[uint32_t] ccolumn_indices = column_indices
  *     cdef vector[string] ccolumn_names = [c.encode('utf8') for c in column_names]             # <<<<<<<<<<<<<<
  * 
  *     if index_file_path is None:
  */
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
   { /* enter inner scope */
 
-#line 35 "palletjack/palletjack_cython.pyx"
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     __Pyx_GOTREF(__pyx_t_3);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     if (likely(PyList_CheckExact(__pyx_v_column_names)) || PyTuple_CheckExact(__pyx_v_column_names)) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __pyx_t_4 = __pyx_v_column_names; __Pyx_INCREF(__pyx_t_4);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __pyx_t_10 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __pyx_t_11 = NULL;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     } else {
       __pyx_t_10 = -1; 
-#line 35 "palletjack/palletjack_cython.pyx"
-__pyx_t_4 = PyObject_GetIter(__pyx_v_column_names); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+__pyx_t_4 = PyObject_GetIter(__pyx_v_column_names); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __Pyx_GOTREF(__pyx_t_4);
 
-#line 35 "palletjack/palletjack_cython.pyx"
-      __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+      __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     for (;;) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       if (likely(!__pyx_t_11)) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         if (likely(PyList_CheckExact(__pyx_t_4))) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             #if !CYTHON_ASSUME_SAFE_MACROS
 
-#line 35 "palletjack/palletjack_cython.pyx"
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             if (__pyx_t_10 >= __pyx_temp) break;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
 
-#line 35 "palletjack/palletjack_cython.pyx"
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           #else
 
-#line 35 "palletjack/palletjack_cython.pyx"
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           __Pyx_GOTREF(__pyx_t_5);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           #endif
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         } else {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             #if !CYTHON_ASSUME_SAFE_MACROS
 
-#line 35 "palletjack/palletjack_cython.pyx"
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             if (__pyx_t_10 >= __pyx_temp) break;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
 
-#line 35 "palletjack/palletjack_cython.pyx"
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_10); __Pyx_INCREF(__pyx_t_5); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           #else
 
-#line 35 "palletjack/palletjack_cython.pyx"
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           __Pyx_GOTREF(__pyx_t_5);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           #endif
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         }
       } else 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
 {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         __pyx_t_5 = __pyx_t_11(__pyx_t_4);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         if (unlikely(!__pyx_t_5)) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           PyObject* exc_type = PyErr_Occurred();
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           if (exc_type) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
 
-#line 35 "palletjack/palletjack_cython.pyx"
-            else __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+            else __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           break;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         __Pyx_GOTREF(__pyx_t_5);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_c, __pyx_t_5);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __pyx_t_5 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_c, __pyx_n_s_encode); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_7genexpr__pyx_v_c, __pyx_n_s_encode); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __Pyx_GOTREF(__pyx_t_12);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __pyx_t_13 = NULL;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __pyx_t_6 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       #if CYTHON_UNPACK_METHODS
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       if (likely(PyMethod_Check(__pyx_t_12))) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_12);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         if (likely(__pyx_t_13)) {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           __Pyx_INCREF(__pyx_t_13);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           __Pyx_INCREF(function);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           __Pyx_DECREF_SET(__pyx_t_12, function);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
           __pyx_t_6 = 1;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       #endif
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       {
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_n_u_utf8};
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         __Pyx_GOTREF(__pyx_t_5);
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       }
 
-#line 35 "palletjack/palletjack_cython.pyx"
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 35, __pyx_L5_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 36, __pyx_L5_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     }
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_c); __pyx_7genexpr__pyx_v_c = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     goto __pyx_L9_exit_scope;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     __pyx_L5_error:;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_c); __pyx_7genexpr__pyx_v_c = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     goto __pyx_L1_error;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
     __pyx_L9_exit_scope:;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
   } /* exit inner scope */
 
-#line 35 "palletjack/palletjack_cython.pyx"
-  __pyx_t_14 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 35, __pyx_L1_error)
+#line 36 "palletjack/palletjack_cython.pyx"
+  __pyx_t_14 = __pyx_convert_vector_from_py_std_3a__3a_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 36, __pyx_L1_error)
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-#line 35 "palletjack/palletjack_cython.pyx"
+#line 36 "palletjack/palletjack_cython.pyx"
   __pyx_v_ccolumn_names = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_14);
 
-  /* "palletjack/palletjack_cython.pyx":37
+  /* "palletjack/palletjack_cython.pyx":38
  *     cdef vector[string] ccolumn_names = [c.encode('utf8') for c in column_names]
  * 
  *     if index_file_path is None:             # <<<<<<<<<<<<<<
- *         with nogil:
- *             c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
+ *         with cython.boundscheck(False):
+ *             with nogil:
  */
 
-#line 37 "palletjack/palletjack_cython.pyx"
+#line 38 "palletjack/palletjack_cython.pyx"
   __pyx_t_2 = (__pyx_v_index_file_path == Py_None);
 
-#line 37 "palletjack/palletjack_cython.pyx"
+#line 38 "palletjack/palletjack_cython.pyx"
   if (__pyx_t_2) {
 
-    /* "palletjack/palletjack_cython.pyx":38
- * 
+    /* "palletjack/palletjack_cython.pyx":40
  *     if index_file_path is None:
- *         with nogil:             # <<<<<<<<<<<<<<
- *             c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
+ *         with cython.boundscheck(False):
+ *             with nogil:             # <<<<<<<<<<<<<<
+ *                 c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
  *     else:
  */
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
     {
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         #ifdef WITH_THREAD
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         PyThreadState *_save;
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         _save = NULL;
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         Py_UNBLOCK_THREADS
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         __Pyx_FastGIL_Remember();
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         #endif
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         /*try:*/ {
 
-          /* "palletjack/palletjack_cython.pyx":39
- *     if index_file_path is None:
- *         with nogil:
- *             c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)             # <<<<<<<<<<<<<<
+          /* "palletjack/palletjack_cython.pyx":41
+ *         with cython.boundscheck(False):
+ *             with nogil:
+ *                 c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)             # <<<<<<<<<<<<<<
  *     else:
  *         with nogil:
  */
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
           __pyx_t_15 = 0;
 
-#line 39 "palletjack/palletjack_cython.pyx"
-          __pyx_t_6 = -1;
-
-#line 39 "palletjack/palletjack_cython.pyx"
-          if (__pyx_t_15 < 0) {
-
-#line 39 "palletjack/palletjack_cython.pyx"
-            __pyx_t_15 += __pyx_v_mv.shape[0];
-
-#line 39 "palletjack/palletjack_cython.pyx"
-            if (unlikely(__pyx_t_15 < 0)) __pyx_t_6 = 0;
-          } else 
-#line 39 "palletjack/palletjack_cython.pyx"
-if (unlikely(__pyx_t_15 >= __pyx_v_mv.shape[0])) __pyx_t_6 = 0;
-
-#line 39 "palletjack/palletjack_cython.pyx"
-          if (unlikely(__pyx_t_6 != -1)) {
-
-#line 39 "palletjack/palletjack_cython.pyx"
-            __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_6);
-
-#line 39 "palletjack/palletjack_cython.pyx"
-            __PYX_ERR(1, 39, __pyx_L12_error)
-
-#line 39 "palletjack/palletjack_cython.pyx"
-          }
+#line 41 "palletjack/palletjack_cython.pyx"
+          if (__pyx_t_15 < 0) __pyx_t_15 += __pyx_v_mv.shape[0];
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
           __pyx_t_10 = __Pyx_MemoryView_Len(__pyx_v_mv); 
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
           try {
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
             __pyx_t_16 = ReadMetadata((&(*((unsigned char const  *) ( /* dim=0 */ ((char *) (((unsigned char const  *) __pyx_v_mv.data) + __pyx_t_15)) )))), __pyx_t_10, __pyx_v_crow_groups, __pyx_v_ccolumn_indices, __pyx_v_ccolumn_names);
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
           } catch(...) {
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
             PyGILState_STATE 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
 __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
             __Pyx_CppExn2PyErr();
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
             __Pyx_PyGILState_Release(__pyx_gilstate_save);
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 39 "palletjack/palletjack_cython.pyx"
-            __PYX_ERR(1, 39, __pyx_L12_error)
+#line 41 "palletjack/palletjack_cython.pyx"
+            __PYX_ERR(1, 41, __pyx_L12_error)
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
           }
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
           __pyx_v_c_metadata = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_16);
 
-#line 39 "palletjack/palletjack_cython.pyx"
+#line 41 "palletjack/palletjack_cython.pyx"
         }
 
-        /* "palletjack/palletjack_cython.pyx":38
- * 
+        /* "palletjack/palletjack_cython.pyx":40
  *     if index_file_path is None:
- *         with nogil:             # <<<<<<<<<<<<<<
- *             c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
+ *         with cython.boundscheck(False):
+ *             with nogil:             # <<<<<<<<<<<<<<
+ *                 c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
  *     else:
  */
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         /*finally:*/ {
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
           /*normal exit:*/{
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             goto __pyx_L13;
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
           }
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
           __pyx_L12_error: {
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
             goto __pyx_L1_error;
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
           }
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
           __pyx_L13:;
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
         }
 
-#line 38 "palletjack/palletjack_cython.pyx"
+#line 40 "palletjack/palletjack_cython.pyx"
     }
 
-    /* "palletjack/palletjack_cython.pyx":37
+    /* "palletjack/palletjack_cython.pyx":38
  *     cdef vector[string] ccolumn_names = [c.encode('utf8') for c in column_names]
  * 
  *     if index_file_path is None:             # <<<<<<<<<<<<<<
- *         with nogil:
- *             c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
+ *         with cython.boundscheck(False):
+ *             with nogil:
  */
 
-#line 37 "palletjack/palletjack_cython.pyx"
+#line 38 "palletjack/palletjack_cython.pyx"
     goto __pyx_L10;
 
-#line 37 "palletjack/palletjack_cython.pyx"
+#line 38 "palletjack/palletjack_cython.pyx"
   }
 
-  /* "palletjack/palletjack_cython.pyx":41
- *             c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
+  /* "palletjack/palletjack_cython.pyx":43
+ *                 c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
  *     else:
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_metadata = cpalletjack.ReadMetadata(encoded_path.c_str(), crow_groups, ccolumn_indices, ccolumn_names)
  * 
  */
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
   /*else*/ {
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
     {
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         #ifdef WITH_THREAD
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         PyThreadState *_save;
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         _save = NULL;
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         Py_UNBLOCK_THREADS
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         __Pyx_FastGIL_Remember();
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         #endif
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         /*try:*/ {
 
-          /* "palletjack/palletjack_cython.pyx":42
+          /* "palletjack/palletjack_cython.pyx":44
  *     else:
  *         with nogil:
  *             c_metadata = cpalletjack.ReadMetadata(encoded_path.c_str(), crow_groups, ccolumn_indices, ccolumn_names)             # <<<<<<<<<<<<<<
  * 
  *     cdef FileMetaData m = FileMetaData.__new__(FileMetaData)
  */
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
           try {
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
             __pyx_t_16 = ReadMetadata(__pyx_v_encoded_path.c_str(), __pyx_v_crow_groups, __pyx_v_ccolumn_indices, __pyx_v_ccolumn_names);
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
           } catch(...) {
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
             PyGILState_STATE 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
 __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
             __Pyx_CppExn2PyErr();
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
             __Pyx_PyGILState_Release(__pyx_gilstate_save);
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 42 "palletjack/palletjack_cython.pyx"
-            __PYX_ERR(1, 42, __pyx_L15_error)
+#line 44 "palletjack/palletjack_cython.pyx"
+            __PYX_ERR(1, 44, __pyx_L15_error)
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
           }
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
           __pyx_v_c_metadata = __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_16);
 
-#line 42 "palletjack/palletjack_cython.pyx"
+#line 44 "palletjack/palletjack_cython.pyx"
         }
 
-        /* "palletjack/palletjack_cython.pyx":41
- *             c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
+        /* "palletjack/palletjack_cython.pyx":43
+ *                 c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
  *     else:
  *         with nogil:             # <<<<<<<<<<<<<<
  *             c_metadata = cpalletjack.ReadMetadata(encoded_path.c_str(), crow_groups, ccolumn_indices, ccolumn_names)
  * 
  */
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         /*finally:*/ {
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
           /*normal exit:*/{
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             goto __pyx_L16;
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
           }
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
           __pyx_L15_error: {
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             #ifdef WITH_THREAD
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             __Pyx_FastGIL_Forget();
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             Py_BLOCK_THREADS
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             #endif
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
             goto __pyx_L1_error;
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
           }
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
           __pyx_L16:;
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
         }
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
     }
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
   }
 
-#line 41 "palletjack/palletjack_cython.pyx"
+#line 43 "palletjack/palletjack_cython.pyx"
   __pyx_L10:;
 
-  /* "palletjack/palletjack_cython.pyx":44
+  /* "palletjack/palletjack_cython.pyx":46
  *             c_metadata = cpalletjack.ReadMetadata(encoded_path.c_str(), crow_groups, ccolumn_indices, ccolumn_names)
  * 
  *     cdef FileMetaData m = FileMetaData.__new__(FileMetaData)             # <<<<<<<<<<<<<<
  *     m.init(c_metadata)
  *     return m
  */
 
-#line 44 "palletjack/palletjack_cython.pyx"
-  __pyx_t_3 = __Pyx_tp_new(((PyObject *)__pyx_ptype_7pyarrow_8_parquet_FileMetaData), __pyx_empty_tuple); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 44, __pyx_L1_error)
+#line 46 "palletjack/palletjack_cython.pyx"
+  __pyx_t_3 = __Pyx_tp_new(((PyObject *)__pyx_ptype_7pyarrow_8_parquet_FileMetaData), __pyx_empty_tuple); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 46, __pyx_L1_error)
 
-#line 44 "palletjack/palletjack_cython.pyx"
+#line 46 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_3);
 
-#line 44 "palletjack/palletjack_cython.pyx"
-  if (!(likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7pyarrow_8_parquet_FileMetaData)))) __PYX_ERR(1, 44, __pyx_L1_error)
+#line 46 "palletjack/palletjack_cython.pyx"
+  if (!(likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_7pyarrow_8_parquet_FileMetaData)))) __PYX_ERR(1, 46, __pyx_L1_error)
 
-#line 44 "palletjack/palletjack_cython.pyx"
+#line 46 "palletjack/palletjack_cython.pyx"
   __pyx_v_m = ((struct __pyx_obj_7pyarrow_8_parquet_FileMetaData *)__pyx_t_3);
 
-#line 44 "palletjack/palletjack_cython.pyx"
+#line 46 "palletjack/palletjack_cython.pyx"
   __pyx_t_3 = 0;
 
-  /* "palletjack/palletjack_cython.pyx":45
+  /* "palletjack/palletjack_cython.pyx":47
  * 
  *     cdef FileMetaData m = FileMetaData.__new__(FileMetaData)
  *     m.init(c_metadata)             # <<<<<<<<<<<<<<
  *     return m
  */
 
-#line 45 "palletjack/palletjack_cython.pyx"
-  __pyx_t_3 = __pyx_f_7pyarrow_8_parquet_12FileMetaData_init(__pyx_v_m, __pyx_v_c_metadata); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 45, __pyx_L1_error)
+#line 47 "palletjack/palletjack_cython.pyx"
+  __pyx_t_3 = __pyx_f_7pyarrow_8_parquet_12FileMetaData_init(__pyx_v_m, __pyx_v_c_metadata); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
 
-#line 45 "palletjack/palletjack_cython.pyx"
+#line 47 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_3);
 
-#line 45 "palletjack/palletjack_cython.pyx"
+#line 47 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "palletjack/palletjack_cython.pyx":46
+  /* "palletjack/palletjack_cython.pyx":48
  *     cdef FileMetaData m = FileMetaData.__new__(FileMetaData)
  *     m.init(c_metadata)
  *     return m             # <<<<<<<<<<<<<<
  */
 
-#line 46 "palletjack/palletjack_cython.pyx"
+#line 48 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_r);
 
-#line 46 "palletjack/palletjack_cython.pyx"
+#line 48 "palletjack/palletjack_cython.pyx"
   __Pyx_INCREF((PyObject *)__pyx_v_m);
 
-#line 46 "palletjack/palletjack_cython.pyx"
+#line 48 "palletjack/palletjack_cython.pyx"
   __pyx_r = ((PyObject *)__pyx_v_m);
 
-#line 46 "palletjack/palletjack_cython.pyx"
+#line 48 "palletjack/palletjack_cython.pyx"
   goto __pyx_L0;
 
-  /* "palletjack/palletjack_cython.pyx":28
+  /* "palletjack/palletjack_cython.pyx":29
  *     return None
  * 
  * cpdef read_metadata(index_file_path = None, row_groups = [], column_indices = [], column_names = [], index_data = None):             # <<<<<<<<<<<<<<
  * 
  *     cdef shared_ptr[CFileMetaData] c_metadata
  */
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   /* function exit code */
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L1_error:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_3);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_4);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_5);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __PYX_XCLEAR_MEMVIEW(&__pyx_t_8, 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_12);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_13);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_AddTraceback("palletjack.palletjack_cython.read_metadata", __pyx_clineno, __pyx_lineno, __pyx_filename);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_r = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L0:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_mv, 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF((PyObject *)__pyx_v_m);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_c);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XGIVEREF(__pyx_r);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_r;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 /* Python wrapper */
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pw_10palletjack_17palletjack_cython_3read_metadata(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 PyDoc_STRVAR(__pyx_doc_10palletjack_17palletjack_cython_2read_metadata, "read_metadata(index_file_path=None, row_groups=[], column_indices=[], column_names=[], index_data=None)");
 static PyMethodDef __pyx_mdef_10palletjack_17palletjack_cython_3read_metadata = 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 {"read_metadata", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10palletjack_17palletjack_cython_3read_metadata, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_10palletjack_17palletjack_cython_2read_metadata};
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pw_10palletjack_17palletjack_cython_3read_metadata(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_index_file_path = 0
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   PyObject *__pyx_v_row_groups = 0
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   PyObject *__pyx_v_column_indices = 0
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   PyObject *__pyx_v_column_names = 0
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
   PyObject *__pyx_v_index_data = 0
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 ;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_METH_FASTCALL
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject* values[5] = {0,0,0,0,0};
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_lineno = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   const char *__pyx_filename = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_clineno = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_r = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyDeclarations
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannySetupContext("read_metadata (wrapper)", 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_METH_FASTCALL
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_ASSUME_SAFE_MACROS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_index_file_path,&__pyx_n_s_row_groups,&__pyx_n_s_column_indices,&__pyx_n_s_column_names,&__pyx_n_s_index_data,0};
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     values[0] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     values[1] = __Pyx_Arg_NewRef_FASTCALL(__pyx_k__16);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     values[2] = __Pyx_Arg_NewRef_FASTCALL(__pyx_k__17);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     values[3] = __Pyx_Arg_NewRef_FASTCALL(__pyx_k__18);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (__pyx_kwds) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       Py_ssize_t kw_args;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       switch (__pyx_nargs) {
         case  5: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  4: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  3: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  2: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  1: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  0: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 break;
         default: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 goto __pyx_L5_argtuple_error;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       switch (__pyx_nargs) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         case  0:
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         if (kw_args > 0) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index_file_path);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           if (value) { values[0] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
 
-#line 28 "palletjack/palletjack_cython.pyx"
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 28, __pyx_L3_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 29, __pyx_L3_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         case  1:
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         if (kw_args > 0) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_row_groups);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
 
-#line 28 "palletjack/palletjack_cython.pyx"
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 28, __pyx_L3_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 29, __pyx_L3_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         case  2:
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         if (kw_args > 0) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_column_indices);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
 
-#line 28 "palletjack/palletjack_cython.pyx"
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 28, __pyx_L3_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 29, __pyx_L3_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         case  3:
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         if (kw_args > 0) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_column_names);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
 
-#line 28 "palletjack/palletjack_cython.pyx"
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 28, __pyx_L3_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 29, __pyx_L3_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         case  4:
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         if (kw_args > 0) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index_data);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
 
-#line 28 "palletjack/palletjack_cython.pyx"
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 28, __pyx_L3_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 29, __pyx_L3_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       if (unlikely(kw_args > 0)) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "read_metadata") < 0)) __PYX_ERR(1, 28, __pyx_L3_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "read_metadata") < 0)) __PYX_ERR(1, 29, __pyx_L3_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     } else {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       switch (__pyx_nargs) {
         case  5: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  4: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  3: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  2: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  1: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
         CYTHON_FALLTHROUGH;
         case  0: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 break;
         default: 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 goto __pyx_L5_argtuple_error;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_v_index_file_path = values[0];
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_v_row_groups = values[1];
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_v_column_indices = values[2];
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_v_column_names = values[3];
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_v_index_data = values[4];
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   goto __pyx_L6_skip;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L5_argtuple_error:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __Pyx_RaiseArgtupleInvalid("read_metadata", 0, 0, 5, __pyx_nargs); __PYX_ERR(1, 28, __pyx_L3_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __Pyx_RaiseArgtupleInvalid("read_metadata", 0, 0, 5, __pyx_nargs); __PYX_ERR(1, 29, __pyx_L3_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L6_skip:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   goto __pyx_L4_argument_unpacking_done;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L3_error:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     Py_ssize_t __pyx_temp;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_AddTraceback("palletjack.palletjack_cython.read_metadata", __pyx_clineno, __pyx_lineno, __pyx_filename);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 __pyx_pf_10palletjack_17palletjack_cython_2read_metadata(__pyx_self, __pyx_v_index_file_path, __pyx_v_row_groups, __pyx_v_column_indices, __pyx_v_column_names, __pyx_v_index_data);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   /* function exit code */
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     Py_ssize_t __pyx_temp;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_r;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_pf_10palletjack_17palletjack_cython_2read_metadata(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_index_file_path, PyObject *__pyx_v_row_groups, PyObject *__pyx_v_column_indices, PyObject *__pyx_v_column_names, PyObject *__pyx_v_index_data) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_r = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyDeclarations
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *__pyx_t_1 = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_opt_args_10palletjack_17palletjack_cython_read_metadata __pyx_t_2;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_lineno = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   const char *__pyx_filename = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int __pyx_clineno = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannySetupContext("read_metadata", 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_r);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.__pyx_n = 5;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.index_file_path = __pyx_v_index_file_path;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.row_groups = __pyx_v_row_groups;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.column_indices = __pyx_v_column_indices;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.column_names = __pyx_v_column_names;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_2.index_data = __pyx_v_index_data;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_1 = __pyx_f_10palletjack_17palletjack_cython_read_metadata(0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_1 = __pyx_f_10palletjack_17palletjack_cython_read_metadata(0, &__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_r = __pyx_t_1;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_1 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   goto __pyx_L0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   /* function exit code */
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L1_error:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XDECREF(__pyx_t_1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_AddTraceback("palletjack.palletjack_cython.read_metadata", __pyx_clineno, __pyx_lineno, __pyx_filename);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_r = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L0:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_XGIVEREF(__pyx_r);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_r;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_array_obj *p;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_LIMITED_API
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   o = alloc_func(t, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o = (*t->tp_alloc)(t, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   } else {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely(!o)) return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p = ((struct __pyx_array_obj *)o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->__pyx_vtab = __pyx_vtabptr_array;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->mode = ((PyObject*)Py_None); Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->_format = ((PyObject*)Py_None); Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely(__pyx_array___cinit__(o, a, k) < 0)) goto bad;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   bad:
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_DECREF(o); o = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static void __pyx_tp_dealloc_array(PyObject *o) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_array) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       if (PyObject_CallFinalizerFromDealloc(o)) return;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyObject *etype, *eval, *etb;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Fetch(&etype, &eval, &etb);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_array___dealloc__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Restore(etype, eval, etb);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->mode);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->_format);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   (*Py_TYPE(o)->tp_free)(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (tp_free) tp_free(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_sq_item_array(PyObject *o, Py_ssize_t i) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *r;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *x = PyInt_FromSsize_t(i); if(!x) return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   r = Py_TYPE(o)->tp_as_mapping->mp_subscript(o, x);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_DECREF(x);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return r;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_mp_ass_subscript_array(PyObject *o, PyObject *i, PyObject *v) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (v) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     return __pyx_array___setitem__(o, i, v);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   else {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_TypeName o_type_name;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o_type_name = __Pyx_PyType_GetName(Py_TYPE(o));
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Format(PyExc_NotImplementedError,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       "Subscript deletion not supported by " __Pyx_FMT_TYPENAME, o_type_name);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF_TypeName(o_type_name);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     return -1;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_tp_getattro_array(PyObject *o, PyObject *n) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *v = __Pyx_PyObject_GenericGetAttr(o, n);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (!v && PyErr_ExceptionMatches(PyExc_AttributeError)) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Clear();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     v = __pyx_array___getattr__(o, n);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return v;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_array_memview(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_5array_7memview_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyMethodDef __pyx_methods_array[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__getattr__", (PyCFunction)__pyx_array___getattr__, METH_O|METH_COEXIST, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_array_1__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_array_3__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0, 0, 0}
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static struct PyGetSetDef __pyx_getsets_array[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"memview", __pyx_getprop___pyx_array_memview, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0, 0, 0, 0}
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #if CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #if !CYTHON_COMPILING_IN_LIMITED_API
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyBufferProcs __pyx_tp_as_buffer_array = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getreadbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getwritebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getsegcount*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getcharbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_array_getbuffer, /*bf_getbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_releasebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Slot __pyx_type___pyx_array_slots[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_array},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_sq_length, (void *)__pyx_array___len__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_sq_item, (void *)__pyx_sq_item_array},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_mp_length, (void *)__pyx_array___len__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_mp_subscript, (void *)__pyx_array___getitem__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_mp_ass_subscript, (void *)__pyx_mp_ass_subscript_array},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_getattro, (void *)__pyx_tp_getattro_array},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if defined(Py_bf_getbuffer)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_bf_getbuffer, (void *)__pyx_array_getbuffer},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_methods, (void *)__pyx_methods_array},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_getset, (void *)__pyx_getsets_array},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_new, (void *)__pyx_tp_new_array},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Spec __pyx_type___pyx_array_spec = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython.array",
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_array_obj),
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_SEQUENCE,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_type___pyx_array_slots,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PySequenceMethods __pyx_tp_as_sequence_array = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_array___len__, /*sq_length*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_concat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_repeat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_sq_item_array, /*sq_item*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_slice*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_ass_item*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_ass_slice*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_contains*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_inplace_concat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_inplace_repeat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyMappingMethods __pyx_tp_as_mapping_array = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_array___len__, /*mp_length*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_array___getitem__, /*mp_subscript*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_mp_ass_subscript_array, /*mp_ass_subscript*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyBufferProcs __pyx_tp_as_buffer_array = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getreadbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getwritebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getsegcount*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getcharbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_array_getbuffer, /*bf_getbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_releasebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyTypeObject __pyx_type___pyx_array = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyVarObject_HEAD_INIT(0, 0)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython.""array", /*tp_name*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_array_obj), /*tp_basicsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_itemsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_dealloc_array, /*tp_dealloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX < 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall_offset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_compare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION >= 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_async*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_repr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_number*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   &__pyx_tp_as_sequence_array, /*tp_as_sequence*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   &__pyx_tp_as_mapping_array, /*tp_as_mapping*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_hash*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_call*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_str*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_getattro_array, /*tp_getattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   &__pyx_tp_as_buffer_array, /*tp_as_buffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_SEQUENCE, /*tp_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_doc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_traverse*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_clear*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_richcompare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklistoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iter*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iternext*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_methods_array, /*tp_methods*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_members*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_getsets_array, /*tp_getset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_base*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dict*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_get*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_set*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dictoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_init*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_alloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_new_array, /*tp_new*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_free*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_is_gc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_bases*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_mro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_cache*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_subclasses*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklist*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_del*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_version_tag*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030400a1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   NULL, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if __PYX_NEED_TP_PRINT_SLOT == 1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030C0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_watched*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_pypy_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_MemviewEnum_obj *p;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_LIMITED_API
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   o = alloc_func(t, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o = (*t->tp_alloc)(t, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   } else {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely(!o)) return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p = ((struct __pyx_MemviewEnum_obj *)o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->name = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_Enum) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       if (PyObject_CallFinalizerFromDealloc(o)) return;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject_GC_UnTrack(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->name);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   (*Py_TYPE(o)->tp_free)(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (tp_free) tp_free(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_tp_traverse_Enum(PyObject *o, visitproc v, void *a) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (p->name) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     e = (*v)(p->name, a); if (e) return e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_tp_clear_Enum(PyObject *o) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject* tmp;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   tmp = ((PyObject*)p->name);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->name = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_XDECREF(tmp);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_specialmethod___pyx_MemviewEnum___repr__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_MemviewEnum___repr__(self);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyMethodDef __pyx_methods_Enum[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__repr__", (PyCFunction)__pyx_specialmethod___pyx_MemviewEnum___repr__, METH_NOARGS|METH_COEXIST, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0, 0, 0}
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #if CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Slot __pyx_type___pyx_MemviewEnum_slots[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_Enum},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_repr, (void *)__pyx_MemviewEnum___repr__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_traverse, (void *)__pyx_tp_traverse_Enum},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_clear, (void *)__pyx_tp_clear_Enum},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_methods, (void *)__pyx_methods_Enum},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_init, (void *)__pyx_MemviewEnum___init__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_new, (void *)__pyx_tp_new_Enum},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Spec __pyx_type___pyx_MemviewEnum_spec = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython.Enum",
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_MemviewEnum_obj),
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_type___pyx_MemviewEnum_slots,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyTypeObject __pyx_type___pyx_MemviewEnum = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyVarObject_HEAD_INIT(0, 0)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython.""Enum", /*tp_name*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_MemviewEnum_obj), /*tp_basicsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_itemsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_dealloc_Enum, /*tp_dealloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX < 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall_offset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_compare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION >= 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_async*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_MemviewEnum___repr__, /*tp_repr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_number*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_sequence*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_mapping*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_hash*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_call*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_str*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_buffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_doc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_traverse_Enum, /*tp_traverse*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_clear_Enum, /*tp_clear*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_richcompare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklistoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iter*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iternext*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_methods_Enum, /*tp_methods*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_members*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_base*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dict*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_get*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_set*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dictoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_MemviewEnum___init__, /*tp_init*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_alloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_new_Enum, /*tp_new*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_free*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_is_gc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_bases*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_mro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_cache*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_subclasses*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklist*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_del*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_version_tag*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030400a1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   NULL, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if __PYX_NEED_TP_PRINT_SLOT == 1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030C0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_watched*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_pypy_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryview_obj *p;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_LIMITED_API
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   o = alloc_func(t, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o = (*t->tp_alloc)(t, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   } else {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely(!o)) return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p = ((struct __pyx_memoryview_obj *)o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->__pyx_vtab = __pyx_vtabptr_memoryview;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->obj = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->_size = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->_array_interface = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->view.obj = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely(__pyx_memoryview___cinit__(o, a, k) < 0)) goto bad;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   bad:
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_DECREF(o); o = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_memoryview) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       if (PyObject_CallFinalizerFromDealloc(o)) return;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject_GC_UnTrack(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyObject *etype, *eval, *etb;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Fetch(&etype, &eval, &etb);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_memoryview___dealloc__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Restore(etype, eval, etb);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->obj);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->_size);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->_array_interface);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   (*Py_TYPE(o)->tp_free)(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (tp_free) tp_free(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_tp_traverse_memoryview(PyObject *o, visitproc v, void *a) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (p->obj) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     e = (*v)(p->obj, a); if (e) return e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (p->_size) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     e = (*v)(p->_size, a); if (e) return e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (p->_array_interface) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     e = (*v)(p->_array_interface, a); if (e) return e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (p->view.obj) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     e = (*v)(p->view.obj, a); if (e) return e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_tp_clear_memoryview(PyObject *o) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject* tmp;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   tmp = ((PyObject*)p->obj);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->obj = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_XDECREF(tmp);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   tmp = ((PyObject*)p->_size);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->_size = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_XDECREF(tmp);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   tmp = ((PyObject*)p->_array_interface);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->_array_interface = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_XDECREF(tmp);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->view.obj);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_sq_item_memoryview(PyObject *o, Py_ssize_t i) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *r;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *x = PyInt_FromSsize_t(i); if(!x) return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   r = Py_TYPE(o)->tp_as_mapping->mp_subscript(o, x);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_DECREF(x);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return r;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_mp_ass_subscript_memoryview(PyObject *o, PyObject *i, PyObject *v) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (v) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     return __pyx_memoryview___setitem__(o, i, v);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   else {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_TypeName o_type_name;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     o_type_name = __Pyx_PyType_GetName(Py_TYPE(o));
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Format(PyExc_NotImplementedError,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       "Subscript deletion not supported by " __Pyx_FMT_TYPENAME, o_type_name);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_DECREF_TypeName(o_type_name);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     return -1;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_T(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_1T_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_base(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_4base_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_shape(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_5shape_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_strides(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_7strides_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_suboffsets(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_10suboffsets_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_ndim(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_4ndim_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_itemsize(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_8itemsize_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_nbytes(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_6nbytes_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_getprop___pyx_memoryview_size(PyObject *o, CYTHON_UNUSED void *x) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_pw_15View_dot_MemoryView_10memoryview_4size_1__get__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_specialmethod___pyx_memoryview___repr__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return __pyx_memoryview___repr__(self);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyMethodDef __pyx_methods_memoryview[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__repr__", (PyCFunction)__pyx_specialmethod___pyx_memoryview___repr__, METH_NOARGS|METH_COEXIST, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"is_c_contig", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_memoryview_is_c_contig, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"is_f_contig", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_memoryview_is_f_contig, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"copy", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_memoryview_copy, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"copy_fortran", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_memoryview_copy_fortran, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_memoryview_1__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_memoryview_3__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0, 0, 0}
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static struct PyGetSetDef __pyx_getsets_memoryview[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"T", __pyx_getprop___pyx_memoryview_T, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"base", __pyx_getprop___pyx_memoryview_base, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"shape", __pyx_getprop___pyx_memoryview_shape, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"strides", __pyx_getprop___pyx_memoryview_strides, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"suboffsets", __pyx_getprop___pyx_memoryview_suboffsets, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"ndim", __pyx_getprop___pyx_memoryview_ndim, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"itemsize", __pyx_getprop___pyx_memoryview_itemsize, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"nbytes", __pyx_getprop___pyx_memoryview_nbytes, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {(char *)"size", __pyx_getprop___pyx_memoryview_size, 0, (char *)0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0, 0, 0, 0}
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #if CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #if !CYTHON_COMPILING_IN_LIMITED_API
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyBufferProcs __pyx_tp_as_buffer_memoryview = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getreadbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getwritebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getsegcount*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getcharbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview_getbuffer, /*bf_getbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_releasebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Slot __pyx_type___pyx_memoryview_slots[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_repr, (void *)__pyx_memoryview___repr__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_sq_length, (void *)__pyx_memoryview___len__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_sq_item, (void *)__pyx_sq_item_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_mp_length, (void *)__pyx_memoryview___len__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_mp_subscript, (void *)__pyx_memoryview___getitem__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_mp_ass_subscript, (void *)__pyx_mp_ass_subscript_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_str, (void *)__pyx_memoryview___str__},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if defined(Py_bf_getbuffer)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_bf_getbuffer, (void *)__pyx_memoryview_getbuffer},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_traverse, (void *)__pyx_tp_traverse_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_clear, (void *)__pyx_tp_clear_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_methods, (void *)__pyx_methods_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_getset, (void *)__pyx_getsets_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_new, (void *)__pyx_tp_new_memoryview},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Spec __pyx_type___pyx_memoryview_spec = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython.memoryview",
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_memoryview_obj),
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_type___pyx_memoryview_slots,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PySequenceMethods __pyx_tp_as_sequence_memoryview = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview___len__, /*sq_length*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_concat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_repeat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_sq_item_memoryview, /*sq_item*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_slice*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_ass_item*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_ass_slice*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_contains*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_inplace_concat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*sq_inplace_repeat*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyMappingMethods __pyx_tp_as_mapping_memoryview = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview___len__, /*mp_length*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview___getitem__, /*mp_subscript*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_mp_ass_subscript_memoryview, /*mp_ass_subscript*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyBufferProcs __pyx_tp_as_buffer_memoryview = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getreadbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getwritebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getsegcount*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_getcharbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview_getbuffer, /*bf_getbuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*bf_releasebuffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyTypeObject __pyx_type___pyx_memoryview = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyVarObject_HEAD_INIT(0, 0)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython.""memoryview", /*tp_name*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_memoryview_obj), /*tp_basicsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_itemsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_dealloc_memoryview, /*tp_dealloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX < 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall_offset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_compare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION >= 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_async*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview___repr__, /*tp_repr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_number*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   &__pyx_tp_as_sequence_memoryview, /*tp_as_sequence*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   &__pyx_tp_as_mapping_memoryview, /*tp_as_mapping*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_hash*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_call*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview___str__, /*tp_str*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   &__pyx_tp_as_buffer_memoryview, /*tp_as_buffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_doc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_traverse_memoryview, /*tp_traverse*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_clear_memoryview, /*tp_clear*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_richcompare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklistoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iter*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iternext*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_methods_memoryview, /*tp_methods*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_members*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_getsets_memoryview, /*tp_getset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_base*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dict*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_get*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_set*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dictoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_init*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_alloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_new_memoryview, /*tp_new*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_free*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_is_gc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_bases*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_mro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_cache*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_subclasses*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklist*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_del*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_version_tag*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030400a1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   NULL, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if __PYX_NEED_TP_PRINT_SLOT == 1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030C0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_watched*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_pypy_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryviewslice_obj *p;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject *o = __pyx_tp_new_memoryview(t, a, k);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely(!o)) return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p = ((struct __pyx_memoryviewslice_obj *)o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->__pyx_base.__pyx_vtab = (struct __pyx_vtabstruct_memoryview*)__pyx_vtabptr__memoryviewslice;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   new((void*)&(p->from_slice)) __Pyx_memviewslice();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->from_object = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->from_slice.memview = NULL;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc__memoryviewslice) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
       if (PyObject_CallFinalizerFromDealloc(o)) return;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject_GC_UnTrack(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyObject *etype, *eval, *etb;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Fetch(&etype, &eval, &etb);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __pyx_memoryviewslice___dealloc__(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     PyErr_Restore(etype, eval, etb);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_call_destructor(p->from_slice);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_CLEAR(p->from_object);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject_GC_Track(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_dealloc_memoryview(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_tp_traverse__memoryviewslice(PyObject *o, visitproc v, void *a) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   int e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   e = __pyx_tp_traverse_memoryview(o, v, a); if (e) return e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   if (p->from_object) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
     e = (*v)(p->from_object, a); if (e) return e;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static int __pyx_tp_clear__memoryviewslice(PyObject *o) {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyObject* tmp;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_clear_memoryview(o);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   tmp = ((PyObject*)p->from_object);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   p->from_object = Py_None; Py_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_XDECREF(tmp);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __PYX_XCLEAR_MEMVIEW(&p->from_slice, 1);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyMethodDef __pyx_methods__memoryviewslice[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_memoryviewslice_1__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw___pyx_memoryviewslice_3__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0, 0, 0}
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #if CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Slot __pyx_type___pyx_memoryviewslice_slots[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc__memoryviewslice},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_doc, (void *)PyDoc_STR("Internal class for passing memoryview slices to Python")},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_traverse, (void *)__pyx_tp_traverse__memoryviewslice},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_clear, (void *)__pyx_tp_clear__memoryviewslice},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_methods, (void *)__pyx_methods__memoryviewslice},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {Py_tp_new, (void *)__pyx_tp_new__memoryviewslice},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0},
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyType_Spec __pyx_type___pyx_memoryviewslice_spec = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython._memoryviewslice",
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_memoryviewslice_obj),
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_SEQUENCE,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_type___pyx_memoryviewslice_slots,
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyTypeObject __pyx_type___pyx_memoryviewslice = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyVarObject_HEAD_INIT(0, 0)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   "palletjack.palletjack_cython.""_memoryviewslice", /*tp_name*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   sizeof(struct __pyx_memoryviewslice_obj), /*tp_basicsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_itemsize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_dealloc__memoryviewslice, /*tp_dealloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX < 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b4
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall_offset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION < 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_compare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_MAJOR_VERSION >= 3
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_async*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_PYPY || 0
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview___repr__, /*tp_repr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_repr*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_number*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_sequence*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_mapping*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_hash*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_call*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_PYPY || 0
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_memoryview___str__, /*tp_str*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_str*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_setattro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_as_buffer*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_SEQUENCE, /*tp_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   PyDoc_STR("Internal class for passing memoryview slices to Python"), /*tp_doc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_traverse__memoryviewslice, /*tp_traverse*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_clear__memoryviewslice, /*tp_clear*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_richcompare*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklistoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iter*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_iternext*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_methods__memoryviewslice, /*tp_methods*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_members*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_getset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_base*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dict*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_get*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_descr_set*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if !CYTHON_USE_TYPE_SPECS
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_dictoffset*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_init*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_alloc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_tp_new__memoryviewslice, /*tp_new*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_free*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_is_gc*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_bases*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_mro*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_cache*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_subclasses*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_weaklist*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_del*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_version_tag*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030400a1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_USE_TP_FINALIZE
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #else
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   NULL, /*tp_finalize*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_vectorcall*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if __PYX_NEED_TP_PRINT_SLOT == 1
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_print*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if PY_VERSION_HEX >= 0x030C0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_watched*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   0, /*tp_pypy_flags*/
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #endif
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 static PyMethodDef __pyx_methods[] = {
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   {0, 0, 0, 0}
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 };
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
@@ -48327,96 +48346,96 @@
 
 #line 1 "(tree fragment)"
   __Pyx_GIVEREF(__pyx_tuple__28);
 
 #line 1 "(tree fragment)"
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 1, __pyx_L1_error)
 
-  /* "palletjack/palletjack_cython.pyx":4
- * 
+  /* "palletjack/palletjack_cython.pyx":5
+ * import cython
  * import pyarrow as pa
  * import pyarrow.parquet as pq             # <<<<<<<<<<<<<<
  * from cython.cimports.palletjack import cpalletjack
  * from libcpp.string cimport string
  */
 
-#line 4 "palletjack/palletjack_cython.pyx"
-  __pyx_tuple__30 = PyTuple_Pack(2, __pyx_n_s_pyarrow, __pyx_n_s_parquet); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 4, __pyx_L1_error)
+#line 5 "palletjack/palletjack_cython.pyx"
+  __pyx_tuple__30 = PyTuple_Pack(2, __pyx_n_s_pyarrow, __pyx_n_s_parquet); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 5, __pyx_L1_error)
 
-#line 4 "palletjack/palletjack_cython.pyx"
+#line 5 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_tuple__30);
 
-#line 4 "palletjack/palletjack_cython.pyx"
+#line 5 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_tuple__30);
 
-  /* "palletjack/palletjack_cython.pyx":12
+  /* "palletjack/palletjack_cython.pyx":13
  * from pyarrow._parquet cimport *
  * 
  * cpdef generate_metadata_index(parquet_path, index_file_path = None):             # <<<<<<<<<<<<<<
  *     cdef string encoded_parquet_path = parquet_path.encode('utf8')
  *     cdef string encoded_index_file_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  */
 
-#line 12 "palletjack/palletjack_cython.pyx"
-  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_s_parquet_path, __pyx_n_s_index_file_path); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 12, __pyx_L1_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+  __pyx_tuple__31 = PyTuple_Pack(2, __pyx_n_s_parquet_path, __pyx_n_s_index_file_path); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 13, __pyx_L1_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_tuple__31);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_tuple__31);
 
-#line 12 "palletjack/palletjack_cython.pyx"
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_palletjack_palletjack_cython_pyx, __pyx_n_s_generate_metadata_index, 12, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 12, __pyx_L1_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_palletjack_palletjack_cython_pyx, __pyx_n_s_generate_metadata_index, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 13, __pyx_L1_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
-  __pyx_tuple__33 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 12, __pyx_L1_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+  __pyx_tuple__33 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 13, __pyx_L1_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_tuple__33);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_tuple__33);
 
-  /* "palletjack/palletjack_cython.pyx":28
+  /* "palletjack/palletjack_cython.pyx":29
  *     return None
  * 
  * cpdef read_metadata(index_file_path = None, row_groups = [], column_indices = [], column_names = [], index_data = None):             # <<<<<<<<<<<<<<
  * 
  *     cdef shared_ptr[CFileMetaData] c_metadata
  */
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_tuple__34 = PyTuple_Pack(5, __pyx_n_s_index_file_path, __pyx_n_s_row_groups, __pyx_n_s_column_indices, __pyx_n_s_column_names, __pyx_n_s_index_data); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_tuple__34 = PyTuple_Pack(5, __pyx_n_s_index_file_path, __pyx_n_s_row_groups, __pyx_n_s_column_indices, __pyx_n_s_column_names, __pyx_n_s_index_data); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_tuple__34);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_tuple__34);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_palletjack_palletjack_cython_pyx, __pyx_n_s_read_metadata, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_palletjack_palletjack_cython_pyx, __pyx_n_s_read_metadata, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_L1_error:;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_RefNannyFinishContext();
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   return -1;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -48643,214 +48662,214 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("datetime"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_3_0_9(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 70, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_3_0_9(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 83, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_3_0_9(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 109, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_3_0_9(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 147, __pyx_L1_error)
-  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_3_0_9(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 160, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_date = __Pyx_ImportType_3_0_10(__pyx_t_1, "datetime", "date", sizeof(PyDateTime_Date), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyDateTime_Date),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_8datetime_date) __PYX_ERR(3, 70, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_time = __Pyx_ImportType_3_0_10(__pyx_t_1, "datetime", "time", sizeof(PyDateTime_Time), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyDateTime_Time),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_8datetime_time) __PYX_ERR(3, 83, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_datetime = __Pyx_ImportType_3_0_10(__pyx_t_1, "datetime", "datetime", sizeof(PyDateTime_DateTime), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyDateTime_DateTime),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_8datetime_datetime) __PYX_ERR(3, 109, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_timedelta = __Pyx_ImportType_3_0_10(__pyx_t_1, "datetime", "timedelta", sizeof(PyDateTime_Delta), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyDateTime_Delta),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_8datetime_timedelta) __PYX_ERR(3, 147, __pyx_L1_error)
+  __pyx_ptype_7cpython_8datetime_tzinfo = __Pyx_ImportType_3_0_10(__pyx_t_1, "datetime", "tzinfo", sizeof(PyDateTime_TZInfo), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyDateTime_TZInfo),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_8datetime_tzinfo) __PYX_ERR(3, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("pyarrow.lib"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7pyarrow_3lib__Weakrefable = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "_Weakrefable", sizeof(struct __pyx_obj_7pyarrow_3lib__Weakrefable), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib__Weakrefable),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib__Weakrefable) __PYX_ERR(8, 71, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_IpcWriteOptions = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "IpcWriteOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_IpcWriteOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_IpcWriteOptions),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_IpcWriteOptions) __PYX_ERR(8, 75, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_IpcReadOptions = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "IpcReadOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_IpcReadOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_IpcReadOptions),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_IpcReadOptions) __PYX_ERR(8, 80, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Message = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Message", sizeof(struct __pyx_obj_7pyarrow_3lib_Message), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Message),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Message) __PYX_ERR(8, 85, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_MemoryPool = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "MemoryPool", sizeof(struct __pyx_obj_7pyarrow_3lib_MemoryPool), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_MemoryPool),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_MemoryPool) __PYX_ERR(8, 90, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__Weakrefable = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_Weakrefable", sizeof(struct __pyx_obj_7pyarrow_3lib__Weakrefable), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__Weakrefable),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__Weakrefable) __PYX_ERR(8, 71, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_IpcWriteOptions = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "IpcWriteOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_IpcWriteOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_IpcWriteOptions),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_IpcWriteOptions) __PYX_ERR(8, 75, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_IpcReadOptions = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "IpcReadOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_IpcReadOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_IpcReadOptions),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_IpcReadOptions) __PYX_ERR(8, 80, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Message = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Message", sizeof(struct __pyx_obj_7pyarrow_3lib_Message), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Message),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Message) __PYX_ERR(8, 85, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_MemoryPool = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MemoryPool", sizeof(struct __pyx_obj_7pyarrow_3lib_MemoryPool), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MemoryPool),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MemoryPool) __PYX_ERR(8, 90, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_MemoryPool = (struct __pyx_vtabstruct_7pyarrow_3lib_MemoryPool*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MemoryPool); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MemoryPool)) __PYX_ERR(8, 90, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DataType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "DataType", sizeof(struct __pyx_obj_7pyarrow_3lib_DataType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_DataType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_DataType) __PYX_ERR(8, 103, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DataType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DataType", sizeof(struct __pyx_obj_7pyarrow_3lib_DataType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DataType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DataType) __PYX_ERR(8, 103, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_DataType = (struct __pyx_vtabstruct_7pyarrow_3lib_DataType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DataType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DataType)) __PYX_ERR(8, 103, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ListType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "ListType", sizeof(struct __pyx_obj_7pyarrow_3lib_ListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_ListType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_ListType) __PYX_ERR(8, 113, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ListType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ListType", sizeof(struct __pyx_obj_7pyarrow_3lib_ListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ListType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ListType) __PYX_ERR(8, 113, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_ListType = (struct __pyx_vtabstruct_7pyarrow_3lib_ListType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ListType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ListType)) __PYX_ERR(8, 113, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_LargeListType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "LargeListType", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_LargeListType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_LargeListType) __PYX_ERR(8, 118, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_LargeListType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "LargeListType", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_LargeListType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_LargeListType) __PYX_ERR(8, 118, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_LargeListType = (struct __pyx_vtabstruct_7pyarrow_3lib_LargeListType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_LargeListType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_LargeListType)) __PYX_ERR(8, 118, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_MapType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "MapType", sizeof(struct __pyx_obj_7pyarrow_3lib_MapType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_MapType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_MapType) __PYX_ERR(8, 123, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_MapType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MapType", sizeof(struct __pyx_obj_7pyarrow_3lib_MapType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MapType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MapType) __PYX_ERR(8, 123, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_MapType = (struct __pyx_vtabstruct_7pyarrow_3lib_MapType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MapType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MapType)) __PYX_ERR(8, 123, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeListType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "FixedSizeListType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListType) __PYX_ERR(8, 128, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeListType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeListType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListType) __PYX_ERR(8, 128, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_FixedSizeListType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeListType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeListType)) __PYX_ERR(8, 128, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StructType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "StructType", sizeof(struct __pyx_obj_7pyarrow_3lib_StructType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_StructType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_StructType) __PYX_ERR(8, 133, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StructType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StructType", sizeof(struct __pyx_obj_7pyarrow_3lib_StructType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StructType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StructType) __PYX_ERR(8, 133, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_StructType = (struct __pyx_vtabstruct_7pyarrow_3lib_StructType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StructType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StructType)) __PYX_ERR(8, 133, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DictionaryMemo = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "DictionaryMemo", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_DictionaryMemo) __PYX_ERR(8, 140, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DictionaryType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "DictionaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_DictionaryType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_DictionaryType) __PYX_ERR(8, 148, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DictionaryMemo = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryMemo", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryMemo) __PYX_ERR(8, 140, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DictionaryType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryType) __PYX_ERR(8, 148, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_DictionaryType = (struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DictionaryType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DictionaryType)) __PYX_ERR(8, 148, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_TimestampType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "TimestampType", sizeof(struct __pyx_obj_7pyarrow_3lib_TimestampType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_TimestampType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_TimestampType) __PYX_ERR(8, 153, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_TimestampType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "TimestampType", sizeof(struct __pyx_obj_7pyarrow_3lib_TimestampType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_TimestampType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_TimestampType) __PYX_ERR(8, 153, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_TimestampType = (struct __pyx_vtabstruct_7pyarrow_3lib_TimestampType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_TimestampType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_TimestampType)) __PYX_ERR(8, 153, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Time32Type = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Time32Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time32Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Time32Type),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Time32Type) __PYX_ERR(8, 158, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Time32Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Time32Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time32Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Time32Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Time32Type) __PYX_ERR(8, 158, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Time32Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Time32Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Time32Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Time32Type)) __PYX_ERR(8, 158, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Time64Type = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Time64Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time64Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Time64Type),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Time64Type) __PYX_ERR(8, 163, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Time64Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Time64Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time64Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Time64Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Time64Type) __PYX_ERR(8, 163, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Time64Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Time64Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Time64Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Time64Type)) __PYX_ERR(8, 163, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DurationType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "DurationType", sizeof(struct __pyx_obj_7pyarrow_3lib_DurationType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_DurationType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_DurationType) __PYX_ERR(8, 168, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DurationType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DurationType", sizeof(struct __pyx_obj_7pyarrow_3lib_DurationType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DurationType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DurationType) __PYX_ERR(8, 168, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_DurationType = (struct __pyx_vtabstruct_7pyarrow_3lib_DurationType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DurationType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DurationType)) __PYX_ERR(8, 168, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType) __PYX_ERR(8, 173, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType) __PYX_ERR(8, 173, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType)) __PYX_ERR(8, 173, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal128Type = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Decimal128Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Decimal128Type),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Type) __PYX_ERR(8, 178, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal128Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal128Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal128Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Type) __PYX_ERR(8, 178, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Decimal128Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal128Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal128Type)) __PYX_ERR(8, 178, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal256Type = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Decimal256Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Decimal256Type),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Type) __PYX_ERR(8, 183, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal256Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal256Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal256Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Type) __PYX_ERR(8, 183, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Decimal256Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal256Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal256Type)) __PYX_ERR(8, 183, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_RunEndEncodedType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "RunEndEncodedType", sizeof(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_RunEndEncodedType) __PYX_ERR(8, 188, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_RunEndEncodedType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RunEndEncodedType", sizeof(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RunEndEncodedType) __PYX_ERR(8, 188, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType = (struct __pyx_vtabstruct_7pyarrow_3lib_RunEndEncodedType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_RunEndEncodedType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType)) __PYX_ERR(8, 188, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BaseExtensionType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "BaseExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_BaseExtensionType) __PYX_ERR(8, 193, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BaseExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BaseExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BaseExtensionType) __PYX_ERR(8, 193, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_BaseExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BaseExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BaseExtensionType)) __PYX_ERR(8, 193, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ExtensionType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "ExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_ExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_ExtensionType) __PYX_ERR(8, 198, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ExtensionType) __PYX_ERR(8, 198, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_ExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ExtensionType)) __PYX_ERR(8, 198, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedShapeTensorType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "FixedShapeTensorType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_FixedShapeTensorType) __PYX_ERR(8, 203, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedShapeTensorType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedShapeTensorType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedShapeTensorType) __PYX_ERR(8, 203, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedShapeTensorType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedShapeTensorType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType)) __PYX_ERR(8, 203, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_PyExtensionType = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "PyExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_PyExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_PyExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_PyExtensionType) __PYX_ERR(8, 208, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_PyExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "PyExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_PyExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_PyExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_PyExtensionType) __PYX_ERR(8, 208, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_PyExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_PyExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_PyExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_PyExtensionType)) __PYX_ERR(8, 208, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__Metadata = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "_Metadata", sizeof(struct __pyx_obj_7pyarrow_3lib__Metadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib__Metadata),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib__Metadata) __PYX_ERR(8, 212, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_KeyValueMetadata = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "KeyValueMetadata", sizeof(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_KeyValueMetadata) __PYX_ERR(8, 218, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__Metadata = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_Metadata", sizeof(struct __pyx_obj_7pyarrow_3lib__Metadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__Metadata),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__Metadata) __PYX_ERR(8, 212, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_KeyValueMetadata = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "KeyValueMetadata", sizeof(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_KeyValueMetadata) __PYX_ERR(8, 218, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_KeyValueMetadata = (struct __pyx_vtabstruct_7pyarrow_3lib_KeyValueMetadata*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_KeyValueMetadata); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_KeyValueMetadata)) __PYX_ERR(8, 218, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Field = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Field", sizeof(struct __pyx_obj_7pyarrow_3lib_Field), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Field),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Field) __PYX_ERR(8, 230, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Field = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Field", sizeof(struct __pyx_obj_7pyarrow_3lib_Field), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Field),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Field) __PYX_ERR(8, 230, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Field = (struct __pyx_vtabstruct_7pyarrow_3lib_Field*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Field); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Field)) __PYX_ERR(8, 230, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Schema = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Schema", sizeof(struct __pyx_obj_7pyarrow_3lib_Schema), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Schema),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Schema) __PYX_ERR(8, 241, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Schema = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Schema", sizeof(struct __pyx_obj_7pyarrow_3lib_Schema), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Schema),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Schema) __PYX_ERR(8, 241, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Schema = (struct __pyx_vtabstruct_7pyarrow_3lib_Schema*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Schema); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Schema)) __PYX_ERR(8, 241, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Scalar = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Scalar", sizeof(struct __pyx_obj_7pyarrow_3lib_Scalar), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Scalar),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Scalar) __PYX_ERR(8, 250, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Scalar = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Scalar", sizeof(struct __pyx_obj_7pyarrow_3lib_Scalar), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Scalar),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Scalar) __PYX_ERR(8, 250, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Scalar = (struct __pyx_vtabstruct_7pyarrow_3lib_Scalar*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Scalar); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Scalar)) __PYX_ERR(8, 250, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__PandasConvertible = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "_PandasConvertible", sizeof(struct __pyx_obj_7pyarrow_3lib__PandasConvertible), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib__PandasConvertible),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib__PandasConvertible) __PYX_ERR(8, 262, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Array) __PYX_ERR(8, 266, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__PandasConvertible = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_PandasConvertible", sizeof(struct __pyx_obj_7pyarrow_3lib__PandasConvertible), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__PandasConvertible),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__PandasConvertible) __PYX_ERR(8, 262, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Array) __PYX_ERR(8, 266, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Array)) __PYX_ERR(8, 266, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Tensor = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Tensor", sizeof(struct __pyx_obj_7pyarrow_3lib_Tensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Tensor),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Tensor) __PYX_ERR(8, 281, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Tensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Tensor", sizeof(struct __pyx_obj_7pyarrow_3lib_Tensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Tensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Tensor) __PYX_ERR(8, 281, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Tensor = (struct __pyx_vtabstruct_7pyarrow_3lib_Tensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Tensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Tensor)) __PYX_ERR(8, 281, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCSRMatrix = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "SparseCSRMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_SparseCSRMatrix) __PYX_ERR(8, 292, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCSRMatrix = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSRMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSRMatrix) __PYX_ERR(8, 292, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_SparseCSRMatrix = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSRMatrix*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSRMatrix); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSRMatrix)) __PYX_ERR(8, 292, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCSCMatrix = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "SparseCSCMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_SparseCSCMatrix) __PYX_ERR(8, 303, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCSCMatrix = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSCMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSCMatrix) __PYX_ERR(8, 303, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_SparseCSCMatrix = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSCMatrix*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSCMatrix); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSCMatrix)) __PYX_ERR(8, 303, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCOOTensor = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "SparseCOOTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_SparseCOOTensor) __PYX_ERR(8, 314, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCOOTensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCOOTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCOOTensor) __PYX_ERR(8, 314, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_SparseCOOTensor = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCOOTensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCOOTensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCOOTensor)) __PYX_ERR(8, 314, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCSFTensor = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "SparseCSFTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_SparseCSFTensor) __PYX_ERR(8, 325, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCSFTensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSFTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSFTensor) __PYX_ERR(8, 325, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_SparseCSFTensor = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSFTensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSFTensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSFTensor)) __PYX_ERR(8, 325, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_NullArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "NullArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NullArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_NullArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_NullArray) __PYX_ERR(8, 336, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_NullArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NullArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NullArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NullArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NullArray) __PYX_ERR(8, 336, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_NullArray = (struct __pyx_vtabstruct_7pyarrow_3lib_NullArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NullArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NullArray)) __PYX_ERR(8, 336, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BooleanArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "BooleanArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BooleanArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_BooleanArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_BooleanArray) __PYX_ERR(8, 340, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BooleanArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BooleanArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BooleanArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BooleanArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BooleanArray) __PYX_ERR(8, 340, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_BooleanArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BooleanArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BooleanArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BooleanArray)) __PYX_ERR(8, 340, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_NumericArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "NumericArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NumericArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_NumericArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_NumericArray) __PYX_ERR(8, 344, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_NumericArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NumericArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NumericArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NumericArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NumericArray) __PYX_ERR(8, 344, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_NumericArray = (struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NumericArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NumericArray)) __PYX_ERR(8, 344, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_IntegerArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "IntegerArray", sizeof(struct __pyx_obj_7pyarrow_3lib_IntegerArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_IntegerArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_IntegerArray) __PYX_ERR(8, 348, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_IntegerArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "IntegerArray", sizeof(struct __pyx_obj_7pyarrow_3lib_IntegerArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_IntegerArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_IntegerArray) __PYX_ERR(8, 348, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_IntegerArray = (struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_IntegerArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_IntegerArray)) __PYX_ERR(8, 348, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FloatingPointArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "FloatingPointArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_FloatingPointArray) __PYX_ERR(8, 352, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FloatingPointArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FloatingPointArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FloatingPointArray) __PYX_ERR(8, 352, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_FloatingPointArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FloatingPointArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FloatingPointArray)) __PYX_ERR(8, 352, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int8Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Int8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Int8Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Int8Array) __PYX_ERR(8, 356, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int8Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int8Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int8Array) __PYX_ERR(8, 356, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Int8Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int8Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int8Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int8Array)) __PYX_ERR(8, 356, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt8Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "UInt8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_UInt8Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_UInt8Array) __PYX_ERR(8, 360, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt8Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt8Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt8Array) __PYX_ERR(8, 360, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_UInt8Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt8Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt8Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt8Array)) __PYX_ERR(8, 360, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int16Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Int16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Int16Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Int16Array) __PYX_ERR(8, 364, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int16Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int16Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int16Array) __PYX_ERR(8, 364, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Int16Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int16Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int16Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int16Array)) __PYX_ERR(8, 364, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt16Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "UInt16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_UInt16Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_UInt16Array) __PYX_ERR(8, 368, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt16Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt16Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt16Array) __PYX_ERR(8, 368, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_UInt16Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt16Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt16Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt16Array)) __PYX_ERR(8, 368, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int32Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Int32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Int32Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Int32Array) __PYX_ERR(8, 372, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int32Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int32Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int32Array) __PYX_ERR(8, 372, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Int32Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int32Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int32Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int32Array)) __PYX_ERR(8, 372, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt32Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "UInt32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_UInt32Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_UInt32Array) __PYX_ERR(8, 376, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt32Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt32Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt32Array) __PYX_ERR(8, 376, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_UInt32Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt32Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt32Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt32Array)) __PYX_ERR(8, 376, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int64Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Int64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Int64Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Int64Array) __PYX_ERR(8, 380, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int64Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int64Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int64Array) __PYX_ERR(8, 380, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Int64Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int64Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int64Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int64Array)) __PYX_ERR(8, 380, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt64Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "UInt64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_UInt64Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_UInt64Array) __PYX_ERR(8, 384, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt64Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt64Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt64Array) __PYX_ERR(8, 384, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_UInt64Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt64Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt64Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt64Array)) __PYX_ERR(8, 384, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_HalfFloatArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "HalfFloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_HalfFloatArray) __PYX_ERR(8, 388, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_HalfFloatArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "HalfFloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_HalfFloatArray) __PYX_ERR(8, 388, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_HalfFloatArray = (struct __pyx_vtabstruct_7pyarrow_3lib_HalfFloatArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_HalfFloatArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_HalfFloatArray)) __PYX_ERR(8, 388, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FloatArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "FloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_FloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_FloatArray) __PYX_ERR(8, 392, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FloatArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FloatArray) __PYX_ERR(8, 392, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_FloatArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FloatArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FloatArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FloatArray)) __PYX_ERR(8, 392, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DoubleArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "DoubleArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DoubleArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_DoubleArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_DoubleArray) __PYX_ERR(8, 396, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DoubleArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DoubleArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DoubleArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DoubleArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DoubleArray) __PYX_ERR(8, 396, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_DoubleArray = (struct __pyx_vtabstruct_7pyarrow_3lib_DoubleArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DoubleArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DoubleArray)) __PYX_ERR(8, 396, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray) __PYX_ERR(8, 400, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray) __PYX_ERR(8, 400, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray)) __PYX_ERR(8, 400, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal128Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Decimal128Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Decimal128Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Array) __PYX_ERR(8, 404, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal128Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal128Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal128Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Array) __PYX_ERR(8, 404, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Decimal128Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal128Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal128Array)) __PYX_ERR(8, 404, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal256Array = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Decimal256Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Decimal256Array),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Array) __PYX_ERR(8, 408, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal256Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal256Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal256Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Array) __PYX_ERR(8, 408, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Decimal256Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal256Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal256Array)) __PYX_ERR(8, 408, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StructArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "StructArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StructArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_StructArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_StructArray) __PYX_ERR(8, 412, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StructArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StructArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StructArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StructArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StructArray) __PYX_ERR(8, 412, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_StructArray = (struct __pyx_vtabstruct_7pyarrow_3lib_StructArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StructArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StructArray)) __PYX_ERR(8, 412, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BaseListArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "BaseListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_BaseListArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_BaseListArray) __PYX_ERR(8, 416, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BaseListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BaseListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BaseListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BaseListArray) __PYX_ERR(8, 416, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_BaseListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BaseListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BaseListArray)) __PYX_ERR(8, 416, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ListArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "ListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_ListArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_ListArray) __PYX_ERR(8, 420, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ListArray) __PYX_ERR(8, 420, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_ListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ListArray)) __PYX_ERR(8, 420, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_LargeListArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "LargeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_LargeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_LargeListArray) __PYX_ERR(8, 424, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_LargeListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "LargeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_LargeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_LargeListArray) __PYX_ERR(8, 424, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_LargeListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_LargeListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_LargeListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_LargeListArray)) __PYX_ERR(8, 424, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_MapArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "MapArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MapArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_MapArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_MapArray) __PYX_ERR(8, 428, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_MapArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MapArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MapArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MapArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MapArray) __PYX_ERR(8, 428, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_MapArray = (struct __pyx_vtabstruct_7pyarrow_3lib_MapArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MapArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MapArray)) __PYX_ERR(8, 428, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeListArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "FixedSizeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListArray) __PYX_ERR(8, 432, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListArray) __PYX_ERR(8, 432, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray)) __PYX_ERR(8, 432, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UnionArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "UnionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_UnionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_UnionArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_UnionArray) __PYX_ERR(8, 436, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UnionArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UnionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_UnionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UnionArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UnionArray) __PYX_ERR(8, 436, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_UnionArray = (struct __pyx_vtabstruct_7pyarrow_3lib_UnionArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UnionArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UnionArray)) __PYX_ERR(8, 436, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StringArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "StringArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StringArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_StringArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_StringArray) __PYX_ERR(8, 440, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StringArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StringArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StringArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StringArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StringArray) __PYX_ERR(8, 440, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_StringArray = (struct __pyx_vtabstruct_7pyarrow_3lib_StringArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StringArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StringArray)) __PYX_ERR(8, 440, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BinaryArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "BinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_BinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_BinaryArray) __PYX_ERR(8, 444, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BinaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BinaryArray) __PYX_ERR(8, 444, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_BinaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BinaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BinaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BinaryArray)) __PYX_ERR(8, 444, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DictionaryArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "DictionaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_DictionaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_DictionaryArray) __PYX_ERR(8, 448, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DictionaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryArray) __PYX_ERR(8, 448, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_DictionaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DictionaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DictionaryArray)) __PYX_ERR(8, 448, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ExtensionArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "ExtensionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_ExtensionArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_ExtensionArray) __PYX_ERR(8, 453, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ExtensionArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ExtensionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ExtensionArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ExtensionArray) __PYX_ERR(8, 453, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_ExtensionArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ExtensionArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ExtensionArray)) __PYX_ERR(8, 453, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "MonthDayNanoIntervalArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray) __PYX_ERR(8, 457, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MonthDayNanoIntervalArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray) __PYX_ERR(8, 457, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_MonthDayNanoIntervalArray = (struct __pyx_vtabstruct_7pyarrow_3lib_MonthDayNanoIntervalArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MonthDayNanoIntervalArray)) __PYX_ERR(8, 457, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ChunkedArray = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "ChunkedArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ChunkedArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_ChunkedArray),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_ChunkedArray) __PYX_ERR(8, 465, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ChunkedArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ChunkedArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ChunkedArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ChunkedArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ChunkedArray) __PYX_ERR(8, 465, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_ChunkedArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ChunkedArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ChunkedArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ChunkedArray)) __PYX_ERR(8, 465, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__Tabular = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "_Tabular", sizeof(struct __pyx_obj_7pyarrow_3lib__Tabular), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib__Tabular),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib__Tabular) __PYX_ERR(8, 478, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Table = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Table", sizeof(struct __pyx_obj_7pyarrow_3lib_Table), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Table),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Table) __PYX_ERR(8, 482, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__Tabular = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_Tabular", sizeof(struct __pyx_obj_7pyarrow_3lib__Tabular), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__Tabular),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__Tabular) __PYX_ERR(8, 478, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Table = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Table", sizeof(struct __pyx_obj_7pyarrow_3lib_Table), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Table),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Table) __PYX_ERR(8, 482, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Table = (struct __pyx_vtabstruct_7pyarrow_3lib_Table*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Table); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Table)) __PYX_ERR(8, 482, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_RecordBatch = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "RecordBatch", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatch), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_RecordBatch),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_RecordBatch) __PYX_ERR(8, 490, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_RecordBatch = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RecordBatch", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatch), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RecordBatch),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RecordBatch) __PYX_ERR(8, 490, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_RecordBatch = (struct __pyx_vtabstruct_7pyarrow_3lib_RecordBatch*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_RecordBatch); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_RecordBatch)) __PYX_ERR(8, 490, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Buffer = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Buffer", sizeof(struct __pyx_obj_7pyarrow_3lib_Buffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Buffer),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Buffer) __PYX_ERR(8, 499, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Buffer = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Buffer", sizeof(struct __pyx_obj_7pyarrow_3lib_Buffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Buffer),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Buffer) __PYX_ERR(8, 499, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Buffer = (struct __pyx_vtabstruct_7pyarrow_3lib_Buffer*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Buffer); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Buffer)) __PYX_ERR(8, 499, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ResizableBuffer = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "ResizableBuffer", sizeof(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_ResizableBuffer) __PYX_ERR(8, 509, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ResizableBuffer = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ResizableBuffer", sizeof(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ResizableBuffer) __PYX_ERR(8, 509, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_ResizableBuffer = (struct __pyx_vtabstruct_7pyarrow_3lib_ResizableBuffer*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ResizableBuffer); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ResizableBuffer)) __PYX_ERR(8, 509, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_NativeFile = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "NativeFile", sizeof(struct __pyx_obj_7pyarrow_3lib_NativeFile), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_NativeFile),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_NativeFile) __PYX_ERR(8, 514, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_NativeFile = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NativeFile", sizeof(struct __pyx_obj_7pyarrow_3lib_NativeFile), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NativeFile),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NativeFile) __PYX_ERR(8, 514, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_NativeFile = (struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NativeFile); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NativeFile)) __PYX_ERR(8, 514, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BufferedInputStream = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "BufferedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_BufferedInputStream) __PYX_ERR(8, 538, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BufferedInputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BufferedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BufferedInputStream) __PYX_ERR(8, 538, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_BufferedInputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_BufferedInputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BufferedInputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BufferedInputStream)) __PYX_ERR(8, 538, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BufferedOutputStream = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "BufferedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_BufferedOutputStream) __PYX_ERR(8, 542, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BufferedOutputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BufferedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BufferedOutputStream) __PYX_ERR(8, 542, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_BufferedOutputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_BufferedOutputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BufferedOutputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BufferedOutputStream)) __PYX_ERR(8, 542, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_CompressedInputStream = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "CompressedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_CompressedInputStream) __PYX_ERR(8, 546, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_CompressedInputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CompressedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CompressedInputStream) __PYX_ERR(8, 546, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_CompressedInputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_CompressedInputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CompressedInputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CompressedInputStream)) __PYX_ERR(8, 546, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_CompressedOutputStream = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "CompressedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_CompressedOutputStream) __PYX_ERR(8, 550, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_CompressedOutputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CompressedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CompressedOutputStream) __PYX_ERR(8, 550, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_CompressedOutputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_CompressedOutputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CompressedOutputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CompressedOutputStream)) __PYX_ERR(8, 550, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__CRecordBatchWriter = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "_CRecordBatchWriter", sizeof(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib__CRecordBatchWriter) __PYX_ERR(8, 554, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_RecordBatchReader = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "RecordBatchReader", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_RecordBatchReader) __PYX_ERR(8, 559, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_CacheOptions = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "CacheOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_CacheOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_CacheOptions),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_CacheOptions) __PYX_ERR(8, 564, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__CRecordBatchWriter = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_CRecordBatchWriter", sizeof(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__CRecordBatchWriter) __PYX_ERR(8, 554, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_RecordBatchReader = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RecordBatchReader", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RecordBatchReader) __PYX_ERR(8, 559, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_CacheOptions = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CacheOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_CacheOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CacheOptions),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CacheOptions) __PYX_ERR(8, 564, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_CacheOptions = (struct __pyx_vtabstruct_7pyarrow_3lib_CacheOptions*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CacheOptions); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CacheOptions)) __PYX_ERR(8, 564, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Codec = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "Codec", sizeof(struct __pyx_obj_7pyarrow_3lib_Codec), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_Codec),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_Codec) __PYX_ERR(8, 576, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Codec = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Codec", sizeof(struct __pyx_obj_7pyarrow_3lib_Codec), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Codec),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Codec) __PYX_ERR(8, 576, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_Codec = (struct __pyx_vtabstruct_7pyarrow_3lib_Codec*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Codec); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Codec)) __PYX_ERR(8, 576, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StopToken = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow.lib", "StopToken", sizeof(struct __pyx_obj_7pyarrow_3lib_StopToken), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_3lib_StopToken),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_3lib_StopToken) __PYX_ERR(8, 584, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StopToken = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StopToken", sizeof(struct __pyx_obj_7pyarrow_3lib_StopToken), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StopToken),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StopToken) __PYX_ERR(8, 584, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_StopToken = (struct __pyx_vtabstruct_7pyarrow_3lib_StopToken*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StopToken); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StopToken)) __PYX_ERR(8, 584, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("pyarrow._parquet"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow._parquet", "FileEncryptionProperties", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileEncryptionProperties), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_8_parquet_FileEncryptionProperties),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties) __PYX_ERR(4, 564, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "FileEncryptionProperties", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileEncryptionProperties), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_FileEncryptionProperties),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties) __PYX_ERR(4, 564, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_8_parquet_FileEncryptionProperties = (struct __pyx_vtabstruct_7pyarrow_8_parquet_FileEncryptionProperties*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties); if (unlikely(!__pyx_vtabptr_7pyarrow_8_parquet_FileEncryptionProperties)) __PYX_ERR(4, 564, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_8_parquet_ParquetSchema = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow._parquet", "ParquetSchema", sizeof(struct __pyx_obj_7pyarrow_8_parquet_ParquetSchema), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_8_parquet_ParquetSchema),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_8_parquet_ParquetSchema) __PYX_ERR(4, 608, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_8_parquet_FileMetaData = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow._parquet", "FileMetaData", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileMetaData), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_8_parquet_FileMetaData),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_8_parquet_FileMetaData) __PYX_ERR(4, 613, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_8_parquet_ParquetSchema = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "ParquetSchema", sizeof(struct __pyx_obj_7pyarrow_8_parquet_ParquetSchema), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_ParquetSchema),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_ParquetSchema) __PYX_ERR(4, 608, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_8_parquet_FileMetaData = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "FileMetaData", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileMetaData), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_FileMetaData),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_FileMetaData) __PYX_ERR(4, 613, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_8_parquet_FileMetaData = (struct __pyx_vtabstruct_7pyarrow_8_parquet_FileMetaData*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_8_parquet_FileMetaData); if (unlikely(!__pyx_vtabptr_7pyarrow_8_parquet_FileMetaData)) __PYX_ERR(4, 613, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_8_parquet_RowGroupMetaData = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow._parquet", "RowGroupMetaData", sizeof(struct __pyx_obj_7pyarrow_8_parquet_RowGroupMetaData), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_8_parquet_RowGroupMetaData),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_8_parquet_RowGroupMetaData) __PYX_ERR(4, 623, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_8_parquet_ColumnChunkMetaData = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow._parquet", "ColumnChunkMetaData", sizeof(struct __pyx_obj_7pyarrow_8_parquet_ColumnChunkMetaData), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_8_parquet_ColumnChunkMetaData),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_8_parquet_ColumnChunkMetaData) __PYX_ERR(4, 630, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_8_parquet_RowGroupMetaData = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "RowGroupMetaData", sizeof(struct __pyx_obj_7pyarrow_8_parquet_RowGroupMetaData), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_RowGroupMetaData),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_RowGroupMetaData) __PYX_ERR(4, 623, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_8_parquet_ColumnChunkMetaData = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "ColumnChunkMetaData", sizeof(struct __pyx_obj_7pyarrow_8_parquet_ColumnChunkMetaData), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_ColumnChunkMetaData),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_ColumnChunkMetaData) __PYX_ERR(4, 630, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_8_parquet_ColumnChunkMetaData = (struct __pyx_vtabstruct_7pyarrow_8_parquet_ColumnChunkMetaData*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_8_parquet_ColumnChunkMetaData); if (unlikely(!__pyx_vtabptr_7pyarrow_8_parquet_ColumnChunkMetaData)) __PYX_ERR(4, 630, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_8_parquet_Statistics = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow._parquet", "Statistics", sizeof(struct __pyx_obj_7pyarrow_8_parquet_Statistics), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_8_parquet_Statistics),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_8_parquet_Statistics) __PYX_ERR(4, 641, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_8_parquet_Statistics = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "Statistics", sizeof(struct __pyx_obj_7pyarrow_8_parquet_Statistics), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_Statistics),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_Statistics) __PYX_ERR(4, 641, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_8_parquet_Statistics = (struct __pyx_vtabstruct_7pyarrow_8_parquet_Statistics*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_8_parquet_Statistics); if (unlikely(!__pyx_vtabptr_7pyarrow_8_parquet_Statistics)) __PYX_ERR(4, 641, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_8_parquet_FileDecryptionProperties = __Pyx_ImportType_3_0_9(__pyx_t_1, "pyarrow._parquet", "FileDecryptionProperties", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileDecryptionProperties), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_7pyarrow_8_parquet_FileDecryptionProperties),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7pyarrow_8_parquet_FileDecryptionProperties) __PYX_ERR(4, 660, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_8_parquet_FileDecryptionProperties = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "FileDecryptionProperties", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileDecryptionProperties), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_FileDecryptionProperties),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_FileDecryptionProperties) __PYX_ERR(4, 660, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_8_parquet_FileDecryptionProperties = (struct __pyx_vtabstruct_7pyarrow_8_parquet_FileDecryptionProperties*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_8_parquet_FileDecryptionProperties); if (unlikely(!__pyx_vtabptr_7pyarrow_8_parquet_FileDecryptionProperties)) __PYX_ERR(4, 660, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -50153,221 +50172,221 @@
 
 #line 1 "(tree fragment)"
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_7) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
 
 #line 1 "(tree fragment)"
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "palletjack/palletjack_cython.pyx":3
- * # distutils: include_dirs = .
+  /* "palletjack/palletjack_cython.pyx":4
  * 
+ * import cython
  * import pyarrow as pa             # <<<<<<<<<<<<<<
  * import pyarrow.parquet as pq
  * from cython.cimports.palletjack import cpalletjack
  */
 
-#line 3 "palletjack/palletjack_cython.pyx"
-  __pyx_t_7 = __Pyx_ImportDottedModule(__pyx_n_s_pyarrow, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 3, __pyx_L1_error)
+#line 4 "palletjack/palletjack_cython.pyx"
+  __pyx_t_7 = __Pyx_ImportDottedModule(__pyx_n_s_pyarrow, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 4, __pyx_L1_error)
 
-#line 3 "palletjack/palletjack_cython.pyx"
+#line 4 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_7);
 
-#line 3 "palletjack/palletjack_cython.pyx"
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pa, __pyx_t_7) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+#line 4 "palletjack/palletjack_cython.pyx"
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pa, __pyx_t_7) < 0) __PYX_ERR(1, 4, __pyx_L1_error)
 
-#line 3 "palletjack/palletjack_cython.pyx"
+#line 4 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "palletjack/palletjack_cython.pyx":4
- * 
+  /* "palletjack/palletjack_cython.pyx":5
+ * import cython
  * import pyarrow as pa
  * import pyarrow.parquet as pq             # <<<<<<<<<<<<<<
  * from cython.cimports.palletjack import cpalletjack
  * from libcpp.string cimport string
  */
 
-#line 4 "palletjack/palletjack_cython.pyx"
-  __pyx_t_7 = __Pyx_ImportDottedModule(__pyx_n_s_pyarrow_parquet, __pyx_tuple__30); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 4, __pyx_L1_error)
+#line 5 "palletjack/palletjack_cython.pyx"
+  __pyx_t_7 = __Pyx_ImportDottedModule(__pyx_n_s_pyarrow_parquet, __pyx_tuple__30); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 5, __pyx_L1_error)
 
-#line 4 "palletjack/palletjack_cython.pyx"
+#line 5 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_7);
 
-#line 4 "palletjack/palletjack_cython.pyx"
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pq, __pyx_t_7) < 0) __PYX_ERR(1, 4, __pyx_L1_error)
+#line 5 "palletjack/palletjack_cython.pyx"
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pq, __pyx_t_7) < 0) __PYX_ERR(1, 5, __pyx_L1_error)
 
-#line 4 "palletjack/palletjack_cython.pyx"
+#line 5 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "palletjack/palletjack_cython.pyx":12
+  /* "palletjack/palletjack_cython.pyx":13
  * from pyarrow._parquet cimport *
  * 
  * cpdef generate_metadata_index(parquet_path, index_file_path = None):             # <<<<<<<<<<<<<<
  *     cdef string encoded_parquet_path = parquet_path.encode('utf8')
  *     cdef string encoded_index_file_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
  */
 
-#line 12 "palletjack/palletjack_cython.pyx"
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_10palletjack_17palletjack_cython_1generate_metadata_index, 0, __pyx_n_s_generate_metadata_index, NULL, __pyx_n_s_palletjack_palletjack_cython, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 12, __pyx_L1_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_10palletjack_17palletjack_cython_1generate_metadata_index, 0, __pyx_n_s_generate_metadata_index, NULL, __pyx_n_s_palletjack_palletjack_cython, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 13, __pyx_L1_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_7);
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__33);
 
-#line 12 "palletjack/palletjack_cython.pyx"
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_metadata_index, __pyx_t_7) < 0) __PYX_ERR(1, 12, __pyx_L1_error)
+#line 13 "palletjack/palletjack_cython.pyx"
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_metadata_index, __pyx_t_7) < 0) __PYX_ERR(1, 13, __pyx_L1_error)
 
-#line 12 "palletjack/palletjack_cython.pyx"
+#line 13 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "palletjack/palletjack_cython.pyx":28
+  /* "palletjack/palletjack_cython.pyx":29
  *     return None
  * 
  * cpdef read_metadata(index_file_path = None, row_groups = [], column_indices = [], column_names = [], index_data = None):             # <<<<<<<<<<<<<<
  * 
  *     cdef shared_ptr[CFileMetaData] c_metadata
  */
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_k__16 = __pyx_t_7;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_7 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_k__17 = __pyx_t_7;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_7 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_k__18 = __pyx_t_7;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_7 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_4);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_5);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_9 = PyTuple_New(5); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_9 = PyTuple_New(5); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_9);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 0, Py_None)) __PYX_ERR(1, 28, __pyx_L1_error);
+#line 29 "palletjack/palletjack_cython.pyx"
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 0, Py_None)) __PYX_ERR(1, 29, __pyx_L1_error);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_t_7);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_7)) __PYX_ERR(1, 28, __pyx_L1_error);
+#line 29 "palletjack/palletjack_cython.pyx"
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_7)) __PYX_ERR(1, 29, __pyx_L1_error);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_t_4);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_4)) __PYX_ERR(1, 28, __pyx_L1_error);
+#line 29 "palletjack/palletjack_cython.pyx"
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_4)) __PYX_ERR(1, 29, __pyx_L1_error);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(__pyx_t_5);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 3, __pyx_t_5)) __PYX_ERR(1, 28, __pyx_L1_error);
+#line 29 "palletjack/palletjack_cython.pyx"
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 3, __pyx_t_5)) __PYX_ERR(1, 29, __pyx_L1_error);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_INCREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GIVEREF(Py_None);
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 4, Py_None)) __PYX_ERR(1, 28, __pyx_L1_error);
+#line 29 "palletjack/palletjack_cython.pyx"
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 4, Py_None)) __PYX_ERR(1, 29, __pyx_L1_error);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_7 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_4 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __pyx_t_5 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_10palletjack_17palletjack_cython_3read_metadata, 0, __pyx_n_s_read_metadata, NULL, __pyx_n_s_palletjack_palletjack_cython, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_10palletjack_17palletjack_cython_3read_metadata, 0, __pyx_n_s_read_metadata, NULL, __pyx_n_s_palletjack_palletjack_cython, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_5);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_5, __pyx_t_9);
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-#line 28 "palletjack/palletjack_cython.pyx"
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_metadata, __pyx_t_5) < 0) __PYX_ERR(1, 28, __pyx_L1_error)
+#line 29 "palletjack/palletjack_cython.pyx"
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_metadata, __pyx_t_5) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
 
-#line 28 "palletjack/palletjack_cython.pyx"
+#line 29 "palletjack/palletjack_cython.pyx"
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "palletjack/palletjack_cython.pyx":1
  * # distutils: include_dirs = .             # <<<<<<<<<<<<<<
  * 
- * import pyarrow as pa
+ * import cython
  */
 
 #line 1 "palletjack/palletjack_cython.pyx"
   __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1, __pyx_L1_error)
 
 #line 1 "palletjack/palletjack_cython.pyx"
   __Pyx_GOTREF(__pyx_t_5);
@@ -53163,31 +53182,14 @@
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
     PyObject *arg[2] = {NULL, NULL};
     return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
-/* BufferIndexError */
-static void __Pyx_RaiseBufferIndexError(int axis) {
-  PyErr_Format(PyExc_IndexError,
-     "Out of bounds on buffer access (axis %d)", axis);
-}
-
-/* BufferIndexErrorNogil */
-static void __Pyx_RaiseBufferIndexErrorNogil(int axis) {
-    #ifdef WITH_THREAD
-    PyGILState_STATE gilstate = PyGILState_Ensure();
-    #endif
-    __Pyx_RaiseBufferIndexError(axis);
-    #ifdef WITH_THREAD
-    PyGILState_Release(gilstate);
-    #endif
-}
-
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
@@ -53691,18 +53693,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -53748,23 +53750,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `palletjack-2.1.0/palletjack/palletjack_cython.pyx` & `palletjack-2.1.2/palletjack/palletjack_cython.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # distutils: include_dirs = .
 
+import cython
 import pyarrow as pa
 import pyarrow.parquet as pq
 from cython.cimports.palletjack import cpalletjack
 from libcpp.string cimport string
 from libcpp.memory cimport shared_ptr
 from libcpp.vector cimport vector
 from libc.stdint cimport uint32_t
@@ -31,16 +32,17 @@
     cdef string encoded_path = index_file_path.encode('utf8') if index_file_path is not None else "".encode('utf8')
     cdef const unsigned char[::1] mv = index_data
     cdef vector[uint32_t] crow_groups = row_groups
     cdef vector[uint32_t] ccolumn_indices = column_indices
     cdef vector[string] ccolumn_names = [c.encode('utf8') for c in column_names]
 
     if index_file_path is None:
-        with nogil:
-            c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
+        with cython.boundscheck(False):
+            with nogil:
+                c_metadata = cpalletjack.ReadMetadata(&mv[0], len(mv), crow_groups, ccolumn_indices, ccolumn_names)
     else:
         with nogil:
             c_metadata = cpalletjack.ReadMetadata(encoded_path.c_str(), crow_groups, ccolumn_indices, ccolumn_names)
 
     cdef FileMetaData m = FileMetaData.__new__(FileMetaData)
     m.init(c_metadata)
     return m
```

### Comparing `palletjack-2.1.0/palletjack/parquet_types_palletjack.cpp` & `palletjack-2.1.2/palletjack/parquet_types_palletjack.cpp`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.0/palletjack/parquet_types_palletjack.h` & `palletjack-2.1.2/palletjack/parquet_types_palletjack.h`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.0/palletjack.egg-info/PKG-INFO` & `palletjack-2.1.2/palletjack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palletjack
-Version: 2.1.0
+Version: 2.1.2
 Summary: Faster parquet metadata reading
 Author-email: Marcin Krystianc <marcin.krystianc@gmail.com>
 Project-URL: Homepage, https://github.com/marcin-krystianc/PalletJack
 Project-URL: Issues, https://github.com/marcin-krystianc/PalletJack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -76,47 +76,47 @@
 ```
 
 ### Reading the in-memory metadata index from a file using pyarrow's fs:
 ```
 index_data = fs.LocalFileSystem().open_input_stream(index_path).readall()
 ```
 
-### Reading data with help of index file:
+### Reading data with help of the index file:
 ```
 metadata = pj.read_metadata(index_path, row_groups = [5, 7])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading data with help of in-memory index:
+### Reading data with help of the in-memory index:
 ```
 metadata = pj.read_metadata(index_data = index_data, row_groups = [5, 7])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of columns using column indices:
+### Reading a subset of columns using column indices:
 ```
 metadata = pj.read_metadata(index_path, column_indices = [1, 3])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of columns using column names:
+### Reading a subset of columns using column names:
 ```
 metadata = pj.read_metadata(index_path, column_names = ['column_1', 'column_3'])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 data = pr.read_all()
 ```
 
-### Reading subset of row groups and columns:
+### Reading a subset of row groups and columns:
 ```
 metadata = pj.read_metadata(index_path, row_groups = [5, 7], column_indices = [1, 3])
 pr = pq.ParquetReader()
 pr.open(path, metadata=metadata)
 
 data = pr.read_all()
 ```
```

### Comparing `palletjack-2.1.0/palletjack.egg-info/SOURCES.txt` & `palletjack-2.1.2/palletjack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.0/pyproject.toml` & `palletjack-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "thrift",
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "palletjack"
-version = "2.1.0"
+version = "2.1.2"
 authors = [
   { name="Marcin Krystianc", email="marcin.krystianc@gmail.com" },
 ]
 description = "Faster parquet metadata reading"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `palletjack-2.1.0/setup.py` & `palletjack-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.0/test/test_palletjack.py` & `palletjack-2.1.2/test/test_palletjack.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,14 +69,56 @@
             all_row_groups = list(range(0, n_row_groups))
             for r in range(0, 4):
                 for rp in it.permutations(all_row_groups, r):
                     for c in range(0, 4):
                         for cp in it.permutations(all_columns, c):
                             validate_reading(path, index_path, row_groups = rp, column_indices = cp)
 
+    def test_metadata_roundtrip(self):
+        with tempfile.TemporaryDirectory(ignore_cleanup_errors=True) as tmpdirname:
+            path = os.path.join(tmpdirname, "my.parquet")
+            table = get_table()
+
+            pq.write_table(table, path, row_group_size=chunk_size)
+
+            index_path = path + '.index'
+            pj.generate_metadata_index(path, index_path)
+
+            pr = pq.ParquetReader()
+            pr.open(path)
+            
+            row_groups_columns = [
+                ([], []),
+                ([], range(n_columns)),
+                (range(n_row_groups), []),
+                (range(n_row_groups), range(n_columns)),
+            ]
+            
+            for (row_groups, columns) in row_groups_columns:
+                pj_metadata = pj.read_metadata(index_path, row_groups=row_groups, column_indices=columns)
+                self.assertEqual(pr.metadata, pj_metadata)
+
+    def test_reading_non_pyarrow_files(self):
+        
+            path = os.path.join(current_dir, 'data/no_column_orders.parquet')
+            pr = pq.ParquetReader()
+            pr.open(path)
+            
+            row_groups_columns = [
+                ([], []),
+                ([], range(pr.metadata.num_columns)),
+                (range(pr.metadata.num_row_groups), []),
+                (range(pr.metadata.num_row_groups), range(pr.metadata.num_columns)),
+            ]
+            
+            index_data = pj.generate_metadata_index(path)
+            for (row_groups, columns) in row_groups_columns:
+                pj_metadata = pj.read_metadata(index_data = index_data, row_groups=row_groups, column_indices=columns)
+                self.assertEqual(pr.metadata, pj_metadata)
+                
     def test_reading_invalid_row_group(self):
         with tempfile.TemporaryDirectory() as tmpdirname:
             path = os.path.join(tmpdirname, "my.parquet")
             table = get_table()
 
             pq.write_table(table, path, row_group_size=chunk_size, use_dictionary=False, write_statistics=False, store_schema=False)
 
@@ -127,16 +169,16 @@
                 metadata = pj.read_metadata("not_existing_file.parquet.index", [0])
 
             self.assertTrue(f"I/O error when opening 'not_existing_file.parquet.index'" in str(context.exception), context.exception)
 
     def test_index_file_golden_master(self):
         with tempfile.TemporaryDirectory() as tmpdirname:
             index_path = os.path.join(tmpdirname, 'my.parquet.index')
-            path = os.path.join(current_dir, 'data/sample.parquet')
-            expected_index_path = os.path.join(current_dir, 'data/sample.parquet.index')
+            path = os.path.join(current_dir, 'data/golden_master.parquet')
+            expected_index_path = os.path.join(current_dir, 'data/golden_master.parquet.index')
             pj.generate_metadata_index(path, index_path)
 
             # Read the expected output
             with open(expected_index_path, 'rb') as file:
                 expected_output = file.read()
 
             # Read the expected output
```

### Comparing `palletjack-2.1.0/test/test_readme.py` & `palletjack-2.1.2/test/test_readme.py`

 * *Files identical despite different names*

