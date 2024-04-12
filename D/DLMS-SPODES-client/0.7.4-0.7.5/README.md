# Comparing `tmp/DLMS_SPODES_client-0.7.4.tar.gz` & `tmp/DLMS_SPODES_client-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.7.4.tar", last modified: Wed Apr 10 07:25:33 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.7.5.tar", last modified: Fri Apr 12 10:49:29 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.7.4.tar` & `DLMS_SPODES_client-0.7.5.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.702732 DLMS_SPODES_client-0.7.4/
--rw-rw-rw-   0        0        0      526 2024-04-10 07:25:33.701763 DLMS_SPODES_client-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.4/README.md
--rw-rw-rw-   0        0        0      836 2024-04-10 06:51:44.000000 DLMS_SPODES_client-0.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 07:25:33.702732 DLMS_SPODES_client-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.550071 DLMS_SPODES_client-0.7.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.567732 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   122734 2024-04-09 11:08:43.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/client.py
--rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/enums.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.505443 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.585732 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.632731 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      294 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0    10908 2024-01-22 08:39:08.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3438 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.690732 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.692763 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     5634 2024-04-05 09:00:03.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0     3150 2024-04-09 07:47:34.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/services.py
--rw-rw-rw-   0        0        0    34836 2024-04-09 12:26:31.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.580731 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-10 07:25:33.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3301 2024-04-10 07:25:33.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 07:25:33.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-10 07:25:33.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-10 07:25:33.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-10 07:25:33.000000 DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 07:25:33.699742 DLMS_SPODES_client-0.7.4/test/
--rw-rw-rw-   0        0        0     7036 2024-04-08 07:21:09.000000 DLMS_SPODES_client-0.7.4/test/test_Client.py
--rw-rw-rw-   0        0        0      251 2024-04-09 08:34:38.000000 DLMS_SPODES_client-0.7.4/test/test_services.py
--rw-rw-rw-   0        0        0      164 2023-12-12 05:44:33.000000 DLMS_SPODES_client-0.7.4/test/конфигурация GSM.csv
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.965379 DLMS_SPODES_client-0.7.5/
+-rw-rw-rw-   0        0        0      526 2024-04-12 10:49:29.964380 DLMS_SPODES_client-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.7.5/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-12 10:48:02.000000 DLMS_SPODES_client-0.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 10:49:29.965379 DLMS_SPODES_client-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.779380 DLMS_SPODES_client-0.7.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.803419 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   113785 2024-04-12 08:17:20.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/client.py
+-rw-rw-rw-   0        0        0      323 2024-02-02 12:40:34.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/enums.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.731492 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.828381 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.886378 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.951378 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.953378 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1586 2024-02-02 08:19:41.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     5599 2024-04-11 08:53:09.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3188 2024-04-11 13:02:39.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    43047 2024-04-12 09:08:36.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.822384 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-12 10:49:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3248 2024-04-12 10:49:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 10:49:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-12 10:49:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-12 10:49:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-12 10:49:29.000000 DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.7.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:49:29.961411 DLMS_SPODES_client-0.7.5/test/
+-rw-rw-rw-   0        0        0     8082 2024-04-12 09:11:11.000000 DLMS_SPODES_client-0.7.5/test/test_Client.py
+-rw-rw-rw-   0        0        0      251 2024-04-09 08:34:38.000000 DLMS_SPODES_client-0.7.5/test/test_services.py
+-rw-rw-rw-   0        0        0      164 2023-12-12 05:44:33.000000 DLMS_SPODES_client-0.7.5/test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.7.4/PKG-INFO` & `DLMS_SPODES_client-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.7.4
+Version: 0.7.5
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.4/pyproject.toml` & `DLMS_SPODES_client-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.7.4"
+version = "0.7.5"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS-SPODES == 0.69.4",
+    "DLMS-SPODES == 0.69.5",
     "DLMS-SPODES-communications >= 1.2.4",
     "pycryptodomex>=3.15"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=['dlms', 'spodes', 'client']
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import time
 from functools import cached_property, reduce
 from struct import pack
 from collections import deque
 from itertools import count
-from enum import IntEnum, auto
+from enum import IntEnum, auto, IntFlag
 from typing import TextIO, Deque, Any
 import threading
 import datetime
 import os
 import hashlib
 from Cryptodome.Cipher import AES
-from DLMS_SPODES_communications import Network, SerialPort, RS485, BLE, AsyncNetwork, AsyncSerial
+from DLMS_SPODES_communications import Network, SerialPort, RS485, BLE, AsyncNetwork, AsyncSerial, base
 from DLMS_SPODES.cosem_interface_classes import collection, overview
 from DLMS_SPODES.cosem_interface_classes.collection import Collection, InterfaceClass, ic, cdt, cst, ut, Data, AssociationLN
 from DLMS_SPODES.cosem_interface_classes.security_setup.ver1 import SecuritySuite
 from DLMS_SPODES.enums import (
     Transmit, Application, ActionRequest, ReadResponse, ServiceError, AssociationResult, Conformance, SetRequest, ConfirmedServiceError, AARQapdu, ACSEAPDU, XDLMSAPDU,
     VariableAccessSpecification, AcseServiceUser
 )
 from DLMS_SPODES.cosem_interface_classes.association_ln import mechanism_id
-from DLMS_SPODES.cosem_interface_classes.association_ln.ver0 import AuthenticationMechanismName
+from DLMS_SPODES.cosem_interface_classes.association_ln.authentication_mechanism_name import AuthenticationMechanismName
 from DLMS_SPODES.hdlc import frame, sub_layer, negotiation
 from DLMS_SPODES.version import AppVersion
 from DLMS_SPODES import pdu_enums as pdu, exceptions as exc
 from DLMS_SPODES.types.implementations import enums, long_unsigneds, bitstrings, octet_string, structs
 from .gurux_common.enums.TraceLevel import TraceLevel
 from .gurux_dlms import GXDLMSSettings, GXByteBuffer, GXReplyData, GXDLMSException
 from .gurux_dlms.enums import InterfaceType, Security, Standard, BerType, RequestTypes, Service
-from .gurux_dlms.ConnectionState import ConnectionState
 from .gurux_dlms.GXDLMS import GXDLMS
 from .gurux_dlms.GXDLMSLNParameters import GXDLMSLNParameters
 from .gurux_dlms.GXDLMSSNParameters import GXDLMSSNParameters
 from .gurux_dlms.AesGcmParameter import AesGcmParameter
 from .gurux_dlms.GXCiphering import GXCiphering
 from .gurux_dlms.GXDLMSConfirmedServiceError import GXDLMSConfirmedServiceError
 from .gurux_dlms.GXDLMSChippering import GXDLMSChippering
@@ -92,19 +91,29 @@
         """ more importance error or None if errors is absence"""
         try:
             return reduce(lambda a, b: a if a.importance > b.importance else b, self.keys())
         except TypeError:  # errors is empty
             return None
 
 
+class ConnectionState(IntFlag):
+    NONE = 0
+    """no connection"""
+    HDLC = auto()
+    """HDLC level"""
+    DLMS = auto()
+    """DLMS association level."""
+
+
 class Client:
     id_count = count()
-    __status: Status
+    status: Status
+    connection_state: ConnectionState
     log_file: TextIO
-    media: Network | SerialPort | RS485 | BLE | AsyncNetwork | AsyncSerial | None
+    media: Network | SerialPort | RS485 | BLE | base.StreamBase | None
     lock: threading.Lock
     errors: Errors
     last_transfer_time: datetime.timedelta | None
     connection_time_release: int
     received_frames: Deque[frame.Frame]
     __stop_transfer: bool
     current_obj: InterfaceClass | None
@@ -126,25 +135,26 @@
     addr_size: frame.AddressLength
     logging_disable: bool
 
     def __init__(self,
                  SAP: int = 0x10,
                  secret: str = "",
                  conformance: str = None,
-                 addr_size: int = -1):
+                 addr_size: int = -1,
+                 media: base.StreamBase = AsyncSerial(port="COM3")):
         self.__id = next(Client.id_count)
         """for identification before LDN reading"""
         self.logging_disable = False
         """turn off logging by default"""
         self.objects = None
         self.__sap = enums.ClientSAP(SAP)
         """Service Access Point. Default <Public>"""
         self.server_SAP = long_unsigneds.ServerSAP(1)
         self.secret = bytes.fromhex(secret)
