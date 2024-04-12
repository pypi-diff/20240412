# Comparing `tmp/hbase-driver-0.0.9.tar.gz` & `tmp/hbase-driver-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbase-driver-0.0.9.tar", last modified: Wed Feb 21 14:14:48 2024, max compression
+gzip compressed data, was "hbase-driver-1.0.0.tar", last modified: Fri Apr 12 11:50:06 2024, max compression
```

## Comparing `hbase-driver-0.0.9.tar` & `hbase-driver-1.0.0.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.457484 hbase-driver-0.0.9/
--rw-r--r--   0 jeffzhong   (501) staff       (20)    11324 2024-02-09 09:08:07.000000 hbase-driver-0.0.9/LICENSE
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1239 2024-02-21 14:14:48.457263 hbase-driver-0.0.9/PKG-INFO
--rw-r--r--   0 jeffzhong   (501) staff       (20)      954 2024-02-21 14:14:33.000000 hbase-driver-0.0.9/README.md
--rw-r--r--   0 jeffzhong   (501) staff       (20)      515 2024-02-21 14:14:41.000000 hbase-driver-0.0.9/pyproject.toml
--rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-02-21 14:14:48.457526 hbase-driver-0.0.9/setup.cfg
--rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-02-15 05:54:23.000000 hbase-driver-0.0.9/setup.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.431149 hbase-driver-0.0.9/src/
--rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:50.000000 hbase-driver-0.0.9/src/__init__.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.457007 hbase-driver-0.0.9/src/hbase_driver.egg-info/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1239 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/PKG-INFO
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4590 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/SOURCES.txt
--rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/dependency_links.txt
--rw-r--r--   0 jeffzhong   (501) staff       (20)        6 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/requires.txt
--rw-r--r--   0 jeffzhong   (501) staff       (20)       12 2024-02-21 14:14:48.000000 hbase-driver-0.0.9/src/hbase_driver.egg-info/top_level.txt
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.434751 hbase-driver-0.0.9/src/hbasedriver/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     5564 2024-02-18 12:15:14.000000 hbase-driver-0.0.9/src/hbasedriver/Connection.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:42.000000 hbase-driver-0.0.9/src/hbasedriver/__init__.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.435557 hbase-driver-0.0.9/src/hbasedriver/client/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       27 2024-02-13 10:52:12.000000 hbase-driver-0.0.9/src/hbasedriver/client/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      875 2024-02-15 04:35:33.000000 hbase-driver-0.0.9/src/hbasedriver/client/client.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2549 2024-02-18 12:42:23.000000 hbase-driver-0.0.9/src/hbasedriver/client/table.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.436005 hbase-driver-0.0.9/src/hbasedriver/exceptions/
--rw-r--r--   0 jeffzhong   (501) staff       (20)      208 2024-02-13 11:06:09.000000 hbase-driver-0.0.9/src/hbasedriver/exceptions/RemoteException.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-15 04:48:34.000000 hbase-driver-0.0.9/src/hbasedriver/exceptions/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2099 2024-02-18 12:14:57.000000 hbase-driver-0.0.9/src/hbasedriver/master.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1092 2024-02-18 12:50:33.000000 hbase-driver-0.0.9/src/hbasedriver/meta_server.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.436806 hbase-driver-0.0.9/src/hbasedriver/model/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       39 2024-02-15 09:44:07.000000 hbase-driver-0.0.9/src/hbasedriver/model/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      560 2024-02-16 06:16:01.000000 hbase-driver-0.0.9/src/hbasedriver/model/cell.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1076 2024-02-21 14:09:31.000000 hbase-driver-0.0.9/src/hbasedriver/model/row.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.438344 hbase-driver-0.0.9/src/hbasedriver/operations/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       60 2024-02-15 09:36:12.000000 hbase-driver-0.0.9/src/hbasedriver/operations/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1403 2024-02-16 06:24:06.000000 hbase-driver-0.0.9/src/hbasedriver/operations/delete.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      579 2024-02-15 09:10:08.000000 hbase-driver-0.0.9/src/hbasedriver/operations/get.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      565 2024-02-16 11:15:48.000000 hbase-driver-0.0.9/src/hbasedriver/operations/put.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1651 2024-02-21 14:05:47.000000 hbase-driver-0.0.9/src/hbasedriver/operations/scan.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.454191 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6557 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     7736 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    16699 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    18884 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3927 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4557 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2239 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2408 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    18228 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    28375 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1271 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterId_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      408 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterId_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    10609 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    20630 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3727 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3765 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1474 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      896 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2099 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1942 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1671 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1057 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     8649 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    11171 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     9434 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    13837 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2376 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3041 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1317 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      411 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LoadBalancer_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4388 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     5485 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1666 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1232 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    32135 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    51191 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)    52933 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    51311 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4819 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6880 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     7707 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     9897 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3846 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     5095 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1770 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1663 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1327 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      423 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     8348 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     9133 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4569 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2771 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6353 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     7628 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1345 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      466 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3910 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     4966 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1597 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1009 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1321 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TestProcedure_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      420 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TestProcedure_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2142 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2530 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2052 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1028 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6485 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)    10882 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3168 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3381 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)      180 2024-02-15 08:37:54.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2070 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1164 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1837 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      164 2024-02-15 05:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_rpc_service_pb2.pyi
--rw-r--r--   0 jeffzhong   (501) staff       (20)     1290 2024-02-15 09:13:14.000000 hbase-driver-0.0.9/src/hbasedriver/region.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6655 2024-02-21 14:08:38.000000 hbase-driver-0.0.9/src/hbasedriver/regionserver.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-02-10 15:01:32.000000 hbase-driver-0.0.9/src/hbasedriver/request.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      190 2024-02-15 04:47:05.000000 hbase-driver-0.0.9/src/hbasedriver/response.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.454974 hbase-driver-0.0.9/src/hbasedriver/util/
--rw-r--r--   0 jeffzhong   (501) staff       (20)       22 2024-02-15 04:36:36.000000 hbase-driver-0.0.9/src/hbasedriver/util/__init__.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      211 2024-02-13 07:51:10.000000 hbase-driver-0.0.9/src/hbasedriver/util/bytes.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     6044 2024-02-10 15:46:22.000000 hbase-driver-0.0.9/src/hbasedriver/util/varint.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)     3516 2024-02-15 04:47:30.000000 hbase-driver-0.0.9/src/hbasedriver/zk.py
-drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-02-21 14:14:48.456544 hbase-driver-0.0.9/test/
--rw-r--r--   0 jeffzhong   (501) staff       (20)     2024 2024-02-16 12:08:09.000000 hbase-driver-0.0.9/test/test_client.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      809 2024-02-15 09:31:21.000000 hbase-driver-0.0.9/test/test_master.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      444 2024-02-15 03:30:47.000000 hbase-driver-0.0.9/test/test_rs.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      853 2024-02-21 14:12:27.000000 hbase-driver-0.0.9/test/test_scan.py
--rw-r--r--   0 jeffzhong   (501) staff       (20)      207 2024-02-13 09:42:21.000000 hbase-driver-0.0.9/test/test_zk.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.255388 hbase-driver-1.0.0/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    11324 2024-02-09 09:08:07.000000 hbase-driver-1.0.0/LICENSE
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3300 2024-04-12 11:50:06.255163 hbase-driver-1.0.0/PKG-INFO
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3015 2024-04-01 15:06:59.000000 hbase-driver-1.0.0/README.md
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      515 2024-04-12 11:49:48.000000 hbase-driver-1.0.0/pyproject.toml
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-04-12 11:50:06.255434 hbase-driver-1.0.0/setup.cfg
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       38 2024-02-15 05:54:23.000000 hbase-driver-1.0.0/setup.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.228798 hbase-driver-1.0.0/src/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:50.000000 hbase-driver-1.0.0/src/__init__.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.254898 hbase-driver-1.0.0/src/hbase_driver.egg-info/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3300 2024-04-12 11:50:06.000000 hbase-driver-1.0.0/src/hbase_driver.egg-info/PKG-INFO
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4642 2024-04-12 11:50:06.000000 hbase-driver-1.0.0/src/hbase_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-04-12 11:50:06.000000 hbase-driver-1.0.0/src/hbase_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        6 2024-04-12 11:50:06.000000 hbase-driver-1.0.0/src/hbase_driver.egg-info/requires.txt
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       12 2024-04-12 11:50:06.000000 hbase-driver-1.0.0/src/hbase_driver.egg-info/top_level.txt
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.231906 hbase-driver-1.0.0/src/hbasedriver/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     5805 2024-02-25 04:04:03.000000 hbase-driver-1.0.0/src/hbasedriver/Connection.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-13 07:49:42.000000 hbase-driver-1.0.0/src/hbasedriver/__init__.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.232769 hbase-driver-1.0.0/src/hbasedriver/client/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       27 2024-02-13 10:52:12.000000 hbase-driver-1.0.0/src/hbasedriver/client/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4885 2024-04-01 15:11:22.000000 hbase-driver-1.0.0/src/hbasedriver/client/client.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2565 2024-03-12 14:36:10.000000 hbase-driver-1.0.0/src/hbasedriver/client/table.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.233338 hbase-driver-1.0.0/src/hbasedriver/exceptions/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      208 2024-02-13 11:06:09.000000 hbase-driver-1.0.0/src/hbasedriver/exceptions/RemoteException.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        0 2024-02-15 04:48:34.000000 hbase-driver-1.0.0/src/hbasedriver/exceptions/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2986 2024-04-01 15:02:23.000000 hbase-driver-1.0.0/src/hbasedriver/master.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1206 2024-03-12 14:18:46.000000 hbase-driver-1.0.0/src/hbasedriver/meta_server.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.234036 hbase-driver-1.0.0/src/hbasedriver/model/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       39 2024-02-15 09:44:07.000000 hbase-driver-1.0.0/src/hbasedriver/model/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      560 2024-02-16 06:16:01.000000 hbase-driver-1.0.0/src/hbasedriver/model/cell.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1076 2024-02-21 15:06:05.000000 hbase-driver-1.0.0/src/hbasedriver/model/row.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.235911 hbase-driver-1.0.0/src/hbasedriver/operations/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       80 2024-02-21 14:54:04.000000 hbase-driver-1.0.0/src/hbasedriver/operations/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1399 2024-02-25 04:34:00.000000 hbase-driver-1.0.0/src/hbasedriver/operations/column_family_builder.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1527 2024-02-28 14:51:21.000000 hbase-driver-1.0.0/src/hbasedriver/operations/delete.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      579 2024-02-15 09:10:08.000000 hbase-driver-1.0.0/src/hbasedriver/operations/get.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      565 2024-02-16 11:15:48.000000 hbase-driver-1.0.0/src/hbasedriver/operations/put.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1651 2024-02-21 14:05:47.000000 hbase-driver-1.0.0/src/hbasedriver/operations/scan.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.252825 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6557 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/AccessControl_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     7736 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    16699 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Admin_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    18884 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Admin_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3927 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4557 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2239 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Cell_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2408 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Cell_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    18228 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Client_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    28375 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Client_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1271 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ClusterId_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      408 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ClusterId_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    10609 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    20630 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3727 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Comparator_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3765 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Comparator_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1474 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Encryption_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      896 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Encryption_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2099 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1942 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1671 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/FS_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1057 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/FS_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     8649 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Filter_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    11171 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Filter_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     9434 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HBase_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    13837 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HBase_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2376 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HFile_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3041 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HFile_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1317 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      411 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/LoadBalancer_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4388 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/LockService_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     5485 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/LockService_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1666 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MapReduce_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1232 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    32135 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    51191 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    52933 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Master_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    51311 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Master_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4819 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Procedure_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6880 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Procedure_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     7707 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Quota_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     9897 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Quota_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3846 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RPC_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     5095 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RPC_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1770 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RecentLogs_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1663 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1327 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      423 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     8348 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     9133 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4569 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Registry_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2771 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Registry_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6353 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Replication_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     7628 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Replication_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1345 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      466 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3910 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Snapshot_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     4966 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1597 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1009 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1321 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/TestProcedure_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      420 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/TestProcedure_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2142 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2530 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2052 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Tracing_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1028 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Tracing_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6485 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/WAL_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)    10882 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/WAL_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3168 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3381 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      180 2024-02-15 08:37:54.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2070 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/test_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1164 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/test_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1837 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      164 2024-02-15 05:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/protobuf_py/test_rpc_service_pb2.pyi
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     1392 2024-03-31 10:34:07.000000 hbase-driver-1.0.0/src/hbasedriver/region.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6805 2024-02-28 15:00:50.000000 hbase-driver-1.0.0/src/hbasedriver/regionserver.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)        1 2024-02-10 15:01:32.000000 hbase-driver-1.0.0/src/hbasedriver/request.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      368 2024-02-25 09:55:57.000000 hbase-driver-1.0.0/src/hbasedriver/response.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.253409 hbase-driver-1.0.0/src/hbasedriver/util/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)       22 2024-02-15 04:36:36.000000 hbase-driver-1.0.0/src/hbasedriver/util/__init__.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      211 2024-02-13 07:51:10.000000 hbase-driver-1.0.0/src/hbasedriver/util/bytes.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     6044 2024-02-10 15:46:22.000000 hbase-driver-1.0.0/src/hbasedriver/util/varint.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3516 2024-03-12 14:46:27.000000 hbase-driver-1.0.0/src/hbasedriver/zk.py
+drwxr-xr-x   0 jeffzhong   (501) staff       (20)        0 2024-04-12 11:50:06.254608 hbase-driver-1.0.0/test/
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     3372 2024-02-28 15:09:48.000000 hbase-driver-1.0.0/test/test_client.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)     2399 2024-04-06 09:40:18.000000 hbase-driver-1.0.0/test/test_master.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      444 2024-02-15 03:30:47.000000 hbase-driver-1.0.0/test/test_rs.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      857 2024-02-21 14:59:12.000000 hbase-driver-1.0.0/test/test_scan.py
+-rw-r--r--   0 jeffzhong   (501) staff       (20)      207 2024-02-13 09:42:21.000000 hbase-driver-1.0.0/test/test_zk.py
```

### Comparing `hbase-driver-0.0.9/LICENSE` & `hbase-driver-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/pyproject.toml` & `hbase-driver-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'hbase-driver'
-version = "0.0.9"
+version = "1.0.0"
 readme = "README.md"
 dependencies = ['kazoo']
 
 [tool.setuptools]
 package-dir = { "" = "src" }
 packages = ["hbasedriver", "hbasedriver.protobuf_py", "hbasedriver.operations", "hbasedriver.model", "hbasedriver.exceptions", "hbasedriver.client"]
