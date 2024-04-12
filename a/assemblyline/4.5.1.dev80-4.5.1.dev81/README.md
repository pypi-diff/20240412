# Comparing `tmp/assemblyline-4.5.1.dev80.tar.gz` & `tmp/assemblyline-4.5.1.dev81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-4.5.1.dev80.tar", last modified: Fri Apr 12 20:13:51 2024, max compression
+gzip compressed data, was "assemblyline-4.5.1.dev81.tar", last modified: Fri Apr 12 20:47:06 2024, max compression
```

## Comparing `assemblyline-4.5.1.dev80.tar` & `assemblyline-4.5.1.dev81.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (127)       47 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2531 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.789550 assemblyline-4.5.1.dev80/assemblyline/
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-12 20:13:47.000000 assemblyline-4.5.1.dev80/assemblyline/VERSION
--rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.789550 assemblyline-4.5.1.dev80/assemblyline/cachestore/
--rw-r--r--   0 vsts      (1001) docker     (127)     3463 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/cachestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.797550 assemblyline-4.5.1.dev80/assemblyline/common/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7321 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/archiving.py
--rw-r--r--   0 vsts      (1001) docker     (127)  2243670 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/attack_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13368 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/backupmanager.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2369 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/banner.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16341 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/bundling.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5668 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/caching.py
--rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/chunk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41768 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/classification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/classification.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     5811 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/cleanup_filestore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/codec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5031 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2587 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5841 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/custom.magic
--rw-r--r--   0 vsts      (1001) docker     (127)    39467 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/custom.yara
--rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/dict_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2550 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/digests.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2713 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/entropy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1903 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      584 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9003 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/forge.py
--rw-r--r--   0 vsts      (1001) docker     (127)   289190 2024-04-12 20:13:51.000000 assemblyline-4.5.1.dev80/assemblyline/common/frequency.c
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/frequency.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)     6450 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/heuristics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/hexdump.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23161 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/identify.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19801 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/identify_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/importing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4229 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/iprange.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5281 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/isotime.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4310 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/logformat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/lucene.lark
--rw-r--r--   0 vsts      (1001) docker     (127)     1105 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/memory_zip.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5230 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/net.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21606 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/net_static.py
--rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/null.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1515 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/path.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28598 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/random_user.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3379 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/security.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/common/signaturing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7396 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/str_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12687 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/tag_safelist.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     3904 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1052 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/threading.py
--rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/uid.py
--rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/common/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.797550 assemblyline-4.5.1.dev80/assemblyline/datasource/
--rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/datasource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2183 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/datasource/al.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1462 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/datasource/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/datasource/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.797550 assemblyline-4.5.1.dev80/assemblyline/datastore/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/bulk.py
--rw-r--r--   0 vsts      (1001) docker     (127)    88839 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    64390 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/store.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.797550 assemblyline-4.5.1.dev80/assemblyline/datastore/support/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/support/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9424 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/support/build.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/datastore/support/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.797550 assemblyline-4.5.1.dev80/assemblyline/filestore/
--rw-r--r--   0 vsts      (1001) docker     (127)    10460 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.797550 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7891 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/azure.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9648 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/http.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5429 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/local.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6828 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/s3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6558 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/filestore/transport/sftp.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.797550 assemblyline-4.5.1.dev80/assemblyline/odm/
--rw-r--r--   0 vsts      (1001) docker     (127)     1854 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    54612 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/odm/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.801550 assemblyline-4.5.1.dev80/assemblyline/odm/messages/
--rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1505 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/alerter_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1532 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/archive_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/changes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2476 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/dispatcher_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1299 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/dispatching.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1546 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/expiry_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/ingest_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1440 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/retrohunt_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/scaler_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/scaler_status_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1787 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/service_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1275 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/service_timing_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/shard_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2190 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/submission.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4109 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/task.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1116 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/messages/vacuum_heartbeat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.801550 assemblyline-4.5.1.dev80/assemblyline/odm/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3071 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/actions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14239 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3932 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/badlist.py
--rw-r--r--   0 vsts      (1001) docker     (127)      281 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/cached_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)    74970 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/emptyresult.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/error.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5057 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/filescore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/heuristic.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.801550 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/
--rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.801550 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/filetypes/
--rw-r--r--   0 vsts      (1001) docker     (127)       61 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/filetypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24751 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/filetypes/pe.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/ontology.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1843 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/antivirus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13798 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/malware_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/network.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/process.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2507 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/sandbox.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2961 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/signature.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3635 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9421 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2683 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/retrohunt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3098 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/service.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8157 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/service_delta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/signature.py
--rw-r--r--   0 vsts      (1001) docker     (127)      695 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/statistics.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8791 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/submission.py
--rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/submission_summary.py
--rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/submission_tree.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36489 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10462 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/user.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/user_favorites.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/user_settings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1895 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/models/workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/assemblyline/odm/random_data/
--rw-r--r--   0 vsts      (1001) docker     (127)    17983 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/random_data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2956 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/random_data/create_test_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25241 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/odm/random_data/sample_rules.yar
--rw-r--r--   0 vsts      (1001) docker     (127)     9244 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/odm/random_data/sample_suricata.rules
--rw-r--r--   0 vsts      (1001) docker     (127)    14862 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/odm/randomizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/assemblyline/remote/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/remote/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/
--rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/counters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7000 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/exporting_counter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6018 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/hash.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1442 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/lock.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1793 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/comms.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/multi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2871 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/named.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7394 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/priority.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2902 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/set.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/user_quota_tracker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/assemblyline/run/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/run/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53139 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/assemblyline/run/cli.py
--rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/run/pubsub_reader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3760 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/run/suricata_importer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4791 2024-04-12 20:13:30.000000 assemblyline-4.5.1.dev80/assemblyline/run/yara_importer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:13:51.789550 assemblyline-4.5.1.dev80/assemblyline.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2531 2024-04-12 20:13:51.000000 assemblyline-4.5.1.dev80/assemblyline.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-04-12 20:13:51.000000 assemblyline-4.5.1.dev80/assemblyline.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 20:13:51.000000 assemblyline-4.5.1.dev80/assemblyline.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-12 20:13:51.000000 assemblyline-4.5.1.dev80/assemblyline.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-12 20:13:51.000000 assemblyline-4.5.1.dev80/assemblyline.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-12 20:13:51.805550 assemblyline-4.5.1.dev80/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-12 20:13:31.000000 assemblyline-4.5.1.dev80/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.262926 assemblyline-4.5.1.dev81/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       47 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2531 2024-04-12 20:47:06.262926 assemblyline-4.5.1.dev81/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1562 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.226925 assemblyline-4.5.1.dev81/assemblyline/
+-rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-12 20:47:02.000000 assemblyline-4.5.1.dev81/assemblyline/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.226925 assemblyline-4.5.1.dev81/assemblyline/cachestore/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3463 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/cachestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.234926 assemblyline-4.5.1.dev81/assemblyline/common/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7321 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/archiving.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  2243670 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/attack_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13368 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/backupmanager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2369 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/banner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16341 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/bundling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5668 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/caching.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      903 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/chunk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41768 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/classification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4950 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/classification.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     5811 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/cleanup_filestore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2132 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5031 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2587 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5841 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/custom.magic
+-rw-r--r--   0 vsts      (1001) docker     (127)    39467 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/custom.yara
+-rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/dict_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2550 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/digests.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2713 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/entropy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1903 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      584 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9003 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/forge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   289190 2024-04-12 20:47:06.000000 assemblyline-4.5.1.dev81/assemblyline/common/frequency.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/frequency.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)     6450 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/heuristics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1398 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/hexdump.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23161 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19801 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/identify_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      413 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/importing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4229 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/iprange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5281 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/isotime.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4764 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      909 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/logformat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/lucene.lark
+-rw-r--r--   0 vsts      (1001) docker     (127)     1105 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/memory_zip.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5230 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/net.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21606 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/net_static.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      231 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/null.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1515 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28598 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4971 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/random_user.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3379 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/security.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/common/signaturing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7396 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/str_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12687 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/tag_safelist.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3904 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1052 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/threading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       57 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/common/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.234926 assemblyline-4.5.1.dev81/assemblyline/datasource/
+-rw-r--r--   0 vsts      (1001) docker     (127)      433 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/datasource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2183 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/datasource/al.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1462 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/datasource/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/datasource/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.242926 assemblyline-4.5.1.dev81/assemblyline/datastore/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/bulk.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    89006 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      572 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    64390 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15722 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/store.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.242926 assemblyline-4.5.1.dev81/assemblyline/datastore/support/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/support/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9424 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/support/build.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4531 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/datastore/support/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.242926 assemblyline-4.5.1.dev81/assemblyline/filestore/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10460 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.246926 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7891 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/azure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9648 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3752 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/http.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5429 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/local.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6828 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/s3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6558 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/filestore/transport/sftp.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.246926 assemblyline-4.5.1.dev81/assemblyline/odm/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1854 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    54964 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/odm/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.250926 assemblyline-4.5.1.dev81/assemblyline/odm/messages/
+-rw-r--r--   0 vsts      (1001) docker     (127)       75 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      596 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1505 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/alerter_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1532 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/archive_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/changes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2476 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/dispatcher_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1299 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/dispatching.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1546 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/expiry_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/ingest_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1440 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/retrohunt_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/scaler_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1403 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/scaler_status_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1787 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/service_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1275 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/service_timing_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/shard_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2190 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4109 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/task.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1116 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/messages/vacuum_heartbeat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.254926 assemblyline-4.5.1.dev81/assemblyline/odm/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3071 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14239 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3932 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/badlist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      281 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/cached_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75768 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/emptyresult.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5057 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      683 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/filescore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/heuristic.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.254926 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/
+-rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.254926 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/filetypes/
+-rw-r--r--   0 vsts      (1001) docker     (127)       61 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/filetypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24751 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/filetypes/pe.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/ontology.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.258926 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1843 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/antivirus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13798 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/malware_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3838 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/process.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2507 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/sandbox.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2961 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3635 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9421 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2683 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/retrohunt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3098 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/service.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8157 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/service_delta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      695 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/statistics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8791 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/submission_summary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      638 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/submission_tree.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36489 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10462 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/user.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/user_favorites.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2508 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/user_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1895 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/models/workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.258926 assemblyline-4.5.1.dev81/assemblyline/odm/random_data/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17983 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/random_data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2956 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/random_data/create_test_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25241 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/odm/random_data/sample_rules.yar
+-rw-r--r--   0 vsts      (1001) docker     (127)     9244 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/odm/random_data/sample_suricata.rules
+-rw-r--r--   0 vsts      (1001) docker     (127)    14862 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/odm/randomizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.258926 assemblyline-4.5.1.dev81/assemblyline/remote/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/remote/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.262926 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1661 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1984 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/counters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4112 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7000 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/exporting_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6018 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/hash.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1442 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/lock.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.262926 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1793 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/multi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2871 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/named.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7394 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/priority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2902 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/set.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/user_quota_tracker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.262926 assemblyline-4.5.1.dev81/assemblyline/run/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/run/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    52713 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/assemblyline/run/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/run/pubsub_reader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3760 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/run/suricata_importer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4791 2024-04-12 20:46:49.000000 assemblyline-4.5.1.dev81/assemblyline/run/yara_importer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 20:47:06.226925 assemblyline-4.5.1.dev81/assemblyline.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2531 2024-04-12 20:47:06.000000 assemblyline-4.5.1.dev81/assemblyline.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-04-12 20:47:06.000000 assemblyline-4.5.1.dev81/assemblyline.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 20:47:06.000000 assemblyline-4.5.1.dev81/assemblyline.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      512 2024-04-12 20:47:06.000000 assemblyline-4.5.1.dev81/assemblyline.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-12 20:47:06.000000 assemblyline-4.5.1.dev81/assemblyline.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-12 20:47:06.262926 assemblyline-4.5.1.dev81/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3845 2024-04-12 20:46:50.000000 assemblyline-4.5.1.dev81/setup.py
```

### Comparing `assemblyline-4.5.1.dev80/LICENCE.md` & `assemblyline-4.5.1.dev81/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/PKG-INFO` & `assemblyline-4.5.1.dev81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.5.1.dev80
+Version: 4.5.1.dev81
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-4.5.1.dev80/README.md` & `assemblyline-4.5.1.dev81/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/cachestore/__init__.py` & `assemblyline-4.5.1.dev81/assemblyline/cachestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/archiving.py` & `assemblyline-4.5.1.dev81/assemblyline/common/archiving.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/attack_map.py` & `assemblyline-4.5.1.dev81/assemblyline/common/attack_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/backupmanager.py` & `assemblyline-4.5.1.dev81/assemblyline/common/backupmanager.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/banner.py` & `assemblyline-4.5.1.dev81/assemblyline/common/banner.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/bundling.py` & `assemblyline-4.5.1.dev81/assemblyline/common/bundling.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/caching.py` & `assemblyline-4.5.1.dev81/assemblyline/common/caching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/chunk.py` & `assemblyline-4.5.1.dev81/assemblyline/common/chunk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/classification.py` & `assemblyline-4.5.1.dev81/assemblyline/common/classification.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/classification.yml` & `assemblyline-4.5.1.dev81/assemblyline/common/classification.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/cleanup_filestore.py` & `assemblyline-4.5.1.dev81/assemblyline/common/cleanup_filestore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/codec.py` & `assemblyline-4.5.1.dev81/assemblyline/common/codec.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/comms.py` & `assemblyline-4.5.1.dev81/assemblyline/common/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/constants.py` & `assemblyline-4.5.1.dev81/assemblyline/common/constants.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/custom.magic` & `assemblyline-4.5.1.dev81/assemblyline/common/custom.magic`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/custom.yara` & `assemblyline-4.5.1.dev81/assemblyline/common/custom.yara`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/dict_utils.py` & `assemblyline-4.5.1.dev81/assemblyline/common/dict_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/digests.py` & `assemblyline-4.5.1.dev81/assemblyline/common/digests.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/entropy.py` & `assemblyline-4.5.1.dev81/assemblyline/common/entropy.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/exceptions.py` & `assemblyline-4.5.1.dev81/assemblyline/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/file.py` & `assemblyline-4.5.1.dev81/assemblyline/common/file.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/forge.py` & `assemblyline-4.5.1.dev81/assemblyline/common/forge.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/frequency.c` & `assemblyline-4.5.1.dev81/assemblyline/common/frequency.c`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/frequency.pyx` & `assemblyline-4.5.1.dev81/assemblyline/common/frequency.pyx`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/heuristics.py` & `assemblyline-4.5.1.dev81/assemblyline/common/heuristics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/hexdump.py` & `assemblyline-4.5.1.dev81/assemblyline/common/hexdump.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/identify.py` & `assemblyline-4.5.1.dev81/assemblyline/common/identify.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/identify_defaults.py` & `assemblyline-4.5.1.dev81/assemblyline/common/identify_defaults.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/iprange.py` & `assemblyline-4.5.1.dev81/assemblyline/common/iprange.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/isotime.py` & `assemblyline-4.5.1.dev81/assemblyline/common/isotime.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/log.py` & `assemblyline-4.5.1.dev81/assemblyline/common/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,36 @@
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
     "DISABLED": 60
 }
 
 