-        self.__status = Status.READY
+        self.status = Status.READY
         # file_name = F"./Logs/{id_}.log"
         self.trace = TraceLevel.VERBOSE
         self.protocol_version = cdt.BitString('1')  # max 8 bit
         """ Protocol Version of the AARQ APDU """
         # TODO: REMOVE IT BULLSHIT
         self.invocationCounter = '0.0.43.1.0.255'
         self.lock = threading.Lock()
@@ -175,18 +185,19 @@
         self.reply = GXReplyData()
         """ use gurux reply class now """
 
         self.received_frames = deque()
         """ HDLC frames container from server """
 
         self.send_frames = deque()
+        self.connection_state = ConnectionState.NONE
         self.settings = GXDLMSSettings(False)
         self.settings.interfaceType = InterfaceType.HDLC
 
-        self.media = AsyncSerial(port="COM3")
+        self.media = media
         """ physical layer """
 
         # TODO: TEMPORARY COMMENT
         # if self.trace > TraceLevel.WARNING:
         #     self.log(INFO, F'Authentication: {self.objects.current_association.authentication_mechanism_name.mechanism_id_element} ClientAddress: {self.objects.current_association.associated_partners_id.client_SAP} '
         #                 F'ServerAddress: {self.objects.current_association.associated_partners_id.server_SAP}/{int(self.objects.getIECHDLCSetup(self.get_channel_index()).device_address)}')
 
@@ -236,49 +247,44 @@
     def reset_stop_transfer(self):
         self.__stop_transfer = False
 
     @property
     def is_stop_request(self) -> bool:
         return self.__stop_transfer
 
-    @property
-    def status(self) -> Status:
-        """ return connection status """
-        return self.__status
-
     def set_error(self, key: Transmit | Application, message: str):
         if key == Transmit.OK and self.errors.get(Transmit.OK) is not None:
             self.errors[key] += message
         else:
             self.errors[key] = message
         self.__set_status(key)
 
     def __set_status(self, key: Transmit | Application = None):
         """ set status by result after exchange """
         key = self.errors.importance if key is None else key
         match key:
             case Transmit.OK:
                 self.__stop_transfer = False
-                self.__status = Status.READY
-            case Transmit.TIMEOUT:                           self.__status = Status.TIMEOUT
-            case Transmit.READ_ERROR | Transmit.WRITE_ERROR: self.__status = Status.STOP
+                self.status = Status.READY
+            case Transmit.TIMEOUT:                           self.status = Status.TIMEOUT
+            case Transmit.READ_ERROR | Transmit.WRITE_ERROR: self.status = Status.STOP
             case Transmit.ABORT:
-                self.__status = Status.MANUAL_STOP
+                self.status = Status.MANUAL_STOP
                 self.__stop_transfer = False
-            case Transmit.EXECUTE_ERROR:                     self.__status = Status.EXECUTE_ERROR
-            case Transmit.NO_ACCESS:                         self.__status = Status.NO_ACCESS
-            case Transmit.NO_TRANSPORT:                      self.__status = Status.NO_TRANSPORT
-            case Application.MISSING_OBJ:                    self.__status = Status.MISSING_OBJ
-            case Application.VERSION_ERROR:                  self.__status = Status.VERSION_ERROR
-            case Transmit.NO_PORT:                           self.__status = Status.NO_PORT
-            case Application.ID_ERROR:                       self.__status = Status.ID_ERROR
-            case Application.VALUE_ERROR:                    self.__status = Status.UNKNOWN  # TODO: new image for <value error>
-            case Transmit.UNKNOWN:                           self.__status = Status.UNKNOWN
-            case Application.WAITING_RESULT:                 self.__status = Status.UNKNOWN
-            case Application.OK:                             self.__status = Status.READY
+            case Transmit.EXECUTE_ERROR:                     self.status = Status.EXECUTE_ERROR
+            case Transmit.NO_ACCESS:                         self.status = Status.NO_ACCESS
+            case Transmit.NO_TRANSPORT:                      self.status = Status.NO_TRANSPORT
+            case Application.MISSING_OBJ:                    self.status = Status.MISSING_OBJ
+            case Application.VERSION_ERROR:                  self.status = Status.VERSION_ERROR
+            case Transmit.NO_PORT:                           self.status = Status.NO_PORT
+            case Application.ID_ERROR:                       self.status = Status.ID_ERROR
+            case Application.VALUE_ERROR:                    self.status = Status.UNKNOWN  # TODO: new image for <value error>
+            case Transmit.UNKNOWN:                           self.status = Status.UNKNOWN
+            case Application.WAITING_RESULT:                 self.status = Status.UNKNOWN
+            case Application.OK:                             self.status = Status.READY
             case None:                                       pass
             # TODO: other cases
 
     def get_frame(self, read_data: bytearray) -> frame.Frame | None:
         while len(read_data) != 0:
             new_frame = frame.Frame.try_from(read_data)
             self.reply.complete = True
@@ -512,15 +518,15 @@
                 case XDLMSAPDU.GLO_READ_REQUEST | XDLMSAPDU.GLO_WRITE_REQUEST | XDLMSAPDU.GLO_GET_REQUEST | XDLMSAPDU.GLO_SET_REQUEST | XDLMSAPDU.GLO_ACTION_REQUEST | \
                      XDLMSAPDU.DED_GET_REQUEST | XDLMSAPDU.DED_SET_REQUEST | XDLMSAPDU.DED_ACTION_REQUEST:
                     if self.settings.cipher is None:
                         raise ValueError("Secure connection is not supported.")
                     if (self.reply.moreData & RequestTypes.FRAME) == 0:
                         self.reply.data.position = self.reply.data.position - 1
                         p = None
-                        if self.settings.cipher.dedicatedKey and (self.settings.connected & ConnectionState.DLMS) != 0:
+                        if self.settings.cipher.dedicatedKey and (self.connection_state & ConnectionState.DLMS) != 0:
                             p = AesGcmParameter(self.settings.sourceSystemTitle, self.settings.cipher.dedicatedKey, self.settings.cipher.authenticationKey)
                         else:
                             p = AesGcmParameter(self.settings.sourceSystemTitle, self.settings.cipher.blockCipherKey, self.settings.cipher.authenticationKey)
                         tmp = GXCiphering.decrypt(self.settings.cipher, p, self.reply.data)
                         self.reply.data.clear()
                         self.reply.data.set(tmp)
                         self.reply.command = XDLMSAPDU(self.reply.data.getUInt8())
@@ -536,15 +542,15 @@
                     if self.settings.cipher is None:
                         raise ValueError("Secure connection is not supported.")
                     if (self.reply.moreData & RequestTypes.FRAME) == 0:
                         self.reply.data.position = self.reply.data.position - 1
                         bb = GXByteBuffer(self.reply.data)
                         self.reply.data.size = self.reply.data.position = index
                         p = None
-                        if self.settings.cipher.dedicatedKey and (self.settings.connected & ConnectionState.DLMS) != 0:
+                        if self.settings.cipher.dedicatedKey and (self.connection_state & ConnectionState.DLMS) != 0:
                             p = AesGcmParameter(0, self.settings.sourceSystemTitle, self.settings.cipher.dedicatedKey, self.settings.cipher.authenticationKey)
                         else:
                             p = AesGcmParameter(0, self.settings.sourceSystemTitle, self.settings.cipher.blockCipherKey, self.settings.cipher.authenticationKey)
                         self.reply.data.set(GXCiphering.decrypt(self.settings.cipher, p, bb))
                         self.reply.command = None
                         self.getPdu()
                         self.reply.cipherIndex = self.reply.data.size
@@ -771,15 +777,15 @@
                 case 4:                        raise exc.NoObject
                 case _:                        raise GXDLMSException(self.reply.error)
             if self.received_frames[-1].control.is_info() or self.received_frames[-1].control == frame.Control.UI_PF:
                 if self.received_frames[-1].is_segmentation:
                     """pass handle frame. wait all information"""
                 else:
                     llc = sub_layer.LLC(frame.Frame.join_info(self.received_frames))