```

### Comparing `hbase-driver-0.0.9/src/hbase_driver.egg-info/SOURCES.txt` & `hbase-driver-1.0.0/src/hbase_driver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/hbasedriver/client/table.py
 src/hbasedriver/exceptions/RemoteException.py
 src/hbasedriver/exceptions/__init__.py
 src/hbasedriver/model/__init__.py
 src/hbasedriver/model/cell.py
 src/hbasedriver/model/row.py
 src/hbasedriver/operations/__init__.py
+src/hbasedriver/operations/column_family_builder.py
 src/hbasedriver/operations/delete.py
 src/hbasedriver/operations/get.py
 src/hbasedriver/operations/put.py
 src/hbasedriver/operations/scan.py
 src/hbasedriver/protobuf_py/AccessControl_pb2.py
 src/hbasedriver/protobuf_py/AccessControl_pb2.pyi
 src/hbasedriver/protobuf_py/Admin_pb2.py
```

### Comparing `hbase-driver-0.0.9/src/hbasedriver/Connection.py` & `hbase-driver-1.0.0/src/hbasedriver/Connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import random
 import socket
 from abc import abstractmethod
 from struct import pack, unpack
+from threading import Lock
 
 from google.protobuf import message
 
 from hbasedriver.protobuf_py.RPC_pb2 import ConnectionHeader, RequestHeader, ResponseHeader
 from hbasedriver.exceptions.RemoteException import RemoteException
 from hbasedriver.exceptions.RemoteException import TableExistsException
 from hbasedriver.response import response_types