+class PrintLogger(object):
+    @staticmethod
+    def info(msg, end=None):
+        print(msg, end=end)
+
+    @staticmethod
+    def warning(msg, end=None):
+        print(f"[W] {msg}", end=end)
+
+    @staticmethod
+    def warn(msg, end=None):
+        print(f"[W] {msg}", end=end)
+
+    @staticmethod
+    def error(msg, end=None):
+        print(f"[E] {msg}", end=end)
+
+    @staticmethod
+    def exception(msg, end=None):
+        print(f"[EX] {msg}", end=end)
+
+
 class JsonFormatter(logging.Formatter):
     def formatMessage(self, record):
         if record.exc_info:
             record.exc_text = self.formatException(record.exc_info)
             record.exc_info = None
 
         if record.exc_text:
```

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/logformat.py` & `assemblyline-4.5.1.dev81/assemblyline/common/logformat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/lucene.lark` & `assemblyline-4.5.1.dev81/assemblyline/common/lucene.lark`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/memory_zip.py` & `assemblyline-4.5.1.dev81/assemblyline/common/memory_zip.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/metrics.py` & `assemblyline-4.5.1.dev81/assemblyline/common/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/net.py` & `assemblyline-4.5.1.dev81/assemblyline/common/net.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/net_static.py` & `assemblyline-4.5.1.dev81/assemblyline/common/net_static.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/path.py` & `assemblyline-4.5.1.dev81/assemblyline/common/path.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/postprocess.py` & `assemblyline-4.5.1.dev81/assemblyline/common/postprocess.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/random_user.py` & `assemblyline-4.5.1.dev81/assemblyline/common/random_user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/security.py` & `assemblyline-4.5.1.dev81/assemblyline/common/security.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/signaturing.py` & `assemblyline-4.5.1.dev81/assemblyline/common/signaturing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/str_utils.py` & `assemblyline-4.5.1.dev81/assemblyline/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/tag_safelist.yml` & `assemblyline-4.5.1.dev81/assemblyline/common/tag_safelist.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/tagging.py` & `assemblyline-4.5.1.dev81/assemblyline/common/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/threading.py` & `assemblyline-4.5.1.dev81/assemblyline/common/threading.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/common/uid.py` & `assemblyline-4.5.1.dev81/assemblyline/common/uid.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datasource/al.py` & `assemblyline-4.5.1.dev81/assemblyline/datasource/al.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datasource/alert.py` & `assemblyline-4.5.1.dev81/assemblyline/datasource/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datasource/common.py` & `assemblyline-4.5.1.dev81/assemblyline/datasource/common.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datastore/bulk.py` & `assemblyline-4.5.1.dev81/assemblyline/datastore/bulk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datastore/collection.py` & `assemblyline-4.5.1.dev81/assemblyline/datastore/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1923,15 +1923,15 @@
     @staticmethod
     def _get_odm_type(ds_type: str):
         try:
             return back_mapping[ds_type].__name__.lower()
         except KeyError:
             return ds_type.lower()
 