-                    self.log(logL.DEB, F'LLC[{len(llc.info)}]: {llc}...')
+                    # self.log(logL.DEB, F'LLC[{len(llc.info)}]: {llc}...')
 
                     self.reply.data.position = len(self.reply.data)
                     self.reply.data.set(llc.info)
                     ret = self.getPdu()
 
                     # TODO: LLC to PDU
             else:
@@ -987,157 +993,14 @@
                 case {SerialPort.__class__.__name__: dict_}:
                     self.media = eval(F"SerialPort({dict_})")
                 case _: raise ValueError(F"unknown type: {value.__class__.__name__} for set communication channel {self}")
             self.log(logL.INFO, F"set2 to {self} communication channel: {self.media}")
         except Exception as e:
             self.log(logL.ERR, F"not set to {self} communication channel by {value}")
 
-    async def connect(self, is_public: bool = False):
-        """ connect to server with opening port"""
-        self.__status = Status.EXCHANGE
-        self.set_error(Transmit.OK, "Open port")
-        # elif self.__lock.locked():
-        #     self.log(logL.WARN, F"locked by {self.locker_name}")
-        #     if isinstance(self.media, SerialPort):
-        #         raise exc.NoTransport("temporary locked for serial port")
-        # init SA, DA, device_address
-        # if int(self.device_address) == 0:
-        #     self.device_address.set(self.objects.getIECHDLCSetup(self.get_channel_index()).device_address)
-        # match self.media:
-        #     case RS485():                          lower_addr = int(self.device_address)
-        #     case SerialPort() | Network() | BLE(): lower_addr = None
-        #     case err:                              raise ValueError(F"unknouwn {self.media=}")
-        self.errors.clear()  # clear all last session errors
-        self.send_frames.clear()
-        try:
-            # calculate addresses
-            self.DA = frame.Address(
-                upper_address=int(self.server_SAP),
-                lower_address=int(self.device_address) if self.device_address else None,
-                length=self.addr_size
-            )
-            self.SA = frame.Address(upper_address=0x10 if is_public else int(self.SAP))
-            self.log(logL.INFO, F"{self.SA=} {self.DA=}")
-            # initialize connection
-            self.reply.clear()
-            if self.settings.cipher.security != Security.NONE:
-                self.log(logL.DEB, F"Security: {self.settings.cipher.security}/n"
-                                   F"System title: {self.settings.cipher.systemTitle.hex()}"
-                                   F"Authentication key: {self.settings.cipher.authenticationKey.hex()}"
-                                   F"Block cipher key: {self.settings.cipher.blockCipherKey.hex()}")
-                if self.settings.cipher.dedicatedKey:
-                    self.log(logL.DEB, F"Dedicated key: {self.settings.cipher.dedicatedKey.hex()}")
-            # update Frame Counter
-            if self.invocationCounter and self.settings.cipher is not None and self.settings.cipher.security != Security.NONE:
-                # create IC object. TODO: remove it after close connection, maybe???
-                self.settings.proposedConformance |= Conformance.GENERAL_PROTECTION
-
-                #my block
-                IC: Data = self.objects.add_if_missing(ut.CosemClassId(1),
-                                                       logical_name=cst.LogicalName(bytearray((0, self.get_channel_index(), 43, 1,
-                                                                                               self.current_association.security_setup_reference.e, 255))),
-                                                       version=cdt.Unsigned(0))
-                tmp_client_SAP = self.current_association.associated_partners_id.client_SAP
-                challenge = self.settings.ctoSChallenge
-                try:
-                    self.current_association.associated_partners_id.client_SAP.set(0x10)
-                    self.get_SNRM_request()
-                    self.__status = Status.READ
-                    await self.read_data_block()
-                    self.objects.getIECHDLCSetup(self.get_channel_index()).set_from_info(self.reply.data.get_data())
-                    self.settings.connected = ConnectionState.HDLC
-                    self.reply.clear()
-                    self.aarqRequest(self.m_id)
-                    await self.read_data_block()
-                    self.parseAareResponse(self.reply.data)
-                    self.reply.clear()
-                    self.read_attribute(IC, 2)
-                    self.settings.cipher.invocationCounter = 1 + IC.value.decode()
-                    self.log(logL.DEB, "Invocation counter: " + str(self.settings.cipher.invocationCounter))
-                    # disconnect
-                    if self.media and self.media.is_open():
-                        self.log(logL.DEB, "DisconnectRequest")
-                        self.disconnect_request()
-                finally:
-                    self.SAP = tmp_client_SAP
-                    self.settings.useCustomChallenge = challenge is not None
-                    self.settings.ctoSChallenge = challenge
-
-                # gurux with several removed methods
-                # add = self.settings.clientAddress
-                # auth = self.settings.authentication
-                # security = self.client.ciphering.security
-                # challenge = self.client.ctoSChallenge
-                # try:
-                #     self.client.clientAddress = 16
-                #     self.settings.authentication = Authentication.NONE
-                #     self.client.ciphering.security = Security.NONE
-                #     reply = GXReplyData()
-                #     self.get_SNRM_request()
-                #     self.__status = Status.READ
-                #     self.read_data_block2()
-                #     self.objects.IEC_HDLS_setup.set_from_info(self.reply.data.get_data())
-                #     self.settings.connected = ConnectionState.HDLC
-                #     self.reply.clear()
-                #     self.aarqRequest()
-                #     self.read_data_block2()
-                #     self.parseAareResponse(reply.data)
-                #     reply.clear()
-                #     item = GXDLMSData(self.invocationCounter)
-                #     data = self.client.read(item, 2)[0]
-                #     reply = GXReplyData()
-                #     self.read_data_block(data, reply)
-                #     item.encodings[2] = reply.data.get_data()
-                #     Update data type on read.
-                #     if item.getDataType(2) == cdt.NullData.TAG:
-                #         item.setDataType(2, reply.valueType)
-                #     self.client.updateValue(item, 2, reply.value)
-                #     self.client.ciphering.invocationCounter = 1 + item.value
-                #     print("Invocation counter: " + str(self.client.ciphering.invocationCounter))
-                #     if self.media and self.media.isOpen():
-                #         self.log(logL.INFO, "DisconnectRequest")
-                #         self.disconnect_request()
-                # finally:
-                #     self.settings.clientAddress = add
-                #     self.settings.authentication = auth
-                #     self.client.ciphering.security = security
-                #     self.client.ctoSChallenge = challenge
-
-            #  SNRM request is not used in network connections.
-            if self.settings.interfaceType == InterfaceType.HDLC:
-                self.get_SNRM_request()
-                self.__status = Status.READ
-                await self.read_data_block()
-                self.__status = Status.EXCHANGE
-                self.settings.connected = ConnectionState.HDLC
-                self.reply.clear()
-                self.aarqRequest(mechanism_id.NONE if is_public else self.m_id)
-                await self.read_data_block()
-                # await self.read_attr(ut.CosemAttributeDescriptor((collection.ClassID.ASSOCIATION_LN, ut.CosemObjectInstanceId("0.0.40.0.0.255"), ut.CosemObjectAttributeId(6)))) # for test only
-            match self.parseAareResponse(self.reply.data):
-                case AcseServiceUser.NULL:                                             self.log(logL.INFO, 'Authentication success')
-                case AcseServiceUser.AUTHENTICATION_FAILURE as diag if is_public: self.log(logL.WARN, F'On Public connection type got {diag.name}, broad force turn ON')
-                case AcseServiceUser.AUTHENTICATION_REQUIRED:
-                    self.reply.clear()
-                    self.getApplicationAssociationRequest()
-                    await self.read_data_block()
-                    self.parseApplicationAssociationResponse()
-                case _ as diagnostic:                                                   raise exc.AssociationResultError(diagnostic)
-            self.set_error(Transmit.OK, "Initialize connection")
-            # TODO: remove DIMA crutch dummy read for correct write
-            if self.objects is not None:
-                self.get_get_request_normal(self.objects.LDN.get_attr_descriptor(2))
-                await self.read_data_block()
-                self.matching_LDN(octet_string.LDN(self.reply.data.get_data()))
-            return
-        except GXDLMSException as e:
-            raise exc.UnknownError(F'При соединении {e}')
-        except TimeoutError as e:
-            raise exc.Timeout('При соединении')
-
     async def close(self):
         """ send DISC to server and after close media """
         self.log(logL.DEB, "DisconnectRequest")
         try:
             # Release is call only for secured connections. All meters are not supporting Release and it's causing problems.
             if self.settings.interfaceType == InterfaceType.WRAPPER or \
                     (self.settings.interfaceType == InterfaceType.HDLC and self.settings.cipher.security != Security.NONE):