@@ -18,59 +19,62 @@
         assert service_name in ["ClientService", "MasterService"]
         self.service_name = service_name
         self.meta_region = None
         self.host = None
         self.port = None
         self.timeout = 60
         self.user = "pythonHbaseDriver"
+        self.lock = Lock()  # Mutex
 
     def connect(self, host, port=16000, timeout=60, user="pythonHbaseDriver"):
-        if type(host) != str:
-            host = host.decode("utf-8")
-        if type(port) != int:
-            port = int(port)
-        self.conn = socket.create_connection((host, port), timeout=timeout)
-        ch = ConnectionHeader()
-        ch.user_info.effective_user = self.user
-        ch.service_name = self.service_name
-        serialized = ch.SerializeToString()
-        # 6 bytes : 'HBas' + RPC_VERSION(0) + AUTH_CODE(80) +
-        msg = b"HBas\x00\x50" + pack(">I", len(serialized)) + serialized
-        self.conn.send(msg)
-        self.host = host
-        self.port = port
-        self.timeout = timeout
-        self.user = user
-        return self
+        with self.lock:
+            if type(host) != str:
+                host = host.decode("utf-8")
+            if type(port) != int:
+                port = int(port)
+            self.conn = socket.create_connection((host, port), timeout=timeout)
+            ch = ConnectionHeader()
+            ch.user_info.effective_user = self.user
+            ch.service_name = self.service_name
+            serialized = ch.SerializeToString()
+            # 6 bytes : 'HBas' + RPC_VERSION(0) + AUTH_CODE(80) +
+            msg = b"HBas\x00\x50" + pack(">I", len(serialized)) + serialized
+            self.conn.send(msg)
+            self.host = host
+            self.port = port
+            self.timeout = timeout
+            self.user = user
+            return self
 
     @abstractmethod
     def clone(self):
         """
         build another new connection with the same settings as this.
         """
         pass
 
     def send_request(self, req: message.Message, method_name: str, need_response=True):