-    def fields(self) -> dict[str, dict[str, Any]]:
+    def fields(self, include_description=False) -> dict[str, dict[str, Any]]:
         """
         This function should return all the fields in the index with their types
 
         :return:
         """
 
         def flatten_fields(props):
@@ -1968,14 +1968,16 @@
             collection_data[p_name] = {
                 "default": self.DEFAULT_SEARCH_FIELD in p_val.get('copy_to', []),
                 "indexed": p_val.get('index', p_val.get('enabled', True)),
                 "list": field_model.multivalued if field_model else False,
                 "stored": field_model.store if field_model else False,
                 "type": f_type
             }
+            if include_description:
+                collection_data[p_name]['description'] = field_model.description if field_model else ''
 
         return collection_data
 
     def _get_index_settings(self, archive=False) -> dict:
         default_stub: dict = deepcopy(default_index)
         settings: dict = default_stub.pop('settings', {})
```

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datastore/exceptions.py` & `assemblyline-4.5.1.dev81/assemblyline/datastore/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datastore/helper.py` & `assemblyline-4.5.1.dev81/assemblyline/datastore/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datastore/store.py` & `assemblyline-4.5.1.dev81/assemblyline/datastore/store.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datastore/support/build.py` & `assemblyline-4.5.1.dev81/assemblyline/datastore/support/build.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/datastore/support/schemas.py` & `assemblyline-4.5.1.dev81/assemblyline/datastore/support/schemas.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/__init__.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/transport/azure.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/transport/azure.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/transport/base.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/transport/base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/transport/ftp.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/transport/ftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/transport/http.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/transport/http.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/transport/local.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/transport/local.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/transport/s3.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/transport/s3.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/filestore/transport/sftp.py` & `assemblyline-4.5.1.dev81/assemblyline/filestore/transport/sftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/__init__.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/base.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1089,53 +1089,57 @@
         if skip_mappings:
             cls._odm_field_cache_skip = out
         else:
             cls._odm_field_cache = out
         return out
 
     @staticmethod
-    def _recurse_fields(name, field, show_compound, skip_mappings, multivalued=False, optional=False):
+    def _recurse_fields(name, field, show_compound, skip_mappings, multivalued=False, optional=False, description=None):
         out = dict()
 
         # Optionals and Lists do not need to be parsed, we can just analyse their inner type
         if isinstance(field, (Optional, List)):
             out.update(Model._recurse_fields(name, field.child_type, show_compound, skip_mappings,
                                              multivalued=multivalued or isinstance(field, List),
-                                             optional=optional or isinstance(field, Optional)))
+                                             optional=optional or isinstance(field, Optional),
+                                             description=field.description or description))
             return out
 
         # If field is a Compound and were asked to show it, add it to the field list
         if show_compound and isinstance(field, Compound):
             # Set the multivalued and optional flag on the field
             field.multivalued = multivalued
             field.optional = optional
+            field.description = field.description or description
 
             # Compound when showed will absorb multivalue and optional flag
             multivalued = False
             optional = False
 
             out[name] = field
 
         for sub_name, sub_field in field.fields().items():
             # Set the multivalued and optional flag on the field
             sub_field.multivalued = multivalued
             sub_field.optional = optional
+            sub_field.description = sub_field.description or description
 
             # Make sure the Compound name is propagated as the parent_name
             if isinstance(field, Compound):
                 sub_field.parent_name = name
 
             if skip_mappings and isinstance(sub_field, Mapping):
                 continue
 
             elif isinstance(sub_field, (List, Optional, Compound)) and sub_name != "":
                 out.update(Model._recurse_fields(".".join([name, sub_name]), sub_field.child_type,
                                                  show_compound, skip_mappings,
                                                  multivalued=multivalued or isinstance(sub_field, List),
-                                                 optional=optional or isinstance(sub_field, Optional)))
+                                                 optional=optional or isinstance(sub_field, Optional),
+                                                 description=sub_field.description or field.description))
 
             elif sub_name:
                 out[".".join([name, sub_name])] = sub_field
 
             else:
                 out[name] = sub_field
```

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/alert.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/alerter_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/alerter_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/archive_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/archive_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/changes.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/changes.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/dispatcher_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/dispatcher_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/dispatching.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/dispatching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/expiry_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/expiry_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/ingest_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/ingest_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/metrics.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/retrohunt_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/retrohunt_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/scaler_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/scaler_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/scaler_status_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/scaler_status_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/service_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/service_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/service_timing_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/service_timing_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/shard_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/shard_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/submission.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/task.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/task.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/messages/vacuum_heartbeat.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/messages/vacuum_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/actions.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/actions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/alert.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/badlist.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/badlist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/config.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1098,33 +1098,49 @@
     model_name: str = odm.Keyword(description="Name of the model to be used for the AI analysis.")
     verify: bool = odm.Boolean(description="Should the SSL connection to the AI API be verified.")
     proxies: Dict[str, str] = odm.Optional(odm.Mapping(odm.Keyword()),
                                            description="Proxies used by the _call_ai_backend method")
 
 
 DEFAULT_AI_ASSISTANT = {
-    'system_message': """
-You are the Assemblyline AI Assistant, you are here to help users understand the results produced by Assemblyline.
+    'system_message': """## Task And Context
+
+You are the Assemblyline AI Assistant. You help people answer their questions and other requests interactively
+regarding Assemblyline. Please answer using only the information provided to you in the prompt. If there is not
+enough information in the prompt to answer the user's question, please say so. Please do NOT use any information
+you know about Assemblyline unless it is provided to you.
+
+## Style Guide
+
+- Your answer must be written in plain $(LANG).
 """,
     'max_tokens': 1024,
     'options': {
         "frequency_penalty": 0,
         "presence_penalty": 0,
         "temperature": 0,
         "top_p": 0
     }
 }
 
 
 DEFAULT_AI_CODE = {
-    'system_message': """
+    'system_message': """## Task And Context
+
 You are an assistant that provides explanation of code snippets found in AssemblyLine,
 a malware detection and analysis tool. Start by providing a short summary of the intent behind the
-code and then follow with a detailed explanation of what the code is doing. Format your explanation
-using the Markdown syntax. Your answer must be written in plain $(LANG).
+code and then follow with a detailed explanation of what the code is doing.
+
+## Style Guide
+
+- Your output must be formatted in standard Markdown syntax
+- Highlight important information using backticks
+- Your answer must be written in plain $(LANG).
+
+## Exemple output
 
 User: print("Hello World!")
 Assistant:
 ## Summary
 The given code is printing "Hello World!" to the console.
 ## Details
 The code has only one line of code and prints a string to the console using the print() function.
@@ -1135,44 +1151,62 @@
         "presence_penalty": 0,
         "temperature": 0,
         "top_p": 0
     }
 }
 
 DEFAULT_AI_DETAILED_REPORT = {
-    'system_message': """
-You are an assistant that summarizes the output of AssemblyLine, a malware detection and analysis tool.  Your role is
-to extract information of importance and discard what is not. Assemblyline uses a scoring mechanism where any scores
-below 0 is considered safe, scores between 0 and 300 are considered informational, scores between 300 and 700 are
-considered suspicious, scores between 700 and 1000 are considered highly-suspicious and scores with 1000 points and
-up are considered malicious.
-
-Once YAML has been submitted, the user expects a two-part result in plain $(LANG)..  The first part is a one or two
-paragraph executive summary which provides some highlights of the results, and the second part is a detailed description
-of the observations found in the report.  Format your answer using the Markdown syntax.
+    'system_message': """## Task And Context
+
+You are an assistant that summarizes the output of AssemblyLine, a malware detection and analysis tool. Your role is
+to extract information of importance and discard what is not. Once a YAML Assemblyline report is submitted to you, the
+user expects a two-part result.
+
+The first part is a one or two paragraph executive summary which provides some highlights of the results, and the
+second part is a detailed description of the observations found in the report.
+
+## Assemblyline scoring definition
+
+Assemblyline uses a scoring mechanism where any scores below 0 is considered safe, scores between 0 and 300 are
+considered informational, scores between 300 and 700 are considered suspicious, scores between 700 and 1000 are
+considered highly-suspicious and scores with 1000 points and up are considered malicious.
+
+## Style Guide
+
+- Your output must be formatted in standard Markdown syntax
+- Highlight important information using backticks
+- Your answer must be written in plain $(LANG).
 """,
     'max_tokens': 2048,
     'options': {
         "frequency_penalty": 0,
         "presence_penalty": 0,
         "temperature": 0,
         "top_p": 0
     }
 }
 
 DEFAULT_AI_EXECUTIVE_SUMMARY = {
-    "system_message": """
+    "system_message": """## Task And Context
+
 You are an assistant that summarizes the output of AssemblyLine, a malware detection and analysis tool. Your role
-is to extract information of importance and discard what is not.  Assemblyline uses a scoring mechanism where any scores
-below 0 is considered safe, scores between 0 and 300 are considered informational, scores between 300 and 700 are
-considered suspicious, scores between 700 and 1000 are considered highly-suspicious and scores with 1000 points and up
-are considered malicious.
+is to extract information of importance and discard what is not. Once YAML has been submitted, the user expects a one
+or two paragraph executive summary of the output of AssemblyLine.
+
+## Assemblyline scoring definition
+
+Assemblyline uses a scoring mechanism where any scores below 0 is considered safe, scores between 0 and 300 are
+considered informational, scores between 300 and 700 are considered suspicious, scores between 700 and 1000 are
+considered highly-suspicious and scores with 1000 points and up are considered malicious.
+
+## Style Guide
 
-Once YAML has been submitted, the user expects a one or two paragraph executive summary of the output of AssemblyLine in
-plain $(LANG)..  Highlight important information using inline code block from the Markdown syntax.
+- Your output must be formatted in standard Markdown syntax
+- Highlight important information using backticks
+- Your answer must be written in plain $(LANG).
 """,
     'max_tokens': 512,
     'options': {
         "frequency_penalty": 0,
         "presence_penalty": 0,
         "temperature": 0,
         "top_p": 0
```

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/error.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/error.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/file.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/file.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/filescore.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/filescore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/heuristic.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/heuristic.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/filetypes/pe.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/filetypes/pe.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/ontology.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/antivirus.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/antivirus.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/malware_config.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/malware_config.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/network.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/network.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/process.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/process.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/sandbox.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/sandbox.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/ontology/results/signature.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/ontology/results/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/replay.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/result.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/result.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/retrohunt.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/retrohunt.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/safelist.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/service.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/service.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/service_delta.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/service_delta.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/signature.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/statistics.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/statistics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/submission.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/submission_summary.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/submission_summary.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/submission_tree.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/submission_tree.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/tagging.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/user.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/user_favorites.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/user_favorites.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/user_settings.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/models/workflow.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/models/workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/random_data/__init__.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/random_data/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/random_data/create_test_data.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/random_data/create_test_data.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/random_data/sample_rules.yar` & `assemblyline-4.5.1.dev81/assemblyline/odm/random_data/sample_rules.yar`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/random_data/sample_suricata.rules` & `assemblyline-4.5.1.dev81/assemblyline/odm/random_data/sample_suricata.rules`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/odm/randomizer.py` & `assemblyline-4.5.1.dev81/assemblyline/odm/randomizer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/__init__.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/cache.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/cache.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/counters.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/counters.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/events.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/events.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/exporting_counter.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/exporting_counter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/hash.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/hash.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/lock.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/lock.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/comms.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/multi.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/multi.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/named.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/named.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/queues/priority.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/queues/priority.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/set.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/set.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/remote/datatypes/user_quota_tracker.py` & `assemblyline-4.5.1.dev81/assemblyline/remote/datatypes/user_quota_tracker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/run/cli.py` & `assemblyline-4.5.1.dev81/assemblyline/run/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,52 +83,30 @@
         print(f"    [E] {msg}", end=end)
 
     @staticmethod
     def exception(msg, end=None):
         print(f"    [EX] {msg}", end=end)
 
 
-class PrintLogger(object):
-    @staticmethod
-    def info(msg, end=None):
-        print(msg, end=end)
-
-    @staticmethod
-    def warning(msg, end=None):
-        print(f"[W] {msg}", end=end)
-
-    @staticmethod
-    def warn(msg, end=None):
-        print(f"[W] {msg}", end=end)
-
-    @staticmethod
-    def error(msg, end=None):
-        print(f"[E] {msg}", end=end)
-
-    @staticmethod
-    def exception(msg, end=None):
-        print(f"[EX] {msg}", end=end)
-
-
 def init():
     global DATASTORE
     DATASTORE = forge.get_datastore(archive_access=True)
     signal.signal(signal.SIGINT, signal.SIG_IGN)
 
 
 def submission_delete_tree(key, logger):
     try:
         with forge.get_filestore() as f_transport:
             # noinspection PyUnresolvedReferences
             DATASTORE.delete_submission_tree_bulk(key, transport=f_transport)
     except Exception as e:
         logger.error(e)
-        return "DELETE", "submission", key, False, isinstance(logger, PrintLogger)
+        return "DELETE", "submission", key, False, isinstance(logger, al_log.PrintLogger)
 
-    return "deleted", "submission", key, True, isinstance(logger, PrintLogger)
+    return "deleted", "submission", key, True, isinstance(logger, al_log.PrintLogger)
 
 
 def action_done(args):
     global t_count, t_last, COUNT_INCREMENT
     action, index, key, success, do_print = args
     if success:
         t_count += 1
@@ -141,15 +119,15 @@
     elif do_print:
         print(f"!!ERROR!! [{index}] {action} ==> {key}")
 
 
 # noinspection PyMethodMayBeStatic,PyProtectedMember,PyBroadException
 class ALCommandLineInterface(cmd.Cmd):  # pylint:disable=R0904
 
-    def __init__(self, show_prompt=True, logger_class=PrintLogger):
+    def __init__(self, show_prompt=True, logger_class=al_log.PrintLogger):
         cmd.Cmd.__init__(self)
         self.logger = logger_class()
         self.prompt = ""
         self.intro = ""
         self.datastore = forge.get_datastore(archive_access=True)
         self.config = forge.get_config()
         if show_prompt:
@@ -1020,15 +998,15 @@
                 else:
                     self.logger.info("Fixing shards on all indices...")
                     indices = valid_indices
 
                 for index in indices:
                     collection = self.datastore.get_collection(index)
                     collection.fix_shards(logger=IndentedPrintLogger()
-                                          if isinstance(self.logger, PrintLogger) else self.logger)
+                                          if isinstance(self.logger, al_log.PrintLogger) else self.logger)
                     self.logger.info(f"    Index {index.upper()} shards configuration updated.")
 
                 self.logger.info("Completed!")
             elif action_type == 'fix_ilm':
                 indices = []
                 if index:
                     self.logger.info(f"Fixing ILM on index {index.upper()}...")
```

### Comparing `assemblyline-4.5.1.dev80/assemblyline/run/pubsub_reader.py` & `assemblyline-4.5.1.dev81/assemblyline/run/pubsub_reader.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/run/suricata_importer.py` & `assemblyline-4.5.1.dev81/assemblyline/run/suricata_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline/run/yara_importer.py` & `assemblyline-4.5.1.dev81/assemblyline/run/yara_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline.egg-info/PKG-INFO` & `assemblyline-4.5.1.dev81/assemblyline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.5.1.dev80
+Version: 4.5.1.dev81
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-4.5.1.dev80/assemblyline.egg-info/SOURCES.txt` & `assemblyline-4.5.1.dev81/assemblyline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/assemblyline.egg-info/requires.txt` & `assemblyline-4.5.1.dev81/assemblyline.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-4.5.1.dev80/setup.py` & `assemblyline-4.5.1.dev81/setup.py`

 * *Files identical despite different names*