@@ -1148,24 +1011,24 @@
             pass
             #  All meters don't support release.
         try:
             await self.disconnect_request()
         except Exception as e:
             self.log(logL.ERR, F'Disconnect request ERROR: {e.args[0]}')
         self.log(logL.DEB, F'Close communication channel: {self.media}')
-        if self.__status == Status.CONNECTED:
-            self.__status = Status.READY
+        if self.status == Status.CONNECTED:
+            self.status = Status.READY
 
     async def disconnect_request(self, force=False):
         """ Sent to server DISC """
         # self.settings.maxPduSize = int(self.current_association.xDLMS_context_info.max_receive_pdu_size)
-        if not force and self.settings.connected == ConnectionState.NONE:
+        if not force and self.connection_state == ConnectionState.NONE:
             return
         if self.settings.interfaceType == InterfaceType.HDLC:
-            self.settings.connected = ConnectionState.NONE
+            self.connection_state = ConnectionState.NONE
             self.add_frames_to_queue(frame.Control.DISC_P)
         else:
             self.releaseRequest()
         await self.read_data_block()
 
     def matching_LDN(self, value: octet_string.LDN):
         if value == self.objects.LDN.value:
@@ -1215,22 +1078,22 @@
                 tmp2.set(self.settings.cipher.systemTitle)
                 tmp2.set(self.settings.ctoSChallenge)
                 tmp2.set(self.settings.stoCChallenge)
                 secret = tmp2.array()
             case mechanism_id.HIGH:                      secret = self.secret
             case mechanism_id.HIGH_ECDSA:                raise ValueError("ECDSA is not supported.")
             case _ as mech_id:                                    raise ValueError(F'{mech_id} is not supported')
-        tmp = self.secure(ic, self.settings.getCtoSChallenge(), bytes(secret))
+        tmp = self.secure(ic, self.settings.ctoSChallenge, bytes(secret))
         challenge = cdt.OctetString(bytearray(tmp))
         equals = challenge == value
         if not equals:
             self.log(logL.DEB, "Invalid StoC:" + GXByteBuffer.hex(value, True) + "-" + GXByteBuffer.hex(tmp, True))
         if not equals:
             raise Exception("parseApplicationAssociationResponse failed. " + " Server to Client do not match.")
-        self.settings.connected |= ConnectionState.DLMS
+        self.connection_state |= ConnectionState.DLMS
 
     def secure(self, ic, data, secret: bytes) -> bytes:
         """ TODO: """
         if not isinstance(secret, bytes):
             raise ValueError(F'cipher is not bytes type, got {secret.__class__}')
         #  Get server Challenge.
         challenge = GXByteBuffer()
@@ -1623,15 +1486,15 @@
         return resultDiagnosticValue
 
     def parseAareResponse(self, reply) -> AcseServiceUser:
         """ TODO: need refactoring. Parses the AARE response.  Parse method will update the following data: DLMSVersion, MaxReceivePDUSize, UseLogicalNameReferencing, LNSettings or SNSettings,
         LNSettings or SNSettings will be updated, depending on the referencing, Logical name or Short name.
         Received data. GXDLMSClient#aarqRequest GXDLMSClient#useLogicalNameReferencing GXDLMSClient#negotiatedConformance GXDLMSClient#proposedConformance """
         if (ret := self.parseAARE(reply)) != AcseServiceUser.AUTHENTICATION_REQUIRED:
-            self.settings.connected = self.settings.connected | ConnectionState.DLMS
+            self.connection_state = self.connection_state | ConnectionState.DLMS
         if self.settings.dlmsVersion != 6:
             raise ValueError("Invalid DLMS version number.")
         return ret
 
     def generate_user_information(self, cipher, encryptedData) -> bytes:
         info = pack('B', BerType.CONTEXT | BerType.CONSTRUCTED | AARQapdu.USER_INFORMATION)
         if not cipher or not cipher.isCiphered():
@@ -1678,27 +1541,18 @@
             self.quality_of_service,
             self.objects.dlms_ver if self.objects else self.DEF_DLMS_VER,
             b'\x5f\x1f\x04\x00',        # <5f1f> Tag for conformance block + <04>length of the conformance block + <00> encoding the number of unused bits in the bit string
             self.proposed_conformance.contents,
             self.receive_pdu_size)
         return info
 
-    @property
-    def mechanism_name(self) -> bytes:
-        if self.objects is None:
-            ret = AuthenticationMechanismName()
-            ret.mechanism_id_element.set(int(self.m_id))
-            return ret.get_a_xdr()
-        else:
-            return self.current_association.authentication_mechanism_name.get_a_xdr()
-
     def aarqRequest(self, m_id: mechanism_id.MechanismIdElement):
         """ Generate AARQ request.  Because all_ meters can't read all_ data in one packet, the packet must be split first, by using SplitDataToPackets method.  AARQ request as
         byte array. @see GXDLMSClient#parseAareResponse """
-        self.settings.connected = self.settings.connected & ~ConnectionState.DLMS
+        self.connection_state = self.connection_state & ~ConnectionState.DLMS
         info = bytes()
         self.settings.resetBlockIndex()
         self.settings.setStoCChallenge(None)
         # if self.auto_increase_invoke_ID:
         #     self.settings.setInvokeID(0)
         # else:
         #     self.settings.setInvokeID(1)
@@ -1727,15 +1581,17 @@
             info += pack(F'4sB',
                          b'\xa9\x03\x02\x01',
                          self.settings.userId)
         # Retrieves the string that indicates the level of authentication, if any.
         if m_id != mechanism_id.NONE or (self.settings.cipher and self.settings.cipher.security != Security.NONE):
             info += b'\x8a\x02\x07\x80'
             # Where: 8b - Tag(CONTEXT(0x80) + AARQ-apdu.MECHANISM_NAME(0x0b)), 07 - info length
-            info += b'\x8b\x07' + self.mechanism_name
+            info += b'\x8b\x07' + AuthenticationMechanismName.get_AARQ_mechanism_name(
+                cryptographic=2,
+                algorithm_id=int(m_id))
         #  Add Calling authentication information.
         if m_id != mechanism_id.NONE:
             if m_id == mechanism_id.LOW:
                 c_a_v = self.secret
                 """ calling-authentication-value """
             elif m_id == mechanism_id.HIGH:
                 self.settings.ctoSChallenge = os.urandom(16)
@@ -1997,15 +1853,15 @@
             info = pack('H', len(info)) + info
         buff = GXByteBuffer(info)
         if self.settings.getUseLogicalNameReferencing():
             p = GXDLMSLNParameters(self.settings, 0, ACSEAPDU.RLRQ, 0, buff, None, 0xff)
             reply = self.getLnMessages(p)
         else:
             reply = self.getSnMessages(GXDLMSSNParameters(self.settings, ACSEAPDU.RLRQ, 0xFF, 0xFF, None, buff))
-        self.settings.connected = self.settings.connected & ~ConnectionState.DLMS
+        self.connection_state = self.connection_state & ~ConnectionState.DLMS
         return reply
 
     @classmethod
     def getGloMessage(cls, command: XDLMSAPDU | ACSEAPDU) -> XDLMSAPDU | ACSEAPDU:
         """ Get used glo message. Executed command. Integer value of glo message."""
         match command:
             case XDLMSAPDU.READ_REQUEST:      return XDLMSAPDU.GLO_READ_REQUEST