-        rpc_serialized = req.SerializeToString()
-        call_id = random.randint(1, 999)
-        # call_id = 66
-        serialized_header = self._get_call_header_bytes(method_name, call_id)
-        rpc_length_bytes = to_varint(len(rpc_serialized)).encode('utf-8')
-        total_size = 4 + 1 + len(serialized_header) + len(rpc_length_bytes) + len(rpc_serialized)
-
-        # Total length doesn't include the initial 4 bytes (for the total_length uint32)
-        # size(4bytes) + header size(1byte)
-        to_send = pack(">IB", total_size - 4, len(serialized_header))
-        to_send += serialized_header + rpc_length_bytes + rpc_serialized
-
-        self.conn.send(to_send)
-        if need_response:
-            return self.receive_rpc(call_id, req, method_name)
-        else:
-            return
+        with self.lock:
+            rpc_serialized = req.SerializeToString()
+            call_id = random.randint(1, 999)
+            # call_id = 66
+            serialized_header = self._get_call_header_bytes(method_name, call_id)
+            rpc_length_bytes = to_varint(len(rpc_serialized)).encode('utf-8')
+            total_size = 4 + 1 + len(serialized_header) + len(rpc_length_bytes) + len(rpc_serialized)
+
+            # Total length doesn't include the initial 4 bytes (for the total_length uint32)
+            # size(4bytes) + header size(1byte)
+            to_send = pack(">IB", total_size - 4, len(serialized_header))
+            to_send += serialized_header + rpc_length_bytes + rpc_serialized
+
+            self.conn.send(to_send)
+            if need_response:
+                return self._receive_rpc(call_id, req, method_name)
+            else:
+                return
 
     @staticmethod
     def _get_call_header_bytes(method_name, call_id: int):
         header = RequestHeader()
         header.call_id = call_id
         header.method_name = method_name
         header.request_param = True
