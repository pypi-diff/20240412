# Comparing `tmp/protobuf_to_pydantic-0.2.6.tar.gz` & `tmp/protobuf_to_pydantic-0.2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protobuf_to_pydantic-0.2.6.tar", max compression
+gzip compressed data, was "protobuf_to_pydantic-0.2.6.1.tar", max compression
```

## Comparing `protobuf_to_pydantic-0.2.6.tar` & `protobuf_to_pydantic-0.2.6.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.2.6/LICENSE
--rw-r--r--   0        0        0    52809 2024-02-12 17:31:10.807300 protobuf_to_pydantic-0.2.6/README.md
--rw-r--r--   0        0        0      157 2023-07-25 07:16:59.663544 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/__init__.py
--rw-r--r--   0        0        0       23 2024-03-19 16:50:45.551031 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/__version__.py
--rw-r--r--   0        0        0     3600 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/_pydantic_adapter.py
--rw-r--r--   0        0        0     1915 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/constant.py
--rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/contrib/__init__.py
--rw-r--r--   0        0        0    15428 2023-09-11 08:36:58.424118 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/contrib/proto_parser.py
--rw-r--r--   0        0        0      134 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_con_type/__init__.py
--rw-r--r--   0        0        0     7954 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_con_type/v1.py
--rw-r--r--   0        0        0    14102 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_con_type/v2.py
--rw-r--r--   0        0        0      177 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_validator/__init__.py
--rw-r--r--   0        0        0     9782 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_validator/rule.py
--rw-r--r--   0        0        0     8204 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_validator/v1.py
--rw-r--r--   0        0        0     9648 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_validator/v2.py
--rw-r--r--   0        0        0     2579 2023-09-14 10:22:59.213024 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/desc_template/__init__.py
--rw-r--r--   0        0        0    35039 2023-12-29 09:41:55.115358 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/gen_code.py
--rw-r--r--   0        0        0    35234 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/gen_model.py
--rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/__init__.py
--rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
--rw-r--r--   0        0        0    20179 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pb_option/base.py
--rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
--rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
--rw-r--r--   0        0        0     4349 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pb_option/types.py
--rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_proto_file.py
--rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pyi_file.py
--rw-r--r--   0        0        0     7514 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/grpc_types.py
--rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/__init__.py
--rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/__main__.py
--rw-r--r--   0        0        0     2655 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/cli.py
--rw-r--r--   0        0        0     6402 2023-11-07 16:10:23.558322 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/code_gen.py
--rw-r--r--   0        0        0     2841 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/config.py
--rw-r--r--   0        0        0    28873 2024-03-19 16:46:00.139644 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
--rwxr-xr-x   0        0        0      413 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/main.py
--rw-r--r--   0        0        0      423 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/my_types.py
--rw-r--r--   0        0        0   414477 2024-03-19 12:31:49.627933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   198324 2024-03-19 12:31:49.627933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.711467 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0   121461 2024-03-19 12:31:49.627933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2024-03-19 12:31:49.627933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.723467 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0    36974 2024-03-19 12:31:57.711933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   198324 2024-03-19 12:31:57.711933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0    13403 2024-03-19 12:31:57.711933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2024-03-19 12:31:57.711933 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/validate_pb2.py
--rw-r--r--   0        0        0     2683 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/types.py
--rw-r--r--   0        0        0     7158 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/util.py
--rw-r--r--   0        0        0     3606 2024-03-19 16:50:45.547031 protobuf_to_pydantic-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    55395 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6/setup.py
--rw-r--r--   0        0        0    54068 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.2.6.1/LICENSE
+-rw-r--r--   0        0        0    53105 2024-04-12 16:29:25.422060 protobuf_to_pydantic-0.2.6.1/README.md
+-rw-r--r--   0        0        0      157 2023-07-25 07:16:59.663544 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-12 16:30:50.520666 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/__version__.py
+-rw-r--r--   0        0        0     3600 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/_pydantic_adapter.py
+-rw-r--r--   0        0        0     1915 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/constant.py
+-rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/contrib/__init__.py
+-rw-r--r--   0        0        0    15428 2023-09-11 08:36:58.424118 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/contrib/proto_parser.py
+-rw-r--r--   0        0        0      134 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/__init__.py
+-rw-r--r--   0        0        0     7954 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v1.py
+-rw-r--r--   0        0        0    14102 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v2.py
+-rw-r--r--   0        0        0      177 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/__init__.py
+-rw-r--r--   0        0        0     9782 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/rule.py
+-rw-r--r--   0        0        0     8204 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v1.py
+-rw-r--r--   0        0        0     9648 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v2.py
+-rw-r--r--   0        0        0     2579 2023-09-14 10:22:59.213024 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/desc_template/__init__.py
+-rw-r--r--   0        0        0    35019 2024-03-29 06:52:18.350469 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_code.py
+-rw-r--r--   0        0        0    35234 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_model.py
+-rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/__init__.py
+-rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
+-rw-r--r--   0        0        0    20179 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/base.py
+-rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
+-rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
+-rw-r--r--   0        0        0     4349 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/types.py
+-rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_proto_file.py
+-rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pyi_file.py
+-rw-r--r--   0        0        0     7514 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/grpc_types.py
+-rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/__main__.py
+-rw-r--r--   0        0        0     2655 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/cli.py
+-rw-r--r--   0        0        0     6402 2023-11-07 16:10:23.558322 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/code_gen.py
+-rw-r--r--   0        0        0     2841 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/config.py
+-rw-r--r--   0        0        0    29201 2024-03-29 07:16:25.193672 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
+-rwxr-xr-x   0        0        0      413 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/main.py
+-rw-r--r--   0        0        0      423 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/my_types.py
+-rw-r--r--   0        0        0   414477 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   198324 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.711467 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0   121461 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.723467 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0    36680 2024-04-12 16:29:25.426060 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   198324 2024-04-12 08:25:53.378232 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13083 2024-04-12 16:29:25.426060 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2024-04-12 08:25:53.378232 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/validate_pb2.py
+-rw-r--r--   0        0        0     2683 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/types.py
+-rw-r--r--   0        0        0     7158 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/util.py
+-rw-r--r--   0        0        0     3631 2024-04-12 16:30:50.516667 protobuf_to_pydantic-0.2.6.1/pyproject.toml
+-rw-r--r--   0        0        0    55696 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6.1/setup.py
+-rw-r--r--   0        0        0    54355 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6.1/PKG-INFO
```

### Comparing `protobuf_to_pydantic-0.2.6/LICENSE` & `protobuf_to_pydantic-0.2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/README.md` & `protobuf_to_pydantic-0.2.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,22 @@
 #### 1.1.1.Use plugins
 Plug-in is the `Pydantic Model` source code generation method recommended by `protobuf-to-pydantic`.
 It supports the most complete functions and is also very simple to use.
 
 Assume that it is usually generated through the following command Code corresponding to Protobuf file:
 ```bash
 python -m grpc_tools.protoc -I. example.proto
+# or
+protoc -I. --python_out=. example.proto
 ```
 After installing `protobuf-to-pydantic`,can use the `protobuf-to-pydantic` plugin with the `--protobuf-to-pydantic_out` option with the following command:
 ```bash
 python -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=. example.proto
+# or
+protoc -I. --protobuf-to-pydantic_out=. example.proto
 ```
 
 In this command, `--protobuf-to-pydantic_out=.` means using the `prorobuf-to-pydantic` plug-in,
 And it is declared that the output location of the `protobuf-to-pydantic` plug-in is `.`
 
 > `.` indicates the output path used by `grpc_tools.proto`.
 
@@ -109,14 +113,16 @@
 file_name_suffix = "_p2p"
 ```
 Next, in order to be able to read this file, need to change the `--protobuf-to-pydantic_out=. ` to ` --protobuf-to-pydantic_out=config_path=plugin_config.py:. `.
 where the left side of `:` indicates that the configuration file path to be read is `plugin_config.py`, and the right side of `:` declares that the output location of the `protobuf-to-pydantic` plugin is `. `
 The final complete command is as follows：
 ```bash
 python -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto
+# or
+protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto
 ```
 Through this command, can load the corresponding configuration and run the `protobuf-to-pydantic` plug-in。
 
 In addition to the configuration options in the example configuration file,
 the `protobuf-to-pydantic` plug-in also supports other configuration options.
 The specific configuration instructions are as follows：
 
@@ -159,15 +165,15 @@
   int32 age=2;
   float height=3;
   SexType sex=4;
   bool is_adult=5;
   string user_name=6;
 }
 ```
-`grpc_tools.protoc` can be used to generate the Python code file corresponding to the `Protobuf` file (the file name is `demo_pb2.py`), and the code related to the `UserMessage` is stored in the code file.
+`protoc` can be used to generate the Python code file corresponding to the `Protobuf` file (the file name is `demo_pb2.py`), and the code related to the `UserMessage` is stored in the code file.
 
 At `Python` runtime, The func `msg_to_pydantic_model` can be called to read the `UserMessage` object from the `demo_pb2` module and generate the corresponding `Pydantic Model` object as follows:
 ```Python
 from typing import Type
 from protobuf_to_pydantic import msg_to_pydantic_model
 from pydantic import BaseModel
 
@@ -343,14 +349,19 @@
 ```bash
 cd example
 
 python -m grpc_tools.protoc
   --python_out=./python_example_proto_code \
   --grpc_python_out=./python_example_proto_code \
   -I. \
+# or
+protoc
+  --python_out=./python_example_proto_code \
+  --grpc_python_out=./python_example_proto_code \
+  -I. \
 ```
 Then the path that needs to be filled in for `parse_msg_desc_method` at this time is `./protobuf_to_pydantic/example`.
 The following sample code:
 ```python
 # pydantic Version v1
 from typing import Type
 from protobuf_to_pydantic import msg_to_pydantic_model
```

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/_pydantic_adapter.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/_pydantic_adapter.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/constant.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/constant.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/contrib/proto_parser.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/contrib/proto_parser.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_con_type/v1.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v1.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_con_type/v2.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_validator/rule.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/rule.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_validator/v1.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v1.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/customer_validator/v2.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/desc_template/__init__.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/desc_template/__init__.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/gen_code.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,20 +358,19 @@
 
     def _model_field_handle(self, model: Type[BaseModel], indent: int = 0) -> str:
         field_str: str = ""
         for key, value in _pydantic_adapter.model_fields(model).items():
             if hasattr(value, "annotation"):
                 value_outer_type = value.annotation  # type: ignore
                 value_type = value.annotation  # type: ignore
+            elif _pydantic_adapter.is_v1:
+                value_outer_type = value.annotation  # type: ignore
+                value_type = value.annotation  # type: ignore
             else:
-                if _pydantic_adapter.is_v1:
-                    value_outer_type = value.annotation  # type: ignore
-                    value_type = value.annotation  # type: ignore
-                else:
-                    raise RuntimeError("can not load value type")
+                raise RuntimeError("can not load value type")
             # Type Hint handler
             if value_outer_type.__module__ != "builtins":
                 if inspect.isclass(value_type) and issubclass(value_type, IntEnum):
                     # Parse protobuf enum
                     self._import_set.add("from enum import IntEnum")
                     enum_code: str = self._gen_enum_py_code(value_type, indent=indent - self.code_indent)
                     if enum_code:
@@ -457,22 +456,22 @@
         else:
             self._add_import_code(base_class.__module__, base_class.__name__)
 
         class_str: str = " " * indent + f"class {model.__name__}({base_class.__name__}):\n"
         if model.__doc__:
             class_str += " " * (indent + self.code_indent) + '"""' + model.__doc__ + '"""\n'
 
-        config_class: str = self._model_config_handle(model, indent=indent + self.code_indent)
-        if config_class:
-            class_str += config_class + "\n"
-
         nested_class_str: str = self._model_nested_handle(model, indent=indent + self.code_indent)
         if nested_class_str:
             class_str += nested_class_str + "\n"
 
+        config_class: str = self._model_config_handle(model, indent=indent + self.code_indent)
+        if config_class:
+            class_str += config_class + "\n"
+
         attribute_str: str = self._model_attribute_handle(model, indent=indent + self.code_indent)
         if attribute_str:
             class_str += attribute_str + "\n"
 
         field_str = self._model_field_handle(model, indent=indent + self.code_indent)
         if field_str:
             class_str += field_str + "\n"
@@ -489,14 +488,15 @@
 
     def _gen_pydantic_model_py_code_to_content_deque(self, model: Type[BaseModel], indent: int = 0) -> None:
         if model in self._create_set:
             # ignore parsed model
             return None
         pydantic_model_code: str = self._gen_pydantic_model_py_code(model, indent=indent)
         if pydantic_model_code:
+            pydantic_model_code += "\n"
             self._content_deque.append(pydantic_model_code)
         self._create_set.add(model)
 
     def _parse_type_to_import_code(self, type_: Any) -> None:
         """Parse the type and generate the corresponding import"""
         type_module: Optional[ModuleType] = inspect.getmodule(type_)
         if not type_module:
@@ -564,15 +564,14 @@
     def _field_info_handle(self, field_info: FieldInfo) -> str:
         # Introduce the corresponding class for FieldInfo's properties
         if _pydantic_adapter.is_v1:
             # in v1, field_info is ModelField
             field_info = field_info.field_info  # type: ignore[attr-defined]
 
         field_param_dict: Dict[str, Any] = {}
-        field_param_code_list: List[str] = []
         for k, v in field_info.__repr_args__():
             if k not in field_param_set:
                 continue
             v = getattr(field_info, k)
             if k == "default" and str(v) == "PydanticUndefined":
                 # Ignore the default value of the pydantic field
                 continue
@@ -588,23 +587,24 @@
                             # If the value obtained is the same as the default value,
                             # it will not be added to the field param dict
                             continue
                         # Field's metadata will hold duplicate values, but Field only needs the first value
                         if metadata_key in field_param_dict:
                             continue
                         field_param_dict[metadata_key] = metadata_value
-            elif k == "extra" or k == "json_schema_extra":
+            elif k in ("extra", "json_schema_extra"):
                 if not v:
                     # Ignore cases where the value of extra is empty
                     continue
                 for extra_k, extra_v in v.items():
                     field_param_dict[extra_k] = extra_v
             else:
                 field_param_dict[k] = v
 
+        field_param_code_list: List[str] = []
         for k, v in field_param_dict.items():
             field_param_code_list.append(f"{k}={self._get_value_code(v)}")
             self._parse_type_to_import_code(v)
 
         # For different versions of pydantic, their fields are the same, but the position of the parameters is different
         # need to ensure that the generated code is consistent across different versions of pydantic
         # field_param_code_list.sort()
@@ -640,15 +640,15 @@
                         " " * indent
                         + f"{validator_name} = validator({field_param_str}, {', '.join(param_list)})({func.__name__})\n"
                     )
                 elif hasattr(validator_class, "__root_validator_config__"):
                     validator_instance = validator_class.__root_validator_config__
                     func = validator_instance.func
 
-                    if not validator_instance.func.__module__.startswith(customer_validator.__name__):
+                    if not func.__module__.startswith(customer_validator.__name__):
                         continue
                     self._add_import_code("pydantic", "root_validator")
                     self._add_import_code(func.__module__, func.__name__)
                     param_list = [
                         f"{i}={self._get_value_code(getattr(validator_instance, i))}"
                         for i in ["pre", "skip_on_failure"]
                         if getattr(validator_instance, i) != root_validator_sig.parameters[i].default
```

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/gen_model.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_model.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pb_option/base.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/base.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pb_option/types.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_proto_file.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_proto_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/get_desc/from_pyi_file.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pyi_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/grpc_types.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/grpc_types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/cli.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/code_gen.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/code_gen.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/config.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/config.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 import inspect
 import logging
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Set, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Set, Tuple
 
 from mypy_protobuf.main import PYTHON_RESERVED, Descriptors, SourceCodeLocation
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo
 from typing_extensions import NotRequired, TypedDict
 
 from protobuf_to_pydantic import _pydantic_adapter
@@ -97,15 +97,15 @@
 
         logger.info((self._fd.name, other_fd.name, index))
         if index != -1:
             # Add relative parts: ..b.include_p2p
             module_name = "." * (len(message_path_list) - (index + 1)) + module_name
         self._add_import_code(module_name, type_str)
 
-    def _enum(self, enums: Iterable[EnumDescriptorProto], scl_prefix: SourceCodeLocation, indent: int = 0) -> str:
+    def _enum(self, enums: Iterable[EnumDescriptorProto], scl_prefix: SourceCodeLocation, indent: int = 0) -> List[str]:
         """
         e.g:
             enums:
                 {
                     "name": "State",
                     [
                         "value": {
@@ -117,39 +117,41 @@
             python code:
                 from enum import IntEnum
 
                 class State(IntEnum):
                     INACTIVE = 0
         """
         if not enums:
-            return ""
+            return []
         self._add_import_code("enum", "IntEnum")
-        content: str = ""
+        content_list = []
         for i, enum in enumerate(enums):
             class_name = enum.name if enum.name not in PYTHON_RESERVED else "_r_" + enum.name
-            content += " " * indent + f"class {class_name}(IntEnum):\n"
+            content = " " * indent + f"class {class_name}(IntEnum):\n"
             for enum_item in enum.value:
                 content += " " * (self.code_indent + indent) + f"{enum_item.name} = {enum_item.number}\n"
-            content += "\n\n"
-        return content
+            content_list.append(content)
+        return content_list
 
     def _message_nested_type_handle(
         self, desc: DescriptorProto, scl_prefix: SourceCodeLocation, indent: int, nested_message_config_dict: dict
-    ) -> str:
+    ) -> List[str]:
         """Parse the nested information of Message"""
-        content: str = ""
+        content_list: List[str] = []
         for nested_message in desc.nested_type:
             if nested_message.options.map_entry:
                 # Some data of Map Entry in nested type array
                 continue
             skip_validate_rule = nested_message_config_dict.get(nested_message.name, {}).get("skip", False)