@@ -2039,15 +1895,15 @@
             case _:                         raise Exception("Invalid DED command.")
 
     def cipher0(self, p: GXDLMSLNParameters, data: GXByteBuffer):
         cmd = 0
         key = None
         cipher = p.settings.cipher
         if not self.negotiated_conformance.general_protection:
-            if cipher.dedicatedKey and (p.settings.connected & ConnectionState.DLMS) != 0:
+            if cipher.dedicatedKey and (p.connection_state & ConnectionState.DLMS) != 0:
                 cmd = self.getDedMessage(p.command)
                 key = cipher.dedicatedKey
             else:
                 cmd = self.getGloMessage(p.command)
                 key = cipher.blockCipherKey
         else:
             if cipher.dedicatedKey:
@@ -2078,15 +1934,15 @@
     def current_association(self) -> AssociationLN:
         return self.objects.getAssociationBySAP(self.SAP)
 
     def get_SNRM_request(self):
         """ Generates SNRM request.  his method is used to generate send SNRMRequest. Before the SNRM request can be generated, at least the following properties must be set:
         ClientAddress, ServerAddress.
         According to IEC 62056-47: when communicating using TCP/IP, the SNRM request is not send. """
-        self.settings.connected = ConnectionState.NONE
+        self.connection_state = ConnectionState.NONE
         self.add_frames_to_queue(control=frame.Control.SNRM_P)
 
     def add_frames_to_queue(self, control: frame.Control, data: bytes = bytes()):
         """ Create and set new frames to queue """
         new_frames: Deque[frame.Frame] = deque()
         """ frames container """
         if control == frame.Control.SNRM_P:
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,10 @@
-#
-#  --------------------------------------------------------------------------
-#   Gurux Ltd
-#
-#
-#
-#  Filename: $HeadURL$
-#
-#  Version: $Revision$,
-#                   $Date$
-#                   $Author$
-#
-#  Copyright (c) Gurux Ltd
-#
-# ---------------------------------------------------------------------------
-#
-#   DESCRIPTION
-#
-#  This file is a part of Gurux Device Framework.
-#
-#  Gurux Device Framework is Open Source software; you can redistribute it
-#  and/or modify it under the terms of the GNU General Public License
-#  as published by the Free Software Foundation; version 2 of the License.
-#  Gurux Device Framework is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
-#  See the GNU General Public License for more details.
-#
-#  More information of Gurux products: http://www.gurux.org
-#
-#  This code is licensed under the GNU General Public License v2.
-#  Full text may be retrieved at http://www.gnu.org/licenses/gpl-2.0.txt
-# ---------------------------------------------------------------------------
 from __future__ import print_function
 from ..gurux_dlms.GXCiphering import GXCiphering
 from .enums import Priority, ServiceClass, InterfaceType, Authentication, Standard
-from .ConnectionState import ConnectionState
 from DLMS_SPODES.hdlc.frame import Control
 from DLMS_SPODES.enums import Conformance
 
 
 class GXDLMSSettings:
     """ This class includes DLMS communication settings. """
     ctoSChallenge: bytes | None
@@ -68,15 +34,14 @@
         self.password = None
         self.kek = None
         self.count = 0
         self.index = 0
         self.targetEphemeralKey = None
         self.dlmsVersion = 6
         """ deprecated """
-        self.connected = ConnectionState.NONE
         self.allowAnonymousAccess = False
         self.maxPduSize = 0xFFFF
         self.maxServerPDUSize = 0xFFFF
         self.startingPacketIndex = 1
         # Gets current block index.
         self.blockIndex = 1
         self.cipher = GXCiphering("ABCDEFGH".encode())
@@ -95,69 +60,36 @@
         self.negotiatedConformance = Conformance.NONE
         self.receiverFrame = Control.S0_R0  # 0
         self.senderFrame = Control.S0_R0      # 0
         self.command = 0
         self.commandType = 0
         self.useUtc2NormalTime = False
 
-    def getCtoSChallenge(self):
-        """ Client to Server challenge getter """
-        return self.ctoSChallenge
-
     def setCtoSChallenge(self, value):
         """ Client to Server challenge setter """
         if not self.customChallenges or self.ctoSChallenge is None:
             self.ctoSChallenge = value
 
     def getStoCChallenge(self):
         """ Server to Client challenge getter """
         return self.stoCChallenge
 
     def setStoCChallenge(self, value):
         """ Server to Client challenge setter """
         if not self.customChallenges or self.stoCChallenge is None:
             self.stoCChallenge = value
 
-    def is_connection_accept(self):
-        return self.connected != ConnectionState.NONE or self.allowAnonymousAccess or (self.cipher and self.cipher.sharedSecret)
-
     def resetFrameSequence(self):
         if self.isServer:
             self.senderFrame = Control.S7_R0_PF
             self.receiverFrame = Control.S7_R7_PF
         else:
             self.senderFrame = Control.S7_R7_PF
             self.receiverFrame = Control.S7_R0_PF
 
-    def checkFrame(self, control: Control):
-        #  If notify
-        if control == Control.UI_PF:
-            return True
-        if control.is_unnumbered():
-            if control in (Control.UA_F, Control.SNRM_P):
-                self.resetFrameSequence()
-                return True
-            expected = 0
-        elif control.is_supervisory():
-            self.receiverFrame = Control.next_receiver_sequence(self.receiverFrame)
-            return True
-        elif self.senderFrame.is_info():
-            expected = Control.next_receiver_sequence(Control.next_send_sequence(self.receiverFrame))
-            if control == expected:
-                self.receiverFrame = control
-                return True
-        else:
-            expected = Control.next_send_sequence(self.receiverFrame)
-            #  If answer for RR.
-            if control == expected:
-                self.receiverFrame = control
-                return True
-        print("Invalid HDLC Frame: " + hex(control) + " Expected: " + hex(expected))
-        return False
-
     def getNextSend(self, is_first: bool) -> int:
         """  Generates I-frame. Is this first packet. """
         if is_first:
             self.senderFrame = Control.next_receiver_sequence(Control.next_send_sequence(self.senderFrame))
         else:
             self.senderFrame = Control.next_send_sequence(self.senderFrame)
         return self.senderFrame
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .ConnectionState import ConnectionState
 from .ResponseType import ResponseType
 from .GXByteBuffer import GXByteBuffer
 from .GXDLMS import GXDLMS
 from .GXDLMSConfirmedServiceError import GXDLMSConfirmedServiceError
 from .GXDLMSException import GXDLMSException
 from .GXDLMSLNParameters import GXDLMSLNParameters
 from .GXDLMSSettings import GXDLMSSettings
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/servers.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,16 @@
             c.set_error(Transmit.NO_TRANSPORT, F"При соединении{e}")
             result.complete = True
             result.errors = c.errors
             return result
     #
     try:
         if c.objects is None:
-            await c.connect(True)
-            await task.InitType().exchange(c)
-            await c.close()  # todo: change to DiscRequest
-        await c.connect(is_public)
+            await task.InitType().exchange(c, is_public=True)
+            await c.close()  # todo: change to DiscRequest, or make not closed
         result.value = await t.exchange(c)
         await c.close()  # todo: change to DiscRequest
     except TimeoutError as e:
         c.set_error(Transmit.TIMEOUT, 'Таймаут при обмене')
     except exc.DLMSException as e:
         c.set_error(e.error, e.args[0])
     except Exception as e:
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/services.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,13 +66,14 @@
                 if all(map(lambda name: name in field_names, ('ip',))):
                     csv_file.seek(0)
                     reader = csv.DictReader(csv_file, fieldnames=field_names, dialect=dialect)
                     next(reader)
                     res: list[Client] = list()
                     for i in reader:
                         if IpAddress.is_valid(i['ip']):
-                            res.append(c := Client())
+                            res.append(c := Client(
+                                media=AsyncNetwork(
+                                    host=i.get("ip", "127.0.0.1"),
+                                    port=int(i.get("port", "8888")))
+                            ))
                             c.secret = bytes(i.get('secret', '0000000000000000'), 'utf-8')