@@ -88,15 +92,15 @@
             packet = sock.recv(n - partial_len)
             if not packet:
                 raise socket.error()
             partial_len += len(packet)
             res += packet
         return res
 
-    def receive_rpc(self, call_id, rq: message.Message, rq_type: str, data=None):
+    def _receive_rpc(self, call_id, rq: message.Message, rq_type: str, data=None):
         # Total message length is going to be the first four bytes
         # (little-endian uint32)
         try:
             msg_length = self._recv_n(self.conn, 4)
             if msg_length is None:
                 raise
             msg_length = unpack(">I", msg_length)[0]
```

### Comparing `hbase-driver-0.0.9/src/hbasedriver/client/table.py` & `hbase-driver-1.0.0/src/hbasedriver/client/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class Table:
     """
     This class contains data operations within a table.
     """
 
-    def __init__(self, zk_quorum, ns, tb):
+    def __init__(self, zk_quorum, ns, tb, meta_conn=None):
         self.ns = ns
         self.tb = tb
         self.meta_rs_host, self.meta_rs_port = locate_meta_region(zk_quorum)
         # cache metadata for regions that we touched.
         self.regions = {}
         # we might maintain connections to different regionserver.
         self.rs_conns: dict[(bytes, int), RsConnection] = {}
```

### Comparing `hbase-driver-0.0.9/src/hbasedriver/meta_server.py` & `hbase-driver-1.0.0/src/hbasedriver/meta_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from hbasedriver.protobuf_py.Client_pb2 import ScanRequest, Column, ScanResponse
 from hbasedriver.Connection import Connection
 from hbasedriver.region import Region
 
 
 class MetaRsConnection(Connection):