-            content += self._message(
-                nested_message, desc, scl_prefix, indent + self.code_indent, skip_validate_rule=skip_validate_rule
+            content_list.append(
+                self._message(
+                    nested_message, desc, scl_prefix, indent + self.code_indent, skip_validate_rule=skip_validate_rule
+                )
             )
-        return content
+        return content_list
 
     # flake8: noqa: C901
     def _message_field_handle(
         self,
         desc: DescriptorProto,
         root_desc: DescriptorProto,
         field: FieldDescriptorProto,
@@ -460,16 +462,17 @@
         indent: int = 0,
         skip_validate_rule: bool = False,
     ) -> str:
         self._add_import_code("google.protobuf.message", "Message")
         class_name = desc.name if desc.name not in PYTHON_RESERVED else "_r_" + desc.name
         if class_name in self._parse_desc_name_dict:
             return self._parse_desc_name_dict[class_name]
-        class_content = " " * indent + f"class {class_name}({self.config.base_model_class.__name__}):\n"
-        class_head_content = ""
+        class_name_content = " " * indent + f"class {class_name}({self.config.base_model_class.__name__}):"
+        class_var_str_list = []
+        class_sub_c_str_list = []
         class_validate_handler_content = ""
         class_field_content = ""
 
         use_custom_type: bool = False
         one_of_dict, optional_dict, nested_message_config_dict = {}, {}, {}  # type: dict, dict, dict
 
         if desc.oneof_decl:
@@ -491,64 +494,68 @@
                 skip_validate_rule=skip_validate_rule,
             )
             if _content_tuple:
                 class_validate_handler_content += _content_tuple[0]
                 class_field_content += _content_tuple[1]
 
         if desc.nested_type:
-            class_head_content += self._message_nested_type_handle(desc, scl_prefix, indent, nested_message_config_dict)
+            class_sub_c_str_list.extend(
+                self._message_nested_type_handle(desc, scl_prefix, indent, nested_message_config_dict)
+            )
         if desc.enum_type:
-            class_head_content += self._enum(desc.enum_type, scl_prefix, indent + self.code_indent)
+            class_sub_c_str_list.extend(self._enum(desc.enum_type, scl_prefix, indent + self.code_indent))
 
         if one_of_dict:
-            class_head_content += (
-                f"{' ' * (indent + self.code_indent)}_one_of_dict = {self._get_value_code(one_of_dict)}\n"
+            class_var_str_list.append(
+                f"{' ' * (indent + self.code_indent)}_one_of_dict = {self._get_value_code(one_of_dict)}"
             )
 
             self._add_import_code("protobuf_to_pydantic.customer_validator", "check_one_of")
             if _pydantic_adapter.is_v1:
-                class_head_content += (
+                class_var_str_list.append(
                     f"{' ' * (indent + self.code_indent)}"
-                    f"one_of_validator = root_validator(pre=True, allow_reuse=True)(check_one_of)\n"
+                    f"one_of_validator = root_validator(pre=True, allow_reuse=True)(check_one_of)"
                 )
                 self._add_import_code("pydantic", "root_validator")
             else:
-                class_head_content += (
+                class_var_str_list.append(
                     f"{' ' * (indent + self.code_indent)}"
-                    f'one_of_validator = model_validator(mode="before")(check_one_of)\n'
+                    f'one_of_validator = model_validator(mode="before")(check_one_of)'
                 )
                 self._add_import_code("pydantic", "model_validator")
 
         if use_custom_type:
             if _pydantic_adapter.is_v1:
                 # Pydantic V1 output:
                 #   class Config:
                 #       arbitrary_types_allowed = False
                 config_content: str = f"{' ' * (indent + self.code_indent)}class Config:\n"
                 config_content += f"{' ' * (indent + self.code_indent * 2)}arbitrary_types_allowed = True\n\n"
+                class_sub_c_str_list.append(config_content)
             else:
                 # Pydantic V2 output:
                 #   model_config = ConfigDict(arbitrary_types_allowed=False)
-                config_content = (
-                    f"{' ' * (indent + self.code_indent)}model_config = ConfigDict(arbitrary_types_allowed=True)\n\n"
+                class_var_str_list.append(
+                    f"{' ' * (indent + self.code_indent)}model_config = ConfigDict(arbitrary_types_allowed=True)"
                 )
                 self._add_import_code("pydantic", "ConfigDict")
 
-            class_head_content = config_content + class_head_content
-
+        class_head_content = "\n".join(class_sub_c_str_list)
+        if class_head_content and class_var_str_list:
+            class_head_content += "\n"
+        class_head_content += "\n".join(class_var_str_list)
         content = "\n".join(
-            [i for i in [class_content, class_head_content, class_field_content, class_validate_handler_content] if i]
+            [
+                i
+                for i in [class_name_content, class_head_content, class_field_content, class_validate_handler_content]
+                if i
+            ]
         )
         if not any([class_head_content, class_field_content]):
             content += " " * (indent + self.code_indent) + "pass\n"
-        while True:
-            if content[-1] != "\n":
-                break
-            content = content[:-1]
-        content += "\n" if indent > 0 else "\n\n"
         self._parse_desc_name_dict[class_name] = content
         return content
 
     def _get_protobuf_type_model(self, field: FieldDescriptorProto) -> ProtobufTypeModel:
         type_factory: Optional[Any] = None
         use_custom_type = False
         # TODO use gen_model.py _message_default_factory_dict_by_type_name
@@ -622,10 +629,12 @@
                 # and the type_ field will not be used at this time
                 type_factory=None,
                 rule_type_str="message",
                 py_type_str=field.type_name.split(".")[-1],
             )
 
     def _parse_field_descriptor(self) -> None:
-        self._content_deque.append(self._enum(self._fd.enum_type, [FileDescriptorProto.ENUM_TYPE_FIELD_NUMBER]))
+        self._content_deque.append(
+            "\n\n".join(self._enum(self._fd.enum_type, [FileDescriptorProto.ENUM_TYPE_FIELD_NUMBER]))
+        )
         for desc in self._fd.message_type:
             self._content_deque.append(self._message(desc, desc, [FileDescriptorProto.ENUM_TYPE_FIELD_NUMBER]))
```

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/validate_pb2.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: protos/p2p_validate.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/p2p_validate.proto\x12\x0cp2p_validate\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x1e\n\nOneofRules\x12\x10\n\x08optional\x18\x01 \x03(\t\"\x81\x08\n\nFieldRules\x12\x30\n\x07message\x18\x11 \x01(\x0b\x32\x1a.p2p_validate.MessageRulesH\x01\x88\x01\x01\x12)\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x18.p2p_validate.FloatRulesH\x00\x12+\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x19.p2p_validate.DoubleRulesH\x00\x12)\n\x05int32\x18\x03 \x01(\x0b\x32\x18.p2p_validate.Int32RulesH\x00\x12)\n\x05int64\x18\x04 \x01(\x0b\x32\x18.p2p_validate.Int64RulesH\x00\x12+\n\x06uint32\x18\x05 \x01(\x0b\x32\x19.p2p_validate.UInt32RulesH\x00\x12+\n\x06uint64\x18\x06 \x01(\x0b\x32\x19.p2p_validate.UInt64RulesH\x00\x12+\n\x06sint32\x18\x07 \x01(\x0b\x32\x19.p2p_validate.SInt32RulesH\x00\x12+\n\x06sint64\x18\x08 \x01(\x0b\x32\x19.p2p_validate.SInt64RulesH\x00\x12-\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x1a.p2p_validate.Fixed32RulesH\x00\x12-\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x1a.p2p_validate.Fixed64RulesH\x00\x12/\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x1b.p2p_validate.SFixed32RulesH\x00\x12/\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x1b.p2p_validate.SFixed64RulesH\x00\x12\'\n\x04\x62ool\x18\r \x01(\x0b\x32\x17.p2p_validate.BoolRulesH\x00\x12+\n\x06string\x18\x0e \x01(\x0b\x32\x19.p2p_validate.StringRulesH\x00\x12)\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x18.p2p_validate.BytesRulesH\x00\x12\'\n\x04\x65num\x18\x10 \x01(\x0b\x32\x17.p2p_validate.EnumRulesH\x00\x12/\n\x08repeated\x18\x12 \x01(\x0b\x32\x1b.p2p_validate.RepeatedRulesH\x00\x12%\n\x03map\x18\x13 \x01(\x0b\x32\x16.p2p_validate.MapRulesH\x00\x12%\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x16.p2p_validate.AnyRulesH\x00\x12/\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x1b.p2p_validate.DurationRulesH\x00\x12\x31\n\ttimestamp\x18\x16 \x01(\x0b\x32\x1c.p2p_validate.TimestampRulesH\x00\x42\x06\n\x04typeB\n\n\x08_message\"\xf6\x04\n\nFloatRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x02H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x02H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x02H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x02H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x02H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x02\x12\x0e\n\x06not_in\x18\x07 \x03(\x02\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf7\x04\n\x0b\x44oubleRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x01H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x01H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x01H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x01H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x01H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x01\x12\x0e\n\x06not_in\x18\x07 \x03(\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf6\x04\n\nInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x05H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x05H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x05H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x05H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x05\x12\x0e\n\x06not_in\x18\x07 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf6\x04\n\nInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x03H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x03H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x03H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x03H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x03H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x03\x12\x0e\n\x06not_in\x18\x07 \x03(\x03\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf7\x04\n\x0bUInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\rH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\rH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\rH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\rH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\rH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\r\x12\x0e\n\x06not_in\x18\x07 \x03(\r\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf7\x04\n\x0bUInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x04H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x04H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x04H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x04\x12\x0e\n\x06not_in\x18\x07 \x03(\x04\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf7\x04\n\x0bSInt32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x11H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x11H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x11H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x11H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x11H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x11\x12\x0e\n\x06not_in\x18\x07 \x03(\x11\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf7\x04\n\x0bSInt64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x12H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x12H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x12H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x12H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x12H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x12\x12\x0e\n\x06not_in\x18\x07 \x03(\x12\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf8\x04\n\x0c\x46ixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x07H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x07H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x07H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x07H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x07H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x07\x12\x0e\n\x06not_in\x18\x07 \x03(\x07\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf8\x04\n\x0c\x46ixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x06H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x06H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x06H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x06H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x06H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x06\x12\x0e\n\x06not_in\x18\x07 \x03(\x06\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf9\x04\n\rSFixed32Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0fH\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x0fH\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x0fH\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x0fH\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x0fH\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x0f\x12\x0e\n\x06not_in\x18\x07 \x03(\x0f\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf9\x04\n\rSFixed64Rules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x10H\x02\x88\x01\x01\x12\x0f\n\x02lt\x18\x02 \x01(\x10H\x03\x88\x01\x01\x12\x0f\n\x02le\x18\x03 \x01(\x10H\x04\x88\x01\x01\x12\x0f\n\x02gt\x18\x04 \x01(\x10H\x05\x88\x01\x01\x12\x0f\n\x02ge\x18\x05 \x01(\x10H\x06\x88\x01\x01\x12\n\n\x02in\x18\x06 \x03(\x10\x12\x0e\n\x06not_in\x18\x07 \x03(\x10\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x07\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x0e \x01(\x02H\n\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0e\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x96\x03\n\tBoolRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x08H\x01\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x02 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x03 \x01(\x08H\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x04\x88\x01\x01\x12\x14\n\x07\x65xample\x18\x07 \x01(\x08H\x05\x88\x01\x01\x12\x12\n\x05\x66ield\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x11\n\x04type\x18\t \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\t\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\n\n\x08_exampleB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc8\x07\n\x0bStringRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\tH\x03\x88\x01\x01\x12\x10\n\x03len\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmin_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x17\n\nmax_length\x18\x04 \x01(\x04H\x06\x88\x01\x01\x12\x14\n\x07pattern\x18\x05 \x01(\tH\x07\x88\x01\x01\x12\x13\n\x06prefix\x18\x06 \x01(\tH\x08\x88\x01\x01\x12\x13\n\x06suffix\x18\x07 \x01(\tH\t\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x08 \x01(\tH\n\x88\x01\x01\x12\x19\n\x0cnot_contains\x18\t \x01(\tH\x0b\x88\x01\x01\x12\n\n\x02in\x18\n \x03(\t\x12\x0e\n\x06not_in\x18\x0b \x03(\t\x12\x0f\n\x05\x65mail\x18\x0c \x01(\x08H\x00\x12\x12\n\x08hostname\x18\r \x01(\x08H\x00\x12\x0c\n\x02ip\x18\x0e \x01(\x08H\x00\x12\x0e\n\x04ipv4\x18\x0f \x01(\x08H\x00\x12\x0e\n\x04ipv6\x18\x10 \x01(\x08H\x00\x12\r\n\x03uri\x18\x11 \x01(\x08H\x00\x12\x11\n\x07uri_ref\x18\x12 \x01(\x08H\x00\x12\x11\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08H\x00\x12\x0e\n\x04uuid\x18\x16 \x01(\x08H\x00\x12\x17\n\rpydantic_type\x18\x63 \x01(\tH\x00\x12\x13\n\x06\x65nable\x18\x17 \x01(\x08H\x0c\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x18 \x01(\tH\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x19 \x01(\tH\x01\x12\x16\n\x0cmiss_default\x18\x1a \x01(\x08H\x01\x12\x12\n\x08required\x18# \x01(\x08H\x01\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18$ \x01(\tH\x01\x12\x12\n\x05\x61lias\x18\x1b \x01(\tH\r\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x1c \x01(\tH\x0e\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x1e \x01(\tH\x02\x12\x19\n\x0f\x65xample_factory\x18\x1f \x01(\tH\x02\x12\x12\n\x05\x66ield\x18  \x01(\tH\x0f\x88\x01\x01\x12\x11\n\x04type\x18! \x01(\tH\x10\x88\x01\x01\x12\x12\n\x05title\x18\" \x01(\tH\x11\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x12\x88\x01\x01\x42\x0c\n\nwell_knownB\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x06\n\x04_lenB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\n\n\x08_patternB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\x0f\n\r_not_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\x86\x06\n\nBytesRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x0cH\x03\x88\x01\x01\x12\x17\n\nmin_length\x18\x02 \x01(\x04H\x04\x88\x01\x01\x12\x17\n\nmax_length\x18\x03 \x01(\x04H\x05\x88\x01\x01\x12\x13\n\x06prefix\x18\x05 \x01(\x0cH\x06\x88\x01\x01\x12\x13\n\x06suffix\x18\x06 \x01(\x0cH\x07\x88\x01\x01\x12\x15\n\x08\x63ontains\x18\x07 \x01(\x0cH\x08\x88\x01\x01\x12\n\n\x02in\x18\x08 \x03(\x0c\x12\x0e\n\x06not_in\x18\t \x03(\x0c\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\t\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0cH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x08required\x18\x1a \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18$ \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\n\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0bmultiple_of\x18\x10 \x01(\x02H\x0c\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x11 \x01(\x0cH\x01\x12\x19\n\x0f\x65xample_factory\x18\x12 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x13 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x14 \x01(\tH\x0e\x88\x01\x01\x12\x0c\n\x02ip\x18\x15 \x01(\x08H\x02\x12\x0e\n\x04ipv4\x18\x16 \x01(\x08H\x02\x12\x0e\n\x04ipv6\x18\x17 \x01(\x08H\x02\x12\x12\n\x05title\x18\x18 \x01(\tH\x0f\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x19 \x01(\tH\x10\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\nwell_knownB\x08\n\x06_constB\r\n\x0b_min_lengthB\r\n\x0b_max_lengthB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x0e\n\x0c_multiple_ofB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xcf\x03\n\tEnumRules\x12\x12\n\x05\x63onst\x18\x01 \x01(\x05H\x02\x88\x01\x01\x12\n\n\x02in\x18\x03 \x03(\x05\x12\x0e\n\x06not_in\x18\x04 \x03(\x05\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x05H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x05H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05title\x18\x12 \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x08\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_titleB\x08\n\x06_extra\"\xd0\x03\n\x0cMessageRules\x12\x11\n\x04skip\x18\x01 \x01(\x08H\x02\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x02H\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x02 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x04\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x05\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0f \x01(\x02H\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\x06\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x07\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x08\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\t\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x07\n\x05_skipB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xb3\x04\n\rRepeatedRules\x12\x16\n\tmin_items\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_items\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12\x13\n\x06unique\x18\x03 \x01(\x08H\x04\x88\x01\x01\x12,\n\x05items\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_itemsB\x0c\n\n_max_itemsB\t\n\x07_uniqueB\x08\n\x06_itemsB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xc6\x04\n\x08MapRules\x12\x16\n\tmin_pairs\x18\x01 \x01(\x04H\x02\x88\x01\x01\x12\x16\n\tmax_pairs\x18\x02 \x01(\x04H\x03\x88\x01\x01\x12+\n\x04keys\x18\x04 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x04\x88\x01\x01\x12-\n\x06values\x18\x05 \x01(\x0b\x32\x18.p2p_validate.FieldRulesH\x05\x88\x01\x01\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x06\x88\x01\x01\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x15 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x07\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x08\x88\x01\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\t\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\n\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x0c\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x0c\n\n_min_pairsB\x0c\n\n_max_pairsB\x07\n\x05_keysB\t\n\x07_valuesB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xb0\x03\n\x08\x41nyRules\x12\n\n\x02in\x18\x02 \x03(\t\x12\x0e\n\x06not_in\x18\x03 \x03(\t\x12\x13\n\x06\x65nable\x18\x08 \x01(\x08H\x02\x88\x01\x01\x12\x11\n\x07\x64\x65\x66\x61ult\x18\t \x01(\tH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x01 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x04\x88\x01\x01\x12\x11\n\x07\x65xample\x18\x0e \x01(\tH\x01\x12\x19\n\x0f\x65xample_factory\x18\x0f \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x10 \x01(\tH\x05\x88\x01\x01\x12\x12\n\x05title\x18\x11 \x01(\tH\x06\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\x07\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x08\n\x06_titleB\x08\n\x06_extra\"\xc2\x06\n\rDurationRules\x12-\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationH\x02\x88\x01\x01\x12*\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationH\x03\x88\x01\x01\x12*\n\x02le\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationH\x04\x88\x01\x01\x12*\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationH\x05\x88\x01\x01\x12*\n\x02ge\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationH\x06\x88\x01\x01\x12%\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.Duration\x12)\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x06\x65nable\x18\x0e \x01(\x08H\x07\x88\x01\x01\x12,\n\x07\x64\x65\x66\x61ult\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\n \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\x0b \x01(\x08H\x00\x12\x12\n\x08required\x18\x01 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0c \x01(\tH\x08\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\t\x88\x01\x01\x12,\n\x07\x65xample\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationH\x01\x12\x19\n\x0f\x65xample_factory\x18\x10 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x11 \x01(\tH\n\x88\x01\x01\x12\x11\n\x04type\x18\x12 \x01(\tH\x0b\x88\x01\x01\x12\x12\n\x05title\x18\x13 \x01(\tH\x0c\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x14 \x01(\tH\r\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra\"\xf3\x06\n\x0eTimestampRules\x12.\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12+\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12+\n\x02le\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x12+\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12+\n\x02ge\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x13\n\x06lt_now\x18\x07 \x01(\x08H\x07\x88\x01\x01\x12\x13\n\x06gt_now\x18\x08 \x01(\x08H\x08\x88\x01\x01\x12.\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationH\t\x88\x01\x01\x12\x13\n\x06\x65nable\x18\n \x01(\x08H\n\x88\x01\x01\x12-\n\x07\x64\x65\x66\x61ult\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12\x19\n\x0f\x64\x65\x66\x61ult_factory\x18\x0c \x01(\tH\x00\x12\x16\n\x0cmiss_default\x18\r \x01(\x08H\x00\x12\x12\n\x08required\x18\x01 \x01(\x08H\x00\x12\x1a\n\x10\x64\x65\x66\x61ult_template\x18\x16 \x01(\tH\x00\x12\x12\n\x05\x61lias\x18\x0e \x01(\tH\x0b\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x0f \x01(\tH\x0c\x88\x01\x01\x12-\n\x07\x65xample\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x12\x19\n\x0f\x65xample_factory\x18\x11 \x01(\tH\x01\x12\x12\n\x05\x66ield\x18\x12 \x01(\tH\r\x88\x01\x01\x12\x11\n\x04type\x18\x13 \x01(\tH\x0e\x88\x01\x01\x12\x12\n\x05title\x18\x14 \x01(\tH\x0f\x88\x01\x01\x12\x12\n\x05\x65xtra\x18\x15 \x01(\tH\x10\x88\x01\x01\x42\x10\n\x0e\x64\x65\x66\x61ult_configB\x10\n\x0e\x65xample_configB\x08\n\x06_constB\x05\n\x03_ltB\x05\n\x03_leB\x05\n\x03_gtB\x05\n\x03_geB\t\n\x07_lt_nowB\t\n\x07_gt_nowB\t\n\x07_withinB\t\n\x07_enableB\x08\n\x06_aliasB\x0e\n\x0c_descriptionB\x08\n\x06_fieldB\x07\n\x05_typeB\x08\n\x06_titleB\x08\n\x06_extra:4\n\x07ignored\x12\x1f.google.protobuf.MessageOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:3\n\x08required\x12\x1d.google.protobuf.OneofOptions\x18\xb1\x08 \x01(\x08\x88\x01\x01:Q\n\x0coneof_extend\x12\x1d.google.protobuf.OneofOptions\x18\xb2\x08 \x01(\x0b\x32\x18.p2p_validate.OneofRules\x88\x01\x01:J\n\x05rules\x12\x1d.google.protobuf.FieldOptions\x18\xb1\x08 \x01(\x0b\x32\x18.p2p_validate.FieldRules\x88\x01\x01\x62\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protos.p2p_validate_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protos.p2p_validate_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
+  google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(ignored)
+  google_dot_protobuf_dot_descriptor__pb2.OneofOptions.RegisterExtension(required)
+  google_dot_protobuf_dot_descriptor__pb2.OneofOptions.RegisterExtension(oneof_extend)
+  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(rules)
+
   DESCRIPTOR._options = None
-  _globals['_ONEOFRULES']._serialized_start=142
-  _globals['_ONEOFRULES']._serialized_end=172
-  _globals['_FIELDRULES']._serialized_start=175
-  _globals['_FIELDRULES']._serialized_end=1200
-  _globals['_FLOATRULES']._serialized_start=1203
-  _globals['_FLOATRULES']._serialized_end=1833
-  _globals['_DOUBLERULES']._serialized_start=1836
-  _globals['_DOUBLERULES']._serialized_end=2467
-  _globals['_INT32RULES']._serialized_start=2470
-  _globals['_INT32RULES']._serialized_end=3100
-  _globals['_INT64RULES']._serialized_start=3103
-  _globals['_INT64RULES']._serialized_end=3733
-  _globals['_UINT32RULES']._serialized_start=3736
-  _globals['_UINT32RULES']._serialized_end=4367
-  _globals['_UINT64RULES']._serialized_start=4370
-  _globals['_UINT64RULES']._serialized_end=5001
-  _globals['_SINT32RULES']._serialized_start=5004
-  _globals['_SINT32RULES']._serialized_end=5635
-  _globals['_SINT64RULES']._serialized_start=5638
-  _globals['_SINT64RULES']._serialized_end=6269
-  _globals['_FIXED32RULES']._serialized_start=6272
-  _globals['_FIXED32RULES']._serialized_end=6904
-  _globals['_FIXED64RULES']._serialized_start=6907
-  _globals['_FIXED64RULES']._serialized_end=7539
-  _globals['_SFIXED32RULES']._serialized_start=7542
-  _globals['_SFIXED32RULES']._serialized_end=8175
-  _globals['_SFIXED64RULES']._serialized_start=8178
-  _globals['_SFIXED64RULES']._serialized_end=8811
-  _globals['_BOOLRULES']._serialized_start=8814
-  _globals['_BOOLRULES']._serialized_end=9220
-  _globals['_STRINGRULES']._serialized_start=9223
-  _globals['_STRINGRULES']._serialized_end=10191
-  _globals['_BYTESRULES']._serialized_start=10194
-  _globals['_BYTESRULES']._serialized_end=10968
-  _globals['_ENUMRULES']._serialized_start=10971
-  _globals['_ENUMRULES']._serialized_end=11434
-  _globals['_MESSAGERULES']._serialized_start=11437
-  _globals['_MESSAGERULES']._serialized_end=11901
-  _globals['_REPEATEDRULES']._serialized_start=11904
-  _globals['_REPEATEDRULES']._serialized_end=12467
-  _globals['_MAPRULES']._serialized_start=12470
-  _globals['_MAPRULES']._serialized_end=13052
-  _globals['_ANYRULES']._serialized_start=13055
-  _globals['_ANYRULES']._serialized_end=13487
-  _globals['_DURATIONRULES']._serialized_start=13490
-  _globals['_DURATIONRULES']._serialized_end=14324
-  _globals['_TIMESTAMPRULES']._serialized_start=14327
-  _globals['_TIMESTAMPRULES']._serialized_end=15210
+  _ONEOFRULES._serialized_start=142
+  _ONEOFRULES._serialized_end=172
+  _FIELDRULES._serialized_start=175
+  _FIELDRULES._serialized_end=1200
+  _FLOATRULES._serialized_start=1203
+  _FLOATRULES._serialized_end=1833
+  _DOUBLERULES._serialized_start=1836
+  _DOUBLERULES._serialized_end=2467
+  _INT32RULES._serialized_start=2470
+  _INT32RULES._serialized_end=3100
+  _INT64RULES._serialized_start=3103
+  _INT64RULES._serialized_end=3733
+  _UINT32RULES._serialized_start=3736
+  _UINT32RULES._serialized_end=4367
+  _UINT64RULES._serialized_start=4370
+  _UINT64RULES._serialized_end=5001
+  _SINT32RULES._serialized_start=5004
+  _SINT32RULES._serialized_end=5635
+  _SINT64RULES._serialized_start=5638
+  _SINT64RULES._serialized_end=6269
+  _FIXED32RULES._serialized_start=6272
+  _FIXED32RULES._serialized_end=6904
+  _FIXED64RULES._serialized_start=6907
+  _FIXED64RULES._serialized_end=7539
+  _SFIXED32RULES._serialized_start=7542
+  _SFIXED32RULES._serialized_end=8175
+  _SFIXED64RULES._serialized_start=8178
+  _SFIXED64RULES._serialized_end=8811
+  _BOOLRULES._serialized_start=8814
+  _BOOLRULES._serialized_end=9220
+  _STRINGRULES._serialized_start=9223
+  _STRINGRULES._serialized_end=10191
+  _BYTESRULES._serialized_start=10194
+  _BYTESRULES._serialized_end=10968
+  _ENUMRULES._serialized_start=10971
+  _ENUMRULES._serialized_end=11434
+  _MESSAGERULES._serialized_start=11437
+  _MESSAGERULES._serialized_end=11901
+  _REPEATEDRULES._serialized_start=11904
+  _REPEATEDRULES._serialized_end=12467
+  _MAPRULES._serialized_start=12470
+  _MAPRULES._serialized_end=13052
+  _ANYRULES._serialized_start=13055
+  _ANYRULES._serialized_end=13487
+  _DURATIONRULES._serialized_start=13490
+  _DURATIONRULES._serialized_end=14324
+  _TIMESTAMPRULES._serialized_start=14327
+  _TIMESTAMPRULES._serialized_end=15210
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/validate_pb2.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: protos/validate.proto
-# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15protos/validate.proto\x12\x08validate\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x98\x07\n\nFieldRules\x12\'\n\x07message\x18\x11 \x01(\x0b\x32\x16.validate.MessageRules\x12%\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x14.validate.FloatRulesH\x00\x12\'\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x15.validate.DoubleRulesH\x00\x12%\n\x05int32\x18\x03 \x01(\x0b\x32\x14.validate.Int32RulesH\x00\x12%\n\x05int64\x18\x04 \x01(\x0b\x32\x14.validate.Int64RulesH\x00\x12\'\n\x06uint32\x18\x05 \x01(\x0b\x32\x15.validate.UInt32RulesH\x00\x12\'\n\x06uint64\x18\x06 \x01(\x0b\x32\x15.validate.UInt64RulesH\x00\x12\'\n\x06sint32\x18\x07 \x01(\x0b\x32\x15.validate.SInt32RulesH\x00\x12\'\n\x06sint64\x18\x08 \x01(\x0b\x32\x15.validate.SInt64RulesH\x00\x12)\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x16.validate.Fixed32RulesH\x00\x12)\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x16.validate.Fixed64RulesH\x00\x12+\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x17.validate.SFixed32RulesH\x00\x12+\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x17.validate.SFixed64RulesH\x00\x12#\n\x04\x62ool\x18\r \x01(\x0b\x32\x13.validate.BoolRulesH\x00\x12\'\n\x06string\x18\x0e \x01(\x0b\x32\x15.validate.StringRulesH\x00\x12%\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x14.validate.BytesRulesH\x00\x12#\n\x04\x65num\x18\x10 \x01(\x0b\x32\x13.validate.EnumRulesH\x00\x12+\n\x08repeated\x18\x12 \x01(\x0b\x32\x17.validate.RepeatedRulesH\x00\x12!\n\x03map\x18\x13 \x01(\x0b\x32\x12.validate.MapRulesH\x00\x12!\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x12.validate.AnyRulesH\x00\x12+\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x17.validate.DurationRulesH\x00\x12-\n\ttimestamp\x18\x16 \x01(\x0b\x32\x18.validate.TimestampRulesH\x00\x42\x06\n\x04type\"\x7f\n\nFloatRules\x12\r\n\x05\x63onst\x18\x01 \x01(\x02\x12\n\n\x02lt\x18\x02 \x01(\x02\x12\x0b\n\x03lte\x18\x03 \x01(\x02\x12\n\n\x02gt\x18\x04 \x01(\x02\x12\x0b\n\x03gte\x18\x05 \x01(\x02\x12\n\n\x02in\x18\x06 \x03(\x02\x12\x0e\n\x06not_in\x18\x07 \x03(\x02\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x80\x01\n\x0b\x44oubleRules\x12\r\n\x05\x63onst\x18\x01 \x01(\x01\x12\n\n\x02lt\x18\x02 \x01(\x01\x12\x0b\n\x03lte\x18\x03 \x01(\x01\x12\n\n\x02gt\x18\x04 \x01(\x01\x12\x0b\n\x03gte\x18\x05 \x01(\x01\x12\n\n\x02in\x18\x06 \x03(\x01\x12\x0e\n\x06not_in\x18\x07 \x03(\x01\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x7f\n\nInt32Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x05\x12\n\n\x02lt\x18\x02 \x01(\x05\x12\x0b\n\x03lte\x18\x03 \x01(\x05\x12\n\n\x02gt\x18\x04 \x01(\x05\x12\x0b\n\x03gte\x18\x05 \x01(\x05\x12\n\n\x02in\x18\x06 \x03(\x05\x12\x0e\n\x06not_in\x18\x07 \x03(\x05\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x7f\n\nInt64Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x03\x12\n\n\x02lt\x18\x02 \x01(\x03\x12\x0b\n\x03lte\x18\x03 \x01(\x03\x12\n\n\x02gt\x18\x04 \x01(\x03\x12\x0b\n\x03gte\x18\x05 \x01(\x03\x12\n\n\x02in\x18\x06 \x03(\x03\x12\x0e\n\x06not_in\x18\x07 \x03(\x03\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x80\x01\n\x0bUInt32Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\r\x12\n\n\x02lt\x18\x02 \x01(\r\x12\x0b\n\x03lte\x18\x03 \x01(\r\x12\n\n\x02gt\x18\x04 \x01(\r\x12\x0b\n\x03gte\x18\x05 \x01(\r\x12\n\n\x02in\x18\x06 \x03(\r\x12\x0e\n\x06not_in\x18\x07 \x03(\r\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x80\x01\n\x0bUInt64Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x04\x12\n\n\x02lt\x18\x02 \x01(\x04\x12\x0b\n\x03lte\x18\x03 \x01(\x04\x12\n\n\x02gt\x18\x04 \x01(\x04\x12\x0b\n\x03gte\x18\x05 \x01(\x04\x12\n\n\x02in\x18\x06 \x03(\x04\x12\x0e\n\x06not_in\x18\x07 \x03(\x04\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x80\x01\n\x0bSInt32Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x11\x12\n\n\x02lt\x18\x02 \x01(\x11\x12\x0b\n\x03lte\x18\x03 \x01(\x11\x12\n\n\x02gt\x18\x04 \x01(\x11\x12\x0b\n\x03gte\x18\x05 \x01(\x11\x12\n\n\x02in\x18\x06 \x03(\x11\x12\x0e\n\x06not_in\x18\x07 \x03(\x11\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x80\x01\n\x0bSInt64Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x12\x12\n\n\x02lt\x18\x02 \x01(\x12\x12\x0b\n\x03lte\x18\x03 \x01(\x12\x12\n\n\x02gt\x18\x04 \x01(\x12\x12\x0b\n\x03gte\x18\x05 \x01(\x12\x12\n\n\x02in\x18\x06 \x03(\x12\x12\x0e\n\x06not_in\x18\x07 \x03(\x12\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x81\x01\n\x0c\x46ixed32Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x07\x12\n\n\x02lt\x18\x02 \x01(\x07\x12\x0b\n\x03lte\x18\x03 \x01(\x07\x12\n\n\x02gt\x18\x04 \x01(\x07\x12\x0b\n\x03gte\x18\x05 \x01(\x07\x12\n\n\x02in\x18\x06 \x03(\x07\x12\x0e\n\x06not_in\x18\x07 \x03(\x07\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x81\x01\n\x0c\x46ixed64Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x06\x12\n\n\x02lt\x18\x02 \x01(\x06\x12\x0b\n\x03lte\x18\x03 \x01(\x06\x12\n\n\x02gt\x18\x04 \x01(\x06\x12\x0b\n\x03gte\x18\x05 \x01(\x06\x12\n\n\x02in\x18\x06 \x03(\x06\x12\x0e\n\x06not_in\x18\x07 \x03(\x06\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x82\x01\n\rSFixed32Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x0f\x12\n\n\x02lt\x18\x02 \x01(\x0f\x12\x0b\n\x03lte\x18\x03 \x01(\x0f\x12\n\n\x02gt\x18\x04 \x01(\x0f\x12\x0b\n\x03gte\x18\x05 \x01(\x0f\x12\n\n\x02in\x18\x06 \x03(\x0f\x12\x0e\n\x06not_in\x18\x07 \x03(\x0f\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x82\x01\n\rSFixed64Rules\x12\r\n\x05\x63onst\x18\x01 \x01(\x10\x12\n\n\x02lt\x18\x02 \x01(\x10\x12\x0b\n\x03lte\x18\x03 \x01(\x10\x12\n\n\x02gt\x18\x04 \x01(\x10\x12\x0b\n\x03gte\x18\x05 \x01(\x10\x12\n\n\x02in\x18\x06 \x03(\x10\x12\x0e\n\x06not_in\x18\x07 \x03(\x10\x12\x14\n\x0cignore_empty\x18\x08 \x01(\x08\"\x1a\n\tBoolRules\x12\r\n\x05\x63onst\x18\x01 \x01(\x08\"\xfd\x03\n\x0bStringRules\x12\r\n\x05\x63onst\x18\x01 \x01(\t\x12\x0b\n\x03len\x18\x13 \x01(\x04\x12\x0f\n\x07min_len\x18\x02 \x01(\x04\x12\x0f\n\x07max_len\x18\x03 \x01(\x04\x12\x11\n\tlen_bytes\x18\x14 \x01(\x04\x12\x11\n\tmin_bytes\x18\x04 \x01(\x04\x12\x11\n\tmax_bytes\x18\x05 \x01(\x04\x12\x0f\n\x07pattern\x18\x06 \x01(\t\x12\x0e\n\x06prefix\x18\x07 \x01(\t\x12\x0e\n\x06suffix\x18\x08 \x01(\t\x12\x10\n\x08\x63ontains\x18\t \x01(\t\x12\x14\n\x0cnot_contains\x18\x17 \x01(\t\x12\n\n\x02in\x18\n \x03(\t\x12\x0e\n\x06not_in\x18\x0b \x03(\t\x12\x0f\n\x05\x65mail\x18\x0c \x01(\x08H\x00\x12\x12\n\x08hostname\x18\r \x01(\x08H\x00\x12\x0c\n\x02ip\x18\x0e \x01(\x08H\x00\x12\x0e\n\x04ipv4\x18\x0f \x01(\x08H\x00\x12\x0e\n\x04ipv6\x18\x10 \x01(\x08H\x00\x12\r\n\x03uri\x18\x11 \x01(\x08H\x00\x12\x11\n\x07uri_ref\x18\x12 \x01(\x08H\x00\x12\x11\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08H\x00\x12\x0e\n\x04uuid\x18\x16 \x01(\x08H\x00\x12\x30\n\x10well_known_regex\x18\x18 \x01(\x0e\x32\x14.validate.KnownRegexH\x00\x12\x14\n\x06strict\x18\x19 \x01(\x08:\x04true\x12\x14\n\x0cignore_empty\x18\x1a \x01(\x08\x42\x0c\n\nwell_known\"\xfb\x01\n\nBytesRules\x12\r\n\x05\x63onst\x18\x01 \x01(\x0c\x12\x0b\n\x03len\x18\r \x01(\x04\x12\x0f\n\x07min_len\x18\x02 \x01(\x04\x12\x0f\n\x07max_len\x18\x03 \x01(\x04\x12\x0f\n\x07pattern\x18\x04 \x01(\t\x12\x0e\n\x06prefix\x18\x05 \x01(\x0c\x12\x0e\n\x06suffix\x18\x06 \x01(\x0c\x12\x10\n\x08\x63ontains\x18\x07 \x01(\x0c\x12\n\n\x02in\x18\x08 \x03(\x0c\x12\x0e\n\x06not_in\x18\t \x03(\x0c\x12\x0c\n\x02ip\x18\n \x01(\x08H\x00\x12\x0e\n\x04ipv4\x18\x0b \x01(\x08H\x00\x12\x0e\n\x04ipv6\x18\x0c \x01(\x08H\x00\x12\x14\n\x0cignore_empty\x18\x0e \x01(\x08\x42\x0c\n\nwell_known\"L\n\tEnumRules\x12\r\n\x05\x63onst\x18\x01 \x01(\x05\x12\x14\n\x0c\x64\x65\x66ined_only\x18\x02 \x01(\x08\x12\n\n\x02in\x18\x03 \x03(\x05\x12\x0e\n\x06not_in\x18\x04 \x03(\x05\".\n\x0cMessageRules\x12\x0c\n\x04skip\x18\x01 \x01(\x08\x12\x10\n\x08required\x18\x02 \x01(\x08\"\x80\x01\n\rRepeatedRules\x12\x11\n\tmin_items\x18\x01 \x01(\x04\x12\x11\n\tmax_items\x18\x02 \x01(\x04\x12\x0e\n\x06unique\x18\x03 \x01(\x08\x12#\n\x05items\x18\x04 \x01(\x0b\x32\x14.validate.FieldRules\x12\x14\n\x0cignore_empty\x18\x05 \x01(\x08\"\xa3\x01\n\x08MapRules\x12\x11\n\tmin_pairs\x18\x01 \x01(\x04\x12\x11\n\tmax_pairs\x18\x02 \x01(\x04\x12\x11\n\tno_sparse\x18\x03 \x01(\x08\x12\"\n\x04keys\x18\x04 \x01(\x0b\x32\x14.validate.FieldRules\x12$\n\x06values\x18\x05 \x01(\x0b\x32\x14.validate.FieldRules\x12\x14\n\x0cignore_empty\x18\x06 \x01(\x08\"8\n\x08\x41nyRules\x12\x10\n\x08required\x18\x01 \x01(\x08\x12\n\n\x02in\x18\x02 \x03(\t\x12\x0e\n\x06not_in\x18\x03 \x03(\t\"\xbb\x02\n\rDurationRules\x12\x10\n\x08required\x18\x01 \x01(\x08\x12(\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12%\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03lte\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12%\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03gte\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12%\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.Duration\x12)\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.Duration\"\xba\x02\n\x0eTimestampRules\x12\x10\n\x08required\x18\x01 \x01(\x08\x12)\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x03lte\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x03gte\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06lt_now\x18\x07 \x01(\x08\x12\x0e\n\x06gt_now\x18\x08 \x01(\x08\x12)\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration*F\n\nKnownRegex\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x14\n\x10HTTP_HEADER_NAME\x10\x01\x12\x15\n\x11HTTP_HEADER_VALUE\x10\x02:2\n\x08\x64isabled\x12\x1f.google.protobuf.MessageOptions\x18\xaf\x08 \x01(\x08:1\n\x07ignored\x12\x1f.google.protobuf.MessageOptions\x18\xb0\x08 \x01(\x08:0\n\x08required\x12\x1d.google.protobuf.OneofOptions\x18\xaf\x08 \x01(\x08:C\n\x05rules\x12\x1d.google.protobuf.FieldOptions\x18\xaf\x08 \x01(\x0b\x32\x14.validate.FieldRulesBP\n\x1aio.envoyproxy.pgv.validateZ2github.com/envoyproxy/protoc-gen-validate/validate')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protos.validate_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protos.validate_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'\n\032io.envoyproxy.pgv.validateZ2github.com/envoyproxy/protoc-gen-validate/validate'
-  _globals['_KNOWNREGEX']._serialized_start=4539
-  _globals['_KNOWNREGEX']._serialized_end=4609
-  _globals['_FIELDRULES']._serialized_start=135
-  _globals['_FIELDRULES']._serialized_end=1055
-  _globals['_FLOATRULES']._serialized_start=1057
-  _globals['_FLOATRULES']._serialized_end=1184
-  _globals['_DOUBLERULES']._serialized_start=1187
-  _globals['_DOUBLERULES']._serialized_end=1315
-  _globals['_INT32RULES']._serialized_start=1317
-  _globals['_INT32RULES']._serialized_end=1444
-  _globals['_INT64RULES']._serialized_start=1446
-  _globals['_INT64RULES']._serialized_end=1573
-  _globals['_UINT32RULES']._serialized_start=1576
-  _globals['_UINT32RULES']._serialized_end=1704
-  _globals['_UINT64RULES']._serialized_start=1707
-  _globals['_UINT64RULES']._serialized_end=1835
-  _globals['_SINT32RULES']._serialized_start=1838
-  _globals['_SINT32RULES']._serialized_end=1966
-  _globals['_SINT64RULES']._serialized_start=1969
-  _globals['_SINT64RULES']._serialized_end=2097
-  _globals['_FIXED32RULES']._serialized_start=2100
-  _globals['_FIXED32RULES']._serialized_end=2229
-  _globals['_FIXED64RULES']._serialized_start=2232
-  _globals['_FIXED64RULES']._serialized_end=2361
-  _globals['_SFIXED32RULES']._serialized_start=2364
-  _globals['_SFIXED32RULES']._serialized_end=2494
-  _globals['_SFIXED64RULES']._serialized_start=2497
-  _globals['_SFIXED64RULES']._serialized_end=2627
-  _globals['_BOOLRULES']._serialized_start=2629
-  _globals['_BOOLRULES']._serialized_end=2655
-  _globals['_STRINGRULES']._serialized_start=2658
-  _globals['_STRINGRULES']._serialized_end=3167
-  _globals['_BYTESRULES']._serialized_start=3170
-  _globals['_BYTESRULES']._serialized_end=3421
-  _globals['_ENUMRULES']._serialized_start=3423
-  _globals['_ENUMRULES']._serialized_end=3499
-  _globals['_MESSAGERULES']._serialized_start=3501
-  _globals['_MESSAGERULES']._serialized_end=3547
-  _globals['_REPEATEDRULES']._serialized_start=3550
-  _globals['_REPEATEDRULES']._serialized_end=3678
-  _globals['_MAPRULES']._serialized_start=3681
-  _globals['_MAPRULES']._serialized_end=3844
-  _globals['_ANYRULES']._serialized_start=3846
-  _globals['_ANYRULES']._serialized_end=3902
-  _globals['_DURATIONRULES']._serialized_start=3905
-  _globals['_DURATIONRULES']._serialized_end=4220
-  _globals['_TIMESTAMPRULES']._serialized_start=4223
-  _globals['_TIMESTAMPRULES']._serialized_end=4537
+  google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(disabled)
+  google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(ignored)
+  google_dot_protobuf_dot_descriptor__pb2.OneofOptions.RegisterExtension(required)
+  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(rules)
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\032io.envoyproxy.pgv.validateZ2github.com/envoyproxy/protoc-gen-validate/validate'
+  _KNOWNREGEX._serialized_start=4539
+  _KNOWNREGEX._serialized_end=4609
+  _FIELDRULES._serialized_start=135
+  _FIELDRULES._serialized_end=1055
+  _FLOATRULES._serialized_start=1057
+  _FLOATRULES._serialized_end=1184
+  _DOUBLERULES._serialized_start=1187
+  _DOUBLERULES._serialized_end=1315
+  _INT32RULES._serialized_start=1317
+  _INT32RULES._serialized_end=1444
+  _INT64RULES._serialized_start=1446
+  _INT64RULES._serialized_end=1573
+  _UINT32RULES._serialized_start=1576
+  _UINT32RULES._serialized_end=1704
+  _UINT64RULES._serialized_start=1707
+  _UINT64RULES._serialized_end=1835
+  _SINT32RULES._serialized_start=1838
+  _SINT32RULES._serialized_end=1966
+  _SINT64RULES._serialized_start=1969
+  _SINT64RULES._serialized_end=2097
+  _FIXED32RULES._serialized_start=2100
+  _FIXED32RULES._serialized_end=2229
+  _FIXED64RULES._serialized_start=2232
+  _FIXED64RULES._serialized_end=2361
+  _SFIXED32RULES._serialized_start=2364
+  _SFIXED32RULES._serialized_end=2494
+  _SFIXED64RULES._serialized_start=2497
+  _SFIXED64RULES._serialized_end=2627
+  _BOOLRULES._serialized_start=2629
+  _BOOLRULES._serialized_end=2655
+  _STRINGRULES._serialized_start=2658
+  _STRINGRULES._serialized_end=3167
+  _BYTESRULES._serialized_start=3170
+  _BYTESRULES._serialized_end=3421
+  _ENUMRULES._serialized_start=3423
+  _ENUMRULES._serialized_end=3499
+  _MESSAGERULES._serialized_start=3501
+  _MESSAGERULES._serialized_end=3547
+  _REPEATEDRULES._serialized_start=3550
+  _REPEATEDRULES._serialized_end=3678
+  _MAPRULES._serialized_start=3681
+  _MAPRULES._serialized_end=3844
+  _ANYRULES._serialized_start=3846
+  _ANYRULES._serialized_end=3902
+  _DURATIONRULES._serialized_start=3905
+  _DURATIONRULES._serialized_end=4220
+  _TIMESTAMPRULES._serialized_start=4223
+  _TIMESTAMPRULES._serialized_end=4537
 # @@protoc_insertion_point(module_scope)
```

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/protos/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/types.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/protobuf_to_pydantic/util.py` & `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/util.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6/pyproject.toml` & `protobuf_to_pydantic-0.2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protobuf_to_pydantic"
-version = "v0.2.6"
+version = "v0.2.6.1"
 description = "Generate the `pydantic.BaseModel` class (and the corresponding source code) with parameter verification function through the Protobuf file"
 authors = ["So1n <so1n897046026@gmail.com>"]
 license = "Apache Software License"
 readme = "./README.md"
 repository = "https://github.com/so1n/protobuf_to_pydantic"
 homepage = "https://github.com/so1n/protobuf_to_pydantic"
 packages = [
@@ -14,15 +14,15 @@
 [tool.poetry.scripts]
 protoc-gen-protobuf-to-pydantic = "protobuf_to_pydantic.plugin.main:main"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = ">=1.9.2, <3.0.0"
-grpcio-tools = "^1.40.0"
+protobuf = ">=3.20.3"
 
 toml = {version = "^0.10.2", optional = true}
 lark = { version = "^1.1.2", optional = true }
 mypy-protobuf = { version = "^3.2.0", optional = true }
 
 [tool.poetry.extras]
 lark = ["lark"]
@@ -39,14 +39,15 @@
 pre-commit = "2.14.0"
 autoflake = "1.4"
 flake8 = "3.9.2"
 # if pydantic version >= 2.0.0, email-validator version must >= 2.0.0
 email-validator = "2.0.0"
 # fix flake8 run bug: https://stackoverflow.com/questions/73929564/entrypoints-object-has-no-attribute-get-digital-ocean
 importlib-metadata = "4.11.4"
+grpcio-tools = ">=1.40.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "6.2.5"
 
 [tool.protobuf-to-pydantic.format]
 black = true
 isort = true
```

### Comparing `protobuf_to_pydantic-0.2.6/setup.py` & `protobuf_to_pydantic-0.2.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'protobuf_to_pydantic.protos.old.protos',
  'protobuf_to_pydantic.protos.protos']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['grpcio-tools>=1.40.0,<2.0.0', 'pydantic>=1.9.2,<3.0.0']
+['protobuf>=3.20.3', 'pydantic>=1.9.2,<3.0.0']
 
 extras_require = \
 {'all': ['toml>=0.10.2,<0.11.0',
          'lark>=1.1.2,<2.0.0',
          'mypy-protobuf>=3.2.0,<4.0.0'],
  'lark': ['lark>=1.1.2,<2.0.0'],
  'mypy-protobuf': ['mypy-protobuf>=3.2.0,<4.0.0'],
@@ -30,17 +30,17 @@
 
 entry_points = \
 {'console_scripts': ['protoc-gen-protobuf-to-pydantic = '
                      'protobuf_to_pydantic.plugin.main:main']}
 
 setup_kwargs = {
     'name': 'protobuf-to-pydantic',
-    'version': '0.2.6',
+    'version': '0.2.6.1',
     'description': 'Generate the `pydantic.BaseModel` class (and the corresponding source code) with parameter verification function through the Protobuf file',
-    'long_description': '# protobuf_to_pydantic\nGenerate Pydantic Model or source code with parameter verification function based on Protobuf file (Proto3).\n\n\n[中文文档](https://github.com/so1n/protobuf_to_pydantic/blob/master/README_ZH.md)\n\n# Feature\n\nFeature：\n- [x] Generate source code through `Protobuf` plugin。\n- [x] Generate `Pydantic Model` or source code by parsing `Protobuf Message` in `Python` runtime.\n- [x] Compatible with `V1` and `V2` versions of `Pydantic`。\n- [x] Supports multiple verification rules and is compatible with `proto-gen-validate` (subsequent versions will support the rules of `proto-gen-validate` 1.0)。\n- [x] Support custom functionality through templates。\n- [ ] Supports `protovalidate` verification rules（`proto-gen-validate` version >= 1.0）\n\nThe following is a functional overview diagram of `protobuf-to-pydantic`.\nIn the picture `P2P` represents `protobuf-to-pydantic`, `Protoc` represents the command for `Protobuf` to generate code, and `plugin` represents ` Plugin for Protoc`:\n![protobuf-to-pydantic](https://github.com/so1n/protobuf_to_pydantic/blob/master/images/protobuf-to-pydantic_index.png?raw=true)\n\n# Installation\nBy default, `protobuf-to-pydantic` can be installed directly via the following command:\n```bash\npip install protobuf_to_pydantic\n```\nIf want to use the full functionality of `protobuf-to-pydantic`, can install `protobuf-to-pydantic` with the following command:.\n```bash\npip install protobuf_to_pydantic[all]\n```\n# Usage\n## 1.code generation\n`protobuf-to-pydantic` currently has two methods to generate `Pydantic Model` objects based on Protobuf files.：\n- 1: Use the `Protoc` plug-in to generate the corresponding `Python` code file through the Protobuf file。\n- 2: Generate the corresponding `Pydantic Model` object through the `Message` object in `Python` runtime。\n\n### 1.1.Directly generate `Pydantic Model` code files through plug-ins\n#### 1.1.0.Install dependencies\nThe `protobuf-to-pydantic` plug-in depends on `mypy-protobuf`, need to install `mypy-protobuf` through the following command first:\n```bash\npython -m pip install protobuf-to-pydantic[mypy-protobuf]\n```\nor\n```bash\npoetry add protobuf-to-pydantic -E mypy-protobuf\n```\n#### 1.1.1.Use plugins\nPlug-in is the `Pydantic Model` source code generation method recommended by `protobuf-to-pydantic`.\nIt supports the most complete functions and is also very simple to use.\n\nAssume that it is usually generated through the following command Code corresponding to Protobuf file:\n```bash\npython -m grpc_tools.protoc -I. example.proto\n```\nAfter installing `protobuf-to-pydantic`,can use the `protobuf-to-pydantic` plugin with the `--protobuf-to-pydantic_out` option with the following command:\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=. example.proto\n```\n\nIn this command, `--protobuf-to-pydantic_out=.` means using the `prorobuf-to-pydantic` plug-in,\nAnd it is declared that the output location of the `protobuf-to-pydantic` plug-in is `.`\n\n> `.` indicates the output path used by `grpc_tools.proto`.\n\nAfter running the command, the `protobuf-to-pydantic` plugin writes the generated source code to a file with the filename suffix `p2p.py`, e.g., `example.proto` generates a file with the name `example_p2p.py`.\n\n\n#### 1.1.2.Plug-in configuration\nThe `protobuf-to-pydantic` plugin supports loading configuration by reading a `Python` file。\n\n> In order to ensure that the variables of the configuration file can be introduced normally, the configuration file must be stored in the current path of the running command.。\n\nAn example configuration that can be read by `protobuf-to-pydantic` is as follows:\n```Python\nimport logging\nfrom typing import List, Type\n\nfrom google.protobuf.any_pb2 import Any  # type: ignore\nfrom pydantic import confloat, conint\nfrom pydantic.fields import FieldInfo\n\nfrom protobuf_to_pydantic.desc_template import DescTemplate\n\n# Configure the log output format and log level of the plugin, which is very useful when debugging\nlogging.basicConfig(format="[%(asctime)s %(levelname)s] %(message)s", datefmt="%y-%m-%d %H:%M:%S", level=logging.DEBUG)\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\ndef customer_any() -> Any:\n    return Any  # type: ignore\n\n\n# For the configuration of the local template, see the use of the local template for details\nlocal_dict = {\n    "CustomerField": CustomerField,\n    "confloat": confloat,\n    "conint": conint,\n    "customer_any": customer_any,\n}\n# Specifies the start of key comments\ncomment_prefix = "p2p"\n# Specify the class of the template, can extend the template by inheriting this class, see the chapter on custom templates for details\ndesc_template: Type[DescTemplate] = DescTemplate\n# Specify the protobuf files of which packages to ignore, and the messages of the ignored packages will not be parsed\nignore_pkg_list: List[str] = ["validate", "p2p_validate"]\n# Specifies the generated file name suffix (without .py)\nfile_name_suffix = "_p2p"\n```\nNext, in order to be able to read this file, need to change the `--protobuf-to-pydantic_out=. ` to ` --protobuf-to-pydantic_out=config_path=plugin_config.py:. `.\nwhere the left side of `:` indicates that the configuration file path to be read is `plugin_config.py`, and the right side of `:` declares that the output location of the `protobuf-to-pydantic` plugin is `. `\nThe final complete command is as follows：\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto\n```\nThrough this command, can load the corresponding configuration and run the `protobuf-to-pydantic` plug-in。\n\nIn addition to the configuration options in the example configuration file,\nthe `protobuf-to-pydantic` plug-in also supports other configuration options.\nThe specific configuration instructions are as follows：\n\n| Configuration name            | Functional module                      | Type                                            | Hidden meaning                                                                                                                                      |\n|-------------------------------|----------------------------------------|-------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|\n| local_dict                    | Template                               | dict                                            | Holds variables for the `local` template                                                                                                            |\n| desc_template                 | Template                               | protobuf_to_pydantic.desc_template.DescTemplate | Implementation of the template class                                                                                                                |\n| comment_prefix                | Template                               | str                                             | Comment prefix.Only strings with a fixed prefix will be used by the template                                                                        |\n| customer_import_set           | Code generation                        | `Set[str]`                                      | A collection of custom import statements, such as `from typing import Set`or `import typing`, that will write data in order to the source code file |\n| customer_deque                | Code generation                        | `deque[str]`                                    | Custom source file content, used to add custom content                                                                                              |\n| module_path                   | str                                    | str                                             | Used to define the root path of the project or module, which helps `protobuf-to-pydantic`to better automatically generate module import statements   |\n| pyproject_file_path           | Code generation                        | str                                             | Define the pyproject file path, which defaults to the current project path                                                                          |\n| code_indent                   | Code generation                        | int                                             | Defines the number of indentation Spaces in the code; the default is 4                                                                              |\n| ignore_pkg_list               | Code generation(Limit plug-ins only)   | `list[str]`                                     | Definition ignores parsing of the specified package file                                                                                            |\n| base_model_class              | Model Code generation, Code generation | `Type[BaseModel]`                               | Define the parent class of the generated Model                                                                                                      |\n| file_name_suffix              | Code generation                        | str                                             | Define the generated file suffix, default `_p2p.py`                                                                                                 |\n| file_descriptor_proto_to_code | Code generation(Limit plug-ins only)   | `Type[FileDescriptorProtoToCode]`               | Define the `FileDescriptorProtoToCode` to use                                                                                                       |\n\n\n#### 1.1.3.buf-cli\nIf you are using `buf-cli` to manage Protobuf files,\nthen you can also use `protobuf-to-pydantic` in `buf-cli`, See [How to use `protobuf-to-pydantic` in `buf-cli`](https://github.com/so1n/protobuf_to_pydantic/blob/master/buf-plugin/README.md)\n\n### 1.2.Generate a `Pydantic Model` object in Python runtime\n`protobuf_to_pydantic` can generate the corresponding `PydanticModel` object based on the `Message` object at runtime。\n\nFor example, the `UserMessage` in the following Protobuf file named `demo.proto`:\n```protobuf\n// path: ./demo.proto\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\nmessage UserMessage {\n  string uid=1;\n  int32 age=2;\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  string user_name=6;\n}\n```\n`grpc_tools.protoc` can be used to generate the Python code file corresponding to the `Protobuf` file (the file name is `demo_pb2.py`), and the code related to the `UserMessage` is stored in the code file.\n\nAt `Python` runtime, The func `msg_to_pydantic_model` can be called to read the `UserMessage` object from the `demo_pb2` module and generate the corresponding `Pydantic Model` object as follows:\n```Python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom . import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n\n# output\n# {\n#   `uid`: FieldInfo(default=``, extra={}),\n#   `age`: FieldInfo(default=0, extra={}),\n#   `height`: FieldInfo(default=0.0, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, extra={})\n#  }\n```\nThrough the output results, it can be found that the generated `pydantic.BaseModel` object also contains `uid`, `age`, `height`, `sex`, `is adult` and `user name` fields,\nand the `default` property matches the zero value of the Protobuf type。\n\nThe `msg_to_pydantic_model` func is customizable just like plugins, with the following extension parameters:\n\n| Fields                                    | Meaning                                                   |\n|-------------------------------------------|-----------------------------------------------------------|\n| default_field                             | Generate a `Field` for each field in the `Pydantic Model` |\n| comment_prefix                            | The prefix of a comment that can be parsed                |\n| parse_msg_desc_method                     | Parsing rules to use                                      |\n| local_dict                                | Variables used by the `local` template                    |\n| pydantic_base                             | Generates the parent class of the `Pydantic Model` object |\n| pydantic_module                           | Generate the `Module` of the `Pydantic Model` object      |\n| desc_template                             | Template class to use                                     |\n| message_type_dict_by_type_name            | Protobuf type mapping to `Python` type                    |\n| message_default_factory_dict_by_type_name | Protobuf type mapping to the Python type factory          |\n\n\nIn addition to generating the corresponding `Pydantic Model` object at runtime,\n`protobuf-to-pydantic` also supports converting `Pydantic Model` objects to Python code text at runtime (only compatible with `Pydantic Model` objects generated by `protobuf-to-pydantic`).\nThe `pydantic_model_to_py_code` func is used to generate the source code, and the `pydantic_model_to_py_file` func is used to generate the code file. The example code of the `pydantic_model_to_py_file` func is as follows:\n\n```Python\nfrom protobuf_to_pydantic import msg_to_pydantic_model, pydantic_model_to_py_file\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\npydantic_model_to_py_file(\n    "./demo_gen_code.py",\n    msg_to_pydantic_model(demo_pb2.NestedMessage),\n)\n```\nWhen the code runs, it converts`demo_pb2.NestedMessage`to a Pydantic Model object and passes it to the  `pydantic_model_to_py_file`. `pydantic_model_to_py_file` generates the source code and writes it to a `demo_gen_code.py` file.\n\n\n## 2.Parameter validation\nIn the previous section, the `Pydantic Model` object generated by the Protobuf file is very simple because the Protobuf file does not have enough parameters to verify the relevant information.\nIn order for each field in the generated `Pydantic Model` object to have parameter validation capabilities, the corresponding parameter checking rules for the field need to be refined in the Protobuf file.\n\nCurrently, `protobuf-to-pydantic` supports three validation rules：\n- 1.Text annotations\n- 2.PGV(protoc-geb-validate)\n- 3.P2P\n\nWith these rules, the `Pydantic Model` object generated by `protobuf-to-pydantic` will have parameter validation feature.\nAmong them, text annotations and P2P rules are consistent, they both support most of the parameters in `Pydantic Field`, some of the variations and new parameters are seen\n[2.4.`P2P` and text annotation rule other parameter support](#24p2p-and-text-comment-rule-other-parameter-support)\n\n> NOTE:\n>  - 1.Text annotation rules are not the focus of subsequent functional iterative development, and it is recommended to use P2P verification rules.\n>  - 2.`Protoc Plug-in` only support `PGV` and `P2P` rule.\n\n\n### 2.1.Text annotations\nIn the Protobuf file, can write annotations for each field that meet the requirements of `protobuf-to-pydantic`,\nso that `protobuf-to-pydantic` can obtain the validation information of the parameters when parsing the Protobuf file, such as the following example\n```protobuf\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\n// user info\nmessage UserMessage {\n  // p2p: {"required": true, "example": "10086"}\n  // p2p: {"title": "UID"}\n  string uid=1; // p2p: {"description": "user union id"}\n  // p2p: {"example": 18, "title": "use age", "ge": 0}\n  int32 age=2;\n  // p2p: {"ge": 0, "le": 2.5}\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  // p2p: {"description": "user name"}\n  // p2p: {"default": "", "min_length": 1, "max_length": "10", "example": "so1n"}\n  string user_name=6;\n}\n```\n\nIn this example, each annotation that can be used by `protobuf_to_pydantic` starts with `p2p:` (supports customization) and is followed by a complete Json string. If are familiar with the usage of `pydantic`, can find This Json string contains the verification information corresponding to `pydantic.Field`. For example, the `uid` field in `UserMessage` contains a total of 4 pieces of information as follows：\n\n| Column      | Meaning                                                                               |\n|-------------|---------------------------------------------------------------------------------------|\n| required    | Indicates that the generated field does not have a default value                      |\n| example     | An example value representing the generated field is 10086                            |\n| title       | Indicates that the schema name of the field is UID                                    |\n | description | The schema documentation for the representation field is described as `user_union_id` |\n\n> Note:\n>   - 1.Currently only single-line comments are supported and comments must be a complete Json data (no line breaks).\n>   - 2.multi line comments are not supported。\n\nWhen these annotations are written, `protobuf_to_pydantic` will bring the corresponding information for each field when converting the Message into the corresponding `Pydantic.BaseModel` object, as follows:\n\n```python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage, parse_msg_desc_method=demo_pb2)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `uid`: FieldInfo(default=PydanticUndefined, title=`UID`, description=`user union id`, extra={`example`: `10086`}),\n#   `age`: FieldInfo(default=0, title=`use age`, ge=0, extra={`example`: 18}),\n#   `height`: FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, description=`user name`, min_length=1, max_length=10, extra={`example`: `so1n`})\n# }\n```\nIt can be seen that the output fields carry the corresponding information, which is consistent with the comments of the Protobuf file.\n\nIn addition, this code differs from the previous section in that the `msg_to_pydantic_model` function has a keyword argument named `parse_msg_desc_method` and its value is the \'demo_pb2\' module.\nThis parameter enables `protobuf-to-pydantic` to obtain additional information about each field in the Message object through comments in the `.pyi` file of the `demo_pb2` module.\n\n> Note: This function needs to use the [mypy-protobuf](https://github.com/nipunn1313/mypy-protobuf) plugin when generating the corresponding `Python code through the Protobuf file, and the specified pyi file output path is the same as the generated `Python` code path to take effect.\n> And need to install `protobuf-to-pydantic` via the `python -m pip install protobuf-to-pydantic[mypy-protobuf]` command\n\nIn addition to getting comments from the `.pyi` file, `protobuf-to-pydantic` also supports getting comment information for each field through comments on the Protobuf file to which the Message object belongs.\nUsing this feature is as simple as setting the value of `parse_msg_desc_method` to the root directory path specified when the Message object was generated.\n\n> When using this method, make sure to install `protobuf-to-pydantic` via `python -m pip install protobuf-to-pydantic[lark]`, and also make sure that the Protobuf file exists in the project.\n\nFor example, the project structure of the `protobuf-to-pydantic` sample code is as follows:\n```bash\n./protobuf_to_pydantic/\n├── example/\n│ ├── python_example_proto_code/\n│ └── example_proto/\n├── protobuf_to_pydantic/\n└── /\n```\n\nThe Protobuf file is stored in the `example/example_proto` folder, and then run the following command in the `example` directory to generate the `Python` code file corresponding to Protobuf:\n```bash\ncd example\n\npython -m grpc_tools.protoc\n  --python_out=./python_example_proto_code \\\n  --grpc_python_out=./python_example_proto_code \\\n  -I. \\\n```\nThen the path that needs to be filled in for `parse_msg_desc_method` at this time is `./protobuf_to_pydantic/example`.\nThe following sample code:\n```python\n# pydantic Version v1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.UserMessage, parse_msg_desc_method="./protobuf_to_pydantic/example"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `uid`: FieldInfo(default=PydanticUndefined, title=`UID`, description=`user union id`, extra={`example`: `10086`}),\n#   `age`: FieldInfo(default=0, title=`use age`, ge=0, extra={`example`: 18}),\n#   `height`: FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, description=`user name`, min_length=1, max_length=10, extra={`example`: `so1n`})\n# }\n```\nAs you can see, the only difference in this code is the value of the `parse_msg_desc_method`, but through the output result, you can see that the field carries the same information as the result obtained through the module.\n\n### 2.2.PGV(protoc-gen-validate)\nAt present, the commonly used parameter verification project in the Protobuf ecosystem is [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate)，\nIt has become a common standard in Protobuf because it supports multiple languages and requires only one writing of `PGV` rules to make the generated `Message` object support the corresponding validation rules.\n\n> Currently `protobuf-to-pydantic` only supports rules that [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate) is less than version 1.0.0\n\n`protobuf-to-pydantic` supports parsing of `PGV` validation rules and generates `Pydantic Model` objects with validation logic functions.\nUsing `PGV` checksum rules in `protobuf-to-pydantic` is very simple, just write the corresponding `PGV` rules in the Protobuf file first,\nand then specify the value of `parse_msg_desc_method` to be `PGV` when calling `msg_to_pydantic_model` as the code below:\n```Python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.validate import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest, parse_msg_desc_method="PGV"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `const_test`: FieldInfo(default=1.0, const=True, extra={}),\n#   `range_e_test`: FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   `range_test`: FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   `in_test`: FieldInfo(default=0.0, extra={`in`: [1.0, 2.0, 3.0]}),\n#   `not_in_test`: FieldInfo(default=0.0, extra={`not_in`: [1.0, 2.0, 3.0]}),\n#   `ignore_test`: FieldInfo(default=0.0, extra={})\n# }\n```\n\n> Note:\n>  - 1.For the usage of `PGV`, see: [protoc-gen-validate doc](https://github.com/bufbuild/protoc-gen-validate/blob/v0.10.2-SNAPSHOT.17/README.md)\n>  - 2.Need to install `PGV` through `pip install protoc_gen_validate` or download [validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/common/validate.proto) to the protobuf directory in the project to write pgv rules in the Protobuf file.\n\n\n### 2.3.P2P\nThe `PGV` verification rules are written in the Option attribute of each field of `Message` and have a better code specification,\nso Protobuf that use `PGV` checksum rules will be more readable than Protobuf that use annotation .\n\nAt the same time, when writing `PGV` rules, can also experience the convenience of the IDE\'s auto-completion and the security of checksumming when generating the corresponding language objects from Protobuf files, but it only supports checksumming-related logic, which is not as rich as the file annotation mode.\n\n\nThe `P2P` verification rule that comes with `protobuf-to-pydantic` expands on the `PGV` verification rule by incorporating some of the functionality of the text annotation verification rule, which satisfies most of the customization of the properties of each `Field` in the `Pydantic Model`, such as the following Protobuf file.\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\n\nimport "example_proto/common/p2p_validate.proto";\n\n\nmessage FloatTest {\n  float const_test = 1 [(p2p_validate.rules).float.const = 1];\n  float range_e_test = 2 [(p2p_validate.rules).float = {ge: 1, le: 10}];\n  float range_test = 3[(p2p_validate.rules).float = {gt: 1, lt: 10}];\n  float in_test = 4[(p2p_validate.rules).float = {in: [1,2,3]}];\n  float not_in_test = 5[(p2p_validate.rules).float = {not_in: [1,2,3]}];\n  float default_test = 6[(p2p_validate.rules).float.default = 1.0];\n  float not_enable_test = 7[(p2p_validate.rules).float.enable = false];\n  float default_factory_test = 8[(p2p_validate.rules).float.default_factory = "p2p@builtin|float"];\n  float miss_default_test = 9[(p2p_validate.rules).float.miss_default = true];\n  float alias_test = 10 [(p2p_validate.rules).float.alias = "alias"];\n  float desc_test = 11 [(p2p_validate.rules).float.description = "test desc"];\n  float multiple_of_test = 12 [(p2p_validate.rules).float.multiple_of = 3.0];\n  float example_test = 13 [(p2p_validate.rules).float.example = 1.0];\n  float example_factory = 14 [(p2p_validate.rules).float.example_factory = "p2p@builtin|float"];\n  float field_test = 15[(p2p_validate.rules).float.field = "p2p@local|CustomerField"];\n  float type_test = 16[(p2p_validate.rules).float.type = "p2p@local|confloat"];\n  float title_test = 17 [(p2p_validate.rules).float.title = "title_test"];\n}\n```\n`protobuf-to-pydantic` can read the generated Message object at runtime and generate a `Pydantic Model` object with the corresponding information:\n\n```python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel, confloat\nfrom pydantic.fields import FieldInfo\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.p2p_validate import demo_pb2\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\nDemoModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest,\n    local_dict={"CustomerField": CustomerField, "confloat": confloat},\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in DemoModel.__fields__.items()\n    }\n)\n# output:\n# {\n#   \'const_test\': FieldInfo(default=1.0, const=True, extra={}),\n#   \'range_e_test\': FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   \'range_test\': FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   \'in_test\': FieldInfo(default=0.0, extra={\'in\': [1.0, 2.0, 3.0]}),\n#   \'not_in_test\': FieldInfo(default=0.0, extra={\'not_in\': [1.0, 2.0, 3.0]}),\n#   \'default_test\': FieldInfo(default=1.0, extra={}),\n#   \'default_factory_test\': FieldInfo(default=PydanticUndefined, default_factory=<class \'float\'>, extra={}),\n#   \'miss_default_test\': FieldInfo(extra={}),\n#   \'alias_test\': FieldInfo(default=0.0, alias=\'alias\', alias_priority=2, extra={}),\n#   \'desc_test\': FieldInfo(default=0.0, description=\'test desc\', extra={}),\n#   \'multiple_of_test\': FieldInfo(default=0.0, multiple_of=3, extra={}),\n#   \'example_test\': FieldInfo(default=0.0, extra={\'example\': 1.0}),\n#   \'example_factory\': FieldInfo(default=0.0, extra={\'example\': <class \'float\'>}),\n#   \'field_test\': CustomerField(default=0.0, extra={}),\n#   \'type_test\': FieldInfo(default=0.0, extra={}),\n#   \'title_test\': FieldInfo(default=0.0, title=\'title_test\', extra={})\n#   }\n```\n\n> Note:\n>  - 1.See the [2.5.template](#25Template) for the usage of `local_dict`\n>  - 2.If the reference to the Proto file fails, need to download [p2p_validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/protos/protobuf_to_pydantic/protos/p2p_validate.proto) in the project and use it in the Protobuf file。\n\n\n\n### 2.4.`P2P` and text annotation rule other parameter support\nThe `protobuf-to-pydantic` text annotation rules and the `P2P` rules support most of the parameters in `FieldInfo`, as described in the [Pydantic Field doc](https://docs.pydantic.dev/latest/usage/fields/)。\n\n> The new parameters added to `Pydantic V2` will be supported in version 2.1, for now `P2P` rule naming is still written on the basis of `Pydantic V1`, but automatic mapping to `Pydantic V2` naming is supported.\n\nOther partial changes in meaning and new parameters are described as follows:\n\n| Parameter        | Default value | Illustrate                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |\n|------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| required         | False         | By default, the default value of each field in the generated `Pydantic Model` object is the same as the zero value of its corresponding type. When `required` is `True`, no more default values are generated for the fields.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| enable           | True          | By default, `protobuf-to-pydantic` generates all fields for `Message`, if don\'t want the generated `Message` to have this field, can set `enable` to `False`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |\n| const            | None          | Used to specify a constant value for a field, though different `Pydantic` versions behave differently<br/>  For `Pydantic V1`, the value of `default` in `Field` is set to the value specified by `const`, and `const` in `Field` is set to True.Note: `Pydantic Model`\'s const only supports bool variables, when `const` is `True`, the accepted value can only be the value set by `default`, and the default value carried by the message generated by protobuf is the zero value of the corresponding type does not match with `Pydantic Model`, so ` protobuf-to-pydantic` makes some changes to the input of this value.<br/> For `Pydantic V2`, the value of `default` in `Field` remains the same, but the type annotation changes to `typing_extensions.Literal[xxx]` |\n| type             | None          | By default, the default type of a field is the same as Protobuf\'s, but use the [2.5.template](#25Template) function to modify the type of a field.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |\n| extra            | None          | The `extra` parameter accepted by `Pydantic` is of type `Python Dict`, which is not supported by Protobuf, and requires the use of either [2.5.Templates](#25Templates) or the corresponding Json structure `protobuf-to-pydantic` in the Protobuf file to parse it properly.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| field            | None          | By default, the `Field` of the parameter is `Pydantic FieldInfo`, although it can be customized using the [2.5.Templates](#25Templates) function                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| default_template | None          | Similar to `default`, default values can be customized in fields that are not of string type using the [2.5.Templates](#25Templates) feature.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n\nIn addition to the above parameters, also support for fast import of `Pydantic type` for string types. For example, if want to add a check for card numbers via the `pydantic.types.PaymentCardNumber` type, can specify the type of the `pydantic_type` parameter field to be `PaymentCardNumber`, which is similar to the use of template imports in the `type` rule, as follows:\n- Text annotation rules：\n  ```protobuf\n  syntax = "proto3";\n  package common_validate_test;\n\n  // common example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"pydantic_type": "PaymentCardNumber"}\n    string other_bank_number=2; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  ```\n- P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n    string other_bank_number=2[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n> See [Extra Types Overview](https://docs.pydantic.dev/latest/usage/types/extra_types/extra_types/) for supported `Pydantic Types\'.\n### 2.5.Template\nWhen working with definition fields, will find that some fields are filled with values that are methods or functions of one of the libraries in `Python` (e.g., the values of the `type` parameter and the `default_factory` parameter), which can\'t be accomplished with the Json syntax.\nAt this point, templates can be used to solve the corresponding problem, and currently `protobuf-to-pydantic` supports a variety of template functi\n\n> Note: The `p2p` string at the beginning of a template can be defined via the comment_prefix variable\n\n#### 2.5.1.`p2p@import`Template\nThe `p2p@import` template is used to represent variables in other modules that need to be introduced before they can be used, as follows.\n- Examples of text annotation rules：\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n\n  // comment example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  ```\n\n- Examples of P2P rules (1)：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "example_proto/common/p2p_validate.proto";\n\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n- Examples of P2P rules (2)：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_other_validate_test;\n  import "example_proto/common/p2p_validate.proto";\n  // p2p other example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n  }\n  ```\n\nThe example Protobuf file uses a syntax in the format `p2p@{methods of the template}|{modules to be imported:A}|{variables in modules:B}`, indicating that a `B` object needs to be imported by `from A import B` and used by the corresponding rule.\nWith the definition of the template, `protobuf-to-pydantic` converts the corresponding Message into a `Pydantic Model`, as follows:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n# p2p@import|pydantic.types|PaymentCardNumber\nfrom pydantic.types import PaymentCardNumber\n\nclass UserPayMessage(BaseModel):\n    bank_number: PaymentCardNumber = FieldInfo(default="", extra={})\n```\n\n#### 2.5.2.`p2p@import_instance` Template\nThe `p2p@import_instance` template introduces the class of a library and then instantiates it in combination with the specified parameters before it is used by the corresponding rule, which is used as follows:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\nimport "google/protobuf/any.proto";\nimport "example_proto/common/p2p_validate.proto";\n// p2p example\nmessage AnyTest {\n  google.protobuf.Any default_test = 23 [\n    (p2p_validate.rules).any.default = \'p2p@import_instance|google.protobuf.any_pb2|Any|{"type_url": "type.googleapis.com/google.protobuf.Duration"}\'\n  ];\n}\n```\nThe syntax used here is `p2p@{methods of the template}|{modules to be introduced}|{classes to be introduced}|{initialization parameters}`, and the definition of `protobuf-to-pydantic` through the template will turn the corresponding Message into the following `Pydantic Model` object:\n```python\nfrom google.protobuf.any_pb2 import Any as AnyMessage\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass AnyTest(BaseModel):\n    default_test: AnyMessage = FieldInfo(\n        default=AnyMessage(type_url="type.googleapis.com/google.protobuf.Duration")\n    )\n```\n\n#### 2.5.3.`p2p@local` Template\nThis template is used to introduce user-defined variables, using a syntax in the format `{method of the template}|{local variable to be used}`, as follows:\n\n- Example of text annotation:\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // comment example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1; // p2p: {"default_factory": "p2p@local|exp_time"}\n  }\n  ```\n- Examples of P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.default_factory= "p2p@local|exp_time"];\n  }\n  ```\nHowever, the `msg_to_pydantic_model` func needs to be called with the parameter `local_dict` to register the corresponding value, the pseudo-code is as follows:\n```Python\n# a.py\nimport time\n\nfrom example.proto_3_20_pydanticv1.example.example_proto.p2p_validate import demo_pb2\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\n\ndef exp_time() -> float:\n  return time.time()\n\nmsg_to_pydantic_model(\n    demo_pb2.NestedMessage,\n    local_dict={"exp_time": exp_time},  # <----  use local_dict\n)\n```\nIn this way, `protobuf-to-pydantic` generates a conforming `Pydantic Model` object:\n```python\n# b.py\nfrom datetime import datetime\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nfrom a import exp_time  # <-- exp_time in a.py\n\nclass UserPayMessage(BaseModel):\n    exp: datetime = FieldInfo(default_factory=exp_time, extra={})\n```\n\n\n#### 2.5.4.`p2p@builtin` Template\nThis template (which can be thought of as a simplified version of the `p2p@local` template) can be used directly when the variables to be used come from `Python` built-in functions,the syntax is used as follows:\n- Examples of text annotation rules:\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // comment example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1; // p2p: {"type": "p2p@builtin|float"}\n  }\n  ```\n- Examples of P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.type= "p2p@builtin|float"];\n  }\n  ```\nThen can directly generate a conforming `Pydantic Model` object by calling the `msg_to_pydantic_model` function, as follows:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass UserPayMessage(BaseModel):\n    exp: float = FieldInfo()\n```\n#### 2.5.5.Customized templates\nCurrently `protobuf-to-pydantic` only supports a few simple templates, if have more template needs, can extend the templates by inheriting the `DescTemplate` class.\n\nFor example, there is an odd feature that requires the default value of a field to be the timestamp of the time when the `Pydantic Model` object was generated, but the timestamps used are available in lengths of 10 and 13, so the following Protobuf file needs to be written to support defining the length of the timestamps:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\nimport "google/protobuf/timestamp.proto";\nimport "example_proto/common/p2p_validate.proto";\n\nmessage TimestampTest{\n  int32 timestamp_10 = 1[(p2p_validate.rules).int32.default_template = "p2p@timestamp|10"];\n  int32 timestamp_13 = 2[(p2p_validate.rules).int32.default_template = "p2p@timestamp|13"];\n}\n```\nAs you can see, the Protobuf file customizes the syntax of `p2p@timestamp|{x}`, where `x` has only two values, 10 and 13. The next step is to write code based on this template behavior, which looks like this.\n```python\nimport time\nfrom protobuf_to_pydantic.gen_model import DescTemplate\n\nclass CustomDescTemplate(DescTemplate):\n    def template_timestamp(self, length_str: str) -> int:\n        timestamp: float = time.time()\n        if length_str == "10":\n            return int(timestamp)\n        elif length_str == "13":\n            return int(timestamp * 100)\n        else:\n            raise KeyError(f"timestamp template not support value:{length_str}")\n\n\nfrom .demo_pb2 import TimestampTest # fake code\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\nmsg_to_pydantic_model(\n    TimestampTest,\n    desc_template=CustomDescTemplate   # <-- Use a custom template class\n)\n```\nThis code first creates a class `CustomDescTemplate` that inherits from `DescTemplate`.\n`DescTemplate` will forwards to the corresponding `template_{template name}` method based on the naming of the template, so this class needs to define the `template_timestamp` method to implement the `p2p@timestamp` template functionality.\nIn addition, the `length_str` variable received in this method is either 10 in `p2p@timestamp|10` or 13 in `p2p@timestamp|13`.\n\nThen load the `CustomDescTemplate` through the `msg_to_pydantic_model` function, then the following code will be generated (assuming that the code is generated at a timestamp of 1600000000):\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nclass TimestampTest(BaseModel):\n    timestamp_10: int = FieldInfo(default=1600000000)\n    timestamp_13: int = FieldInfo(default=1600000000000)\n```\n## 3.Code format\nThe code generated directly through `protobuf-to-pydantic` is not perfect, but it is possible to indirectly generate code that conforms to the `Python` specification through different formatting tools.\nCurrently, `protobuf-to-pydantic` supports formatting tools such as `autoflake`, `black` and `isort`. If the corresponding formatting tool is installed in the current `Python` environment, then `protobuf-to-pydantic` will call the tool to format the generated code before outputting it to a file.\n\nIn addition, the decision to enable or disable a formatting tool can be made through the `pyproject.toml` configuration file, the `pyproject.toml` example of which reads as follows:\n```toml\n# Controls which formatting tools protobuf-to-pydantic uses,\n# if false then no formatting tools are used (default is true)\n[tool.protobuf-to-pydantic.format]\nblack = true\nisort = true\nautoflake = true\n\n# black docc:https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-format\n[tool.black]\nline-length = 120\ntarget-version = [\'py37\']\n\n# isort doc:https://pycqa.github.io/isort/docs/configuration/config_files.html#pyprojecttoml-preferred-format\n[tool.isort]\nprofile = "black"\nmulti_line_output = 3\ninclude_trailing_comma = true\nforce_grid_wrap = 0\nuse_parentheses = true\nensure_newline_before_comments = true\nline_length = 120\n\n# autoflake doc:https://github.com/PyCQA/autoflake#configuration\n[tool.autoflake]\nin-place = true\nremove-all-unused-imports = true\nremove-unused-variables = true\n```\n\n## 4.example\n`protobuf-to-pydantic` provides some simple example code for reference only.\n\n### 4.1.Generate code directly\nProtobuf file: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code.py)\n### 4.2.Text annotation\nProtobuf File: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)\n\n`Pydantic Model` generated based on `pyi` file(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_text_comment_pyi.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_text_comment_pyi.py)\n\n`Pydantic Model` generated based on `pyi` file(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_text_comment_pyi.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_text_comment_pyi.py)\n\n`Pydantic Model` generated based on protobuf file(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_text_comment_protobuf_field.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_text_comment_protobuf_field.py)\n`Pydantic Model` generated based on protobuf file(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_text_comment_protobuf_field.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_text_comment_protobuf_field.py)\nvalidate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/validate/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_pgv.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_pgv.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_pgv.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_pgv.py)\n### 4.4.P2P rule\nProtobuf file: [p2p_validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/p2p_validate/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_p2p.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_p2p.py)\n### 4.5.Protoc Plugin-in\nProtobuf field: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)，[validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/validate/demo.proto)，[p2p_validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/p2p_validate/demo.proto)\n\n> Note: The Protoc plugin only supports P2P and PGV rules\n\n`Pydantic Model` generated via `demo/demo.proto`(Pydantic V1):[example_proto/demo/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/demo/demo_p2p.py)\n\n`Pydantic Model` generated via `demo/demo.proto`(Pydantic V2):[example_proto/demo/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/demo/demo_p2p.py)\n\n`Pydantic Model` generated via `validate/demo.proto`(Pydantic V1):[example_proto/validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/validate/demo_p2p.py)\n\n`Pydantic Model` generated via `validate/demo.proto`(Pydantic V1):[example_proto/validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/validate/demo_p2p.py)\n\n`Pydantic Model` generated via `p2p_validate/demo.proto`(Pydantic V1):[example_proto/p2p_validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/p2p_validate/demo_p2p.py)\n\n`Pydantic Model` generated via `p2p_validate/demo.proto`(Pydantic V1):[example_proto/p2p_validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/p2p_validate/demo_p2p.py)\n',
+    'long_description': '# protobuf_to_pydantic\nGenerate Pydantic Model or source code with parameter verification function based on Protobuf file (Proto3).\n\n\n[中文文档](https://github.com/so1n/protobuf_to_pydantic/blob/master/README_ZH.md)\n\n# Feature\n\nFeature：\n- [x] Generate source code through `Protobuf` plugin。\n- [x] Generate `Pydantic Model` or source code by parsing `Protobuf Message` in `Python` runtime.\n- [x] Compatible with `V1` and `V2` versions of `Pydantic`。\n- [x] Supports multiple verification rules and is compatible with `proto-gen-validate` (subsequent versions will support the rules of `proto-gen-validate` 1.0)。\n- [x] Support custom functionality through templates。\n- [ ] Supports `protovalidate` verification rules（`proto-gen-validate` version >= 1.0）\n\nThe following is a functional overview diagram of `protobuf-to-pydantic`.\nIn the picture `P2P` represents `protobuf-to-pydantic`, `Protoc` represents the command for `Protobuf` to generate code, and `plugin` represents ` Plugin for Protoc`:\n![protobuf-to-pydantic](https://github.com/so1n/protobuf_to_pydantic/blob/master/images/protobuf-to-pydantic_index.png?raw=true)\n\n# Installation\nBy default, `protobuf-to-pydantic` can be installed directly via the following command:\n```bash\npip install protobuf_to_pydantic\n```\nIf want to use the full functionality of `protobuf-to-pydantic`, can install `protobuf-to-pydantic` with the following command:.\n```bash\npip install protobuf_to_pydantic[all]\n```\n# Usage\n## 1.code generation\n`protobuf-to-pydantic` currently has two methods to generate `Pydantic Model` objects based on Protobuf files.：\n- 1: Use the `Protoc` plug-in to generate the corresponding `Python` code file through the Protobuf file。\n- 2: Generate the corresponding `Pydantic Model` object through the `Message` object in `Python` runtime。\n\n### 1.1.Directly generate `Pydantic Model` code files through plug-ins\n#### 1.1.0.Install dependencies\nThe `protobuf-to-pydantic` plug-in depends on `mypy-protobuf`, need to install `mypy-protobuf` through the following command first:\n```bash\npython -m pip install protobuf-to-pydantic[mypy-protobuf]\n```\nor\n```bash\npoetry add protobuf-to-pydantic -E mypy-protobuf\n```\n#### 1.1.1.Use plugins\nPlug-in is the `Pydantic Model` source code generation method recommended by `protobuf-to-pydantic`.\nIt supports the most complete functions and is also very simple to use.\n\nAssume that it is usually generated through the following command Code corresponding to Protobuf file:\n```bash\npython -m grpc_tools.protoc -I. example.proto\n# or\nprotoc -I. --python_out=. example.proto\n```\nAfter installing `protobuf-to-pydantic`,can use the `protobuf-to-pydantic` plugin with the `--protobuf-to-pydantic_out` option with the following command:\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=. example.proto\n# or\nprotoc -I. --protobuf-to-pydantic_out=. example.proto\n```\n\nIn this command, `--protobuf-to-pydantic_out=.` means using the `prorobuf-to-pydantic` plug-in,\nAnd it is declared that the output location of the `protobuf-to-pydantic` plug-in is `.`\n\n> `.` indicates the output path used by `grpc_tools.proto`.\n\nAfter running the command, the `protobuf-to-pydantic` plugin writes the generated source code to a file with the filename suffix `p2p.py`, e.g., `example.proto` generates a file with the name `example_p2p.py`.\n\n\n#### 1.1.2.Plug-in configuration\nThe `protobuf-to-pydantic` plugin supports loading configuration by reading a `Python` file。\n\n> In order to ensure that the variables of the configuration file can be introduced normally, the configuration file must be stored in the current path of the running command.。\n\nAn example configuration that can be read by `protobuf-to-pydantic` is as follows:\n```Python\nimport logging\nfrom typing import List, Type\n\nfrom google.protobuf.any_pb2 import Any  # type: ignore\nfrom pydantic import confloat, conint\nfrom pydantic.fields import FieldInfo\n\nfrom protobuf_to_pydantic.desc_template import DescTemplate\n\n# Configure the log output format and log level of the plugin, which is very useful when debugging\nlogging.basicConfig(format="[%(asctime)s %(levelname)s] %(message)s", datefmt="%y-%m-%d %H:%M:%S", level=logging.DEBUG)\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\ndef customer_any() -> Any:\n    return Any  # type: ignore\n\n\n# For the configuration of the local template, see the use of the local template for details\nlocal_dict = {\n    "CustomerField": CustomerField,\n    "confloat": confloat,\n    "conint": conint,\n    "customer_any": customer_any,\n}\n# Specifies the start of key comments\ncomment_prefix = "p2p"\n# Specify the class of the template, can extend the template by inheriting this class, see the chapter on custom templates for details\ndesc_template: Type[DescTemplate] = DescTemplate\n# Specify the protobuf files of which packages to ignore, and the messages of the ignored packages will not be parsed\nignore_pkg_list: List[str] = ["validate", "p2p_validate"]\n# Specifies the generated file name suffix (without .py)\nfile_name_suffix = "_p2p"\n```\nNext, in order to be able to read this file, need to change the `--protobuf-to-pydantic_out=. ` to ` --protobuf-to-pydantic_out=config_path=plugin_config.py:. `.\nwhere the left side of `:` indicates that the configuration file path to be read is `plugin_config.py`, and the right side of `:` declares that the output location of the `protobuf-to-pydantic` plugin is `. `\nThe final complete command is as follows：\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto\n# or\nprotoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto\n```\nThrough this command, can load the corresponding configuration and run the `protobuf-to-pydantic` plug-in。\n\nIn addition to the configuration options in the example configuration file,\nthe `protobuf-to-pydantic` plug-in also supports other configuration options.\nThe specific configuration instructions are as follows：\n\n| Configuration name            | Functional module                      | Type                                            | Hidden meaning                                                                                                                                      |\n|-------------------------------|----------------------------------------|-------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|\n| local_dict                    | Template                               | dict                                            | Holds variables for the `local` template                                                                                                            |\n| desc_template                 | Template                               | protobuf_to_pydantic.desc_template.DescTemplate | Implementation of the template class                                                                                                                |\n| comment_prefix                | Template                               | str                                             | Comment prefix.Only strings with a fixed prefix will be used by the template                                                                        |\n| customer_import_set           | Code generation                        | `Set[str]`                                      | A collection of custom import statements, such as `from typing import Set`or `import typing`, that will write data in order to the source code file |\n| customer_deque                | Code generation                        | `deque[str]`                                    | Custom source file content, used to add custom content                                                                                              |\n| module_path                   | str                                    | str                                             | Used to define the root path of the project or module, which helps `protobuf-to-pydantic`to better automatically generate module import statements   |\n| pyproject_file_path           | Code generation                        | str                                             | Define the pyproject file path, which defaults to the current project path                                                                          |\n| code_indent                   | Code generation                        | int                                             | Defines the number of indentation Spaces in the code; the default is 4                                                                              |\n| ignore_pkg_list               | Code generation(Limit plug-ins only)   | `list[str]`                                     | Definition ignores parsing of the specified package file                                                                                            |\n| base_model_class              | Model Code generation, Code generation | `Type[BaseModel]`                               | Define the parent class of the generated Model                                                                                                      |\n| file_name_suffix              | Code generation                        | str                                             | Define the generated file suffix, default `_p2p.py`                                                                                                 |\n| file_descriptor_proto_to_code | Code generation(Limit plug-ins only)   | `Type[FileDescriptorProtoToCode]`               | Define the `FileDescriptorProtoToCode` to use                                                                                                       |\n\n\n#### 1.1.3.buf-cli\nIf you are using `buf-cli` to manage Protobuf files,\nthen you can also use `protobuf-to-pydantic` in `buf-cli`, See [How to use `protobuf-to-pydantic` in `buf-cli`](https://github.com/so1n/protobuf_to_pydantic/blob/master/buf-plugin/README.md)\n\n### 1.2.Generate a `Pydantic Model` object in Python runtime\n`protobuf_to_pydantic` can generate the corresponding `PydanticModel` object based on the `Message` object at runtime。\n\nFor example, the `UserMessage` in the following Protobuf file named `demo.proto`:\n```protobuf\n// path: ./demo.proto\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\nmessage UserMessage {\n  string uid=1;\n  int32 age=2;\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  string user_name=6;\n}\n```\n`protoc` can be used to generate the Python code file corresponding to the `Protobuf` file (the file name is `demo_pb2.py`), and the code related to the `UserMessage` is stored in the code file.\n\nAt `Python` runtime, The func `msg_to_pydantic_model` can be called to read the `UserMessage` object from the `demo_pb2` module and generate the corresponding `Pydantic Model` object as follows:\n```Python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom . import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n\n# output\n# {\n#   `uid`: FieldInfo(default=``, extra={}),\n#   `age`: FieldInfo(default=0, extra={}),\n#   `height`: FieldInfo(default=0.0, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, extra={})\n#  }\n```\nThrough the output results, it can be found that the generated `pydantic.BaseModel` object also contains `uid`, `age`, `height`, `sex`, `is adult` and `user name` fields,\nand the `default` property matches the zero value of the Protobuf type。\n\nThe `msg_to_pydantic_model` func is customizable just like plugins, with the following extension parameters:\n\n| Fields                                    | Meaning                                                   |\n|-------------------------------------------|-----------------------------------------------------------|\n| default_field                             | Generate a `Field` for each field in the `Pydantic Model` |\n| comment_prefix                            | The prefix of a comment that can be parsed                |\n| parse_msg_desc_method                     | Parsing rules to use                                      |\n| local_dict                                | Variables used by the `local` template                    |\n| pydantic_base                             | Generates the parent class of the `Pydantic Model` object |\n| pydantic_module                           | Generate the `Module` of the `Pydantic Model` object      |\n| desc_template                             | Template class to use                                     |\n| message_type_dict_by_type_name            | Protobuf type mapping to `Python` type                    |\n| message_default_factory_dict_by_type_name | Protobuf type mapping to the Python type factory          |\n\n\nIn addition to generating the corresponding `Pydantic Model` object at runtime,\n`protobuf-to-pydantic` also supports converting `Pydantic Model` objects to Python code text at runtime (only compatible with `Pydantic Model` objects generated by `protobuf-to-pydantic`).\nThe `pydantic_model_to_py_code` func is used to generate the source code, and the `pydantic_model_to_py_file` func is used to generate the code file. The example code of the `pydantic_model_to_py_file` func is as follows:\n\n```Python\nfrom protobuf_to_pydantic import msg_to_pydantic_model, pydantic_model_to_py_file\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\npydantic_model_to_py_file(\n    "./demo_gen_code.py",\n    msg_to_pydantic_model(demo_pb2.NestedMessage),\n)\n```\nWhen the code runs, it converts`demo_pb2.NestedMessage`to a Pydantic Model object and passes it to the  `pydantic_model_to_py_file`. `pydantic_model_to_py_file` generates the source code and writes it to a `demo_gen_code.py` file.\n\n\n## 2.Parameter validation\nIn the previous section, the `Pydantic Model` object generated by the Protobuf file is very simple because the Protobuf file does not have enough parameters to verify the relevant information.\nIn order for each field in the generated `Pydantic Model` object to have parameter validation capabilities, the corresponding parameter checking rules for the field need to be refined in the Protobuf file.\n\nCurrently, `protobuf-to-pydantic` supports three validation rules：\n- 1.Text annotations\n- 2.PGV(protoc-geb-validate)\n- 3.P2P\n\nWith these rules, the `Pydantic Model` object generated by `protobuf-to-pydantic` will have parameter validation feature.\nAmong them, text annotations and P2P rules are consistent, they both support most of the parameters in `Pydantic Field`, some of the variations and new parameters are seen\n[2.4.`P2P` and text annotation rule other parameter support](#24p2p-and-text-comment-rule-other-parameter-support)\n\n> NOTE:\n>  - 1.Text annotation rules are not the focus of subsequent functional iterative development, and it is recommended to use P2P verification rules.\n>  - 2.`Protoc Plug-in` only support `PGV` and `P2P` rule.\n\n\n### 2.1.Text annotations\nIn the Protobuf file, can write annotations for each field that meet the requirements of `protobuf-to-pydantic`,\nso that `protobuf-to-pydantic` can obtain the validation information of the parameters when parsing the Protobuf file, such as the following example\n```protobuf\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\n// user info\nmessage UserMessage {\n  // p2p: {"required": true, "example": "10086"}\n  // p2p: {"title": "UID"}\n  string uid=1; // p2p: {"description": "user union id"}\n  // p2p: {"example": 18, "title": "use age", "ge": 0}\n  int32 age=2;\n  // p2p: {"ge": 0, "le": 2.5}\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  // p2p: {"description": "user name"}\n  // p2p: {"default": "", "min_length": 1, "max_length": "10", "example": "so1n"}\n  string user_name=6;\n}\n```\n\nIn this example, each annotation that can be used by `protobuf_to_pydantic` starts with `p2p:` (supports customization) and is followed by a complete Json string. If are familiar with the usage of `pydantic`, can find This Json string contains the verification information corresponding to `pydantic.Field`. For example, the `uid` field in `UserMessage` contains a total of 4 pieces of information as follows：\n\n| Column      | Meaning                                                                               |\n|-------------|---------------------------------------------------------------------------------------|\n| required    | Indicates that the generated field does not have a default value                      |\n| example     | An example value representing the generated field is 10086                            |\n| title       | Indicates that the schema name of the field is UID                                    |\n | description | The schema documentation for the representation field is described as `user_union_id` |\n\n> Note:\n>   - 1.Currently only single-line comments are supported and comments must be a complete Json data (no line breaks).\n>   - 2.multi line comments are not supported。\n\nWhen these annotations are written, `protobuf_to_pydantic` will bring the corresponding information for each field when converting the Message into the corresponding `Pydantic.BaseModel` object, as follows:\n\n```python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage, parse_msg_desc_method=demo_pb2)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `uid`: FieldInfo(default=PydanticUndefined, title=`UID`, description=`user union id`, extra={`example`: `10086`}),\n#   `age`: FieldInfo(default=0, title=`use age`, ge=0, extra={`example`: 18}),\n#   `height`: FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, description=`user name`, min_length=1, max_length=10, extra={`example`: `so1n`})\n# }\n```\nIt can be seen that the output fields carry the corresponding information, which is consistent with the comments of the Protobuf file.\n\nIn addition, this code differs from the previous section in that the `msg_to_pydantic_model` function has a keyword argument named `parse_msg_desc_method` and its value is the \'demo_pb2\' module.\nThis parameter enables `protobuf-to-pydantic` to obtain additional information about each field in the Message object through comments in the `.pyi` file of the `demo_pb2` module.\n\n> Note: This function needs to use the [mypy-protobuf](https://github.com/nipunn1313/mypy-protobuf) plugin when generating the corresponding `Python code through the Protobuf file, and the specified pyi file output path is the same as the generated `Python` code path to take effect.\n> And need to install `protobuf-to-pydantic` via the `python -m pip install protobuf-to-pydantic[mypy-protobuf]` command\n\nIn addition to getting comments from the `.pyi` file, `protobuf-to-pydantic` also supports getting comment information for each field through comments on the Protobuf file to which the Message object belongs.\nUsing this feature is as simple as setting the value of `parse_msg_desc_method` to the root directory path specified when the Message object was generated.\n\n> When using this method, make sure to install `protobuf-to-pydantic` via `python -m pip install protobuf-to-pydantic[lark]`, and also make sure that the Protobuf file exists in the project.\n\nFor example, the project structure of the `protobuf-to-pydantic` sample code is as follows:\n```bash\n./protobuf_to_pydantic/\n├── example/\n│ ├── python_example_proto_code/\n│ └── example_proto/\n├── protobuf_to_pydantic/\n└── /\n```\n\nThe Protobuf file is stored in the `example/example_proto` folder, and then run the following command in the `example` directory to generate the `Python` code file corresponding to Protobuf:\n```bash\ncd example\n\npython -m grpc_tools.protoc\n  --python_out=./python_example_proto_code \\\n  --grpc_python_out=./python_example_proto_code \\\n  -I. \\\n# or\nprotoc\n  --python_out=./python_example_proto_code \\\n  --grpc_python_out=./python_example_proto_code \\\n  -I. \\\n```\nThen the path that needs to be filled in for `parse_msg_desc_method` at this time is `./protobuf_to_pydantic/example`.\nThe following sample code:\n```python\n# pydantic Version v1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.UserMessage, parse_msg_desc_method="./protobuf_to_pydantic/example"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `uid`: FieldInfo(default=PydanticUndefined, title=`UID`, description=`user union id`, extra={`example`: `10086`}),\n#   `age`: FieldInfo(default=0, title=`use age`, ge=0, extra={`example`: 18}),\n#   `height`: FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, description=`user name`, min_length=1, max_length=10, extra={`example`: `so1n`})\n# }\n```\nAs you can see, the only difference in this code is the value of the `parse_msg_desc_method`, but through the output result, you can see that the field carries the same information as the result obtained through the module.\n\n### 2.2.PGV(protoc-gen-validate)\nAt present, the commonly used parameter verification project in the Protobuf ecosystem is [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate)，\nIt has become a common standard in Protobuf because it supports multiple languages and requires only one writing of `PGV` rules to make the generated `Message` object support the corresponding validation rules.\n\n> Currently `protobuf-to-pydantic` only supports rules that [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate) is less than version 1.0.0\n\n`protobuf-to-pydantic` supports parsing of `PGV` validation rules and generates `Pydantic Model` objects with validation logic functions.\nUsing `PGV` checksum rules in `protobuf-to-pydantic` is very simple, just write the corresponding `PGV` rules in the Protobuf file first,\nand then specify the value of `parse_msg_desc_method` to be `PGV` when calling `msg_to_pydantic_model` as the code below:\n```Python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.validate import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest, parse_msg_desc_method="PGV"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `const_test`: FieldInfo(default=1.0, const=True, extra={}),\n#   `range_e_test`: FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   `range_test`: FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   `in_test`: FieldInfo(default=0.0, extra={`in`: [1.0, 2.0, 3.0]}),\n#   `not_in_test`: FieldInfo(default=0.0, extra={`not_in`: [1.0, 2.0, 3.0]}),\n#   `ignore_test`: FieldInfo(default=0.0, extra={})\n# }\n```\n\n> Note:\n>  - 1.For the usage of `PGV`, see: [protoc-gen-validate doc](https://github.com/bufbuild/protoc-gen-validate/blob/v0.10.2-SNAPSHOT.17/README.md)\n>  - 2.Need to install `PGV` through `pip install protoc_gen_validate` or download [validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/common/validate.proto) to the protobuf directory in the project to write pgv rules in the Protobuf file.\n\n\n### 2.3.P2P\nThe `PGV` verification rules are written in the Option attribute of each field of `Message` and have a better code specification,\nso Protobuf that use `PGV` checksum rules will be more readable than Protobuf that use annotation .\n\nAt the same time, when writing `PGV` rules, can also experience the convenience of the IDE\'s auto-completion and the security of checksumming when generating the corresponding language objects from Protobuf files, but it only supports checksumming-related logic, which is not as rich as the file annotation mode.\n\n\nThe `P2P` verification rule that comes with `protobuf-to-pydantic` expands on the `PGV` verification rule by incorporating some of the functionality of the text annotation verification rule, which satisfies most of the customization of the properties of each `Field` in the `Pydantic Model`, such as the following Protobuf file.\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\n\nimport "example_proto/common/p2p_validate.proto";\n\n\nmessage FloatTest {\n  float const_test = 1 [(p2p_validate.rules).float.const = 1];\n  float range_e_test = 2 [(p2p_validate.rules).float = {ge: 1, le: 10}];\n  float range_test = 3[(p2p_validate.rules).float = {gt: 1, lt: 10}];\n  float in_test = 4[(p2p_validate.rules).float = {in: [1,2,3]}];\n  float not_in_test = 5[(p2p_validate.rules).float = {not_in: [1,2,3]}];\n  float default_test = 6[(p2p_validate.rules).float.default = 1.0];\n  float not_enable_test = 7[(p2p_validate.rules).float.enable = false];\n  float default_factory_test = 8[(p2p_validate.rules).float.default_factory = "p2p@builtin|float"];\n  float miss_default_test = 9[(p2p_validate.rules).float.miss_default = true];\n  float alias_test = 10 [(p2p_validate.rules).float.alias = "alias"];\n  float desc_test = 11 [(p2p_validate.rules).float.description = "test desc"];\n  float multiple_of_test = 12 [(p2p_validate.rules).float.multiple_of = 3.0];\n  float example_test = 13 [(p2p_validate.rules).float.example = 1.0];\n  float example_factory = 14 [(p2p_validate.rules).float.example_factory = "p2p@builtin|float"];\n  float field_test = 15[(p2p_validate.rules).float.field = "p2p@local|CustomerField"];\n  float type_test = 16[(p2p_validate.rules).float.type = "p2p@local|confloat"];\n  float title_test = 17 [(p2p_validate.rules).float.title = "title_test"];\n}\n```\n`protobuf-to-pydantic` can read the generated Message object at runtime and generate a `Pydantic Model` object with the corresponding information:\n\n```python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel, confloat\nfrom pydantic.fields import FieldInfo\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.p2p_validate import demo_pb2\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\nDemoModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest,\n    local_dict={"CustomerField": CustomerField, "confloat": confloat},\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in DemoModel.__fields__.items()\n    }\n)\n# output:\n# {\n#   \'const_test\': FieldInfo(default=1.0, const=True, extra={}),\n#   \'range_e_test\': FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   \'range_test\': FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   \'in_test\': FieldInfo(default=0.0, extra={\'in\': [1.0, 2.0, 3.0]}),\n#   \'not_in_test\': FieldInfo(default=0.0, extra={\'not_in\': [1.0, 2.0, 3.0]}),\n#   \'default_test\': FieldInfo(default=1.0, extra={}),\n#   \'default_factory_test\': FieldInfo(default=PydanticUndefined, default_factory=<class \'float\'>, extra={}),\n#   \'miss_default_test\': FieldInfo(extra={}),\n#   \'alias_test\': FieldInfo(default=0.0, alias=\'alias\', alias_priority=2, extra={}),\n#   \'desc_test\': FieldInfo(default=0.0, description=\'test desc\', extra={}),\n#   \'multiple_of_test\': FieldInfo(default=0.0, multiple_of=3, extra={}),\n#   \'example_test\': FieldInfo(default=0.0, extra={\'example\': 1.0}),\n#   \'example_factory\': FieldInfo(default=0.0, extra={\'example\': <class \'float\'>}),\n#   \'field_test\': CustomerField(default=0.0, extra={}),\n#   \'type_test\': FieldInfo(default=0.0, extra={}),\n#   \'title_test\': FieldInfo(default=0.0, title=\'title_test\', extra={})\n#   }\n```\n\n> Note:\n>  - 1.See the [2.5.template](#25Template) for the usage of `local_dict`\n>  - 2.If the reference to the Proto file fails, need to download [p2p_validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/protos/protobuf_to_pydantic/protos/p2p_validate.proto) in the project and use it in the Protobuf file。\n\n\n\n### 2.4.`P2P` and text annotation rule other parameter support\nThe `protobuf-to-pydantic` text annotation rules and the `P2P` rules support most of the parameters in `FieldInfo`, as described in the [Pydantic Field doc](https://docs.pydantic.dev/latest/usage/fields/)。\n\n> The new parameters added to `Pydantic V2` will be supported in version 2.1, for now `P2P` rule naming is still written on the basis of `Pydantic V1`, but automatic mapping to `Pydantic V2` naming is supported.\n\nOther partial changes in meaning and new parameters are described as follows:\n\n| Parameter        | Default value | Illustrate                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |\n|------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| required         | False         | By default, the default value of each field in the generated `Pydantic Model` object is the same as the zero value of its corresponding type. When `required` is `True`, no more default values are generated for the fields.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| enable           | True          | By default, `protobuf-to-pydantic` generates all fields for `Message`, if don\'t want the generated `Message` to have this field, can set `enable` to `False`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |\n| const            | None          | Used to specify a constant value for a field, though different `Pydantic` versions behave differently<br/>  For `Pydantic V1`, the value of `default` in `Field` is set to the value specified by `const`, and `const` in `Field` is set to True.Note: `Pydantic Model`\'s const only supports bool variables, when `const` is `True`, the accepted value can only be the value set by `default`, and the default value carried by the message generated by protobuf is the zero value of the corresponding type does not match with `Pydantic Model`, so ` protobuf-to-pydantic` makes some changes to the input of this value.<br/> For `Pydantic V2`, the value of `default` in `Field` remains the same, but the type annotation changes to `typing_extensions.Literal[xxx]` |\n| type             | None          | By default, the default type of a field is the same as Protobuf\'s, but use the [2.5.template](#25Template) function to modify the type of a field.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |\n| extra            | None          | The `extra` parameter accepted by `Pydantic` is of type `Python Dict`, which is not supported by Protobuf, and requires the use of either [2.5.Templates](#25Templates) or the corresponding Json structure `protobuf-to-pydantic` in the Protobuf file to parse it properly.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| field            | None          | By default, the `Field` of the parameter is `Pydantic FieldInfo`, although it can be customized using the [2.5.Templates](#25Templates) function                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| default_template | None          | Similar to `default`, default values can be customized in fields that are not of string type using the [2.5.Templates](#25Templates) feature.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n\nIn addition to the above parameters, also support for fast import of `Pydantic type` for string types. For example, if want to add a check for card numbers via the `pydantic.types.PaymentCardNumber` type, can specify the type of the `pydantic_type` parameter field to be `PaymentCardNumber`, which is similar to the use of template imports in the `type` rule, as follows:\n- Text annotation rules：\n  ```protobuf\n  syntax = "proto3";\n  package common_validate_test;\n\n  // common example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"pydantic_type": "PaymentCardNumber"}\n    string other_bank_number=2; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  ```\n- P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n    string other_bank_number=2[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n> See [Extra Types Overview](https://docs.pydantic.dev/latest/usage/types/extra_types/extra_types/) for supported `Pydantic Types\'.\n### 2.5.Template\nWhen working with definition fields, will find that some fields are filled with values that are methods or functions of one of the libraries in `Python` (e.g., the values of the `type` parameter and the `default_factory` parameter), which can\'t be accomplished with the Json syntax.\nAt this point, templates can be used to solve the corresponding problem, and currently `protobuf-to-pydantic` supports a variety of template functi\n\n> Note: The `p2p` string at the beginning of a template can be defined via the comment_prefix variable\n\n#### 2.5.1.`p2p@import`Template\nThe `p2p@import` template is used to represent variables in other modules that need to be introduced before they can be used, as follows.\n- Examples of text annotation rules：\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n\n  // comment example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  ```\n\n- Examples of P2P rules (1)：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "example_proto/common/p2p_validate.proto";\n\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n- Examples of P2P rules (2)：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_other_validate_test;\n  import "example_proto/common/p2p_validate.proto";\n  // p2p other example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n  }\n  ```\n\nThe example Protobuf file uses a syntax in the format `p2p@{methods of the template}|{modules to be imported:A}|{variables in modules:B}`, indicating that a `B` object needs to be imported by `from A import B` and used by the corresponding rule.\nWith the definition of the template, `protobuf-to-pydantic` converts the corresponding Message into a `Pydantic Model`, as follows:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n# p2p@import|pydantic.types|PaymentCardNumber\nfrom pydantic.types import PaymentCardNumber\n\nclass UserPayMessage(BaseModel):\n    bank_number: PaymentCardNumber = FieldInfo(default="", extra={})\n```\n\n#### 2.5.2.`p2p@import_instance` Template\nThe `p2p@import_instance` template introduces the class of a library and then instantiates it in combination with the specified parameters before it is used by the corresponding rule, which is used as follows:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\nimport "google/protobuf/any.proto";\nimport "example_proto/common/p2p_validate.proto";\n// p2p example\nmessage AnyTest {\n  google.protobuf.Any default_test = 23 [\n    (p2p_validate.rules).any.default = \'p2p@import_instance|google.protobuf.any_pb2|Any|{"type_url": "type.googleapis.com/google.protobuf.Duration"}\'\n  ];\n}\n```\nThe syntax used here is `p2p@{methods of the template}|{modules to be introduced}|{classes to be introduced}|{initialization parameters}`, and the definition of `protobuf-to-pydantic` through the template will turn the corresponding Message into the following `Pydantic Model` object:\n```python\nfrom google.protobuf.any_pb2 import Any as AnyMessage\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass AnyTest(BaseModel):\n    default_test: AnyMessage = FieldInfo(\n        default=AnyMessage(type_url="type.googleapis.com/google.protobuf.Duration")\n    )\n```\n\n#### 2.5.3.`p2p@local` Template\nThis template is used to introduce user-defined variables, using a syntax in the format `{method of the template}|{local variable to be used}`, as follows:\n\n- Example of text annotation:\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // comment example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1; // p2p: {"default_factory": "p2p@local|exp_time"}\n  }\n  ```\n- Examples of P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.default_factory= "p2p@local|exp_time"];\n  }\n  ```\nHowever, the `msg_to_pydantic_model` func needs to be called with the parameter `local_dict` to register the corresponding value, the pseudo-code is as follows:\n```Python\n# a.py\nimport time\n\nfrom example.proto_3_20_pydanticv1.example.example_proto.p2p_validate import demo_pb2\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\n\ndef exp_time() -> float:\n  return time.time()\n\nmsg_to_pydantic_model(\n    demo_pb2.NestedMessage,\n    local_dict={"exp_time": exp_time},  # <----  use local_dict\n)\n```\nIn this way, `protobuf-to-pydantic` generates a conforming `Pydantic Model` object:\n```python\n# b.py\nfrom datetime import datetime\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nfrom a import exp_time  # <-- exp_time in a.py\n\nclass UserPayMessage(BaseModel):\n    exp: datetime = FieldInfo(default_factory=exp_time, extra={})\n```\n\n\n#### 2.5.4.`p2p@builtin` Template\nThis template (which can be thought of as a simplified version of the `p2p@local` template) can be used directly when the variables to be used come from `Python` built-in functions,the syntax is used as follows:\n- Examples of text annotation rules:\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // comment example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1; // p2p: {"type": "p2p@builtin|float"}\n  }\n  ```\n- Examples of P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.type= "p2p@builtin|float"];\n  }\n  ```\nThen can directly generate a conforming `Pydantic Model` object by calling the `msg_to_pydantic_model` function, as follows:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass UserPayMessage(BaseModel):\n    exp: float = FieldInfo()\n```\n#### 2.5.5.Customized templates\nCurrently `protobuf-to-pydantic` only supports a few simple templates, if have more template needs, can extend the templates by inheriting the `DescTemplate` class.\n\nFor example, there is an odd feature that requires the default value of a field to be the timestamp of the time when the `Pydantic Model` object was generated, but the timestamps used are available in lengths of 10 and 13, so the following Protobuf file needs to be written to support defining the length of the timestamps:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\nimport "google/protobuf/timestamp.proto";\nimport "example_proto/common/p2p_validate.proto";\n\nmessage TimestampTest{\n  int32 timestamp_10 = 1[(p2p_validate.rules).int32.default_template = "p2p@timestamp|10"];\n  int32 timestamp_13 = 2[(p2p_validate.rules).int32.default_template = "p2p@timestamp|13"];\n}\n```\nAs you can see, the Protobuf file customizes the syntax of `p2p@timestamp|{x}`, where `x` has only two values, 10 and 13. The next step is to write code based on this template behavior, which looks like this.\n```python\nimport time\nfrom protobuf_to_pydantic.gen_model import DescTemplate\n\nclass CustomDescTemplate(DescTemplate):\n    def template_timestamp(self, length_str: str) -> int:\n        timestamp: float = time.time()\n        if length_str == "10":\n            return int(timestamp)\n        elif length_str == "13":\n            return int(timestamp * 100)\n        else:\n            raise KeyError(f"timestamp template not support value:{length_str}")\n\n\nfrom .demo_pb2 import TimestampTest # fake code\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\nmsg_to_pydantic_model(\n    TimestampTest,\n    desc_template=CustomDescTemplate   # <-- Use a custom template class\n)\n```\nThis code first creates a class `CustomDescTemplate` that inherits from `DescTemplate`.\n`DescTemplate` will forwards to the corresponding `template_{template name}` method based on the naming of the template, so this class needs to define the `template_timestamp` method to implement the `p2p@timestamp` template functionality.\nIn addition, the `length_str` variable received in this method is either 10 in `p2p@timestamp|10` or 13 in `p2p@timestamp|13`.\n\nThen load the `CustomDescTemplate` through the `msg_to_pydantic_model` function, then the following code will be generated (assuming that the code is generated at a timestamp of 1600000000):\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nclass TimestampTest(BaseModel):\n    timestamp_10: int = FieldInfo(default=1600000000)\n    timestamp_13: int = FieldInfo(default=1600000000000)\n```\n## 3.Code format\nThe code generated directly through `protobuf-to-pydantic` is not perfect, but it is possible to indirectly generate code that conforms to the `Python` specification through different formatting tools.\nCurrently, `protobuf-to-pydantic` supports formatting tools such as `autoflake`, `black` and `isort`. If the corresponding formatting tool is installed in the current `Python` environment, then `protobuf-to-pydantic` will call the tool to format the generated code before outputting it to a file.\n\nIn addition, the decision to enable or disable a formatting tool can be made through the `pyproject.toml` configuration file, the `pyproject.toml` example of which reads as follows:\n```toml\n# Controls which formatting tools protobuf-to-pydantic uses,\n# if false then no formatting tools are used (default is true)\n[tool.protobuf-to-pydantic.format]\nblack = true\nisort = true\nautoflake = true\n\n# black docc:https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-format\n[tool.black]\nline-length = 120\ntarget-version = [\'py37\']\n\n# isort doc:https://pycqa.github.io/isort/docs/configuration/config_files.html#pyprojecttoml-preferred-format\n[tool.isort]\nprofile = "black"\nmulti_line_output = 3\ninclude_trailing_comma = true\nforce_grid_wrap = 0\nuse_parentheses = true\nensure_newline_before_comments = true\nline_length = 120\n\n# autoflake doc:https://github.com/PyCQA/autoflake#configuration\n[tool.autoflake]\nin-place = true\nremove-all-unused-imports = true\nremove-unused-variables = true\n```\n\n## 4.example\n`protobuf-to-pydantic` provides some simple example code for reference only.\n\n### 4.1.Generate code directly\nProtobuf file: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code.py)\n### 4.2.Text annotation\nProtobuf File: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)\n\n`Pydantic Model` generated based on `pyi` file(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_text_comment_pyi.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_text_comment_pyi.py)\n\n`Pydantic Model` generated based on `pyi` file(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_text_comment_pyi.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_text_comment_pyi.py)\n\n`Pydantic Model` generated based on protobuf file(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_text_comment_protobuf_field.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_text_comment_protobuf_field.py)\n`Pydantic Model` generated based on protobuf file(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_text_comment_protobuf_field.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_text_comment_protobuf_field.py)\nvalidate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/validate/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_pgv.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_pgv.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_pgv.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_pgv.py)\n### 4.4.P2P rule\nProtobuf file: [p2p_validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/p2p_validate/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_p2p.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_p2p.py)\n### 4.5.Protoc Plugin-in\nProtobuf field: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)，[validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/validate/demo.proto)，[p2p_validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/p2p_validate/demo.proto)\n\n> Note: The Protoc plugin only supports P2P and PGV rules\n\n`Pydantic Model` generated via `demo/demo.proto`(Pydantic V1):[example_proto/demo/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/demo/demo_p2p.py)\n\n`Pydantic Model` generated via `demo/demo.proto`(Pydantic V2):[example_proto/demo/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/demo/demo_p2p.py)\n\n`Pydantic Model` generated via `validate/demo.proto`(Pydantic V1):[example_proto/validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/validate/demo_p2p.py)\n\n`Pydantic Model` generated via `validate/demo.proto`(Pydantic V1):[example_proto/validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/validate/demo_p2p.py)\n\n`Pydantic Model` generated via `p2p_validate/demo.proto`(Pydantic V1):[example_proto/p2p_validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/p2p_validate/demo_p2p.py)\n\n`Pydantic Model` generated via `p2p_validate/demo.proto`(Pydantic V1):[example_proto/p2p_validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/p2p_validate/demo_p2p.py)\n',
     'author': 'So1n',
     'author_email': 'so1n897046026@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/so1n/protobuf_to_pydantic',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `protobuf_to_pydantic-0.2.6/PKG-INFO` & `protobuf_to_pydantic-0.2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf-to-pydantic
-Version: 0.2.6
+Version: 0.2.6.1
 Summary: Generate the `pydantic.BaseModel` class (and the corresponding source code) with parameter verification function through the Protobuf file
 Home-page: https://github.com/so1n/protobuf_to_pydantic
 License: Apache Software License
 Author: So1n
 Author-email: so1n897046026@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: lark
 Provides-Extra: mypy-protobuf
 Provides-Extra: toml
-Requires-Dist: grpcio-tools (>=1.40.0,<2.0.0)
 Requires-Dist: lark (>=1.1.2,<2.0.0) ; extra == "lark" or extra == "all"
 Requires-Dist: mypy-protobuf (>=3.2.0,<4.0.0) ; extra == "mypy-protobuf" or extra == "all"
+Requires-Dist: protobuf (>=3.20.3)
 Requires-Dist: pydantic (>=1.9.2,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "toml" or extra == "all"
 Project-URL: Repository, https://github.com/so1n/protobuf_to_pydantic
 Description-Content-Type: text/markdown
 
 # protobuf_to_pydantic
 Generate Pydantic Model or source code with parameter verification function based on Protobuf file (Proto3).
@@ -74,18 +74,22 @@
 #### 1.1.1.Use plugins
 Plug-in is the `Pydantic Model` source code generation method recommended by `protobuf-to-pydantic`.
 It supports the most complete functions and is also very simple to use.
 
 Assume that it is usually generated through the following command Code corresponding to Protobuf file:
 ```bash
 python -m grpc_tools.protoc -I. example.proto
+# or
+protoc -I. --python_out=. example.proto
 ```
 After installing `protobuf-to-pydantic`,can use the `protobuf-to-pydantic` plugin with the `--protobuf-to-pydantic_out` option with the following command:
 ```bash
 python -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=. example.proto
+# or
+protoc -I. --protobuf-to-pydantic_out=. example.proto
 ```
 
 In this command, `--protobuf-to-pydantic_out=.` means using the `prorobuf-to-pydantic` plug-in,
 And it is declared that the output location of the `protobuf-to-pydantic` plug-in is `.`
 
 > `.` indicates the output path used by `grpc_tools.proto`.
 
@@ -137,14 +141,16 @@
 file_name_suffix = "_p2p"
 ```
 Next, in order to be able to read this file, need to change the `--protobuf-to-pydantic_out=. ` to ` --protobuf-to-pydantic_out=config_path=plugin_config.py:. `.
 where the left side of `:` indicates that the configuration file path to be read is `plugin_config.py`, and the right side of `:` declares that the output location of the `protobuf-to-pydantic` plugin is `. `
 The final complete command is as follows：
 ```bash
 python -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto
+# or
+protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto
 ```
 Through this command, can load the corresponding configuration and run the `protobuf-to-pydantic` plug-in。
 
 In addition to the configuration options in the example configuration file,
 the `protobuf-to-pydantic` plug-in also supports other configuration options.
 The specific configuration instructions are as follows：
 
@@ -187,15 +193,15 @@
   int32 age=2;
   float height=3;
   SexType sex=4;
   bool is_adult=5;
   string user_name=6;
 }
 ```
-`grpc_tools.protoc` can be used to generate the Python code file corresponding to the `Protobuf` file (the file name is `demo_pb2.py`), and the code related to the `UserMessage` is stored in the code file.
+`protoc` can be used to generate the Python code file corresponding to the `Protobuf` file (the file name is `demo_pb2.py`), and the code related to the `UserMessage` is stored in the code file.
 
 At `Python` runtime, The func `msg_to_pydantic_model` can be called to read the `UserMessage` object from the `demo_pb2` module and generate the corresponding `Pydantic Model` object as follows:
 ```Python
 from typing import Type
 from protobuf_to_pydantic import msg_to_pydantic_model
 from pydantic import BaseModel
 
@@ -371,14 +377,19 @@
 ```bash
 cd example
 
 python -m grpc_tools.protoc
   --python_out=./python_example_proto_code \
   --grpc_python_out=./python_example_proto_code \
   -I. \
+# or
+protoc
+  --python_out=./python_example_proto_code \
+  --grpc_python_out=./python_example_proto_code \
+  -I. \
 ```
 Then the path that needs to be filled in for `parse_msg_desc_method` at this time is `./protobuf_to_pydantic/example`.
 The following sample code:
 ```python
 # pydantic Version v1
 from typing import Type
 from protobuf_to_pydantic import msg_to_pydantic_model
```