-                            c.media = AsyncNetwork(
-                                host=i.get("ip", "127.0.0.1"),
-                                port=int(i.get("port", "8888")))
                     return res
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,46 +5,186 @@
 from itertools import count
 import datetime
 import time
 from abc import ABC, abstractmethod
 from DLMS_SPODES.types.implementations import enums, long_unsigneds, bitstrings, octet_string, structs
 from DLMS_SPODES import exceptions as exc
 from DLMS_SPODES.cosem_interface_classes import collection, overview
-from DLMS_SPODES.types import cdt, ut
+from DLMS_SPODES.types import cdt, ut, cst
+from DLMS_SPODES.hdlc import frame
 from DLMS_SPODES.enums import Transmit, Application
 from DLMS_SPODES.obis import media_id
 from DLMS_SPODES.firmwares import get_firmware
 from DLMS_SPODES.cosem_interface_classes.image_transfer import image_transfer_status as i_t_status
-from .client import Client, pdu, logL, AppVersion
+from .client import Client, pdu, logL, AppVersion, ConnectionState, Status, Security, Data, Conformance, mechanism_id, AcseServiceUser
 
 
 class ExTask(ABC):
     """Exchange task for DLMS client"""
+    async def exchange(self, c: Client, is_public: bool = False):
+        if c.connection_state == ConnectionState.NONE:
+            if await get_HDLC(c, is_public) is False:
+                return False
+        return await self.exchange_HDLC(c, is_public)
+
+    async def exchange_HDLC(self, c: Client, is_public: bool = False):
+        if c.connection_state == ConnectionState.HDLC:
+            if await get_AARE(c, is_public) is False:
+                return False
+        return await self.exchange2(c)
+
     @abstractmethod
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         """common exchange in session"""
 
 
+async def get_HDLC(c: Client, is_public: bool = False) -> bool:
+    c.status = Status.EXCHANGE
+    c.set_error(Transmit.OK, "Open port")
+    c.errors.clear()  # clear all last session errors
+    c.send_frames.clear()
+    # calculate addresses
+    c.DA = frame.Address(
+        upper_address=int(c.server_SAP),
+        lower_address=int(c.device_address) if c.device_address else None,
+        length=c.addr_size
+    )
+    c.SA = frame.Address(upper_address=0x10 if is_public else int(c.SAP))
+    c.log(logL.INFO, F"{c.SA=} {c.DA=}")
+    # initialize connection
+    c.reply.clear()
+    # replace this
+    if c.settings.cipher.security != Security.NONE:
+        c.log(logL.DEB, F"Security: {c.settings.cipher.security}/n"
+                           F"System title: {c.settings.cipher.systemTitle.hex()}"
+                           F"Authentication key: {c.settings.cipher.authenticationKey.hex()}"
+                           F"Block cipher key: {c.settings.cipher.blockCipherKey.hex()}")
+        if c.settings.cipher.dedicatedKey:
+            c.log(logL.DEB, F"Dedicated key: {c.settings.cipher.dedicatedKey.hex()}")
+    # SNRM
+    c.get_SNRM_request()
+    c.status = Status.READ
+    await c.read_data_block()
+    c.status = Status.EXCHANGE
+    c.connection_state = ConnectionState.HDLC
+    c.reply.clear()
+    return True
+
+
+async def get_AARE(c: Client, is_public: bool = False) -> bool:
+    if c.invocationCounter and c.settings.cipher is not None and c.settings.cipher.security != Security.NONE:
+        # create IC object. TODO: remove it after close connection, maybe???
+        c.settings.proposedConformance |= Conformance.GENERAL_PROTECTION
+
+        # my block
+        IC: Data = c.objects.add_if_missing(ut.CosemClassId(1),
+                                            logical_name=cst.LogicalName(bytearray((0, c.get_channel_index(), 43, 1,
+                                                                                       c.current_association.security_setup_reference.e, 255))),
+                                            version=cdt.Unsigned(0))
+        tmp_client_SAP = c.current_association.associated_partners_id.client_SAP
+        challenge = c.settings.ctoSChallenge
+        try:
+            c.objects.getIECHDLCSetup(c.get_channel_index()).set_from_info(c.reply.data.get_data())
+            c.aarqRequest(c.m_id)
+            await c.read_data_block()
+            c.parseAareResponse(c.reply.data)
+            c.reply.clear()
+            await c.read_attribute(IC, 2)
+            c.settings.cipher.invocationCounter = 1 + IC.value.decode()
+            c.log(logL.DEB, "Invocation counter: " + str(c.settings.cipher.invocationCounter))
+            # disconnect
+            if c.media and c.media.is_open():
+                c.log(logL.DEB, "DisconnectRequest")
+                await c.disconnect_request()
+        finally:
+            c.SAP = tmp_client_SAP
+            c.settings.useCustomChallenge = challenge is not None
+            c.settings.ctoSChallenge = challenge
+
+        # gurux with several removed methods
+        # add = self.settings.clientAddress
+        # auth = self.settings.authentication
+        # security = self.client.ciphering.security
+        # challenge = self.client.ctoSChallenge
+        # try:
+        #     self.client.clientAddress = 16
+        #     self.settings.authentication = Authentication.NONE
+        #     self.client.ciphering.security = Security.NONE
+        #     reply = GXReplyData()
+        #     self.get_SNRM_request()
+        #     self.status = Status.READ
+        #     self.read_data_block2()
+        #     self.objects.IEC_HDLS_setup.set_from_info(self.reply.data.get_data())
+        #     self.connection_state = ConnectionState.HDLC
+        #     self.reply.clear()
+        #     self.aarqRequest()
+        #     self.read_data_block2()
+        #     self.parseAareResponse(reply.data)
+        #     reply.clear()
+        #     item = GXDLMSData(self.invocationCounter)
+        #     data = self.client.read(item, 2)[0]
+        #     reply = GXReplyData()
+        #     self.read_data_block(data, reply)
+        #     item.encodings[2] = reply.data.get_data()
+        #     Update data type on read.
+        #     if item.getDataType(2) == cdt.NullData.TAG:
+        #         item.setDataType(2, reply.valueType)
+        #     self.client.updateValue(item, 2, reply.value)
+        #     self.client.ciphering.invocationCounter = 1 + item.value
+        #     print("Invocation counter: " + str(self.client.ciphering.invocationCounter))
+        #     if self.media and self.media.isOpen():
+        #         self.log(logL.INFO, "DisconnectRequest")
+        #         self.disconnect_request()
+        # finally:
+        #     self.settings.clientAddress = add
+        #     self.settings.authentication = auth
+        #     self.client.ciphering.security = security
+        #     self.client.ctoSChallenge = challenge
+
+    c.aarqRequest(mechanism_id.NONE if is_public else c.m_id)
+    await c.read_data_block()
+        # await c.read_attr(ut.CosemAttributeDescriptor((collection.ClassID.ASSOCIATION_LN, ut.CosemObjectInstanceId("0.0.40.0.0.255"), ut.CosemObjectAttributeId(6)))) # for test only
+    match c.parseAareResponse(c.reply.data):
+        case AcseServiceUser.NULL:
+            c.log(logL.INFO, 'Authentication success')
+        case AcseServiceUser.AUTHENTICATION_FAILURE as diag if is_public:
+            c.log(logL.WARN, F'On Public connection type got {diag.name}, broad force turn ON')
+        case AcseServiceUser.AUTHENTICATION_REQUIRED:
+            c.reply.clear()
+            c.getApplicationAssociationRequest()
+            await c.read_data_block()
+            c.parseApplicationAssociationResponse()
+        case _ as diagnostic:
+            raise exc.AssociationResultError(diagnostic)
+    c.set_error(Transmit.OK, "Initialize connection")
+    # TODO: remove DIMA crutch dummy read for correct write
+    if c.objects is not None:
+        c.get_get_request_normal(c.objects.LDN.get_attr_descriptor(2))
+        await c.read_data_block()
+        c.matching_LDN(octet_string.LDN(c.reply.data.get_data()))
+    return True
+
+
 class Dummy(ExTask):
     """dummy task"""
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         """"""
         c.log(logL.INFO, "dummy task")
 
 
 @dataclass
 class Loop(ExTask):
     task: ExTask
     func: Callable[[Any], bool]
     delay: int
     attempt_amount: int = 0
     """0 is never end loop"""
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         attempt = count()
         while not self.func(await self.task.exchange(c)):
             if next(attempt) == self.attempt_amount:
                 return False
             await asyncio.sleep(self.delay)
         return True
 