+    def clone(self):
+        return MetaRsConnection.connect(self.host, self.port, self.timeout, user=self.user)
+
     def __init__(self):
         super().__init__("ClientService")
 
     # locate the region with given rowkey and table name. (must be called on rs with meta region)
     def locate_region(self, ns, tb, rowkey) -> Region:
         rq = ScanRequest()
         if ns is None or len(ns) == 0:
```

### Comparing `hbase-driver-0.0.9/src/hbasedriver/model/cell.py` & `hbase-driver-1.0.0/src/hbasedriver/model/cell.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/model/row.py` & `hbase-driver-1.0.0/src/hbasedriver/model/row.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/operations/delete.py` & `hbase-driver-1.0.0/src/hbasedriver/operations/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from collections import defaultdict
 
 from hbasedriver.model.cell import Cell, CellType
 
 
 class Delete:
     def __init__(self, rowkey: bytes):
+        """
+        If no more method call for this Delete object, we will delete everything with this row key.
+        """
         self.rowkey = rowkey
         self.family_cells: dict[bytes, list[Cell]] = defaultdict(list)
 
     # Delete the specified version of the specified column.
     def add_column(self, family: bytes, qualifier: bytes, ts: int):
         self.family_cells[family].append(Cell(self.rowkey, family, qualifier, ts=ts, cell_type=CellType.DELETE))
         return self
