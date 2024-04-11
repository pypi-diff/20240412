# Comparing `tmp/oakvar-2.9.93.tar.gz` & `tmp/oakvar-2.9.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakvar-2.9.93.tar", last modified: Wed Apr 10 11:36:06 2024, max compression
+gzip compressed data, was "oakvar-2.9.94.tar", last modified: Wed Apr 10 23:41:24 2024, max compression
```

## Comparing `oakvar-2.9.93.tar` & `oakvar-2.9.94.tar`

### file list

```diff
@@ -1,552 +1,553 @@
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.420200 oakvar-2.9.93/
--rw-r--r--   0 rick       (501) staff       (20)     1753 2023-12-05 15:09:56.000000 oakvar-2.9.93/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-10 11:36:06.419902 oakvar-2.9.93/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     2339 2024-04-10 11:35:38.000000 oakvar-2.9.93/README.rst
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.310659 oakvar-2.9.93/cravat/
--rw-r--r--   0 rick       (501) staff       (20)       21 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/__main__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.311491 oakvar-2.9.93/cravat/api/
--rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/config.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.312252 oakvar-2.9.93/cravat/api/module/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/module/ls_logic.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/new.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.312406 oakvar-2.9.93/cravat/api/store/
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.312523 oakvar-2.9.93/cravat/api/store/account/
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/system.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/test.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/api/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.314090 oakvar-2.9.93/cravat/cli/
--rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/config.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/gui.py
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/issue.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/license.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.314525 oakvar-2.9.93/cravat/cli/module/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/module/info_fn.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/module/ls.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/new.py
--rw-r--r--   0 rick       (501) staff       (20)      110 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/report.py
--rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/run.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.314646 oakvar-2.9.93/cravat/cli/store/
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.314759 oakvar-2.9.93/cravat/cli/store/account/
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/system.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/test.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/update.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/util.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cli/version.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/constants.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/cravat_report.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/exceptions.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.316341 oakvar-2.9.93/cravat/gui/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/consts.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/job_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/multiuser.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/server.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/serveradmindb.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/store_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/system_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/system_message_db.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/system_worker.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/userjob.py
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/util.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/web_submit.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.316683 oakvar-2.9.93/cravat/gui/webresult/
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/webresult/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       48 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/webresult/jsonreporter.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/webresult/webresult.py
--rw-r--r--   0 rick       (501) staff       (20)       44 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/gui/websocket_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/inout.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.317004 oakvar-2.9.93/cravat/lib/
--rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.304204 oakvar-2.9.93/cravat/lib/assets/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.304546 oakvar-2.9.93/cravat/lib/assets/module_templates/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.317292 oakvar-2.9.93/cravat/lib/assets/module_templates/annotator/
--rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/assets/module_templates/annotator/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.317433 oakvar-2.9.93/cravat/lib/assets/module_templates/converter/
--rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/assets/module_templates/converter/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.317682 oakvar-2.9.93/cravat/lib/assets/module_templates/mapper/
--rw-r--r--   0 rick       (501) staff       (20)       65 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/assets/module_templates/mapper/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.317963 oakvar-2.9.93/cravat/lib/assets/module_templates/postaggregator/
--rw-r--r--   0 rick       (501) staff       (20)       73 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/assets/module_templates/postaggregator/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.318096 oakvar-2.9.93/cravat/lib/assets/module_templates/preparer/
--rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/assets/module_templates/preparer/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.318228 oakvar-2.9.93/cravat/lib/assets/module_templates/reporter/
--rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/assets/module_templates/reporter/template.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.320360 oakvar-2.9.93/cravat/lib/base/
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/aggregator.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/annotator.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/app.py
--rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/commonmodule.py
--rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/converter.py
--rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/mapper.py
--rw-r--r--   0 rick       (501) staff       (20)       47 2024-01-10 14:33:05.000000 oakvar-2.9.93/cravat/lib/base/master_converter.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2024-01-10 14:33:05.000000 oakvar-2.9.93/cravat/lib/base/mp_runners.py
--rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/postaggregator.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/preparer.py
--rw-r--r--   0 rick       (501) staff       (20)       44 2024-01-10 14:33:05.000000 oakvar-2.9.93/cravat/lib/base/report_filter.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/reporter.py
--rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/runner.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/base/vcf2vcf.py
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/consts.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/exceptions.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.320898 oakvar-2.9.93/cravat/lib/module/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/module/cache.py
--rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/module/data_cache.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/module/local.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/module/remote.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.321222 oakvar-2.9.93/cravat/lib/store/
--rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/store/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/store/consts.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/store/db.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.321334 oakvar-2.9.93/cravat/lib/store/ov/
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/store/ov/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.321445 oakvar-2.9.93/cravat/lib/store/ov/account/
--rw-r--r--   0 rick       (501) staff       (20)       42 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/store/ov/account/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.321668 oakvar-2.9.93/cravat/lib/system/
--rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/system/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/system/consts.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.322988 oakvar-2.9.93/cravat/lib/util/
--rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/admin_util.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/asyn.py
--rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:35:34.000000 oakvar-2.9.93/cravat/lib/util/db.py
--rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/download.py
--rw-r--r--   0 rick       (501) staff       (20)       47 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/download_library.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/image.py
--rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/inout.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/run.py
--rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/seq.py
--rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.93/cravat/lib/util/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.323248 oakvar-2.9.93/oakvar/
--rw-r--r--   0 rick       (501) staff       (20)     6681 2024-03-03 15:20:39.000000 oakvar-2.9.93/oakvar/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     7901 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/__main__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.324766 oakvar-2.9.93/oakvar/api/
--rw-r--r--   0 rick       (501) staff       (20)    19785 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/api/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     3144 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/api/config.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.325177 oakvar-2.9.93/oakvar/api/module/
--rw-r--r--   0 rick       (501) staff       (20)    18616 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/api/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     5305 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/api/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)     5687 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/api/module/ls_logic.py
--rw-r--r--   0 rick       (501) staff       (20)     3379 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/api/new.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.325288 oakvar-2.9.93/oakvar/api/store/
--rw-r--r--   0 rick       (501) staff       (20)     7179 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/api/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.325401 oakvar-2.9.93/oakvar/api/store/account/
--rw-r--r--   0 rick       (501) staff       (20)     4130 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/api/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     4510 2023-12-23 13:35:34.000000 oakvar-2.9.93/oakvar/api/system.py
--rw-r--r--   0 rick       (501) staff       (20)    34086 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/api/test.py
--rw-r--r--   0 rick       (501) staff       (20)    18455 2024-02-23 14:56:17.000000 oakvar-2.9.93/oakvar/api/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.327310 oakvar-2.9.93/oakvar/cli/
--rw-r--r--   0 rick       (501) staff       (20)     4470 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     4949 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/config.py
--rw-r--r--   0 rick       (501) staff       (20)    10930 2023-12-23 13:35:34.000000 oakvar-2.9.93/oakvar/cli/gui.py
--rw-r--r--   0 rick       (501) staff       (20)     2297 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/issue.py
--rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/license.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.327823 oakvar-2.9.93/oakvar/cli/module/
--rw-r--r--   0 rick       (501) staff       (20)    15171 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/cli/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     6422 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/module/info_fn.py
--rw-r--r--   0 rick       (501) staff       (20)     2410 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/module/install_defs.py
--rw-r--r--   0 rick       (501) staff       (20)     7792 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/module/ls.py
--rw-r--r--   0 rick       (501) staff       (20)     4408 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/new.py
--rw-r--r--   0 rick       (501) staff       (20)     6925 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/cli/report.py
--rw-r--r--   0 rick       (501) staff       (20)    11084 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/cli/run.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.327952 oakvar-2.9.93/oakvar/cli/store/
--rw-r--r--   0 rick       (501) staff       (20)     9370 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/cli/store/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.328126 oakvar-2.9.93/oakvar/cli/store/account/
--rw-r--r--   0 rick       (501) staff       (20)     7883 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/store/account/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     6736 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/system.py
--rw-r--r--   0 rick       (501) staff       (20)     2886 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/test.py
--rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/update.py
--rw-r--r--   0 rick       (501) staff       (20)     9339 2024-02-23 14:57:11.000000 oakvar-2.9.93/oakvar/cli/util.py
--rw-r--r--   0 rick       (501) staff       (20)     2474 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/cli/version.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.329905 oakvar-2.9.93/oakvar/gui/
--rw-r--r--   0 rick       (501) staff       (20)     2958 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/consts.py
--rw-r--r--   0 rick       (501) staff       (20)    28494 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/job_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)    11215 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/multiuser.py
--rw-r--r--   0 rick       (501) staff       (20)    17290 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/server.py
--rw-r--r--   0 rick       (501) staff       (20)    25415 2024-02-23 14:55:01.000000 oakvar-2.9.93/oakvar/gui/serveradmindb.py
--rw-r--r--   0 rick       (501) staff       (20)    15866 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/store_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)     8553 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/system_handlers.py
--rw-r--r--   0 rick       (501) staff       (20)     3968 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/system_message_db.py
--rw-r--r--   0 rick       (501) staff       (20)     8117 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/system_worker.py
--rw-r--r--   0 rick       (501) staff       (20)     6042 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/userjob.py
--rw-r--r--   0 rick       (501) staff       (20)     7210 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/util.py
--rw-r--r--   0 rick       (501) staff       (20)    17662 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/web_submit.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.331103 oakvar-2.9.93/oakvar/gui/webresult/
--rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.331331 oakvar-2.9.93/oakvar/gui/webresult/css/
--rw-r--r--   0 rick       (501) staff       (20)     2389 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/css/pqselect.min.css
--rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/email.png
--rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/favicon.ico
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.333455 oakvar-2.9.93/oakvar/gui/webresult/fonts/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.356978 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/
--rw-r--r--   0 rick       (501) staff       (20)   138764 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
--rw-r--r--   0 rick       (501) staff       (20)   102868 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
--rw-r--r--   0 rick       (501) staff       (20)   146824 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   108752 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   143208 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
--rw-r--r--   0 rick       (501) staff       (20)   106140 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
--rw-r--r--   0 rick       (501) staff       (20)   151052 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111808 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   142920 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
--rw-r--r--   0 rick       (501) staff       (20)   106108 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
--rw-r--r--   0 rick       (501) staff       (20)   150628 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111708 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   140724 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
--rw-r--r--   0 rick       (501) staff       (20)   104232 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
--rw-r--r--   0 rick       (501) staff       (20)   149996 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111392 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   144372 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
--rw-r--r--   0 rick       (501) staff       (20)   106876 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   140632 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
--rw-r--r--   0 rick       (501) staff       (20)   104332 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
--rw-r--r--   0 rick       (501) staff       (20)   150092 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   111332 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   142552 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
--rw-r--r--   0 rick       (501) staff       (20)   105924 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
--rw-r--r--   0 rick       (501) staff       (20)   150988 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   112184 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   133844 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
--rw-r--r--   0 rick       (501) staff       (20)    98868 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
--rw-r--r--   0 rick       (501) staff       (20)   142932 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
--rw-r--r--   0 rick       (501) staff       (20)   105804 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
--rw-r--r--   0 rick       (501) staff       (20)   151180 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   112048 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   135920 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
--rw-r--r--   0 rick       (501) staff       (20)    99632 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
--rw-r--r--   0 rick       (501) staff       (20)   145480 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
--rw-r--r--   0 rick       (501) staff       (20)   106496 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
--rw-r--r--   0 rick       (501) staff       (20)   245036 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
--rw-r--r--   0 rick       (501) staff       (20)   227180 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
--rw-r--r--   0 rick       (501) staff       (20)   324864 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
--rw-r--r--   0 rick       (501) staff       (20)     5303 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/inter.css
--rw-r--r--   0 rick       (501) staff       (20)    26456 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    19508 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 rick       (501) staff       (20)    25692 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    18980 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
--rw-r--r--   0 rick       (501) staff       (20)    26312 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    19416 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 rick       (501) staff       (20)    33072 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
--rw-r--r--   0 rick       (501) staff       (20)    25740 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.360863 oakvar-2.9.93/oakvar/gui/webresult/images/
--rw-r--r--   0 rick       (501) staff       (20)      326 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)      379 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrow-down-right-circle.svg
--rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrow-down-right.svg
--rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrow-down.svg
--rw-r--r--   0 rick       (501) staff       (20)      311 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrow-left.svg
--rw-r--r--   0 rick       (501) staff       (20)      312 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrow-right.svg
--rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrow-up.svg
--rw-r--r--   0 rick       (501) staff       (20)      706 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/arrows-move.svg
--rw-r--r--   0 rick       (501) staff       (20)     2140 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/camera.svg
--rw-r--r--   0 rick       (501) staff       (20)      291 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/caret-down.svg
--rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/caret-right.svg
--rw-r--r--   0 rick       (501) staff       (20)     3125 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/close.png
--rw-r--r--   0 rick       (501) staff       (20)     2390 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/close.svg
--rw-r--r--   0 rick       (501) staff       (20)      722 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/download-material-black.png
--rw-r--r--   0 rick       (501) staff       (20)     2066 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/download.svg
--rw-r--r--   0 rick       (501) staff       (20)      485 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/grip-vertical.svg
--rw-r--r--   0 rick       (501) staff       (20)     2219 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/pin.svg
--rw-r--r--   0 rick       (501) staff       (20)     2243 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/plus-circle-dotted.svg
--rw-r--r--   0 rick       (501) staff       (20)      280 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/plus-circle-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)     4645 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/sorry.png
--rw-r--r--   0 rick       (501) staff       (20)    25333 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/spinner.gif
--rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/x-lg.svg
--rw-r--r--   0 rick       (501) staff       (20)      332 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/images/x.svg
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.370076 oakvar-2.9.93/oakvar/gui/webresult/js/
--rw-r--r--   0 rick       (501) staff       (20)   398184 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/Chart.js
--rw-r--r--   0 rick       (501) staff       (20)    26580 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/axios.min.js
--rw-r--r--   0 rick       (501) staff       (20)   137820 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/axios.min.js.map
--rw-r--r--   0 rick       (501) staff       (20)     9278 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/dom-to-image.min.js
--rw-r--r--   0 rick       (501) staff       (20)     5839 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/download.js
--rw-r--r--   0 rick       (501) staff       (20)    12091 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
--rw-r--r--   0 rick       (501) staff       (20)   954164 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/graphics.js
--rw-r--r--   0 rick       (501) staff       (20)    86659 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-3.2.1.min.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.376126 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
--rw-r--r--   0 rick       (501) staff       (20)    12660 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rw-r--r--   0 rick       (501) staff       (20)     1817 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.306194 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.376413 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rw-r--r--   0 rick       (501) staff       (20)   293430 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.378185 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
--rw-r--r--   0 rick       (501) staff       (20)     6992 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     6988 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     6999 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)     6299 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 rick       (501) staff       (20)    32588 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
--rw-r--r--   0 rick       (501) staff       (20)    35997 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rw-r--r--   0 rick       (501) staff       (20)   520714 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rw-r--r--   0 rick       (501) staff       (20)    30747 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rw-r--r--   0 rick       (501) staff       (20)   253668 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rw-r--r--   0 rick       (501) staff       (20)    18705 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rw-r--r--   0 rick       (501) staff       (20)    15548 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rw-r--r--   0 rick       (501) staff       (20)    17342 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rw-r--r--   0 rick       (501) staff       (20)    13847 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rw-r--r--   0 rick       (501) staff       (20)     1340 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
--rw-r--r--   0 rick       (501) staff       (20)    13171 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery.tools.min.js
--rw-r--r--   0 rick       (501) staff       (20)     5451 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/jquery.url.js
--rw-r--r--   0 rick       (501) staff       (20)    24103 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/masonry.pkgd.min.js
--rw-r--r--   0 rick       (501) staff       (20)    84772 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/packery.pkgd.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.382987 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/
--rw-r--r--   0 rick       (501) staff       (20)    11583 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
--rw-r--r--   0 rick       (501) staff       (20)   103213 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.384414 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/
--rw-r--r--   0 rick       (501) staff       (20)      230 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rw-r--r--   0 rick       (501) staff       (20)      210 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rw-r--r--   0 rick       (501) staff       (20)      771 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
--rw-r--r--   0 rick       (501) staff       (20)     1668 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
--rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rw-r--r--   0 rick       (501) staff       (20)       76 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rw-r--r--   0 rick       (501) staff       (20)      216 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
--rw-r--r--   0 rick       (501) staff       (20)      201 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.384943 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rw-r--r--   0 rick       (501) staff       (20)     1148 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rw-r--r--   0 rick       (501) staff       (20)    76985 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.387078 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/
--rw-r--r--   0 rick       (501) staff       (20)      755 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rw-r--r--   0 rick       (501) staff       (20)      750 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rw-r--r--   0 rick       (501) staff       (20)      769 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rw-r--r--   0 rick       (501) staff       (20)      802 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rw-r--r--   0 rick       (501) staff       (20)      813 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rw-r--r--   0 rick       (501) staff       (20)      805 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rw-r--r--   0 rick       (501) staff       (20)      636 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rw-r--r--   0 rick       (501) staff       (20)      774 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rw-r--r--   0 rick       (501) staff       (20)      782 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rw-r--r--   0 rick       (501) staff       (20)      822 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rw-r--r--   0 rick       (501) staff       (20)      773 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rw-r--r--   0 rick       (501) staff       (20)      675 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.388317 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
--rw-r--r--   0 rick       (501) staff       (20)     1105 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rw-r--r--   0 rick       (501) staff       (20)      613 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rw-r--r--   0 rick       (501) staff       (20)      541 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rw-r--r--   0 rick       (501) staff       (20)     2973 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rw-r--r--   0 rick       (501) staff       (20)    27759 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rw-r--r--   0 rick       (501) staff       (20)     2383 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rw-r--r--   0 rick       (501) staff       (20)    12577 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rw-r--r--   0 rick       (501) staff       (20)     2408 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rw-r--r--   0 rick       (501) staff       (20)     2026 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rw-r--r--   0 rick       (501) staff       (20)    16145 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rw-r--r--   0 rick       (501) staff       (20)   481365 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rw-r--r--   0 rick       (501) staff       (20)    12757 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
--rw-r--r--   0 rick       (501) staff       (20)   242931 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
--rw-r--r--   0 rick       (501) staff       (20)     1646 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rw-r--r--   0 rick       (501) staff       (20)     1278 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rw-r--r--   0 rick       (501) staff       (20)      555 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.307569 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.388468 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.388724 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.389113 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.389324 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.389478 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.389611 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.389739 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.389875 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.390010 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.390143 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.390298 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.390432 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.390648 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.390902 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.391095 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
--rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.392052 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
--rw-r--r--   0 rick       (501) staff       (20)     1042 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rw-r--r--   0 rick       (501) staff       (20)     1164 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rw-r--r--   0 rick       (501) staff       (20)     2677 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
--rw-r--r--   0 rick       (501) staff       (20)     3716 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rw-r--r--   0 rick       (501) staff       (20)     1847 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rw-r--r--   0 rick       (501) staff       (20)    12583 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/pqselect.min.js
--rw-r--r--   0 rick       (501) staff       (20)    92225 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/raphael-min.js
--rw-r--r--   0 rick       (501) staff       (20)   326538 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/js/tailwind.min.js
--rw-r--r--   0 rick       (501) staff       (20)     2732 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/webresult/jsonreporter.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.392657 oakvar-2.9.93/oakvar/gui/webresult/nocache/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.393131 oakvar-2.9.93/oakvar/gui/webresult/nocache/css/
--rw-r--r--   0 rick       (501) staff       (20)     1714 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/css/singlevariantpage.css
--rw-r--r--   0 rick       (501) staff       (20)    22655 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/css/style.css
--rw-r--r--   0 rick       (501) staff       (20)     2658 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/css/widget.css
--rw-r--r--   0 rick       (501) staff       (20)    21597 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/index.html
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.395925 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/
--rw-r--r--   0 rick       (501) staff       (20)    24858 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/filter.js
--rw-r--r--   0 rick       (501) staff       (20)    13105 2023-12-09 16:39:48.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/infomgr.js
--rw-r--r--   0 rick       (501) staff       (20)    30870 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/main.js
--rw-r--r--   0 rick       (501) staff       (20)   103450 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/setup.js
--rw-r--r--   0 rick       (501) staff       (20)     4903 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/showvariant.js
--rw-r--r--   0 rick       (501) staff       (20)    35998 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/singlevariantpage.js
--rw-r--r--   0 rick       (501) staff       (20)    28858 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/util.js
--rw-r--r--   0 rick       (501) staff       (20)     1696 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/variables.js
--rw-r--r--   0 rick       (501) staff       (20)    22262 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/js/widgethelper.js
--rw-r--r--   0 rick       (501) staff       (20)     5440 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/nocache/variant.html
--rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/question.png
--rw-r--r--   0 rick       (501) staff       (20)    31615 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/webresult/webresult.py
--rw-r--r--   0 rick       (501) staff       (20)      163 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webresult/webviewer.yml
--rw-r--r--   0 rick       (501) staff       (20)     5907 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websocket_handlers.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.307924 oakvar-2.9.93/oakvar/gui/webstore/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.398697 oakvar-2.9.93/oakvar/gui/webstore/images/
--rw-r--r--   0 rick       (501) staff       (20)      446 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/chat-dots-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)      740 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/chat-dots.svg
--rw-r--r--   0 rick       (501) staff       (20)      396 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/chat-left-text-fill.svg
--rw-r--r--   0 rick       (501) staff       (20)      545 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/chat-left-text.svg
--rw-r--r--   0 rick       (501) staff       (20)    22268 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/done.png
--rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/email.png
--rw-r--r--   0 rick       (501) staff       (20)     2226 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/empty.png
--rw-r--r--   0 rick       (501) staff       (20)     1763 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/folder.png
--rw-r--r--   0 rick       (501) staff       (20)    38197 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/genericmodulelogo.png
--rw-r--r--   0 rick       (501) staff       (20)     4766 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/hamburger.png
--rw-r--r--   0 rick       (501) staff       (20)     1194 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/left_arrow.png
--rw-r--r--   0 rick       (501) staff       (20)     3524 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/new.png
--rw-r--r--   0 rick       (501) staff       (20)      474 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/no_logo_module.svg
--rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/question.png
--rw-r--r--   0 rick       (501) staff       (20)     1214 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/right_arrow.png
--rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/webstore/images/x-lg.svg
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.308152 oakvar-2.9.93/oakvar/gui/websubmit/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.401036 oakvar-2.9.93/oakvar/gui/websubmit/images/
--rw-r--r--   0 rick       (501) staff       (20)   372952 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/images/background.png
--rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/images/logo.png
--rw-r--r--   0 rick       (501) staff       (20)    22716 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/images/logo_only.png
--rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/images/logo_transparent.png
--rw-r--r--   0 rick       (501) staff       (20)    22247 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/images/logo_transparent_bw.png
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.401464 oakvar-2.9.93/oakvar/gui/websubmit/inputexamples/
--rw-r--r--   0 rick       (501) staff       (20)     9036 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/inputexamples/exampleinput
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.404618 oakvar-2.9.93/oakvar/gui/websubmit/nocache/
--rw-r--r--   0 rick       (501) staff       (20)      692 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/alerts.js
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/element_constructors.js
--rw-r--r--   0 rick       (501) staff       (20)     6756 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/element_getters.js
--rw-r--r--   0 rick       (501) staff       (20)    55822 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/index.html
--rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/input.js
--rw-r--r--   0 rick       (501) staff       (20)    14408 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/jobstable.js
--rw-r--r--   0 rick       (501) staff       (20)     8242 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/login.html
--rw-r--r--   0 rick       (501) staff       (20)     3796 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/multiuser.css
--rw-r--r--   0 rick       (501) staff       (20)    16797 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/multiuser.js
--rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/select_modules.js
--rw-r--r--   0 rick       (501) staff       (20)      228 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/showhide.js
--rw-r--r--   0 rick       (501) staff       (20)     6783 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/submit.js
--rw-r--r--   0 rick       (501) staff       (20)      484 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/util.js
--rw-r--r--   0 rick       (501) staff       (20)    11319 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/websubmit.css
--rw-r--r--   0 rick       (501) staff       (20)    39200 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/gui/websubmit/nocache/websubmit.js
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.404986 oakvar-2.9.93/oakvar/gui/www/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.405360 oakvar-2.9.93/oakvar/gui/www/assets/
--rw-r--r--   0 rick       (501) staff       (20)    63287 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/www/assets/index.3526e7ae.css
--rw-r--r--   0 rick       (501) staff       (20)   834933 2023-12-09 16:39:48.000000 oakvar-2.9.93/oakvar/gui/www/assets/index.5e1d7274.js
--rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/gui/www/favicon.ico
--rw-r--r--   0 rick       (501) staff       (20)     2074 2023-12-09 16:39:48.000000 oakvar-2.9.93/oakvar/gui/www/index.html
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.407375 oakvar-2.9.93/oakvar/lib/
--rw-r--r--   0 rick       (501) staff       (20)     1946 2024-03-03 16:46:38.000000 oakvar-2.9.93/oakvar/lib/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.408707 oakvar-2.9.93/oakvar/lib/assets/
--rw-r--r--   0 rick       (501) staff       (20)     9036 2024-04-10 11:35:01.000000 oakvar-2.9.93/oakvar/lib/assets/exampleinput
--rw-r--r--   0 rick       (501) staff       (20)    16880 2024-02-08 01:06:28.000000 oakvar-2.9.93/oakvar/lib/assets/hg19.chromAlias.txt
--rw-r--r--   0 rick       (501) staff       (20)    27240 2024-02-08 00:52:40.000000 oakvar-2.9.93/oakvar/lib/assets/hg38.chromAlias.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.409130 oakvar-2.9.93/oakvar/lib/assets/license/
--rw-r--r--   0 rick       (501) staff       (20)     1707 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/license/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)     1330 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/license/liftover.txt
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.308865 oakvar-2.9.93/oakvar/lib/assets/module_templates/
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.409614 oakvar-2.9.93/oakvar/lib/assets/module_templates/annotator/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/annotator/template.md
--rw-r--r--   0 rick       (501) staff       (20)     2109 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/annotator/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1195 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/annotator/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.410032 oakvar-2.9.93/oakvar/lib/assets/module_templates/converter/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/converter/template.md
--rw-r--r--   0 rick       (501) staff       (20)     4366 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/converter/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1249 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/converter/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.410403 oakvar-2.9.93/oakvar/lib/assets/module_templates/mapper/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/mapper/template.md
--rw-r--r--   0 rick       (501) staff       (20)     3078 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/mapper/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1120 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/mapper/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.410784 oakvar-2.9.93/oakvar/lib/assets/module_templates/postaggregator/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/postaggregator/template.md
--rw-r--r--   0 rick       (501) staff       (20)     2563 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/postaggregator/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1335 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/postaggregator/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.411166 oakvar-2.9.93/oakvar/lib/assets/module_templates/preparer/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/preparer/template.md
--rw-r--r--   0 rick       (501) staff       (20)     2033 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/preparer/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1327 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/preparer/template.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.411666 oakvar-2.9.93/oakvar/lib/assets/module_templates/reporter/
--rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/reporter/template.md
--rw-r--r--   0 rick       (501) staff       (20)     3574 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/reporter/template.py
--rw-r--r--   0 rick       (501) staff       (20)     1246 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/module_templates/reporter/template.yml
--rw-r--r--   0 rick       (501) staff       (20)      135 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/oakvar.yml
--rw-r--r--   0 rick       (501) staff       (20)     3060 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/assets/output_columns.yml
--rw-r--r--   0 rick       (501) staff       (20)      768 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/assets/system.yml
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.414351 oakvar-2.9.93/oakvar/lib/base/
--rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/base/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)    22714 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/base/aggregator.py
--rw-r--r--   0 rick       (501) staff       (20)    36762 2024-03-03 18:25:36.000000 oakvar-2.9.93/oakvar/lib/base/annotator.py
--rw-r--r--   0 rick       (501) staff       (20)     2588 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/base/app.py
--rw-r--r--   0 rick       (501) staff       (20)     4546 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/base/commonmodule.py
--rw-r--r--   0 rick       (501) staff       (20)     5216 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/base/converter.py
--rw-r--r--   0 rick       (501) staff       (20)    13627 2024-03-03 16:41:12.000000 oakvar-2.9.93/oakvar/lib/base/mapper.py
--rw-r--r--   0 rick       (501) staff       (20)    43499 2024-02-19 19:29:51.000000 oakvar-2.9.93/oakvar/lib/base/master_converter.py
--rw-r--r--   0 rick       (501) staff       (20)     4982 2024-03-03 18:25:36.000000 oakvar-2.9.93/oakvar/lib/base/mp_runners.py
--rw-r--r--   0 rick       (501) staff       (20)    27573 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/base/postaggregator.py
--rw-r--r--   0 rick       (501) staff       (20)     8852 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/base/preparer.py
--rw-r--r--   0 rick       (501) staff       (20)    44997 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/base/report_filter.py
--rw-r--r--   0 rick       (501) staff       (20)    44831 2024-03-07 14:37:13.000000 oakvar-2.9.93/oakvar/lib/base/reporter.py
--rw-r--r--   0 rick       (501) staff       (20)    84125 2024-03-07 14:36:39.000000 oakvar-2.9.93/oakvar/lib/base/runner.py
--rw-r--r--   0 rick       (501) staff       (20)    17018 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/base/vcf2vcf.py
--rw-r--r--   0 rick       (501) staff       (20)     4452 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/consts.py
--rw-r--r--   0 rick       (501) staff       (20)     9623 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/exceptions.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.415439 oakvar-2.9.93/oakvar/lib/module/
--rw-r--r--   0 rick       (501) staff       (20)    32241 2024-01-24 15:23:36.000000 oakvar-2.9.93/oakvar/lib/module/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     5975 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/module/cache.py
--rw-r--r--   0 rick       (501) staff       (20)     5355 2023-12-05 15:09:56.000000 oakvar-2.9.93/oakvar/lib/module/data_cache.py
--rw-r--r--   0 rick       (501) staff       (20)    31979 2024-03-12 01:32:28.000000 oakvar-2.9.93/oakvar/lib/module/local.py
--rw-r--r--   0 rick       (501) staff       (20)    13243 2023-12-09 16:39:48.000000 oakvar-2.9.93/oakvar/lib/module/remote.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.415739 oakvar-2.9.93/oakvar/lib/store/
--rw-r--r--   0 rick       (501) staff       (20)     6162 2023-12-05 15:09:57.000000 oakvar-2.9.93/oakvar/lib/store/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     2483 2023-12-05 15:09:57.000000 oakvar-2.9.93/oakvar/lib/store/consts.py
--rw-r--r--   0 rick       (501) staff       (20)    28024 2023-12-09 16:39:48.000000 oakvar-2.9.93/oakvar/lib/store/db.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.415853 oakvar-2.9.93/oakvar/lib/store/ov/
--rw-r--r--   0 rick       (501) staff       (20)     9948 2023-12-09 16:39:48.000000 oakvar-2.9.93/oakvar/lib/store/ov/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.416035 oakvar-2.9.93/oakvar/lib/store/ov/account/
--rw-r--r--   0 rick       (501) staff       (20)    21588 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/store/ov/account/__init__.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.417605 oakvar-2.9.93/oakvar/lib/system/
--rw-r--r--   0 rick       (501) staff       (20)    43831 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/system/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     3126 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/system/consts.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.419669 oakvar-2.9.93/oakvar/lib/util/
--rw-r--r--   0 rick       (501) staff       (20)     2214 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/util/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)     7402 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/util/admin_util.py
--rw-r--r--   0 rick       (501) staff       (20)     2576 2023-12-05 15:09:57.000000 oakvar-2.9.93/oakvar/lib/util/asyn.py
--rw-r--r--   0 rick       (501) staff       (20)     8251 2024-02-23 15:11:11.000000 oakvar-2.9.93/oakvar/lib/util/db.py
--rw-r--r--   0 rick       (501) staff       (20)     6939 2023-12-09 16:39:48.000000 oakvar-2.9.93/oakvar/lib/util/download.py
--rw-r--r--   0 rick       (501) staff       (20)    20964 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/util/download_library.py
--rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:57.000000 oakvar-2.9.93/oakvar/lib/util/image.py
--rw-r--r--   0 rick       (501) staff       (20)    23939 2024-02-08 00:22:22.000000 oakvar-2.9.93/oakvar/lib/util/inout.py
--rw-r--r--   0 rick       (501) staff       (20)    10460 2024-03-07 14:36:39.000000 oakvar-2.9.93/oakvar/lib/util/run.py
--rw-r--r--   0 rick       (501) staff       (20)    14974 2024-03-22 00:57:28.000000 oakvar-2.9.93/oakvar/lib/util/seq.py
--rw-r--r--   0 rick       (501) staff       (20)    22030 2024-01-10 14:33:05.000000 oakvar-2.9.93/oakvar/lib/util/util.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 11:36:06.324011 oakvar-2.9.93/oakvar.egg-info/
--rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-10 11:36:05.000000 oakvar-2.9.93/oakvar.egg-info/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)    18948 2024-04-10 11:36:06.000000 oakvar-2.9.93/oakvar.egg-info/SOURCES.txt
--rw-r--r--   0 rick       (501) staff       (20)        1 2024-04-10 11:36:06.000000 oakvar-2.9.93/oakvar.egg-info/dependency_links.txt
--rw-r--r--   0 rick       (501) staff       (20)       44 2024-04-10 11:36:06.000000 oakvar-2.9.93/oakvar.egg-info/entry_points.txt
--rw-r--r--   0 rick       (501) staff       (20)      291 2024-04-10 11:36:06.000000 oakvar-2.9.93/oakvar.egg-info/requires.txt
--rw-r--r--   0 rick       (501) staff       (20)       14 2024-04-10 11:36:06.000000 oakvar-2.9.93/oakvar.egg-info/top_level.txt
--rw-r--r--   0 rick       (501) staff       (20)      625 2023-12-05 15:09:57.000000 oakvar-2.9.93/pyproject.toml
--rw-r--r--   0 rick       (501) staff       (20)       38 2024-04-10 11:36:06.420254 oakvar-2.9.93/setup.cfg
--rw-r--r--   0 rick       (501) staff       (20)     2443 2024-04-10 11:35:19.000000 oakvar-2.9.93/setup.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.479735 oakvar-2.9.94/
+-rw-r--r--   0 rick       (501) staff       (20)     1753 2023-12-05 15:09:56.000000 oakvar-2.9.94/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-10 23:41:24.479581 oakvar-2.9.94/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     2339 2024-04-10 11:35:38.000000 oakvar-2.9.94/README.rst
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.413988 oakvar-2.9.94/cravat/
+-rw-r--r--   0 rick       (501) staff       (20)       21 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/__main__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.414613 oakvar-2.9.94/cravat/api/
+-rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/config.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.414926 oakvar-2.9.94/cravat/api/module/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/module/ls_logic.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/new.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.415044 oakvar-2.9.94/cravat/api/store/
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.415161 oakvar-2.9.94/cravat/api/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/system.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/test.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/api/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.416540 oakvar-2.9.94/cravat/cli/
+-rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/config.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/gui.py
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/issue.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/license.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.416949 oakvar-2.9.94/cravat/cli/module/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/module/info_fn.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/module/ls.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/new.py
+-rw-r--r--   0 rick       (501) staff       (20)      110 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/report.py
+-rw-r--r--   0 rick       (501) staff       (20)       29 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/run.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.417051 oakvar-2.9.94/cravat/cli/store/
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.417158 oakvar-2.9.94/cravat/cli/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/system.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/test.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/update.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/util.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cli/version.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/constants.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/cravat_report.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/exceptions.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.418540 oakvar-2.9.94/cravat/gui/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/job_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/multiuser.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/server.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/serveradmindb.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/store_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/system_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/system_message_db.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/system_worker.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/userjob.py
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/util.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/web_submit.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.418851 oakvar-2.9.94/cravat/gui/webresult/
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/webresult/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       48 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/webresult/jsonreporter.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/webresult/webresult.py
+-rw-r--r--   0 rick       (501) staff       (20)       44 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/gui/websocket_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/inout.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.419163 oakvar-2.9.94/cravat/lib/
+-rw-r--r--   0 rick       (501) staff       (20)       25 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.407450 oakvar-2.9.94/cravat/lib/assets/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.407801 oakvar-2.9.94/cravat/lib/assets/module_templates/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.419274 oakvar-2.9.94/cravat/lib/assets/module_templates/annotator/
+-rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/assets/module_templates/annotator/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.419386 oakvar-2.9.94/cravat/lib/assets/module_templates/converter/
+-rw-r--r--   0 rick       (501) staff       (20)       68 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/assets/module_templates/converter/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.419490 oakvar-2.9.94/cravat/lib/assets/module_templates/mapper/
+-rw-r--r--   0 rick       (501) staff       (20)       65 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/assets/module_templates/mapper/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.419600 oakvar-2.9.94/cravat/lib/assets/module_templates/postaggregator/
+-rw-r--r--   0 rick       (501) staff       (20)       73 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/assets/module_templates/postaggregator/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.419710 oakvar-2.9.94/cravat/lib/assets/module_templates/preparer/
+-rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/assets/module_templates/preparer/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.419822 oakvar-2.9.94/cravat/lib/assets/module_templates/reporter/
+-rw-r--r--   0 rick       (501) staff       (20)       67 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/assets/module_templates/reporter/template.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.421406 oakvar-2.9.94/cravat/lib/base/
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/aggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/annotator.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/app.py
+-rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/commonmodule.py
+-rw-r--r--   0 rick       (501) staff       (20)       40 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/converter.py
+-rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/mapper.py
+-rw-r--r--   0 rick       (501) staff       (20)       47 2024-01-10 14:33:05.000000 oakvar-2.9.94/cravat/lib/base/master_converter.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2024-01-10 14:33:05.000000 oakvar-2.9.94/cravat/lib/base/mp_runners.py
+-rw-r--r--   0 rick       (501) staff       (20)       45 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/postaggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/preparer.py
+-rw-r--r--   0 rick       (501) staff       (20)       44 2024-01-10 14:33:05.000000 oakvar-2.9.94/cravat/lib/base/report_filter.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/reporter.py
+-rw-r--r--   0 rick       (501) staff       (20)       37 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/runner.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/base/vcf2vcf.py
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/exceptions.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.421943 oakvar-2.9.94/cravat/lib/module/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/module/cache.py
+-rw-r--r--   0 rick       (501) staff       (20)       43 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/module/data_cache.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/module/local.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/module/remote.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.422254 oakvar-2.9.94/cravat/lib/store/
+-rw-r--r--   0 rick       (501) staff       (20)       31 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/store/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       38 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/store/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/store/db.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.422362 oakvar-2.9.94/cravat/lib/store/ov/
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/store/ov/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.422476 oakvar-2.9.94/cravat/lib/store/ov/account/
+-rw-r--r--   0 rick       (501) staff       (20)       42 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/store/ov/account/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.422710 oakvar-2.9.94/cravat/lib/system/
+-rw-r--r--   0 rick       (501) staff       (20)       32 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/system/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/system/consts.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.423855 oakvar-2.9.94/cravat/lib/util/
+-rw-r--r--   0 rick       (501) staff       (20)       30 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       41 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/admin_util.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/asyn.py
+-rw-r--r--   0 rick       (501) staff       (20)       33 2023-12-23 13:35:34.000000 oakvar-2.9.94/cravat/lib/util/db.py
+-rw-r--r--   0 rick       (501) staff       (20)       39 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/download.py
+-rw-r--r--   0 rick       (501) staff       (20)       47 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/download_library.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/image.py
+-rw-r--r--   0 rick       (501) staff       (20)       36 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/inout.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/run.py
+-rw-r--r--   0 rick       (501) staff       (20)       34 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/seq.py
+-rw-r--r--   0 rick       (501) staff       (20)       35 2023-12-23 13:33:25.000000 oakvar-2.9.94/cravat/lib/util/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.424071 oakvar-2.9.94/oakvar/
+-rw-r--r--   0 rick       (501) staff       (20)     6681 2024-03-03 15:20:39.000000 oakvar-2.9.94/oakvar/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     7901 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/__main__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.425391 oakvar-2.9.94/oakvar/api/
+-rw-r--r--   0 rick       (501) staff       (20)    19785 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/api/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     3144 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/api/config.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.425739 oakvar-2.9.94/oakvar/api/module/
+-rw-r--r--   0 rick       (501) staff       (20)    18616 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/api/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     5305 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/api/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)     5687 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/api/module/ls_logic.py
+-rw-r--r--   0 rick       (501) staff       (20)     3379 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/api/new.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.425851 oakvar-2.9.94/oakvar/api/store/
+-rw-r--r--   0 rick       (501) staff       (20)     7179 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/api/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.425966 oakvar-2.9.94/oakvar/api/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)     4130 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/api/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     4510 2023-12-23 13:35:34.000000 oakvar-2.9.94/oakvar/api/system.py
+-rw-r--r--   0 rick       (501) staff       (20)    34086 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/api/test.py
+-rw-r--r--   0 rick       (501) staff       (20)    18455 2024-02-23 14:56:17.000000 oakvar-2.9.94/oakvar/api/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.427429 oakvar-2.9.94/oakvar/cli/
+-rw-r--r--   0 rick       (501) staff       (20)     4470 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     4949 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/config.py
+-rw-r--r--   0 rick       (501) staff       (20)    10930 2023-12-23 13:35:34.000000 oakvar-2.9.94/oakvar/cli/gui.py
+-rw-r--r--   0 rick       (501) staff       (20)     2297 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/issue.py
+-rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/license.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.427950 oakvar-2.9.94/oakvar/cli/module/
+-rw-r--r--   0 rick       (501) staff       (20)    15171 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/cli/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     6422 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/module/info_fn.py
+-rw-r--r--   0 rick       (501) staff       (20)     2410 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/module/install_defs.py
+-rw-r--r--   0 rick       (501) staff       (20)     7792 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/module/ls.py
+-rw-r--r--   0 rick       (501) staff       (20)     4408 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/new.py
+-rw-r--r--   0 rick       (501) staff       (20)     6925 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/cli/report.py
+-rw-r--r--   0 rick       (501) staff       (20)    11084 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/cli/run.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.428085 oakvar-2.9.94/oakvar/cli/store/
+-rw-r--r--   0 rick       (501) staff       (20)     9370 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/cli/store/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.428214 oakvar-2.9.94/oakvar/cli/store/account/
+-rw-r--r--   0 rick       (501) staff       (20)     7883 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/store/account/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     6736 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/system.py
+-rw-r--r--   0 rick       (501) staff       (20)     2886 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/test.py
+-rw-r--r--   0 rick       (501) staff       (20)     2299 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/update.py
+-rw-r--r--   0 rick       (501) staff       (20)     9339 2024-02-23 14:57:11.000000 oakvar-2.9.94/oakvar/cli/util.py
+-rw-r--r--   0 rick       (501) staff       (20)     2474 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/cli/version.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.429878 oakvar-2.9.94/oakvar/gui/
+-rw-r--r--   0 rick       (501) staff       (20)     2958 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)    28494 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/job_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)    11215 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/multiuser.py
+-rw-r--r--   0 rick       (501) staff       (20)    17290 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/server.py
+-rw-r--r--   0 rick       (501) staff       (20)    25415 2024-02-23 14:55:01.000000 oakvar-2.9.94/oakvar/gui/serveradmindb.py
+-rw-r--r--   0 rick       (501) staff       (20)    15866 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/store_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)     8553 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/system_handlers.py
+-rw-r--r--   0 rick       (501) staff       (20)     3968 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/system_message_db.py
+-rw-r--r--   0 rick       (501) staff       (20)     8117 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/system_worker.py
+-rw-r--r--   0 rick       (501) staff       (20)     6042 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/userjob.py
+-rw-r--r--   0 rick       (501) staff       (20)     7210 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/util.py
+-rw-r--r--   0 rick       (501) staff       (20)    17662 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/web_submit.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.430690 oakvar-2.9.94/oakvar/gui/webresult/
+-rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.430802 oakvar-2.9.94/oakvar/gui/webresult/css/
+-rw-r--r--   0 rick       (501) staff       (20)     2389 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/css/pqselect.min.css
+-rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/email.png
+-rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/favicon.ico
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.431812 oakvar-2.9.94/oakvar/gui/webresult/fonts/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.447135 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/
+-rw-r--r--   0 rick       (501) staff       (20)   138764 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff
+-rw-r--r--   0 rick       (501) staff       (20)   102868 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   146824 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   108752 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   143208 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106140 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   151052 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111808 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   142920 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106108 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   150628 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111708 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   140724 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff
+-rw-r--r--   0 rick       (501) staff       (20)   104232 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   149996 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111392 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   144372 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106876 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   140632 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff
+-rw-r--r--   0 rick       (501) staff       (20)   104332 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   150092 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   111332 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   142552 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff
+-rw-r--r--   0 rick       (501) staff       (20)   105924 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   150988 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   112184 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   133844 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff
+-rw-r--r--   0 rick       (501) staff       (20)    98868 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   142932 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff
+-rw-r--r--   0 rick       (501) staff       (20)   105804 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   151180 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   112048 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   135920 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff
+-rw-r--r--   0 rick       (501) staff       (20)    99632 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   145480 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff
+-rw-r--r--   0 rick       (501) staff       (20)   106496 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   245036 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   227180 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2
+-rw-r--r--   0 rick       (501) staff       (20)   324864 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2
+-rw-r--r--   0 rick       (501) staff       (20)     5303 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/inter.css
+-rw-r--r--   0 rick       (501) staff       (20)    26456 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    19508 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2
+-rw-r--r--   0 rick       (501) staff       (20)    25692 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-light-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    18980 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2
+-rw-r--r--   0 rick       (501) staff       (20)    26312 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    19416 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2
+-rw-r--r--   0 rick       (501) staff       (20)    33072 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rw-r--r--   0 rick       (501) staff       (20)    25740 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.449630 oakvar-2.9.94/oakvar/gui/webresult/images/
+-rw-r--r--   0 rick       (501) staff       (20)      326 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrow-down-right-circle-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)      379 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrow-down-right-circle.svg
+-rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrow-down-right.svg
+-rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrow-down.svg
+-rw-r--r--   0 rick       (501) staff       (20)      311 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrow-left.svg
+-rw-r--r--   0 rick       (501) staff       (20)      312 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrow-right.svg
+-rw-r--r--   0 rick       (501) staff       (20)      309 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrow-up.svg
+-rw-r--r--   0 rick       (501) staff       (20)      706 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/arrows-move.svg
+-rw-r--r--   0 rick       (501) staff       (20)     2140 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/camera.svg
+-rw-r--r--   0 rick       (501) staff       (20)      291 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/caret-down.svg
+-rw-r--r--   0 rick       (501) staff       (20)      289 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/caret-right.svg
+-rw-r--r--   0 rick       (501) staff       (20)     3125 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/close.png
+-rw-r--r--   0 rick       (501) staff       (20)     2390 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/close.svg
+-rw-r--r--   0 rick       (501) staff       (20)      722 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/download-material-black.png
+-rw-r--r--   0 rick       (501) staff       (20)     2066 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/download.svg
+-rw-r--r--   0 rick       (501) staff       (20)      485 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/grip-vertical.svg
+-rw-r--r--   0 rick       (501) staff       (20)     2219 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/pin.svg
+-rw-r--r--   0 rick       (501) staff       (20)     2243 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/plus-circle-dotted.svg
+-rw-r--r--   0 rick       (501) staff       (20)      280 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/plus-circle-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)     4645 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/sorry.png
+-rw-r--r--   0 rick       (501) staff       (20)    25333 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/spinner.gif
+-rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/x-lg.svg
+-rw-r--r--   0 rick       (501) staff       (20)      332 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/images/x.svg
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.452301 oakvar-2.9.94/oakvar/gui/webresult/js/
+-rw-r--r--   0 rick       (501) staff       (20)   398184 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/Chart.js
+-rw-r--r--   0 rick       (501) staff       (20)    26580 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/axios.min.js
+-rw-r--r--   0 rick       (501) staff       (20)   137820 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/axios.min.js.map
+-rw-r--r--   0 rick       (501) staff       (20)     9278 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/dom-to-image.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     5839 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/download.js
+-rw-r--r--   0 rick       (501) staff       (20)    12091 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/draggabilly.pkgd.min.js
+-rw-r--r--   0 rick       (501) staff       (20)   954164 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/graphics.js
+-rw-r--r--   0 rick       (501) staff       (20)    86659 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-3.2.1.min.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.454267 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/
+-rw-r--r--   0 rick       (501) staff       (20)    12660 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rw-r--r--   0 rick       (501) staff       (20)     1817 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.409451 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.454376 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rw-r--r--   0 rick       (501) staff       (20)   293430 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.455209 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/
+-rw-r--r--   0 rick       (501) staff       (20)     6992 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     6988 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     6999 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     4549 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)     6299 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 rick       (501) staff       (20)    32588 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rw-r--r--   0 rick       (501) staff       (20)    35997 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rw-r--r--   0 rick       (501) staff       (20)   520714 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rw-r--r--   0 rick       (501) staff       (20)    30747 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rw-r--r--   0 rick       (501) staff       (20)   253668 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    18705 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rw-r--r--   0 rick       (501) staff       (20)    15548 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rw-r--r--   0 rick       (501) staff       (20)    17342 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rw-r--r--   0 rick       (501) staff       (20)    13847 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rw-r--r--   0 rick       (501) staff       (20)     1340 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rw-r--r--   0 rick       (501) staff       (20)    13171 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery.tools.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     5451 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/jquery.url.js
+-rw-r--r--   0 rick       (501) staff       (20)    24103 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/masonry.pkgd.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    84772 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/packery.pkgd.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.456818 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/
+-rw-r--r--   0 rick       (501) staff       (20)    11583 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rw-r--r--   0 rick       (501) staff       (20)   103213 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.457862 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/
+-rw-r--r--   0 rick       (501) staff       (20)      230 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rw-r--r--   0 rick       (501) staff       (20)      210 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rw-r--r--   0 rick       (501) staff       (20)      771 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif
+-rw-r--r--   0 rick       (501) staff       (20)     1668 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png
+-rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rw-r--r--   0 rick       (501) staff       (20)       51 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rw-r--r--   0 rick       (501) staff       (20)       76 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rw-r--r--   0 rick       (501) staff       (20)      216 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rw-r--r--   0 rick       (501) staff       (20)      201 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.458084 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rw-r--r--   0 rick       (501) staff       (20)     1148 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rw-r--r--   0 rick       (501) staff       (20)    76985 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.459398 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/
+-rw-r--r--   0 rick       (501) staff       (20)      755 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rw-r--r--   0 rick       (501) staff       (20)      750 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rw-r--r--   0 rick       (501) staff       (20)      769 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rw-r--r--   0 rick       (501) staff       (20)      802 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rw-r--r--   0 rick       (501) staff       (20)      813 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rw-r--r--   0 rick       (501) staff       (20)      805 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rw-r--r--   0 rick       (501) staff       (20)      636 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rw-r--r--   0 rick       (501) staff       (20)      774 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rw-r--r--   0 rick       (501) staff       (20)      782 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rw-r--r--   0 rick       (501) staff       (20)      822 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rw-r--r--   0 rick       (501) staff       (20)      773 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rw-r--r--   0 rick       (501) staff       (20)      675 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460164 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/
+-rw-r--r--   0 rick       (501) staff       (20)     1105 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rw-r--r--   0 rick       (501) staff       (20)      613 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)      541 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rw-r--r--   0 rick       (501) staff       (20)     2973 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)    27759 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rw-r--r--   0 rick       (501) staff       (20)     2383 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rw-r--r--   0 rick       (501) staff       (20)    12577 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     2408 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)     2026 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rw-r--r--   0 rick       (501) staff       (20)    16145 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)   481365 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rw-r--r--   0 rick       (501) staff       (20)    12757 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rw-r--r--   0 rick       (501) staff       (20)   242931 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     1646 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rw-r--r--   0 rick       (501) staff       (20)     1278 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rw-r--r--   0 rick       (501) staff       (20)      555 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.410868 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460282 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460391 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460507 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460620 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460744 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460861 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.460972 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461082 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461193 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461301 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461405 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461509 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461625 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461737 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.461854 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/
+-rw-r--r--   0 rick       (501) staff       (20)     4384 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.462387 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/
+-rw-r--r--   0 rick       (501) staff       (20)     1042 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rw-r--r--   0 rick       (501) staff       (20)     1164 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rw-r--r--   0 rick       (501) staff       (20)     2677 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rw-r--r--   0 rick       (501) staff       (20)     3716 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rw-r--r--   0 rick       (501) staff       (20)     1847 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    12583 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/pqselect.min.js
+-rw-r--r--   0 rick       (501) staff       (20)    92225 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/raphael-min.js
+-rw-r--r--   0 rick       (501) staff       (20)   326538 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/js/tailwind.min.js
+-rw-r--r--   0 rick       (501) staff       (20)     2732 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/webresult/jsonreporter.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.462627 oakvar-2.9.94/oakvar/gui/webresult/nocache/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.463292 oakvar-2.9.94/oakvar/gui/webresult/nocache/css/
+-rw-r--r--   0 rick       (501) staff       (20)     1714 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/css/singlevariantpage.css
+-rw-r--r--   0 rick       (501) staff       (20)    22655 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/css/style.css
+-rw-r--r--   0 rick       (501) staff       (20)     2658 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/css/widget.css
+-rw-r--r--   0 rick       (501) staff       (20)    21597 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/index.html
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.464525 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/
+-rw-r--r--   0 rick       (501) staff       (20)    24858 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/filter.js
+-rw-r--r--   0 rick       (501) staff       (20)    13105 2023-12-09 16:39:48.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/infomgr.js
+-rw-r--r--   0 rick       (501) staff       (20)    30870 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/main.js
+-rw-r--r--   0 rick       (501) staff       (20)   103450 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/setup.js
+-rw-r--r--   0 rick       (501) staff       (20)     4903 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/showvariant.js
+-rw-r--r--   0 rick       (501) staff       (20)    35998 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/singlevariantpage.js
+-rw-r--r--   0 rick       (501) staff       (20)    28858 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/util.js
+-rw-r--r--   0 rick       (501) staff       (20)     1696 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/variables.js
+-rw-r--r--   0 rick       (501) staff       (20)    22262 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/js/widgethelper.js
+-rw-r--r--   0 rick       (501) staff       (20)     5440 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/nocache/variant.html
+-rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/question.png
+-rw-r--r--   0 rick       (501) staff       (20)    31615 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/webresult/webresult.py
+-rw-r--r--   0 rick       (501) staff       (20)      163 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webresult/webviewer.yml
+-rw-r--r--   0 rick       (501) staff       (20)     5907 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websocket_handlers.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.411235 oakvar-2.9.94/oakvar/gui/webstore/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.466402 oakvar-2.9.94/oakvar/gui/webstore/images/
+-rw-r--r--   0 rick       (501) staff       (20)      446 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/chat-dots-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)      740 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/chat-dots.svg
+-rw-r--r--   0 rick       (501) staff       (20)      396 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/chat-left-text-fill.svg
+-rw-r--r--   0 rick       (501) staff       (20)      545 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/chat-left-text.svg
+-rw-r--r--   0 rick       (501) staff       (20)    22268 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/done.png
+-rw-r--r--   0 rick       (501) staff       (20)     4948 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/email.png
+-rw-r--r--   0 rick       (501) staff       (20)     2226 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/empty.png
+-rw-r--r--   0 rick       (501) staff       (20)     1763 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/folder.png
+-rw-r--r--   0 rick       (501) staff       (20)    38197 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/genericmodulelogo.png
+-rw-r--r--   0 rick       (501) staff       (20)     4766 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/hamburger.png
+-rw-r--r--   0 rick       (501) staff       (20)     1194 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/left_arrow.png
+-rw-r--r--   0 rick       (501) staff       (20)     3524 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/new.png
+-rw-r--r--   0 rick       (501) staff       (20)      474 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/no_logo_module.svg
+-rw-r--r--   0 rick       (501) staff       (20)    10263 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/question.png
+-rw-r--r--   0 rick       (501) staff       (20)     1214 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/right_arrow.png
+-rw-r--r--   0 rick       (501) staff       (20)      340 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/webstore/images/x-lg.svg
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.411496 oakvar-2.9.94/oakvar/gui/websubmit/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.468165 oakvar-2.9.94/oakvar/gui/websubmit/images/
+-rw-r--r--   0 rick       (501) staff       (20)   372952 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/images/background.png
+-rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/images/logo.png
+-rw-r--r--   0 rick       (501) staff       (20)    22716 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/images/logo_only.png
+-rw-r--r--   0 rick       (501) staff       (20)    24659 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/images/logo_transparent.png
+-rw-r--r--   0 rick       (501) staff       (20)    22247 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/images/logo_transparent_bw.png
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.468318 oakvar-2.9.94/oakvar/gui/websubmit/inputexamples/
+-rw-r--r--   0 rick       (501) staff       (20)     9036 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/inputexamples/exampleinput
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.470280 oakvar-2.9.94/oakvar/gui/websubmit/nocache/
+-rw-r--r--   0 rick       (501) staff       (20)      692 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/alerts.js
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/element_constructors.js
+-rw-r--r--   0 rick       (501) staff       (20)     6756 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/element_getters.js
+-rw-r--r--   0 rick       (501) staff       (20)    55822 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/index.html
+-rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/input.js
+-rw-r--r--   0 rick       (501) staff       (20)    14408 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/jobstable.js
+-rw-r--r--   0 rick       (501) staff       (20)     8242 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/login.html
+-rw-r--r--   0 rick       (501) staff       (20)     3796 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/multiuser.css
+-rw-r--r--   0 rick       (501) staff       (20)    16797 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/multiuser.js
+-rw-r--r--   0 rick       (501) staff       (20)     2889 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/select_modules.js
+-rw-r--r--   0 rick       (501) staff       (20)      228 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/showhide.js
+-rw-r--r--   0 rick       (501) staff       (20)     6783 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/submit.js
+-rw-r--r--   0 rick       (501) staff       (20)      484 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/util.js
+-rw-r--r--   0 rick       (501) staff       (20)    11319 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/websubmit.css
+-rw-r--r--   0 rick       (501) staff       (20)    39200 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/gui/websubmit/nocache/websubmit.js
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.470521 oakvar-2.9.94/oakvar/gui/www/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.470774 oakvar-2.9.94/oakvar/gui/www/assets/
+-rw-r--r--   0 rick       (501) staff       (20)    63287 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/www/assets/index.3526e7ae.css
+-rw-r--r--   0 rick       (501) staff       (20)   834933 2023-12-09 16:39:48.000000 oakvar-2.9.94/oakvar/gui/www/assets/index.5e1d7274.js
+-rw-r--r--   0 rick       (501) staff       (20)     1150 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/gui/www/favicon.ico
+-rw-r--r--   0 rick       (501) staff       (20)     2074 2023-12-09 16:39:48.000000 oakvar-2.9.94/oakvar/gui/www/index.html
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.471477 oakvar-2.9.94/oakvar/lib/
+-rw-r--r--   0 rick       (501) staff       (20)     1946 2024-03-03 16:46:38.000000 oakvar-2.9.94/oakvar/lib/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.472233 oakvar-2.9.94/oakvar/lib/assets/
+-rw-r--r--   0 rick       (501) staff       (20)     9036 2024-04-10 11:35:01.000000 oakvar-2.9.94/oakvar/lib/assets/exampleinput
+-rw-r--r--   0 rick       (501) staff       (20)    16880 2024-02-08 01:06:28.000000 oakvar-2.9.94/oakvar/lib/assets/hg19.chromAlias.txt
+-rw-r--r--   0 rick       (501) staff       (20)    27240 2024-02-08 00:52:40.000000 oakvar-2.9.94/oakvar/lib/assets/hg38.chromAlias.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.472456 oakvar-2.9.94/oakvar/lib/assets/license/
+-rw-r--r--   0 rick       (501) staff       (20)     1707 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/license/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)     1330 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/license/liftover.txt
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.412260 oakvar-2.9.94/oakvar/lib/assets/module_templates/
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.472807 oakvar-2.9.94/oakvar/lib/assets/module_templates/annotator/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/annotator/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     2109 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/annotator/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1195 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/annotator/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.473133 oakvar-2.9.94/oakvar/lib/assets/module_templates/converter/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/converter/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     4366 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/converter/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1249 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/converter/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.473443 oakvar-2.9.94/oakvar/lib/assets/module_templates/mapper/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/mapper/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     3078 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/mapper/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1120 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/mapper/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.473757 oakvar-2.9.94/oakvar/lib/assets/module_templates/postaggregator/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/postaggregator/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     2563 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/postaggregator/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1335 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/postaggregator/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.474081 oakvar-2.9.94/oakvar/lib/assets/module_templates/preparer/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/preparer/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     2033 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/preparer/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1327 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/preparer/template.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.474404 oakvar-2.9.94/oakvar/lib/assets/module_templates/reporter/
+-rw-r--r--   0 rick       (501) staff       (20)      634 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/reporter/template.md
+-rw-r--r--   0 rick       (501) staff       (20)     3574 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/reporter/template.py
+-rw-r--r--   0 rick       (501) staff       (20)     1246 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/module_templates/reporter/template.yml
+-rw-r--r--   0 rick       (501) staff       (20)      135 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/oakvar.yml
+-rw-r--r--   0 rick       (501) staff       (20)    10314 2024-04-10 12:11:07.000000 oakvar-2.9.94/oakvar/lib/assets/oakvar_example.vcf
+-rw-r--r--   0 rick       (501) staff       (20)     3060 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/assets/output_columns.yml
+-rw-r--r--   0 rick       (501) staff       (20)      768 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/assets/system.yml
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.476776 oakvar-2.9.94/oakvar/lib/base/
+-rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/base/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)    22714 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/base/aggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)    36762 2024-03-03 18:25:36.000000 oakvar-2.9.94/oakvar/lib/base/annotator.py
+-rw-r--r--   0 rick       (501) staff       (20)     2588 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/base/app.py
+-rw-r--r--   0 rick       (501) staff       (20)     4546 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/base/commonmodule.py
+-rw-r--r--   0 rick       (501) staff       (20)     5216 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/base/converter.py
+-rw-r--r--   0 rick       (501) staff       (20)    13627 2024-03-03 16:41:12.000000 oakvar-2.9.94/oakvar/lib/base/mapper.py
+-rw-r--r--   0 rick       (501) staff       (20)    43499 2024-02-19 19:29:51.000000 oakvar-2.9.94/oakvar/lib/base/master_converter.py
+-rw-r--r--   0 rick       (501) staff       (20)     4982 2024-03-03 18:25:36.000000 oakvar-2.9.94/oakvar/lib/base/mp_runners.py
+-rw-r--r--   0 rick       (501) staff       (20)    27573 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/base/postaggregator.py
+-rw-r--r--   0 rick       (501) staff       (20)     8852 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/base/preparer.py
+-rw-r--r--   0 rick       (501) staff       (20)    44997 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/base/report_filter.py
+-rw-r--r--   0 rick       (501) staff       (20)    44831 2024-03-07 14:37:13.000000 oakvar-2.9.94/oakvar/lib/base/reporter.py
+-rw-r--r--   0 rick       (501) staff       (20)    84125 2024-03-07 14:36:39.000000 oakvar-2.9.94/oakvar/lib/base/runner.py
+-rw-r--r--   0 rick       (501) staff       (20)    17018 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/base/vcf2vcf.py
+-rw-r--r--   0 rick       (501) staff       (20)     4452 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)     9623 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/exceptions.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.477372 oakvar-2.9.94/oakvar/lib/module/
+-rw-r--r--   0 rick       (501) staff       (20)    32241 2024-01-24 15:23:36.000000 oakvar-2.9.94/oakvar/lib/module/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     5975 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/module/cache.py
+-rw-r--r--   0 rick       (501) staff       (20)     5355 2023-12-05 15:09:56.000000 oakvar-2.9.94/oakvar/lib/module/data_cache.py
+-rw-r--r--   0 rick       (501) staff       (20)    31979 2024-03-12 01:32:28.000000 oakvar-2.9.94/oakvar/lib/module/local.py
+-rw-r--r--   0 rick       (501) staff       (20)    13243 2023-12-09 16:39:48.000000 oakvar-2.9.94/oakvar/lib/module/remote.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.477721 oakvar-2.9.94/oakvar/lib/store/
+-rw-r--r--   0 rick       (501) staff       (20)     6162 2023-12-05 15:09:57.000000 oakvar-2.9.94/oakvar/lib/store/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     2483 2023-12-05 15:09:57.000000 oakvar-2.9.94/oakvar/lib/store/consts.py
+-rw-r--r--   0 rick       (501) staff       (20)    28024 2023-12-09 16:39:48.000000 oakvar-2.9.94/oakvar/lib/store/db.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.477839 oakvar-2.9.94/oakvar/lib/store/ov/
+-rw-r--r--   0 rick       (501) staff       (20)     9948 2023-12-09 16:39:48.000000 oakvar-2.9.94/oakvar/lib/store/ov/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.477947 oakvar-2.9.94/oakvar/lib/store/ov/account/
+-rw-r--r--   0 rick       (501) staff       (20)    21588 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/store/ov/account/__init__.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.478193 oakvar-2.9.94/oakvar/lib/system/
+-rw-r--r--   0 rick       (501) staff       (20)    43831 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/system/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     3126 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/system/consts.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.479383 oakvar-2.9.94/oakvar/lib/util/
+-rw-r--r--   0 rick       (501) staff       (20)     2214 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/util/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     7408 2024-04-10 23:40:21.000000 oakvar-2.9.94/oakvar/lib/util/admin_util.py
+-rw-r--r--   0 rick       (501) staff       (20)     2576 2023-12-05 15:09:57.000000 oakvar-2.9.94/oakvar/lib/util/asyn.py
+-rw-r--r--   0 rick       (501) staff       (20)     8251 2024-02-23 15:11:11.000000 oakvar-2.9.94/oakvar/lib/util/db.py
+-rw-r--r--   0 rick       (501) staff       (20)     6939 2023-12-09 16:39:48.000000 oakvar-2.9.94/oakvar/lib/util/download.py
+-rw-r--r--   0 rick       (501) staff       (20)    20964 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/util/download_library.py
+-rw-r--r--   0 rick       (501) staff       (20)     1833 2023-12-05 15:09:57.000000 oakvar-2.9.94/oakvar/lib/util/image.py
+-rw-r--r--   0 rick       (501) staff       (20)    23939 2024-02-08 00:22:22.000000 oakvar-2.9.94/oakvar/lib/util/inout.py
+-rw-r--r--   0 rick       (501) staff       (20)    10460 2024-03-07 14:36:39.000000 oakvar-2.9.94/oakvar/lib/util/run.py
+-rw-r--r--   0 rick       (501) staff       (20)    14974 2024-03-22 00:57:28.000000 oakvar-2.9.94/oakvar/lib/util/seq.py
+-rw-r--r--   0 rick       (501) staff       (20)    22030 2024-01-10 14:33:05.000000 oakvar-2.9.94/oakvar/lib/util/util.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2024-04-10 23:41:24.424709 oakvar-2.9.94/oakvar.egg-info/
+-rw-r--r--   0 rick       (501) staff       (20)     2950 2024-04-10 23:41:24.000000 oakvar-2.9.94/oakvar.egg-info/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)    18985 2024-04-10 23:41:24.000000 oakvar-2.9.94/oakvar.egg-info/SOURCES.txt
+-rw-r--r--   0 rick       (501) staff       (20)        1 2024-04-10 23:41:24.000000 oakvar-2.9.94/oakvar.egg-info/dependency_links.txt
+-rw-r--r--   0 rick       (501) staff       (20)       44 2024-04-10 23:41:24.000000 oakvar-2.9.94/oakvar.egg-info/entry_points.txt
+-rw-r--r--   0 rick       (501) staff       (20)      291 2024-04-10 23:41:24.000000 oakvar-2.9.94/oakvar.egg-info/requires.txt
+-rw-r--r--   0 rick       (501) staff       (20)       14 2024-04-10 23:41:24.000000 oakvar-2.9.94/oakvar.egg-info/top_level.txt
+-rw-r--r--   0 rick       (501) staff       (20)      625 2023-12-05 15:09:57.000000 oakvar-2.9.94/pyproject.toml
+-rw-r--r--   0 rick       (501) staff       (20)       38 2024-04-10 23:41:24.479783 oakvar-2.9.94/setup.cfg
+-rw-r--r--   0 rick       (501) staff       (20)     2443 2024-04-10 23:40:52.000000 oakvar-2.9.94/setup.py
```

### Comparing `oakvar-2.9.93/LICENSE` & `oakvar-2.9.94/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/PKG-INFO` & `oakvar-2.9.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.93
+Version: 2.9.94
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 License: UNKNOWN
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
```

### Comparing `oakvar-2.9.93/README.rst` & `oakvar-2.9.94/README.rst`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/__init__.py` & `oakvar-2.9.94/oakvar/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/__main__.py` & `oakvar-2.9.94/oakvar/__main__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/__init__.py` & `oakvar-2.9.94/oakvar/api/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/config.py` & `oakvar-2.9.94/oakvar/api/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/module/__init__.py` & `oakvar-2.9.94/oakvar/api/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/module/install_defs.py` & `oakvar-2.9.94/oakvar/api/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/module/ls_logic.py` & `oakvar-2.9.94/oakvar/api/module/ls_logic.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/new.py` & `oakvar-2.9.94/oakvar/api/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/store/__init__.py` & `oakvar-2.9.94/oakvar/api/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/store/account/__init__.py` & `oakvar-2.9.94/oakvar/api/store/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/system.py` & `oakvar-2.9.94/oakvar/api/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/test.py` & `oakvar-2.9.94/oakvar/api/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/api/util.py` & `oakvar-2.9.94/oakvar/api/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/__init__.py` & `oakvar-2.9.94/oakvar/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/config.py` & `oakvar-2.9.94/oakvar/cli/config.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/gui.py` & `oakvar-2.9.94/oakvar/cli/gui.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/issue.py` & `oakvar-2.9.94/oakvar/cli/issue.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/license.py` & `oakvar-2.9.94/oakvar/cli/license.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/module/__init__.py` & `oakvar-2.9.94/oakvar/cli/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/module/info_fn.py` & `oakvar-2.9.94/oakvar/cli/module/info_fn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/module/install_defs.py` & `oakvar-2.9.94/oakvar/cli/module/install_defs.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/module/ls.py` & `oakvar-2.9.94/oakvar/cli/module/ls.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/new.py` & `oakvar-2.9.94/oakvar/cli/new.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/report.py` & `oakvar-2.9.94/oakvar/cli/report.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/run.py` & `oakvar-2.9.94/oakvar/cli/run.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/store/__init__.py` & `oakvar-2.9.94/oakvar/cli/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/store/account/__init__.py` & `oakvar-2.9.94/oakvar/cli/store/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/system.py` & `oakvar-2.9.94/oakvar/cli/system.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/test.py` & `oakvar-2.9.94/oakvar/cli/test.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/update.py` & `oakvar-2.9.94/oakvar/cli/update.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/util.py` & `oakvar-2.9.94/oakvar/cli/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/cli/version.py` & `oakvar-2.9.94/oakvar/cli/version.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/consts.py` & `oakvar-2.9.94/oakvar/gui/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/job_handlers.py` & `oakvar-2.9.94/oakvar/gui/job_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/multiuser.py` & `oakvar-2.9.94/oakvar/gui/multiuser.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/server.py` & `oakvar-2.9.94/oakvar/gui/server.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/serveradmindb.py` & `oakvar-2.9.94/oakvar/gui/serveradmindb.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/store_handlers.py` & `oakvar-2.9.94/oakvar/gui/store_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/system_handlers.py` & `oakvar-2.9.94/oakvar/gui/system_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/system_message_db.py` & `oakvar-2.9.94/oakvar/gui/system_message_db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/system_worker.py` & `oakvar-2.9.94/oakvar/gui/system_worker.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/userjob.py` & `oakvar-2.9.94/oakvar/gui/userjob.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/util.py` & `oakvar-2.9.94/oakvar/gui/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/web_submit.py` & `oakvar-2.9.94/oakvar/gui/web_submit.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/__init__.py` & `oakvar-2.9.94/oakvar/gui/webresult/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/css/pqselect.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/email.png` & `oakvar-2.9.94/oakvar/gui/webresult/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/favicon.ico` & `oakvar-2.9.94/oakvar/gui/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Black.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BlackItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Bold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLight.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ExtraLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Italic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Light.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Medium.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-Thin.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/Inter.var.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/Inter_Web/inter.css` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/Inter_Web/inter.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-light-webfont.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `oakvar-2.9.94/oakvar/gui/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/arrows-move.svg` & `oakvar-2.9.94/oakvar/gui/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/camera.svg` & `oakvar-2.9.94/oakvar/gui/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/close.png` & `oakvar-2.9.94/oakvar/gui/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/close.svg` & `oakvar-2.9.94/oakvar/gui/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/download-material-black.png` & `oakvar-2.9.94/oakvar/gui/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/download.svg` & `oakvar-2.9.94/oakvar/gui/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/pin.svg` & `oakvar-2.9.94/oakvar/gui/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/plus-circle-dotted.svg` & `oakvar-2.9.94/oakvar/gui/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/sorry.png` & `oakvar-2.9.94/oakvar/gui/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/images/spinner.gif` & `oakvar-2.9.94/oakvar/gui/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/Chart.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/axios.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/axios.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/axios.min.js.map` & `oakvar-2.9.94/oakvar/gui/webresult/js/axios.min.js.map`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/dom-to-image.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/download.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/draggabilly.pkgd.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/draggabilly.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/graphics.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-3.2.1.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery.tools.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/jquery.url.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/masonry.pkgd.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/packery.pkgd.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/pqselect.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/raphael-min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/js/tailwind.min.js` & `oakvar-2.9.94/oakvar/gui/webresult/js/tailwind.min.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/jsonreporter.py` & `oakvar-2.9.94/oakvar/gui/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/css/singlevariantpage.css` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/css/style.css` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/css/widget.css` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/index.html` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/filter.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/filter.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/infomgr.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/infomgr.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/main.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/main.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/setup.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/setup.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/showvariant.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/singlevariantpage.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/util.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/variables.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/js/widgethelper.js` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/nocache/variant.html` & `oakvar-2.9.94/oakvar/gui/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/question.png` & `oakvar-2.9.94/oakvar/gui/webresult/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webresult/webresult.py` & `oakvar-2.9.94/oakvar/gui/webresult/webresult.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websocket_handlers.py` & `oakvar-2.9.94/oakvar/gui/websocket_handlers.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/chat-dots.svg` & `oakvar-2.9.94/oakvar/gui/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/chat-left-text.svg` & `oakvar-2.9.94/oakvar/gui/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/done.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/email.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/empty.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/folder.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/genericmodulelogo.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/hamburger.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/left_arrow.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/new.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/question.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/webstore/images/right_arrow.png` & `oakvar-2.9.94/oakvar/gui/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/images/background.png` & `oakvar-2.9.94/oakvar/gui/websubmit/images/background.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/images/logo.png` & `oakvar-2.9.94/oakvar/gui/websubmit/images/logo.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/images/logo_only.png` & `oakvar-2.9.94/oakvar/gui/websubmit/images/logo_only.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/images/logo_transparent.png` & `oakvar-2.9.94/oakvar/gui/websubmit/images/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/images/logo_transparent_bw.png` & `oakvar-2.9.94/oakvar/gui/websubmit/images/logo_transparent_bw.png`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/inputexamples/exampleinput` & `oakvar-2.9.94/oakvar/gui/websubmit/inputexamples/exampleinput`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/alerts.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/alerts.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/element_getters.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/element_getters.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/index.html` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/input.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/input.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/jobstable.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/jobstable.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/login.html` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/login.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/multiuser.css` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/multiuser.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/multiuser.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/multiuser.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/select_modules.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/select_modules.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/submit.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/submit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/websubmit.css` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/websubmit.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/websubmit/nocache/websubmit.js` & `oakvar-2.9.94/oakvar/gui/websubmit/nocache/websubmit.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/www/assets/index.3526e7ae.css` & `oakvar-2.9.94/oakvar/gui/www/assets/index.3526e7ae.css`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/www/assets/index.5e1d7274.js` & `oakvar-2.9.94/oakvar/gui/www/assets/index.5e1d7274.js`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/www/favicon.ico` & `oakvar-2.9.94/oakvar/gui/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/gui/www/index.html` & `oakvar-2.9.94/oakvar/gui/www/index.html`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/__init__.py` & `oakvar-2.9.94/oakvar/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/exampleinput` & `oakvar-2.9.94/oakvar/lib/assets/exampleinput`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/hg19.chromAlias.txt` & `oakvar-2.9.94/oakvar/lib/assets/hg19.chromAlias.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/hg38.chromAlias.txt` & `oakvar-2.9.94/oakvar/lib/assets/hg38.chromAlias.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/license/LICENSE` & `oakvar-2.9.94/oakvar/lib/assets/license/LICENSE`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/license/liftover.txt` & `oakvar-2.9.94/oakvar/lib/assets/license/liftover.txt`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/annotator/template.md` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/annotator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/annotator/template.py` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/annotator/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/annotator/template.yml` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/annotator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/converter/template.md` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/converter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/converter/template.py` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/converter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/converter/template.yml` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/converter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/mapper/template.md` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/mapper/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/mapper/template.py` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/mapper/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/mapper/template.yml` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/mapper/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/postaggregator/template.md` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/postaggregator/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/postaggregator/template.py` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/postaggregator/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/postaggregator/template.yml` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/postaggregator/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/preparer/template.md` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/preparer/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/preparer/template.py` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/preparer/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/preparer/template.yml` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/preparer/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/reporter/template.md` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/reporter/template.md`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/reporter/template.py` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/reporter/template.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/module_templates/reporter/template.yml` & `oakvar-2.9.94/oakvar/lib/assets/module_templates/reporter/template.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/output_columns.yml` & `oakvar-2.9.94/oakvar/lib/assets/output_columns.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/assets/system.yml` & `oakvar-2.9.94/oakvar/lib/assets/system.yml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/__init__.py` & `oakvar-2.9.94/oakvar/lib/base/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/aggregator.py` & `oakvar-2.9.94/oakvar/lib/base/aggregator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/annotator.py` & `oakvar-2.9.94/oakvar/lib/base/annotator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/app.py` & `oakvar-2.9.94/oakvar/lib/base/app.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/commonmodule.py` & `oakvar-2.9.94/oakvar/lib/base/commonmodule.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/converter.py` & `oakvar-2.9.94/oakvar/lib/base/converter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/mapper.py` & `oakvar-2.9.94/oakvar/lib/base/mapper.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/master_converter.py` & `oakvar-2.9.94/oakvar/lib/base/master_converter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/mp_runners.py` & `oakvar-2.9.94/oakvar/lib/base/mp_runners.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/postaggregator.py` & `oakvar-2.9.94/oakvar/lib/base/postaggregator.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/preparer.py` & `oakvar-2.9.94/oakvar/lib/base/preparer.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/report_filter.py` & `oakvar-2.9.94/oakvar/lib/base/report_filter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/reporter.py` & `oakvar-2.9.94/oakvar/lib/base/reporter.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/runner.py` & `oakvar-2.9.94/oakvar/lib/base/runner.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/base/vcf2vcf.py` & `oakvar-2.9.94/oakvar/lib/base/vcf2vcf.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/consts.py` & `oakvar-2.9.94/oakvar/lib/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/exceptions.py` & `oakvar-2.9.94/oakvar/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/module/__init__.py` & `oakvar-2.9.94/oakvar/lib/module/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/module/cache.py` & `oakvar-2.9.94/oakvar/lib/module/cache.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/module/data_cache.py` & `oakvar-2.9.94/oakvar/lib/module/data_cache.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/module/local.py` & `oakvar-2.9.94/oakvar/lib/module/local.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/module/remote.py` & `oakvar-2.9.94/oakvar/lib/module/remote.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/store/__init__.py` & `oakvar-2.9.94/oakvar/lib/store/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/store/consts.py` & `oakvar-2.9.94/oakvar/lib/store/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/store/db.py` & `oakvar-2.9.94/oakvar/lib/store/db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/store/ov/__init__.py` & `oakvar-2.9.94/oakvar/lib/store/ov/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/store/ov/account/__init__.py` & `oakvar-2.9.94/oakvar/lib/store/ov/account/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/system/__init__.py` & `oakvar-2.9.94/oakvar/lib/system/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/system/consts.py` & `oakvar-2.9.94/oakvar/lib/system/consts.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/__init__.py` & `oakvar-2.9.94/oakvar/lib/util/__init__.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/admin_util.py` & `oakvar-2.9.94/oakvar/lib/util/admin_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     return formats
 
 
 def fn_new_exampleinput(d: str) -> Path:
     from pathlib import Path
     import shutil
 
-    fn = "exampleinput"
+    fn = "oakvar_example.vcf"
     ifn = Path(get_packagedir()) / "lib" / "assets" / fn
     ofn = Path(d) / fn
     shutil.copyfile(ifn, ofn)
     return ofn
 
 
 def create_new_module(module_name: str, module_type: str, outer=None) -> bool:
```