@@ -61,15 +201,15 @@
 
     def append(self, task: ExTask):
         if not self.__is_exchange:
             self.tasks.append(task)
         else:
             raise RuntimeError(F"append to {self.__class__.__name__} not allowed, already exchange started")
 
-    async def exchange(self, c: Client) -> list[cdt.CommonDataType | None]:
+    async def exchange2(self, c: Client) -> list[cdt.CommonDataType | None]:
         ret = list()
         self.__is_exchange = True
         for t in self.tasks:
             # ret.append(await t.exchange(c))
             # TODO: remove in future try-except block with pleasure return value => ret.append(await t.exchange())
             try:
                 res = await t.exchange(c)
@@ -77,15 +217,20 @@
                 res = e
             ret.append(res)
         return ret
 
 
 class InitType(ExTask):
     """nothing params"""
-    async def exchange(self, c: Client):
+    async def exchange(self, c: Client, is_public: bool = False):
+        await c.disconnect_request()
+        c.connection_state = ConnectionState.NONE
+        return await super(InitType, self).exchange(c, is_public=True)
+
+    async def exchange2(self, c: Client):
         # read LDN
         data = await c.read_attr(collection.AttrDesc.LDN_VALUE)
         ldn = octet_string.LDN(data)
         # find device_id(type for Russia)
         type_value, _ = cdt.get_instance_and_pdu_from_value(await c.read_attr(ut.CosemAttributeDescriptor((1, "0.0.96.1.1.255", 2))))
         # find version data
         for desc in (ut.CosemAttributeDescriptor((1, "0.0.0.2.1.255", 2)), ut.CosemAttributeDescriptor((1, "0.0.96.1.2.255", 2))):
@@ -138,15 +283,15 @@
 
 
 @dataclass
 class ReadAttribute(ExTask):
     ln: collection.LNContaining
     index: int
 