```

### Comparing `hbase-driver-0.0.9/src/hbasedriver/operations/get.py` & `hbase-driver-1.0.0/src/hbasedriver/operations/get.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/operations/put.py` & `hbase-driver-1.0.0/src/hbasedriver/operations/put.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/operations/scan.py` & `hbase-driver-1.0.0/src/hbasedriver/operations/scan.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/AccessControl_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/AccessControl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Admin_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Admin_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/BucketCacheEntry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Cell_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Cell_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Cell_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Client_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Client_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterId_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ClusterId_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ClusterStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ClusterStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Comparator_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Comparator_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Comparator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Encryption_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Encryption_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Encryption_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ErrorHandling_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ErrorHandling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/FS_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/FS_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/FS_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Filter_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Filter_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HBase_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HBase_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HBase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HFile_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/HFile_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/HFile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/LoadBalancer_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/LockService_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/LockService_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/LockService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MapReduce_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MapReduce_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MasterProcedure_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/MasterProcedure_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Master_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Master_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Master_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Procedure_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Procedure_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Procedure_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Quota_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Quota_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Quota_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RPC_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RPC_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RPC_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RecentLogs_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RecentLogs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RegionNormalizer_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/RegionServerStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Registry_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Registry_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Registry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Replication_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Replication_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Replication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/SnapshotCleanup_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/StoreFileTracker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TestProcedure_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/TestProcedure_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/TooSlowLog_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/TooSlowLog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Tracing_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/Tracing_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/Tracing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/WAL_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/WAL_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/WAL_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ZooKeeper_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/ZooKeeper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/test_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_pb2.pyi` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py` & `hbase-driver-1.0.0/src/hbasedriver/protobuf_py/test_rpc_service_pb2.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/region.py` & `hbase-driver-1.0.0/src/hbasedriver/region.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     """
 
     def __init__(self, region_encoded: bytes, host: bytes, port: bytes, region_info: RegionInfo):
         self.region_encoded = region_encoded
         self.host = host
         self.port = port
         self.region_info = region_info
+        self.state = None
 
     @staticmethod
     def from_cells(cells):
         row, host, port, region_info = None, None, None, None
         for c in cells:
             qf = c.qualifier
             if qf == b"server":
@@ -34,7 +35,10 @@
         return Region(row, host, port, region_info)
 
     def key_in_region(self, rowkey: bytes):
         """
         This checks the provided row key belong to this region.
         """
         return self.region_info.start_key <= rowkey < self.region_info.end_key
+
+    def get_region_name(self) -> bytes:
+        return self.region_encoded
```

### Comparing `hbase-driver-0.0.9/src/hbasedriver/regionserver.py` & `hbase-driver-1.0.0/src/hbasedriver/regionserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             raise Exception("can not clone connection that is not properly initialized. ")
         new_conn = RsConnection().connect(self.host, self.port)
         return new_conn
 
     def __init__(self):
         super().__init__("ClientService")
 
-    def put(self, region_name_encoded: bytes, put: Put):
+    def put(self, region_name_encoded: bytes, put: Put) -> bool:
         # send put request to the target region and receive response(processed?)
         rq = MutateRequest()
         # set target region
         rq.region.type = 1
         rq.region.value = region_name_encoded
         # set kv pairs
         rq.mutation.mutate_type = MutationProto.MutationType.PUT
@@ -72,15 +72,15 @@
         rq = MutateRequest()
         rq.mutation.mutate_type = MutationProto.MutationType.DELETE
         rq.region.type = 1
         rq.region.value = region.region_encoded
 
         rq.mutation.row = delete.rowkey
 
-        # cfs
+        # add specifications if there is any.
         for cf, cells in delete.family_cells.items():
             col = MutationProto.ColumnValue(family=cf)
 
             # add any qualifier if provided.
             for cell in cells:
                 # delete all columns in the family smaller than the provided timestamp.
                 if cell.type == CellType.DELETE_FAMILY:
@@ -128,15 +128,15 @@
         rq.number_of_rows = scan.limit
         rq.renew = True
         for family, qfs in scan.family_map.items():
             rq.scan.column.append(Column(family=family))
         resp: ScanResponse = self.send_request(rq, 'Scan')
         scanner_id = resp.scanner_id
         # build an iterator to let client iterate through the result set.
-        return ScanResultIterator(scanner_id, scan, self)
+        return iter(ScanResultIterator(scanner_id, scan, self))
 
 
 class ScanResultIterator:
     def __init__(self, scanner_id: int, scan: Scan, rs_conn: RsConnection):
         self.scanner_id = scanner_id
         self.rs_conn = rs_conn
         self.scan = scan
@@ -146,8 +146,13 @@
         rq2.scanner_id = self.scanner_id
         rq2.number_of_rows = self.scan.limit
         resp2: ScanResponse = self.rs_conn.send_request(rq2, "Scan")
         rows = []
         for result in resp2.results:
             row = Row.from_result(result)
             rows.append(row)