### Comparing `oakvar-2.9.93/oakvar/lib/util/asyn.py` & `oakvar-2.9.94/oakvar/lib/util/asyn.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/db.py` & `oakvar-2.9.94/oakvar/lib/util/db.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/download.py` & `oakvar-2.9.94/oakvar/lib/util/download.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/download_library.py` & `oakvar-2.9.94/oakvar/lib/util/download_library.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/image.py` & `oakvar-2.9.94/oakvar/lib/util/image.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/inout.py` & `oakvar-2.9.94/oakvar/lib/util/inout.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/run.py` & `oakvar-2.9.94/oakvar/lib/util/run.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/seq.py` & `oakvar-2.9.94/oakvar/lib/util/seq.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar/lib/util/util.py` & `oakvar-2.9.94/oakvar/lib/util/util.py`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/oakvar.egg-info/PKG-INFO` & `oakvar-2.9.94/oakvar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oakvar
-Version: 2.9.93
+Version: 2.9.94
 Summary: A genomic variant analysis platform
 Home-page: https://github.com/rkimoakbioinformatics/oakvar
 Author: Ryangguk Kim
 Author-email: rkim@oakbioinformatics.com
 License: UNKNOWN
 Project-URL: Documentation, https://oakvar.readthedocs.io
 Project-URL: Source, https://github.com/rkimoakbioinformatics/oakvar