-    async def exchange(self, c: Client) -> cdt.CommonDataType:
+    async def exchange2(self, c: Client) -> cdt.CommonDataType:
         # TODO: check is_readable
         obj = c.objects.get_object(self.ln)
         return await self.read_from_obj(c, obj, self.index)
 
     @staticmethod
     async def read_from_obj(c: Client, obj: collection.InterfaceClass, index: int) -> cdt.CommonDataType | ValueError:
         c.get_get_request_normal(
@@ -165,43 +310,43 @@
 
 @dataclass
 class ReadEmptyAttribute(ExTask):
     """read if attribute is empty"""
     ln: collection.LNContaining
     index: int
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         # TODO: check is_readable
         if c.objects.get_object(self.ln).get_attr(self.index) is None:
             data = await ReadAttribute(
                 ln=self.ln,
                 index=self.index).exchange(c)
 
 
 @dataclass
 class ReadAttributes(ExTask):
     ln: collection.LNContaining
     indexes: tuple[int, ...]
 
-    async def exchange(self, c: Client) -> tuple[cdt.CommonDataType | ValueError]:
+    async def exchange2(self, c: Client) -> tuple[cdt.CommonDataType | ValueError]:
         obj = c.objects.get_object(self.ln)
         ret: list[cdt.CommonDataType | ValueError] = list()
         # TODO: check for Get-Request-With-List
         for i in self.indexes:
             ret.append(await ReadAttribute.read_from_obj(c, obj, i))
         return tuple(ret)
 
 
 @dataclass
 class WriteAttribute(ExTask):
     ln: collection.LNContaining
     index: int
     value: bytes | str | int | list | tuple | datetime.datetime
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         obj = c.objects.get_object(self.ln)
         if isinstance(self.value, (str, int, list, tuple, datetime.datetime)):
             value2 = await c.encode(
                 obj=obj,
                 index=self.index,
                 value=self.value)
             enc = value2.encoding
@@ -216,15 +361,15 @@
 
 @dataclass
 class WriteAttributesOld(ExTask):
     """todo: use for write without value(from object) replace all to WriteAttribute in future."""
     ln: collection.LNContaining
     indexes: tuple[int, ...]
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         for i in self.indexes:
             if c.objects.is_writable(
                     ln=(obj := c.objects.get_object(self.ln)).logical_name,
                     index=i,
                     association_id=c.objects.get_association_id(c.SAP)):
                 data = c.get_set_request_normal(
                     obj=obj,
@@ -235,15 +380,15 @@
 
 
 @dataclass
 class ExecuteByDesc(ExTask):
     """execute method by method descriptor # TODO: rewrite this"""
     desc: ut.CosemMethodDescriptor
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         try:
             await c.execute_method(self.desc)
             c.set_error(Transmit.OK, F'Execute {self.desc}.')
         except Exception as e:
             c.log(logL.INFO, F'ERROR: Исполнение {self.desc}')
             c.set_error(Transmit.EXECUTE_ERROR, F'Исполнение {self.desc}')
 
@@ -251,15 +396,15 @@
 @dataclass
 class Execute(ExTask):
     """execute method by method descriptor # TODO: rewrite this with <value>"""
     ln: collection.LNContaining
     index: int
     value: str
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         obj = c.objects.get_object(self.ln)
         try:
             await c.execute_method(ut.CosemMethodDescriptor(
                 (obj.CLASS_ID,
                  ut.CosemObjectInstanceId(obj.logical_name.contents),
                  ut.CosemObjectMethodId(self.index))
             ))
@@ -268,15 +413,15 @@
             c.log(logL.INFO, F'ERROR: Исполнение {self.ln}: {self.index}')
             c.set_error(Transmit.EXECUTE_ERROR, F'Исполнение {self.ln}: {self.index}')
 
 
 class WriteTime(ExTask):
     """write Clock.time depend from transfer time"""
 
-    async def exchange(self, c: Client):
+    async def exchange2(self, c: Client):
         try:
             obj = c.objects.clock
             c.get_get_request_normal(obj.get_attr_descriptor(3))
             await c.read_data_block()
             tz = obj.get_attr_element(3).DATA_TYPE(c.reply.data.get_data())
             await WriteAttribute(
                 ln=obj.logical_name,
@@ -291,20 +436,37 @@
             # logger.info(F'ERROR: write Clock: attribute 2 {e}')
             c.errors[Transmit.WRITE_ERROR] = F"write time: {e}"
 
 # @dataclass
 # class UpdateResponse:
 #     result:
 
+
 @dataclass
 class UpdateFirmware(ExTask):
     """only for KPZ now"""
-    # firmwares: field(default=dict)
 
-    async def exchange(self, c: Client) -> bool:
+    async def exchange2(self, c: Client) -> bool:
+        # check available action todo: not work in 0.0.38
+        # if c.current_association.object_list is None:
+        #     await ReadAttribute(
+        #         ln=c.current_association.logical_name,
+        #         index=2
+        #     ).exchange(c)
+        # image_objects: collection.ImageTransfer = collection.get_filtered(objects=c.current_association.objects, keys=(overview.ClassID.IMAGE_TRANSFER, ))
+        # if len(image_objects) == 0:
+        #     c.set_error(Application.MISSING_OBJ, "not find image_transfer in current association")
+        #     return False
+        # for obj in image_objects:
+        #     if not c.current_association.is_accessible(
+        #                                         ln=obj.logical_name,
+        #                                         index=4,    # image_activate
+        #                                         m_id=c.m_id):
+        #         c.set_error(Transmit.NO_ACCESS, "not has access for activate image in current association")
+        #         return False
         # read properties for update
         read_seq = Sequence()
         match c.objects.collection_ver:
             case AppVersion(0, 0, patch) if 25 <= patch < 26:
                 read_seq.append(ReadAttribute(
                     ln=c.objects.firmwares_description.logical_name,
                     index=2))
@@ -402,14 +564,17 @@
                 suitable_firmware = compare_version
                 temp_key = key
         if suitable_firmware != c.objects.server_ver[0] and temp_key is not None:
             image: bytes = firmwares.get(temp_key)
             c.objects.firmware_image_transfer.set_image_for_update(
                 value=image,
                 identifier=bytearray(hashlib.md5(image).digest()))
+            c.log(logL.INFO, F"set image to update {suitable_firmware=}")
+        else:
+            c.log(logL.INFO, F"{c.objects.server_ver[0]=} is actual")
         # search boot image
         temp_key = None
         for key in boots:
             match key:
                 case 1 | 2 | 3 | 4 | 5 | 6 as compare_version, desc if firmwares_description in desc:
                     """good"""
                 case 7 | 8 | 9 | 10 | 11 as compare_version, desc if desc.split("_", maxsplit=5)[1:5] == firmwares_description.split("_", maxsplit=5)[:4]:
@@ -426,14 +591,17 @@
                 temp_key = key
         c.objects.boot_image_transfer.clear_image()
         if suitable_boot != boot_version and temp_key is not None:
             image: bytes = boots.get(temp_key)
             c.objects.boot_image_transfer.set_image_for_update(
                 value=image,
                 identifier=bytearray(hashlib.md5(image).digest()))
+            c.log(logL.INFO, F"set image to update {suitable_boot=}")
+        else:
+            c.log(logL.INFO, F"{boot_version=} is actual")
 
         # update
         match c.objects.server_ver[0]:
             case AppVersion(0, 0, 53 | 54) | AppVersion(1, 1 | 2 | 3 | 4 | 5 | 6):
                 if await self.__is_updated_image_3(c=c, obj=c.objects.boot_image_transfer):
                     await ReadAttribute(
                         ln=c.objects.firmwares_description.logical_name,
@@ -462,15 +630,14 @@
                 c.set_error(Transmit.EXECUTE_ERROR, F'Невозможно обновить версию {c.objects.server_ver}')
                 return False
         return False
 
     async def __is_updated_image(self, c: Client, obj: collection.ImageTransfer) -> bool:
         """ update image if blocks is fulls """
         if obj.is_image_exist:
-            is_activating: bool = False
             c.current_obj = obj
             try:
                 await c.execute_method(obj.get_meth_descriptor(1))
                 c.log(logL.INFO, "Start initiate Image Transfer")
                 while True:
                     if c.is_stop_request:
                         c.set_error(Transmit.ABORT, '')
@@ -478,21 +645,19 @@
                     await c.execute_method(obj.get_meth_descriptor(2))
                     c.log(logL.INFO, F"start block: {obj.current_block_transfer} transferred")
                     try:
                         obj.set_next_block()
                     except StopIteration:
                         c.log(logL.INFO, "All blocks transferred")
                         break
-                # c.execute_method(obj.get_meth_descriptor(3))  # Start Verify Transfer. todo: removed Verification because don't work with change to 1.3
-                await c.execute_method(obj.get_meth_descriptor(4))
+                await c.execute_method(obj.get_meth_descriptor(4))  # attention without verification
                 c.log(logL.INFO, "Start Activate Transfer")
-                c.set_error(Application.OK, F'Activated')
                 return True
             except Exception as e:
-                c.set_error(Transmit.EXECUTE_ERROR, F'unhandled update error. {e.args[0]}')
+                c.log(logL.ERR, F'unhandled update error. {e.args[0]}')
                 return False
         else:
             return True
 
     async def __is_updated_image_2(self, c: Client, obj: collection.ImageTransfer, with_abort: bool = True) -> bool:
         """ update image if blocks is fulls ver 2"""
         if obj.is_image_exist:
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.7.4
+Version: 0.7.5
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.7.4/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.7.5/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 src/DLMS_SPODES_client.egg-info/dependency_links.txt
 src/DLMS_SPODES_client.egg-info/entry_points.txt
 src/DLMS_SPODES_client.egg-info/requires.txt
 src/DLMS_SPODES_client.egg-info/top_level.txt
 src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
 src/DLMS_SPODES_client/gurux_common/enums/__init__.py
 src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
-src/DLMS_SPODES_client/gurux_dlms/ConnectionState.py
 src/DLMS_SPODES_client/gurux_dlms/CountType.py
 src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
 src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
 src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
 src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
 src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
 src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
```

### Comparing `DLMS_SPODES_client-0.7.4/test/test_Client.py` & `DLMS_SPODES_client-0.7.5/test/test_Client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,53 +7,57 @@
 from src.DLMS_SPODES_client.servers import TransactionServer
 from src.DLMS_SPODES_client import task
 
 
 class TestType(unittest.TestCase):
     def test_connect(self):
         t_server = TransactionServer(
-            clients=[
-                client := Client(addr_size=1)
-            ],
+            clients=[c := Client(media=AsyncSerial(
+                                port="COM13",
+                                inactivity_timeout=3))],
             tsk=task.Dummy()
         )
-        client.device_address.set(0)
-        client.media = AsyncSerial(
-            port="COM13",
-            inactivity_timeout=3
-        )
         t_server.start()
+        while not t_server.results.is_complete():
+            time.sleep(1)
+        print(c.objects)
 
     def test_Loop(self):
         def foo(res):
             return res == cdt.Long(4)
 
         t_server = TransactionServer(
             clients=[
-                client := Client(addr_size=1)
+                client := Client(
+                    secret="30 30 30 30 30 30 30 30",
+                    addr_size=-1)
             ],
             tsk=task.Loop(
                 task=task.ReadAttribute(
                     ln="0.0.1.0.0.255",
                     index=3),
                 func=lambda res: res == cdt.Long(4),
                 delay=2,
                 attempt_amount=5
             )
         )
-        client.device_address.set(0)
+        client.m_id.set(1)
+        # client.device_address.set(0)
         client.media = AsyncSerial(
             port="COM13",
             inactivity_timeout=3
         )
         t_server.start()
+        while not t_server.results.is_complete():
+            time.sleep(1)
+        print("stop")
 
     def test_async_network(self):
         client = Client(
-            secret="00 00 00 00 00 00 00 00",
+            secret="30 30 30 30 30 30 30 30",
             addr_size=1,
             conformance="010000000001111000011101")
         type_ = "4d324d5f31"
         ver = "1.5.7"
         man = b"KPZ"
         # client.objects = collection.get(
         #     m=man,
@@ -188,27 +192,48 @@
         while not t_server.results.is_complete():
             time.sleep(1)
         a = t_server.results[0]
         print(t_server)
 
     def test_firmware_update(self):
         client = Client(
-            secret="30 30 30 30 30 30 30 30 30 30 30 30 30 30 30 30",
-            addr_size=1,
-            conformance="010000000001111000011101")
-        client.SAP.set(0x30)
-        client.m_id.set(2)
-        client.device_address.set(0)
-        client.media = AsyncSerial(
-            port="COM13",
-            inactivity_timeout=3
-        )
+            secret="30 30 30 30 30 30 30 30",
+            conformance="010000000001111000011101",
+            media=AsyncSerial(
+                port="COM13",
+                inactivity_timeout=3))
+        # client.SAP.set(0x30)  # for KPZ
+        # client.m_id.set(2)  # for KPZ
+        client.m_id.set(1)  # for 101, 102, 103, 104 before ver 1.0
+        client.transmit_pdu_size = 128
         t_server = TransactionServer(
             clients=[client],
             tsk=task.UpdateFirmware())
         t_server.start()
 
         while not t_server.results.is_complete():
             time.sleep(1)
             print(f"{t_server.results.is_complete()=}")
         a = t_server.results[0]
         print(t_server)
+
+    def test_read_association(self):
+        client = Client(
+            secret="30 30 30 30 30 30 30 30",
+            conformance="010000000001111000011101",
+            media=AsyncSerial(
+                port="COM13",
+                inactivity_timeout=3))
+        # client.SAP.set(0x30)  # for KPZ
+        # client.m_id.set(2)  # for KPZ
+        client.m_id.set(1)  # for 101, 102, 103, 104 before ver 1.0
+        t_server = TransactionServer(
+            clients=[client],
+            tsk=task.ReadAttribute(
+                ln='0.0.40.0.1.255',
+                index=2
+            ))
+        t_server.start()
+
+        while not t_server.results.is_complete():
+            time.sleep(1)
+        print(f"{t_server.results.is_complete()=}")
```