+        if len(rows) == 0:
+            raise StopIteration
         return rows
+
+    def __iter__(self):
+        return self
```

### Comparing `hbase-driver-0.0.9/src/hbasedriver/util/varint.py` & `hbase-driver-1.0.0/src/hbasedriver/util/varint.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/src/hbasedriver/zk.py` & `hbase-driver-1.0.0/src/hbasedriver/zk.py`

 * *Files identical despite different names*

### Comparing `hbase-driver-0.0.9/test/test_client.py` & `hbase-driver-1.0.0/test/test_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,39 @@
 import random
 
+import pytest
+
 from hbasedriver.client.client import Client
+from hbasedriver.exceptions.RemoteException import TableExistsException
+from hbasedriver.operations import Scan
+from hbasedriver.operations.column_family_builder import ColumnFamilyDescriptorBuilder
 from hbasedriver.operations.delete import Delete
 from hbasedriver.operations.get import Get
 from hbasedriver.operations.put import Put
 
 
-def test_put():
+@pytest.fixture
+def table():
     client = Client(["127.0.0.1"])
-    table = client.get_table("", "test_table")
+
+    # Define column families
+    cf1_builder = ColumnFamilyDescriptorBuilder(b"cf1")
+    cf1_descriptor = cf1_builder.build()
+    cf2_builder = ColumnFamilyDescriptorBuilder(b"cf2")
+    cf2_descriptor = cf2_builder.build()
+    column_families = [cf1_descriptor, cf2_descriptor]
+    try:
+        client.create_table(b"", b"test_table", column_families)
+    except TableExistsException:
+        pass
+
+    return client.get_table(None, "test_table")
+
+
+def test_put(table):
     resp = table.put(Put(b"row1").add_column(b'cf1', b'qf1', b'123123'))
 
     print(resp)
 
 
 def test_get():
     client = Client(["127.0.0.1"])
@@ -59,7 +80,27 @@
     assert res.get(b"cf1", b"qf1") == b"123123"
 
     processed = table.delete(Delete(rowkey).add_family_version(b'cf1', ts=ts))
     assert processed
 
     res_after_delete = table.get(Get(rowkey).add_family(b"cf1"))
     assert res_after_delete is None
+
+
+def test_delete_whole_row(table):
+    rowkey = b"rowx889577"
+
+    table.put(Put(rowkey).add_column(b"cf1", b'qf1', b'666'))
+    table.put(Put(rowkey).add_column(b"cf1", b'qf2', b'777'))
+    resp = table.put(Put(rowkey).add_column(b"cf1", b'qf3', b'888'))
+    resp = table.put(Put(rowkey).add_column(b"cf2", b'qf3', b'888'))
+    resp = table.put(Put(rowkey).add_column(b"cf2", b'qf4', b'888'))
+    assert resp
+
+    res = table.get(Get(rowkey).add_family(b"cf1"))
+    assert res.get(b"cf1", b"qf1") == b"666"
+
+    processed = table.delete(Delete(rowkey))
+    assert processed
+
+    res_after_delete = table.get(Get(rowkey).add_family(b"cf1").add_family(b"cf2"))
+    assert res_after_delete is None
```

### Comparing `hbase-driver-0.0.9/test/test_scan.py` & `hbase-driver-1.0.0/test/test_scan.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     table.put(Put(b'scan_row_key2').add_column(b'cf1', b'qf1', b'666').add_column(b'cf2', b'qf16', b'6666').add_column(
         b'cf2', b'qf17777', b'666'))
     table.put(Put(b'scan_row_key3').add_column(b'cf1', b'qf1', b'666').add_column(b'cf2', b'qf16', b'6666').add_column(
         b'cf2', b'qf17777', b'666'))
     resp = table.scan(Scan(b"scan_row_key1").add_family(b'cf1').add_family(b'cf2'))
 
     print(resp)
-    res = next(resp)
-    print(res)
+    for row in resp:
+        print(row)
```