```

### Comparing `oakvar-2.9.93/oakvar.egg-info/SOURCES.txt` & `oakvar-2.9.94/oakvar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -385,14 +385,15 @@
 oakvar/lib/__init__.py
 oakvar/lib/consts.py
 oakvar/lib/exceptions.py
 oakvar/lib/assets/exampleinput
 oakvar/lib/assets/hg19.chromAlias.txt
 oakvar/lib/assets/hg38.chromAlias.txt
 oakvar/lib/assets/oakvar.yml
+oakvar/lib/assets/oakvar_example.vcf
 oakvar/lib/assets/output_columns.yml
 oakvar/lib/assets/system.yml
 oakvar/lib/assets/license/LICENSE
 oakvar/lib/assets/license/liftover.txt
 oakvar/lib/assets/module_templates/annotator/template.md
 oakvar/lib/assets/module_templates/annotator/template.py
 oakvar/lib/assets/module_templates/annotator/template.yml
```

### Comparing `oakvar-2.9.93/pyproject.toml` & `oakvar-2.9.94/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oakvar-2.9.93/setup.py` & `oakvar-2.9.94/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 long_description = (this_directory / "README.rst").read_text()
 oakvar_files = []
 cravat_files = []
 walk_and_add("oakvar", oakvar_files)
 walk_and_add("cravat", cravat_files)
 setup(
     name="oakvar",
-    version="2.9.93",
+    version="2.9.94",
     description="A genomic variant analysis platform",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/rkimoakbioinformatics/oakvar",
     author="Ryangguk Kim",
     author_email="rkim@oakbioinformatics.com",
     license="",
```

