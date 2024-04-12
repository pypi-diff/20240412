# Comparing `tmp/kybra-0.5.3rc0.tar.gz` & `tmp/kybra-0.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kybra-0.5.3rc0.tar", last modified: Tue Mar 26 18:39:08 2024, max compression
+gzip compressed data, was "kybra-0.6.0rc0.tar", last modified: Fri Apr 12 13:26:12 2024, max compression
```

## Comparing `kybra-0.5.3rc0.tar` & `kybra-0.6.0rc0.tar`

### file list

```diff
@@ -1,325 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.575518 kybra-0.5.3rc0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/NOTICE_PYTHON
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.523518 kybra-0.5.3rc0/kybra/
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-03-26 18:38:56.000000 kybra-0.5.3rc0/kybra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/build_wasm_binary_or_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.523518 kybra-0.5.3rc0/kybra/canisters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.523518 kybra-0.5.3rc0/kybra/canisters/ledger/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/ledger/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9521 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/ledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/canisters/management/
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/management/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/management/bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/management/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/canisters/management/tecdsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    80489 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/cargotoml.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/compiler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra/compiler/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/compiler/custom_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/custom_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/compiler/custom_modules/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/custom_modules/principal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2609 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/install_rust_dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/compiler/kybra_deployer/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_deployer/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/compiler/kybra_deployer/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_deployer/src/errors.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_deployer/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.527518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.531518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.531518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/
--rw-r--r--   0 runner    (1001) docker     (127)    22283 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/candid.rs
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/does_interpreter_exist.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.531518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/array.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.535518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.535518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.535518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/opt.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.535518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/record/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.535518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.535518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.535518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/variant/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.539518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.543518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.543518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.543518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.543518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/constants.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.543518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/
--rw-r--r--   0 runner    (1001) docker     (127)    33809 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/analyze.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/display_string.rs
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/test_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.547518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/collect_results.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/unreachable.rs
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/exit_codes.rs
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/get_child_class_of.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/get_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.547518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.547518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.547518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/header/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/header/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/header/ref_cells.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/header/traits.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/header/use_statements.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.547518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.555518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.559518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/keywords.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.559518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.559518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/params.rs
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/returns.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.563518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/errors.rs
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.563518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/source_map/
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/source_map/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.563518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/source_map/token_length/
--rw-r--r--   0 runner    (1001) docker     (127)    28330 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.563518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.563518 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.567519 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/tuple.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.567519 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.567519 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.567519 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.567519 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/clear_chunks.rs
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/dfx.rs
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/generate_candid.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/install_app_canister.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/permissions.rs
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/upload_app_canister.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/upload_chunk.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/shared_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/shared_utils/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/shared_utils/src/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/shared_utils/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra/compiler/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/compiler/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/module_bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/run_kybra_generate_or_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/timed.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/kybra/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:39:08.571519 kybra-0.5.3rc0/kybra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16668 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 18:39:08.000000 kybra-0.5.3rc0/kybra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 18:39:08.575518 kybra-0.5.3rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-26 18:37:25.000000 kybra-0.5.3rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.921258 kybra-0.6.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/NOTICE_PYTHON
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.869258 kybra-0.6.0rc0/kybra/
+-rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-04-12 13:25:59.000000 kybra-0.6.0rc0/kybra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/build_wasm_binary_or_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.873258 kybra-0.6.0rc0/kybra/canisters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.873258 kybra-0.6.0rc0/kybra/canisters/ledger/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/ledger/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9521 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/ledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.873258 kybra-0.6.0rc0/kybra/canisters/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/management/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/management/bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/management/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/canisters/management/tecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85709 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/cargotoml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.873258 kybra-0.6.0rc0/kybra/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/LICENSE-RustPython
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.873258 kybra-0.6.0rc0/kybra/compiler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra/compiler/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.873258 kybra-0.6.0rc0/kybra/compiler/custom_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/custom_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.877258 kybra-0.6.0rc0/kybra/compiler/custom_modules/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/custom_modules/principal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3370 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/install_rust_dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.877258 kybra-0.6.0rc0/kybra/compiler/kybra_compile_python_stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_compile_python_stdlib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.877258 kybra-0.6.0rc0/kybra/compiler/kybra_compile_python_stdlib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_compile_python_stdlib/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.877258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.877258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.877258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/
+-rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/guard_against_non_controllers.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.881258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/array.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.881258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.881258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/opt.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.885258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.889258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.889258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.889258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.889258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.889258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.889258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.893258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/constants.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.893258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)    33809 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/analyze.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/display_string.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/test_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.893258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/collect_results.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/unreachable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/exit_codes.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/get_child_class_of.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/get_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.893258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.893258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.897258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/header/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/header/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/header/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/header/use_statements.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.897258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.905258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.905258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/keywords.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.909258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.909258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/returns.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.909258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.909258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/source_map/
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/source_map/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.909258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/
+-rw-r--r--   0 runner    (1001) docker     (127)    28330 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.909258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.913258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.913258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/tuple.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.913258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)   438859 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/python_3_10_13_licenses.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra/compiler/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/compiler/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/module_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/run_kybra_generate_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/kybra/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:26:12.917258 kybra-0.6.0rc0/kybra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 13:26:12.000000 kybra-0.6.0rc0/kybra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:26:12.921258 kybra-0.6.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 13:24:20.000000 kybra-0.6.0rc0/setup.py
```

### Comparing `kybra-0.5.3rc0/LICENSE` & `kybra-0.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/NOTICE` & `kybra-0.6.0rc0/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/NOTICE_PYTHON` & `kybra-0.6.0rc0/NOTICE_PYTHON`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/PKG-INFO` & `kybra-0.6.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.5.3rc0
+Version: 0.6.0rc0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: NOTICE_PYTHON
 Requires-Dist: modulegraph==0.19.3
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kybra Version: 0.5.3rc0 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc0 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE License-File:
 NOTICE_PYTHON Requires-Dist: modulegraph==0.19.3
                                  _[_k_y_b_r_a_ _l_o_g_o_]
                         _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Kybra may have unknown security
 vulnerabilities due to the following: - Kybra does not yet have many live,
```

### Comparing `kybra-0.5.3rc0/README.md` & `kybra-0.6.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/__init__.py` & `kybra-0.6.0rc0/kybra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeAlias,
     Union,
 )
 
 # TODO I think we can simplify this just like we're doing with canisters
 from .compiler.custom_modules.principal import Principal as PrincipalRenamed
 
-__version__ = "0.5.3rc0"
+__version__ = "0.6.0rc0"
 __rust_version__ = "1.77.0"
 
 Principal = PrincipalRenamed
 
 int64 = int
 int32 = int
 int16 = int
@@ -353,16 +353,17 @@
         )
 
     @staticmethod
     def performance_counter(counter_type: nat32) -> nat64:
         return _kybra_ic.performance_counter(counter_type)  # type: ignore
 
     @staticmethod
-    def print(x: Any):
-        _kybra_ic.print(str(x))  # type: ignore
+    def print(*args: Any):
+        string_list = [str(arg) for arg in args]
+        _kybra_ic.print(" ".join(string_list))  # type: ignore
 
     @staticmethod
     def reject(x: str):
         _kybra_ic.reject(x)  # type: ignore
 
     @staticmethod
     def reject_code() -> RejectionCode:
```

### Comparing `kybra-0.5.3rc0/kybra/__main__.py` & `kybra-0.6.0rc0/kybra/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 import time
 import site
 from typing import Any, Callable
 
 import kybra
 from kybra.build_wasm_binary_or_exit import build_wasm_binary_or_exit
 from kybra.cargotoml import generate_cargo_toml, generate_cargo_lock
-from kybra.colors import red, yellow, green, dim
+from kybra.colors import red, green, dim
 from kybra.run_kybra_generate_or_exit import run_kybra_generate_or_exit
 from kybra.timed import timed, timed_inline
 from kybra.types import Args, Paths
 
 
 @timed
 def main():
     args = parse_args_or_exit(sys.argv)
     paths = create_paths(args)
-    is_verbose = args["flags"]["verbose"]
-    is_initial_compile = detect_initial_compile(paths["global_kybra_target_dir"])
+    is_verbose = args["flags"]["verbose"] or os.environ.get("KYBRA_VERBOSE") == "true"
 
     subprocess.run(
         [
             f"{paths['compiler']}/install_rust_dependencies.sh",
             kybra.__version__,
             kybra.__rust_version__,
         ]
@@ -36,96 +35,47 @@
     # This is the name of the canister passed into python -m kybra from the dfx.json build command
     canister_name = args["canister_name"]
 
     verbose_mode_qualifier = " in verbose mode" if is_verbose else ""
 
     print(f"\nBuilding canister {green(canister_name)}{verbose_mode_qualifier}\n")
 
-    if is_initial_compile:
-        print(
-            yellow(
-                "Initial build takes a few minutes. Don't panic. Subsequent builds will be faster.\n"
-            )
-        )
-
     # Copy all of the Rust project structure from the pip package to an area designed for Rust compiling
     if os.path.exists(paths["canister"]):
         shutil.rmtree(paths["canister"])
     shutil.copytree(paths["compiler"], paths["canister"], dirs_exist_ok=True)
     create_file(f"{paths['canister']}/Cargo.toml", generate_cargo_toml(canister_name))
     create_file(f"{paths['canister']}/Cargo.lock", generate_cargo_lock())
-    create_file(
-        f"{paths['canister']}/post_install.sh",
-        generate_post_install_script(
-            canister_name, kybra.__rust_version__, is_verbose, paths["did"]
-        ),
-    )
-    os.system(f"chmod +x {paths['canister']}/post_install.sh")
 
     # Add CARGO_TARGET_DIR to env for all cargo commands
     cargo_env = {
         **os.environ.copy(),
         "CARGO_TARGET_DIR": paths["global_kybra_target_dir"],
         "CARGO_HOME": paths["global_kybra_rust_dir"],
         "RUSTUP_HOME": paths["global_kybra_rust_dir"],
     }
 
     if not os.path.exists(paths["global_kybra_bin_dir"]):
         os.makedirs(paths["global_kybra_bin_dir"])
 
     compile_python_or_exit(
-        paths, cargo_env, verbose=is_verbose, label="[1/3] 🔨 Compiling Python..."
+        paths, cargo_env, verbose=is_verbose, label="[1/2] 🔨 Compiling Python..."
     )
 
     build_wasm_binary_or_exit(
         paths,
         canister_name,
         cargo_env,
         verbose=is_verbose,
-        label=f"[2/3] 🚧 Building Wasm binary...{show_empathy(is_initial_compile)}",
-    )
-
-    optimize_wasm_binary_or_exit(
-        paths,
-        canister_name,
-        cargo_env,
-        verbose=is_verbose,
-        label=f"[3/3] 🚀 Optimizing Wasm binary...{show_empathy(is_initial_compile)}",
+        label=f"[2/2] 🚧 Building Wasm binary...",
     )
 
     print(f"\n🎉 Built canister {green(canister_name)} at {dim(paths['wasm'])}")
 
 
-def generate_post_install_script(
-    canister_name: str, rust_version: str, is_verbose: bool, candid_path: str
-) -> str:
-    main_command = f"KYBRA_VERSION={kybra.__version__} $global_kybra_cargo_bin run --manifest-path=.kybra/{canister_name}/kybra_post_install/Cargo.toml {canister_name} {candid_path}"
-    main_command_not_verbose = f'exec 3>&1; output=$({main_command} 2>&1 1>&3 3>&-); exit_code=$?; exec 3>&-; if [ $exit_code -ne 0 ]; then echo "$output"; exit $exit_code; fi'
-
-    return f"""#!/bin/bash
-
-rust_version="{rust_version}"
-
-global_kybra_config_dir=~/.config/kybra
-global_kybra_rust_dir="$global_kybra_config_dir"/rust/"$rust_version"
-global_kybra_rust_bin_dir="$global_kybra_rust_dir"/bin
-global_kybra_logs_dir="$global_kybra_rust_dir"/logs
-global_kybra_cargo_bin="$global_kybra_rust_bin_dir"/cargo
-global_kybra_rustup_bin="$global_kybra_rust_bin_dir"/rustup
-
-export CARGO_TARGET_DIR="$global_kybra_config_dir"/rust/target
-export CARGO_HOME="$global_kybra_rust_dir"
-export RUSTUP_HOME="$global_kybra_rust_dir"
-
-echo "\nPreparing canister binaries for upload...\n"
-
-{main_command if is_verbose else main_command_not_verbose}
-    """
-
-
 def parse_args_or_exit(args: list[str]) -> Args:
     args = args[1:]  # Discard the path to kybra
 
     flags = [arg for arg in args if (arg.startswith("-") or arg.startswith("--"))]
     args = [arg for arg in args if not (arg.startswith("-") or arg.startswith("--"))]
 
     if len(args) == 0:
@@ -183,14 +133,15 @@
     wasm_path = f"{canister_path}/{canister_name}.wasm"
 
     # This is where we store custom Python modules, such as stripped-down versions of stdlib modules
     custom_modules_path = f"{compiler_path}/custom_modules"
 
     home_dir = os.path.expanduser("~")
     global_kybra_config_dir = f"{home_dir}/.config/kybra"
+    global_kybra_version_dir = f"{global_kybra_config_dir}/{kybra.__version__}"
     global_kybra_rust_dir = f"{global_kybra_config_dir}/rust/{kybra.__rust_version__}"
     global_kybra_rust_bin_dir = f"{global_kybra_rust_dir}/bin"
     global_kybra_target_dir = f"{global_kybra_config_dir}/rust/target"
     global_kybra_bin_dir = f"{global_kybra_config_dir}/{kybra.__version__}/bin"
 
     return {
         "py_entry_file": py_entry_file_path,
@@ -201,38 +152,31 @@
         "did": did_path,
         "compiler": compiler_path,
         "lib": lib_path,
         "generated_did": generated_did_path,
         "wasm": wasm_path,
         "custom_modules": custom_modules_path,
         "global_kybra_config_dir": global_kybra_config_dir,
+        "global_kybra_version_dir": global_kybra_version_dir,
         "global_kybra_rust_dir": global_kybra_rust_dir,
         "global_kybra_rust_bin_dir": global_kybra_rust_bin_dir,
         "global_kybra_target_dir": global_kybra_target_dir,
         "global_kybra_bin_dir": global_kybra_bin_dir,
     }
 
 
-def detect_initial_compile(global_kybra_target_dir: str) -> bool:
-    return not os.path.exists(global_kybra_target_dir)
-
-
 @timed_inline
 def compile_python_or_exit(
     paths: Paths, cargo_env: dict[str, str], verbose: bool = False
 ):
     bundle_python_code(paths)
     run_kybra_generate_or_exit(paths, cargo_env, verbose)
     run_rustfmt_or_exit(paths, cargo_env, verbose)
 
 
-def encourage_patience(is_initial_compile: bool) -> str:
-    return " (be patient, this will take a while)" if is_initial_compile else ""
-
-
 def bundle_python_code(paths: Paths):
     # Begin module bundling/gathering process
     path = (
         list(filter(lambda x: x.startswith(os.getcwd()), sys.path))
         + [
             os.path.dirname(paths["py_entry_file"]),
         ]
@@ -345,100 +289,14 @@
         print(
             f'\nPlease open an issue at https://github.com/demergent-labs/kybra/issues/new\nincluding this message and the following error:\n\n {red(rustfmt_result.stderr.decode("utf-8"))}'
         )
         print("💀 Build failed")
         sys.exit(1)
 
 
-@timed_inline
-def optimize_wasm_binary_or_exit(
-    paths: Paths, canister_name: str, cargo_env: dict[str, str], verbose: bool = False
-):
-    optimization_result = subprocess.run(
-        [
-            f"{paths['global_kybra_rust_bin_dir']}/ic-wasm",
-            f"{paths['canister']}/{canister_name}_app.wasm",
-            "-o",
-            f"{paths['canister']}/{canister_name}_app.wasm",
-            "shrink",
-        ],
-        capture_output=not verbose,
-    )
-
-    if optimization_result.returncode != 0:
-        print(red("\n💣 Kybra error: optimizing generated Wasm"))
-        print(optimization_result.stderr.decode("utf-8"))
-        print("💀 Build failed")
-        sys.exit(1)
-
-    add_metadata_to_wasm_or_exit(paths, canister_name, verbose=verbose)
-
-    os.system(f"gzip -9 -f -k {paths['canister']}/{canister_name}_app.wasm")
-
-
-def add_metadata_to_wasm_or_exit(
-    paths: Paths, canister_name: str, verbose: bool = False
-):
-    # TODO removing this until we solve the Candid issue: https://forum.dfinity.org/t/automatically-generate-candid-from-rust-sources/5924/34
-    # TODO our current solution is to grab the Candid in post_install because of issues with Wasmer
-    # TODO Unfortunately this means that on first deploy the candid:service metadata is incorrect
-    # TODO thus we are relying on __get_candid_interface_tmp_hack for the time being
-    # add_candid_to_wasm_result = subprocess.run(
-    #     [
-    #         f"{paths['global_kybra_rust_bin_dir']}/ic-wasm",
-    #         f"{paths['canister']}/{canister_name}_app.wasm",
-    #         "-o",
-    #         f"{paths['canister']}/{canister_name}_app.wasm",
-    #         "metadata",
-    #         "candid:service",
-    #         "-f",
-    #         paths["did"],
-    #         "-v",
-    #         "public",
-    #     ],
-    #     capture_output=not verbose,
-    # )
-
-    # if add_candid_to_wasm_result.returncode != 0:
-    #     print(red("\n💣 Kybra error: adding candid to Wasm"))
-    #     print(add_candid_to_wasm_result.stderr.decode("utf-8"))
-    #     print("💀 Build failed")
-    #     sys.exit(1)
-
-    add_cdk_info_to_wasm_result = subprocess.run(
-        [
-            f"{paths['global_kybra_rust_bin_dir']}/ic-wasm",
-            f"{paths['canister']}/{canister_name}_app.wasm",
-            "-o",
-            f"{paths['canister']}/{canister_name}_app.wasm",
-            "metadata",
-            "cdk",
-            "-d",
-            f"kybra {kybra.__version__}",
-            "-v",
-            "public",
-        ],
-        capture_output=not verbose,
-    )
-
-    if add_cdk_info_to_wasm_result.returncode != 0:
-        print(red("\n💣 Kybra error: adding cdk name/version to Wasm"))
-        print(add_cdk_info_to_wasm_result.stderr.decode("utf-8"))
-        print("💀 Build failed")
-        sys.exit(1)
-
-
-def show_empathy(is_initial_compile: bool) -> str:
-    return (
-        " (❤ hang in there, this will be faster next time)"
-        if is_initial_compile
-        else ""
-    )
-
-
 def create_file(file_path: str, contents: str):
     file = open(file_path, "w")
     file.write(contents)
     file.close()
 
 
 def inline_timed(
```

### Comparing `kybra-0.5.3rc0/kybra/canisters/ledger/NOTICE` & `kybra-0.6.0rc0/kybra/canisters/ledger/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/canisters/ledger/__init__.py` & `kybra-0.6.0rc0/kybra/canisters/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/canisters/management/__init__.py` & `kybra-0.6.0rc0/kybra/canisters/management/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/canisters/management/basic.py` & `kybra-0.6.0rc0/kybra/canisters/management/basic.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/canisters/management/bitcoin.py` & `kybra-0.6.0rc0/kybra/canisters/management/bitcoin.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/canisters/management/http.py` & `kybra-0.6.0rc0/kybra/canisters/management/http.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/canisters/management/tecdsa.py` & `kybra-0.6.0rc0/kybra/canisters/management/tecdsa.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/cargotoml.py` & `kybra-0.6.0rc0/kybra/cargotoml.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,23 @@
 lto = false
 incremental = true
 codegen-units = 256
 
 [lib]
 crate-type = ["cdylib"]
 
+[features]
+azle_include_stdlib = []
+
 [dependencies]
-ic-cdk = "=0.8.0-beta.0"
-ic-cdk-macros = "0.6.10"
-ic-cdk-timers = "0.1.2"
-candid = {{ version = "0.9.0-beta.2", features = ["parser"] }}
+ic-cdk = "0.13.1"
+ic-cdk-macros = "0.9.0"
+ic-cdk-timers = "0.7.0"
+candid = {{ version = "0.10.6", features = ["value"] }}
+candid_parser = "0.1.4"
 kybra-vm-value-derive = {{ path = "./kybra_vm_value_derive" }}
 
 rustpython = {{ git = "https://github.com/demergent-labs/RustPython", rev = "b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874", default-features = false, features = ["stdlib", "encodings"] }}
 rustpython-vm = {{ git = "https://github.com/demergent-labs/RustPython", rev = "b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874", default-features = false, features = ["ic"] }}
 rustpython-stdlib = {{ git = "https://github.com/demergent-labs/RustPython", rev = "b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874", default-features = false, features = [] }}
 rustpython-derive = {{ git = "https://github.com/demergent-labs/RustPython", rev = "b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874", default-features = false, features = [] }}
 rustpython-compiler-core = {{ git = "https://github.com/demergent-labs/RustPython", rev = "b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874", default-features = false, features = [] }}
@@ -38,19 +42,21 @@
 # rustpython-stdlib = {{ path = "/home/RustPython/stdlib", default-features = false, features = [] }}
 # rustpython-derive = {{ path = "/home/RustPython/derive", default-features = false, features = [] }}
 # TODO add this back once we support the full stdlib: https://github.com/demergent-labs/kybra/issues/12
 # rustpython-pylib = {{ git = "https://github.com/demergent-labs/RustPython", rev = "b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874", default-features = false, features = ["freeze-stdlib"] }}
 # rustpython = {{ path = "../../../../../../RustPython", default-features = false, features = [] }}
 serde = {{ version = "1.0.137", default-features = false, features = [] }}
 async-recursion = "1.0.0"
-ic-stable-structures = "0.5.2"
+ic-stable-structures = "0.5.2" # TODO shall we update? Shall we remove the need to specify max size?
 slotmap = "1.0.6"
-ic-wasi-polyfill = {{ git = "https://github.com/demergent-labs/ic-wasi-polyfill", rev = "9b039919427ccd76bf452f012bdbfe3695e549a6" }}
-# ic-wasi-polyfill = {{ git = "https://github.com/wasm-forge/ic-wasi-polyfill", rev = "5e986cb3b95a58fbbf9386582f5c48847f22dcca" }}
-# ic-wasi-polyfill = {{ path = "/home/lastmjs/development/ic-wasi-polyfill", features = ["transient", "report_wasi_calls"] }}
+
+# TODO transient feature can be removed once https://github.com/demergent-labs/azle/issues/1731 is resolved
+ic-wasi-polyfill = {{ git = "https://github.com/wasm-forge/ic-wasi-polyfill", rev = "2d2edb382816e12da9bc81b786b7cd1a00d36735" , features = [
+    "transient",
+] }}
 
 [patch.crates-io]
 num-bigint = {{ git = "https://github.com/rust-num/num-bigint" }}
     """
 
 
 def generate_cargo_lock() -> str:
@@ -109,14 +115,20 @@
 [[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
+name = "arbitrary"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
+
+[[package]]
 name = "arrayvec"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
 
 [[package]]
 name = "ascii"
@@ -251,28 +263,28 @@
 name = "bstr"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
 dependencies = [
  "lazy_static",
  "memchr",
- "regex-automata",
+ "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byteorder"
-version = "1.4.3"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "candid"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "244005a1917bb7614cd775ca8a5d59efeb5ac74397bb14ba29a19347ebd78591"
 dependencies = [
@@ -280,55 +292,48 @@
  "binread",
  "byteorder",
  "candid_derive 0.5.0",
  "codespan-reporting",
  "crc32fast",
  "data-encoding",
  "hex",
- "lalrpop",
- "lalrpop-util",
+ "lalrpop 0.19.12",
+ "lalrpop-util 0.19.12",
  "leb128",
- "logos",
+ "logos 0.12.1",
  "num-bigint",
  "num-traits",
  "num_enum",
  "paste",
- "pretty",
+ "pretty 0.10.0",
  "serde",
  "serde_bytes",
  "sha2",
  "thiserror",
 ]
 
 [[package]]
 name = "candid"
-version = "0.9.0-beta.4"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3005be607a05b449b5a5a144839c5731699af5c309ce20eb5c812f889683601e"
+checksum = "965e86b1bd1c0c26df70cf0c92ae16c56204ab402eb915c26a541cf949d841cf"
 dependencies = [
  "anyhow",
  "binread",
  "byteorder",
- "candid_derive 0.6.1",
- "codespan-reporting",
- "crc32fast",
- "data-encoding",
+ "candid_derive 0.6.6",
  "hex",
- "lalrpop",
- "lalrpop-util",
+ "ic_principal",
  "leb128",
- "logos",
  "num-bigint",
  "num-traits",
- "num_enum",
  "paste",
- "pretty",
+ "pretty 0.12.3",
  "serde",
  "serde_bytes",
- "sha2",
  "stacker",
  "thiserror",
 ]
 
 [[package]]
 name = "candid_derive"
 version = "0.5.0"
@@ -339,22 +344,41 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "candid_derive"
-version = "0.6.1"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "041ce1020740a400035899b2909a6f4f275b79c8db502cbd59ace9b2cc88af58"
+checksum = "3de398570c386726e7a59d9887b68763c481477f9a043fb998a2e09d428df1a9"
 dependencies = [
  "lazy_static",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "candid_parser"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "48a3da76f989cd350b7342c64c6c6008341bb6186f6832ef04e56dc50ba0fd76"
+dependencies = [
+ "anyhow",
+ "candid 0.10.6",
+ "codespan-reporting",
+ "convert_case",
+ "hex",
+ "lalrpop 0.20.2",
+ "lalrpop-util 0.20.2",
+ "logos 0.13.0",
+ "num-bigint",
+ "pretty 0.12.3",
+ "thiserror",
 ]
 
 [[package]]
 name = "caseless"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "808dab3318747be122cb31d36de18d4d1c81277a76f8332a02b81a3d73463d7f"
@@ -368,15 +392,15 @@
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cdk_framework"
 version = "0.0.0"
-source = "git+https://github.com/demergent-labs/cdk_framework?rev=13c4abdd72bdcfa6a5b1ddf7f08a4fd83eacb419#13c4abdd72bdcfa6a5b1ddf7f08a4fd83eacb419"
+source = "git+https://github.com/demergent-labs/cdk_framework?rev=b006618358f455e4a378552cfe821c934eb2fd3d#b006618358f455e4a378552cfe821c934eb2fd3d"
 dependencies = [
  "proc-macro2",
  "quote",
  "regex",
 ]
 
 [[package]]
@@ -458,32 +482,20 @@
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
-name = "complex_init"
-version = "0.0.0"
+name = "convert_case"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
 dependencies = [
- "async-recursion",
- "candid 0.9.0-beta.4",
- "ic-cdk 0.8.0-beta.0",
- "ic-cdk-macros 0.6.10",
- "ic-cdk-timers",
- "ic-stable-structures",
- "ic-wasi-polyfill",
- "kybra-vm-value-derive",
- "rustpython",
- "rustpython-compiler-core",
- "rustpython-derive",
- "rustpython-stdlib",
- "rustpython-vm",
- "serde",
- "slotmap",
+ "unicode-segmentation",
 ]
 
 [[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
@@ -913,28 +925,41 @@
 name = "ic-cdk"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9beb0bf1dcd0639c313630e34aa547a2b19450ddf1969c176e13225ef3b29048"
 dependencies = [
  "candid 0.8.4",
  "ic-cdk-macros 0.6.10",
- "ic0",
+ "ic0 0.18.10",
+ "serde",
+ "serde_bytes",
+]
+
+[[package]]
+name = "ic-cdk"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9f3d204af0b11c45715169c997858edb58fa8407d08f4fae78a6b415dd39a362"
+dependencies = [
+ "candid 0.10.6",
+ "ic-cdk-macros 0.8.4",
+ "ic0 0.21.1",
  "serde",
  "serde_bytes",
 ]
 
 [[package]]
 name = "ic-cdk"
-version = "0.8.0-beta.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "229a2796b731794363b45ab7b3a8ae28dc4220256997709e52746887425c5135"
+checksum = "c63a6fceb94127bda86bd6d05f859a0e2a67d128a8ffb5ddab17e1f15ac8f555"
 dependencies = [
- "candid 0.9.0-beta.4",
- "ic-cdk-macros 0.8.0-beta.0",
- "ic0",
+ "candid 0.10.6",
+ "ic-cdk-macros 0.9.0",
+ "ic0 0.21.1",
  "serde",
  "serde_bytes",
 ]
 
 [[package]]
 name = "ic-cdk-macros"
 version = "0.6.10"
@@ -947,65 +972,108 @@
  "serde",
  "serde_tokenstream",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "ic-cdk-macros"
-version = "0.8.0-beta.0"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8ed566a9a45e97f8dd7eed3db58c95875272dbf053f0d94a965319cbffdb9e0"
+checksum = "a5a618e4020cea88e933d8d2f8c7f86d570ec06213506a80d4f2c520a9bba512"
 dependencies = [
- "candid 0.9.0-beta.4",
+ "candid 0.10.6",
+ "proc-macro2",
+ "quote",
+ "serde",
+ "serde_tokenstream",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "ic-cdk-macros"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fde5ca6ef1e69825c68916ff1bf7256b8f7ed69ac5ea3f1756f6e57f1503e27"
+dependencies = [
+ "candid 0.10.6",
  "proc-macro2",
  "quote",
  "serde",
  "serde_tokenstream",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "ic-cdk-timers"
-version = "0.1.2"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c739e7c592cb66df4f15c6b6c4859b1195782f63923e2fb1b29553d9c0819bd4"
+checksum = "054727a3a1c486528b96349817d54290ff70df6addf417def456ea708a16f7fb"
 dependencies = [
  "futures",
- "ic-cdk 0.7.4",
- "ic0",
+ "ic-cdk 0.13.1",
+ "ic0 0.21.1",
  "serde",
  "serde_bytes",
  "slotmap",
 ]
 
 [[package]]
 name = "ic-stable-structures"
 version = "0.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4e026318236de13568edafd85534ad29910908bf08cdcf177d4403fd4a5f6c4"
 
 [[package]]
+name = "ic-stable-structures"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a314297eb9edb4bbcc2e04d2e634e38d5900b68eadae661e927946d1aba3f9f7"
+dependencies = [
+ "ic_principal",
+]
+
+[[package]]
 name = "ic-wasi-polyfill"
-version = "0.3.9"
-source = "git+https://github.com/demergent-labs/ic-wasi-polyfill?rev=9b039919427ccd76bf452f012bdbfe3695e549a6#9b039919427ccd76bf452f012bdbfe3695e549a6"
+version = "0.3.14"
+source = "git+https://github.com/wasm-forge/ic-wasi-polyfill?rev=2d2edb382816e12da9bc81b786b7cd1a00d36735#2d2edb382816e12da9bc81b786b7cd1a00d36735"
 dependencies = [
  "function_name",
- "ic-cdk 0.8.0-beta.0",
- "ic-stable-structures",
+ "ic-cdk 0.12.1",
+ "ic-stable-structures 0.6.3",
  "rand",
  "stable-fs",
 ]
 
 [[package]]
 name = "ic0"
 version = "0.18.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "187fa0cecf46628330b7a390a1a65fb0637ea00d3a1121aa847ecbebc0f3ff79"
 
 [[package]]
+name = "ic0"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a54b5297861c651551676e8c43df805dad175cc33bc97dbd992edbbb85dcbcdf"
+
+[[package]]
+name = "ic_principal"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1762deb6f7c8d8c2bdee4b6c5a47b60195b74e9b5280faa5ba29692f8e17429c"
+dependencies = [
+ "arbitrary",
+ "crc32fast",
+ "data-encoding",
+ "serde",
+ "sha2",
+ "thiserror",
+]
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -1053,14 +1121,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "keccak"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f6d5ed8676d904364de097082f4e7d240b571b67989ced0240f08b7f966f940"
 dependencies = [
  "cpufeatures",
 ]
@@ -1082,35 +1159,66 @@
 checksum = "0a1cbf952127589f2851ab2046af368fd20645491bb4b376f04b7f94d7a9837b"
 dependencies = [
  "ascii-canvas",
  "bit-set",
  "diff",
  "ena",
  "is-terminal",
- "itertools",
- "lalrpop-util",
+ "itertools 0.10.5",
+ "lalrpop-util 0.19.12",
  "petgraph",
  "regex",
  "regex-syntax 0.6.29",
  "string_cache",
  "term",
  "tiny-keccak",
  "unicode-xid",
 ]
 
 [[package]]
+name = "lalrpop"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55cb077ad656299f160924eb2912aa147d7339ea7d69e1b5517326fdcec3c1ca"
+dependencies = [
+ "ascii-canvas",
+ "bit-set",
+ "ena",
+ "itertools 0.11.0",
+ "lalrpop-util 0.20.2",
+ "petgraph",
+ "pico-args",
+ "regex",
+ "regex-syntax 0.8.3",
+ "string_cache",
+ "term",
+ "tiny-keccak",
+ "unicode-xid",
+ "walkdir",
+]
+
+[[package]]
 name = "lalrpop-util"
 version = "0.19.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3c48237b9604c5a4702de6b824e02006c3214327564636aef27c1028a8fa0ed"
 dependencies = [
  "regex",
 ]
 
 [[package]]
+name = "lalrpop-util"
+version = "0.20.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "507460a910eb7b32ee961886ff48539633b788a36b65692b95f225b844c82553"
+dependencies = [
+ "regex-automata 0.4.6",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "leb128"
@@ -1189,15 +1297,38 @@
 
 [[package]]
 name = "logos"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf8b031682c67a8e3d5446840f9573eb7fe26efe7ec8d195c9ac4c0647c502f1"
 dependencies = [
- "logos-derive",
+ "logos-derive 0.12.1",
+]
+
+[[package]]
+name = "logos"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c000ca4d908ff18ac99b93a062cb8958d331c3220719c52e77cb19cc6ac5d2c1"
+dependencies = [
+ "logos-derive 0.13.0",
+]
+
+[[package]]
+name = "logos-codegen"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc487311295e0002e452025d6b580b77bb17286de87b57138f3b5db711cded68"
+dependencies = [
+ "beef",
+ "fnv",
+ "proc-macro2",
+ "quote",
+ "regex-syntax 0.6.29",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "logos-derive"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d849148dbaf9661a6151d1ca82b13bb4c4c128146a88d05253b38d4e2f496c"
@@ -1207,14 +1338,23 @@
  "proc-macro2",
  "quote",
  "regex-syntax 0.6.29",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "logos-derive"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dbfc0d229f1f42d790440136d941afd806bc9e949e2bcb8faa813b0f00d1267e"
+dependencies = [
+ "logos-codegen",
+]
+
+[[package]]
 name = "lz4_flex"
 version = "0.9.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a8cbbb2831780bc3b9c15a41f5b49222ef756b6730a95f3decfdd15903eb5a3"
 dependencies = [
  "twox-hash",
 ]
@@ -1248,17 +1388,17 @@
 checksum = "6365506850d44bff6e2fbcb5176cf63650e48bd45ef2fe2665ae1570e0f4b9ca"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.5.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
@@ -1530,14 +1670,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
+name = "pico-args"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5be167a7af36ee22fe3115051bc51f6e6c7054c9348e28deb4f49bd6f705a315"
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
 name = "pin-utils"
@@ -1565,14 +1711,36 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "pre_and_post_upgrade"
+version = "0.0.0"
+dependencies = [
+ "async-recursion",
+ "candid 0.10.6",
+ "candid_parser",
+ "ic-cdk 0.13.1",
+ "ic-cdk-macros 0.9.0",
+ "ic-cdk-timers",
+ "ic-stable-structures 0.5.4",
+ "ic-wasi-polyfill",
+ "kybra-vm-value-derive",
+ "rustpython",
+ "rustpython-compiler-core",
+ "rustpython-derive",
+ "rustpython-stdlib",
+ "rustpython-vm",
+ "serde",
+ "slotmap",
+]
+
+[[package]]
 name = "precomputed-hash"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
 name = "pretty"
@@ -1581,14 +1749,25 @@
 checksum = "ad9940b913ee56ddd94aec2d3cd179dd47068236f42a1a6415ccf9d880ce2a61"
 dependencies = [
  "arrayvec",
  "typed-arena",
 ]
 
 [[package]]
+name = "pretty"
+version = "0.12.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b55c4d17d994b637e2f4daf6e5dc5d660d209d5642377d675d7a1c3ab69fa579"
+dependencies = [
+ "arrayvec",
+ "typed-arena",
+ "unicode-width",
+]
+
+[[package]]
 name = "proc-macro-crate"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
 dependencies = [
  "once_cell",
  "toml_edit",
@@ -1716,26 +1895,43 @@
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
+name = "regex-automata"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax 0.8.3",
+]
+
+[[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
+name = "regex-syntax"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
+
+[[package]]
 name = "result-like"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccc7ce6435c33898517a30e85578cd204cbb696875efb93dec19a2d31294f810"
 dependencies = [
  "result-like-derive",
 ]
@@ -1816,15 +2012,15 @@
 name = "rustpython-codegen"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "ahash",
  "bitflags 1.3.2",
  "indexmap",
- "itertools",
+ "itertools 0.10.5",
  "log",
  "num-complex",
  "num-traits",
  "rustpython-ast",
  "rustpython-compiler-core",
 ]
 
@@ -1834,15 +2030,15 @@
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "ascii",
  "bitflags 1.3.2",
  "bstr",
  "cfg-if",
  "hexf-parse",
- "itertools",
+ "itertools 0.10.5",
  "lexical-parse-float",
  "libc",
  "lock_api",
  "num-bigint",
  "num-complex",
  "num-traits",
  "once_cell",
@@ -1867,15 +2063,15 @@
 [[package]]
 name = "rustpython-compiler-core"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "bitflags 1.3.2",
  "bstr",
- "itertools",
+ "itertools 0.10.5",
  "lz4_flex",
  "num-bigint",
  "num-complex",
 ]
 
 [[package]]
 name = "rustpython-derive"
@@ -1889,15 +2085,15 @@
 
 [[package]]
 name = "rustpython-derive-impl"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "indexmap",
- "itertools",
+ "itertools 0.10.5",
  "maplit",
  "once_cell",
  "proc-macro2",
  "quote",
  "rustpython-compiler-core",
  "rustpython-doc",
  "syn 1.0.109",
@@ -1916,17 +2112,17 @@
 [[package]]
 name = "rustpython-parser"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "ahash",
  "anyhow",
- "itertools",
- "lalrpop",
- "lalrpop-util",
+ "itertools 0.10.5",
+ "lalrpop 0.19.12",
+ "lalrpop-util 0.19.12",
  "log",
  "num-bigint",
  "num-traits",
  "phf",
  "phf_codegen",
  "rustc-hash",
  "rustpython-ast",
@@ -1963,15 +2159,15 @@
  "csv-core",
  "digest",
  "dns-lookup",
  "dyn-clone",
  "flate2",
  "gethostname",
  "hex",
- "itertools",
+ "itertools 0.10.5",
  "libc",
  "libsqlite3-sys",
  "mac_address",
  "md-5",
  "memchr",
  "memmap2",
  "mt19937",
@@ -2032,15 +2228,15 @@
  "getrandom",
  "glob",
  "half",
  "hex",
  "ic-cdk 0.7.4",
  "indexmap",
  "is-macro",
- "itertools",
+ "itertools 0.10.5",
  "libc",
  "log",
  "memchr",
  "memoffset 0.6.5",
  "nix 0.26.2",
  "num-bigint",
  "num-complex",
@@ -2112,14 +2308,23 @@
  "unicode-segmentation",
  "unicode-width",
  "utf8parse",
  "winapi",
 ]
 
 [[package]]
+name = "same-file"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
+dependencies = [
+ "winapi-util",
+]
+
+[[package]]
 name = "schannel"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
  "windows-sys 0.42.0",
 ]
@@ -2257,21 +2462,22 @@
  "bitflags 1.3.2",
  "num_enum",
  "optional",
 ]
 
 [[package]]
 name = "stable-fs"
-version = "0.1.8"
-source = "git+https://github.com/demergent-labs/stable-fs?rev=f85a7919c7468552ec6aa123f80634ebf168093c#f85a7919c7468552ec6aa123f80634ebf168093c"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85e88946666828308003420895ebdca375b0aa8e9b06503cb366aedb4cc0020a"
 dependencies = [
  "bitflags 2.3.2",
  "ciborium",
- "ic-cdk 0.8.0-beta.0",
- "ic-stable-structures",
+ "ic-cdk 0.12.1",
+ "ic-stable-structures 0.6.3",
  "serde",
  "serde_bytes",
 ]
 
 [[package]]
 name = "stacker"
 version = "0.1.15"
@@ -2775,14 +2981,24 @@
 [[package]]
 name = "volatile"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8e76fae08f03f96e166d2dfda232190638c10e0383841252416f9cfe2ae60e6"
 
 [[package]]
+name = "walkdir"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
+dependencies = [
+ "same-file",
+ "winapi-util",
+]
+
+[[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
 
 [[package]]
 name = "wasi"
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc` & `kybra-0.6.0rc0/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 26 18:37:25 2024 UTC, .py size: 4555 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e515 0366 cb11 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 0436 1966 cb11 0000  o........6.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6404 5a08 6405 5a09 6406  m.Z...d.Z.d.Z.d.
 00000070: 5a0a 4700 6407 6408 8400 6408 6505 8303  Z.G.d.d...d.e...
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/custom_modules/principal.py` & `kybra-0.6.0rc0/kybra/compiler/custom_modules/principal.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/Cargo.toml` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 edition = "2018"
 
 [dependencies]
 quote = "1.0.21"
 syn = "1.0.99"
 proc-macro2 = "1.0.43"
 regex = "1.7.0"
-rustpython-parser = { git = "https://github.com/demergent-labs/RustPython", branch = "kybra_initial", default-features = false, features = [] }
+rustpython-parser = { git = "https://github.com/demergent-labs/RustPython", branch = "kybra_initial", default-features = false, features = [
+] }
 annotate-snippets = "0.9.1"
 num-bigint = "0.4.3"
 backtrace = "0.3.67" # The package isn't strickly neccesary. std::backtrace::Backtrace might be able to do what we need, but it isn't clonable and backtrace::Backtrace is, so we are using to avoid adding a buch of lifetime code
 # rustpython = { path = "../../../../RustPython", default-features = false, features = [] }
-cdk_framework = { git = "https://github.com/demergent-labs/cdk_framework", rev = "b006618358f455e4a378552cfe821c934eb2fd3d" }
+cdk_framework = { git = "https://github.com/demergent-labs/cdk_framework", rev = "86b5acf42f2eba83728328b64112f446a3f8f4cb" }
 # cdk_framework = { path = "/home/cdk_framework" }
 # For local rust-analyzer uncomment this line and comment out the line above.
 # Update path/to/local to be the path to your local cdk_framework repo
-shared_utils = { path = "../shared_utils" }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/async_result_handler.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/async_result_handler.rs`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         }
 
         async fn async_result_handler_call(
             vm: &rustpython::vm::VirtualMachine,
             py_object_ref: &rustpython_vm::PyObjectRef,
             args: &Vec<rustpython_vm::PyObjectRef>
         ) -> rustpython_vm::PyResult {
-            let canister_id_principal: ic_cdk::export::Principal = args[0]
+            let canister_id_principal: candid::Principal = args[0]
                 .clone()
                 .try_from_vm_value(vm)?;
             let qual_name: String = args[1].clone().try_from_vm_value(vm)?;
 
             let cross_canister_call_function_name =
                 format!("call_{}", qual_name.replace(".", "_"));
 
@@ -126,15 +126,15 @@
         }
 
         async fn async_result_handler_call_with_payment(
             vm: &rustpython::vm::VirtualMachine,
             py_object_ref: &rustpython_vm::PyObjectRef,
             args: &Vec<rustpython_vm::PyObjectRef>
         ) -> rustpython_vm::PyResult {
-            let canister_id_principal: ic_cdk::export::Principal = args[0]
+            let canister_id_principal: candid::Principal = args[0]
                 .clone()
                 .try_from_vm_value(vm)?;
             let qual_name: String = args[1].clone().try_from_vm_value(vm)?;
 
             let cross_canister_call_with_payment_function_name =
                 format!("call_with_payment_{}", qual_name.replace(".", "_"));
 
@@ -154,15 +154,15 @@
         }
 
         async fn async_result_handler_call_with_payment128(
             vm: &rustpython::vm::VirtualMachine,
             py_object_ref: &rustpython_vm::PyObjectRef,
             args: &Vec<rustpython_vm::PyObjectRef>,
         ) -> rustpython_vm::PyResult {
-            let canister_id_principal: ic_cdk::export::Principal = args[0]
+            let canister_id_principal: candid::Principal = args[0]
                 .clone()
                 .try_from_vm_value(vm)?;
             let qual_name: String = args[1].clone().try_from_vm_value(vm)?;
 
             let cross_canister_call_with_payment128_function_name =
                 format!("call_with_payment128_{}", qual_name.replace(".", "_"));
 
@@ -183,15 +183,15 @@
         }
 
         async fn async_result_handler_call_raw(
             vm: &rustpython::vm::VirtualMachine,
             py_object_ref: &rustpython_vm::PyObjectRef,
             args: &Vec<rustpython_vm::PyObjectRef>
         ) -> rustpython_vm::PyResult {
-            let canister_id_principal: ic_cdk::export::Principal = args[0]
+            let canister_id_principal: candid::Principal = args[0]
                 .clone()
                 .try_from_vm_value(vm)?;
             let method_string: String = args[1].clone().try_from_vm_value(vm)?;
             let args_raw_vec: Vec<u8> = args[2].clone().try_from_vm_value(vm)?;
             let payment: u64 = args[3].clone().try_from_vm_value(vm)?;
 
             let call_raw_result = ic_cdk::api::call::call_raw(
@@ -209,15 +209,15 @@
         }
 
         async fn async_result_handler_call_raw128(
             vm: &rustpython::vm::VirtualMachine,
             py_object_ref: &rustpython_vm::PyObjectRef,
             args: &Vec<rustpython_vm::PyObjectRef>
         ) -> rustpython_vm::PyResult {
-            let canister_id_principal: ic_cdk::export::Principal = args[0]
+            let canister_id_principal: candid::Principal = args[0]
                 .clone()
                 .try_from_vm_value(vm)?;
             let method_string: String = args[1].clone().try_from_vm_value(vm)?;
             let args_raw_vec: Vec<u8> = args[2].clone().try_from_vm_value(vm)?;
             let payment: u128 = args[3].clone().try_from_vm_value(vm)?;
 
             let call_raw_result = ic_cdk::api::call::call_raw128(
@@ -350,15 +350,15 @@
                             quote! {#name}
                         })
                         .collect();
                     let params = tuple::generate_tuple(&param_names);
 
                     quote! {
                         #cross_canister_function_call_name => {
-                            let canister_id_principal: ic_cdk::export::Principal = args[0]
+                            let canister_id_principal: candid::Principal = args[0]
                                 .clone()
                                 .try_from_vm_value(vm)?;
 
                             #(#param_variable_definitions)*
 
                             create_call_result_instance(
                                 vm,
@@ -434,15 +434,15 @@
                     let payment_index = method.params.len() + 2;
                     let payment_variable_definition = quote! {
                         let payment: u64 = args[#payment_index].clone().try_from_vm_value(vm)?;
                     };
 
                     quote! {
                         #cross_canister_function_call_with_payment_name => {
-                            let canister_id_principal: ic_cdk::export::Principal = args[0]
+                            let canister_id_principal: candid::Principal = args[0]
                                 .clone()
                                 .try_from_vm_value(vm)?;
 
                             #(#param_variable_definitions)*
                             #payment_variable_definition
 
                             create_call_result_instance(
@@ -518,15 +518,15 @@
                     let payment_index = method.params.len() + 2;
                     let payment_variable_definition = quote! {
                         let payment: u128 = args[#payment_index].clone().try_from_vm_value(vm)?;
                     };
 
                     quote! {
                         #cross_canister_function_call_with_payment128_name => {
-                            let canister_id_principal: ic_cdk::export::Principal = args[0]
+                            let canister_id_principal: candid::Principal = args[0]
                                 .clone()
                                 .try_from_vm_value(vm)?;
 
                             #(#param_variable_definitions)*
                             #payment_variable_definition
 
                             create_call_result_instance(
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/mod.rs`

 * *Files 23% similar despite different names*

```diff
@@ -4,43 +4,40 @@
 };
 use proc_macro2::TokenStream;
 
 use crate::{ic_object, stable_b_tree_map_nodes::rust, StableBTreeMapNode};
 
 mod async_result_handler;
 mod call_global_python_function;
-mod candid;
-mod does_interpreter_exist;
+mod guard_against_non_controllers;
 mod unwrap_rust_python_result;
 mod utils;
 
 pub fn generate(
     update_methods: &Vec<UpdateMethod>,
     query_methods: &Vec<QueryMethod>,
     services: &Vec<Service>,
     stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
 ) -> TokenStream {
     let async_result_handler = async_result_handler::generate(&services);
     let call_global_python_function = call_global_python_function::generate();
-    let candid = candid::generate();
-    let does_interpreter_exist = does_interpreter_exist::generate();
+    let guard_against_non_controllers = guard_against_non_controllers::generate();
     let ic_object = ic_object::generate(
         update_methods,
         query_methods,
         services,
         stable_b_tree_map_nodes,
     );
     let stable_b_tree_map = rust::generate(stable_b_tree_map_nodes);
     let unwrap_rust_python_result = unwrap_rust_python_result::generate();
     let utils = utils::generate();
 
     quote::quote! {
         #async_result_handler
         #call_global_python_function
-        #candid
-        #does_interpreter_exist
+        #guard_against_non_controllers
         #ic_object
         #stable_b_tree_map
         #unwrap_rust_python_result
         #utils
     }
 }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/body/utils.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/body/utils.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/array.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/array.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 }
 
 pub fn generate_func_from_vm_value(name: &String) -> TokenStream {
     let type_alias_name = name.to_ident().to_token_stream();
     quote! {
         impl CdkActTryFromVmValue<#type_alias_name, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<#type_alias_name, rustpython_vm::builtins::PyBaseExceptionRef> {
-                let candid_func: ic_cdk::export::candid::Func = self.try_from_vm_value(vm)?;
+                let candid_func: candid::Func = self.try_from_vm_value(vm)?;
                 Ok(#type_alias_name::new(candid_func.principal, candid_func.method))
             }
         }
     }
 }
 
 pub fn generate_func_list_from_vm_value(name: &String) -> TokenStream {
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/opt.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/opt.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/primitive.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/primitive.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 self,
                 vm: &rustpython::vm::VirtualMachine,
             ) -> Result<#service_name, rustpython_vm::builtins::PyBaseExceptionRef> {
                 let canister_id = self.get_attr("canister_id", vm)?;
                 let to_str = canister_id.get_attr("to_str", vm)?;
                 let result = to_str.call((), vm)?;
                 let result_string: String = result.try_into_value(vm)?;
-                match ic_cdk::export::Principal::from_text(result_string) {
+                match candid::Principal::from_text(result_string) {
                     Ok(principal) => Ok(#service_name::new(principal)),
                     Err(err) => Err(vm.new_type_error(format!(
                         "TypeError: Could not convert value to Principal: {}",
                         err.to_string()
                     ))),
                 }
             }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs`

 * *Files 7% similar despite different names*

```diff
@@ -23,34 +23,28 @@
             .into());
         }
 
         let heartbeat_function_def_option = heartbeat_function_defs.get(0);
 
         Ok(
             if let Some(heartbeat_function_def) = heartbeat_function_def_option {
-                let (guard_function_name, body, return_type) = (
-                    heartbeat_function_def
-                        .get_guard_function_name()
-                        .map_err(Error::into),
+                let (body, return_type) = (
                     rust::generate(heartbeat_function_def).map_err(Error::into),
                     heartbeat_function_def.build_return_type(),
                 )
                     .collect_results()?;
 
                 if !canister_method::is_void(return_type) {
                     return Err(ReturnTypeMustBeVoid::err_from_stmt(
                         heartbeat_function_def,
                         CanisterMethodType::Heartbeat,
                     )
                     .into());
                 }
 
-                Some(HeartbeatMethod {
-                    body,
-                    guard_function_name,
-                })
+                Some(HeartbeatMethod { body })
             } else {
                 None
             },
         )
     }
 }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs`

 * *Files 6% similar despite different names*

```diff
@@ -26,33 +26,27 @@
             .into());
         }
 
         let inspect_message_function_def_option = inspect_message_function_defs.get(0);
 
         Ok(
             if let Some(inspect_method_function_def) = inspect_message_function_def_option {
-                let (guard_function_name, body, return_type) = (
-                    inspect_method_function_def
-                        .get_guard_function_name()
-                        .map_err(Error::into),
+                let (body, return_type) = (
                     rust::generate(inspect_method_function_def),
                     inspect_method_function_def.build_return_type(),
                 )
                     .collect_results()?;
 
                 if !canister_method::is_void(return_type) {
                     return Err(ReturnTypeMustBeVoid::err_from_stmt(
                         inspect_method_function_def,
                         CanisterMethodType::InspectMessage,
                     )
                     .into());
                 }
-                Some(InspectMessageMethod {
-                    body,
-                    guard_function_name,
-                })
+                Some(InspectMessageMethod { body })
             } else {
                 None
             },
         )
     }
 }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             .iter()
             .fold(vec![], |mut acc, program| {
                 acc.extend(match &program.deref() {
                     Mod::Module { body, .. } => body
                         .iter()
                         .filter(|stmt_kind| {
                             SourceMapped::new(*stmt_kind, program.source_map.clone())
-                                .is_canister_method_type(method_type.clone())
+                                .is_canister_method_type(method_type)
                         })
                         .map(|stmt_kind| SourceMapped::new(stmt_kind, program.source_map.clone()))
                         .collect(),
                     _ => vec![],
                 });
                 acc
             })
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs`

 * *Files 5% similar despite different names*

```diff
@@ -26,34 +26,28 @@
             .into());
         }
 
         let pre_upgrade_function_def_option = pre_upgrade_function_defs.get(0);
 
         Ok(
             if let Some(pre_upgrade_function_def) = pre_upgrade_function_def_option {
-                let (guard_function_name, body, return_type) = (
-                    pre_upgrade_function_def
-                        .get_guard_function_name()
-                        .map_err(Error::into),
+                let (body, return_type) = (
                     rust::generate(pre_upgrade_function_def),
                     pre_upgrade_function_def.build_return_type(),
                 )
                     .collect_results()?;
 
                 if !canister_method::is_void(return_type) {
                     return Err(ReturnTypeMustBeVoid::err_from_stmt(
                         pre_upgrade_function_def,
                         CanisterMethodType::Heartbeat,
                     )
                     .into());
                 }
 
-                Some(PreUpgradeMethod {
-                    body,
-                    guard_function_name,
-                })
+                Some(PreUpgradeMethod { body })
             } else {
                 None
             },
         )
     }
 }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/canister_method/rust.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/canister_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/constants.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/constants.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/analyze.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/analyze.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/display_string.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/display_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/test_error.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/test_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/debug/what_is_it.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/debug/what_is_it.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/collect_results.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/collect_results.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/errors/unreachable.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/errors/unreachable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/get_child_class_of.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/get_child_class_of.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/get_name.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/get_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/guard_function/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/guard_function/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/header/traits.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/header/traits.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/header/use_statements.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/header/use_statements.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,15 @@
         fn candid_encode(
             &self,
             candid_string_py_object_ref: rustpython_vm::PyObjectRef,
             vm: &rustpython_vm::VirtualMachine,
         ) -> rustpython_vm::PyResult {
             let candid_string: String = candid_string_py_object_ref.try_from_vm_value(vm)?;
 
-            let candid_args: candid::IDLArgs = candid_string
-                .parse::<candid::IDLArgs>()
+            let candid_args = candid_parser::parse_idl_args(&candid_string)
                 .map_err(|candid_error| CandidError::new(vm, candid_error.to_string()))?;
 
             let candid_encoded: Vec<u8> = candid_args
                 .to_bytes()
                 .map_err(|candid_error| CandidError::new(vm, candid_error.to_string()))?;
 
             candid_encoded
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     quote! {
                         #[pymethod]
                         fn #wrapper_fn_name(
                             &self,
                             args_py_object_refs: Vec<rustpython_vm::PyObjectRef>,
                             vm: &rustpython_vm::VirtualMachine
                         ) -> rustpython_vm::PyResult {
-                            let canister_id_principal: ic_cdk::export::Principal =
+                            let canister_id_principal: candid::Principal =
                                 args_py_object_refs[0].clone().try_from_vm_value(vm)?;
 
                             #(#param_variable_definitions)*
 
                             let notify_result = #real_function_name(
                                 canister_id_principal,
                                 #params
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             &self,
             canister_id_py_object_ref: rustpython_vm::PyObjectRef,
             method_py_object_ref: rustpython_vm::PyObjectRef,
             args_raw_py_object_ref: rustpython_vm::PyObjectRef,
             payment_py_object_ref: rustpython_vm::PyObjectRef,
             vm: &rustpython_vm::VirtualMachine,
         ) -> rustpython_vm::PyResult {
-            let canister_id_principal: ic_cdk::export::Principal =
+            let canister_id_principal: candid::Principal =
                 canister_id_py_object_ref.try_from_vm_value(vm)?;
 
             let method_string: String = method_py_object_ref.try_from_vm_value(vm)?;
 
             let args_raw_vec: Vec<u8> = args_raw_py_object_ref.try_from_vm_value(vm)?;
 
             let payment: u128 = payment_py_object_ref.try_from_vm_value(vm)?;
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                     quote! {
                         #[pymethod]
                         fn #wrapper_fn_name(
                             &self,
                             args_py_object_refs: Vec<rustpython_vm::PyObjectRef>,
                             vm: &rustpython_vm::VirtualMachine
                         ) -> rustpython_vm::PyResult {
-                            let canister_id_principal: ic_cdk::export::Principal =
+                            let canister_id_principal: candid::Principal =
                                 args_py_object_refs[0].clone().try_from_vm_value(vm)?;
 
                             #(#param_variable_definitions)*
 
                             let cycles: u128 = args_py_object_refs[args_py_object_refs.len() - 1]
                                 .clone()
                                 .try_from_vm_value(vm)?;
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 use proc_macro2::TokenStream;
 use quote::quote;
 
 pub fn generate() -> TokenStream {
     quote! {
         #[pymethod]
-        fn print(
+        fn reject(
             &self,
-            param_py_object_ref: rustpython_vm::PyObjectRef,
+            reject_py_object_ref: rustpython_vm::PyObjectRef,
             vm: &rustpython_vm::VirtualMachine,
         ) -> rustpython_vm::PyResult {
-            let param_string: String = param_py_object_ref.try_from_vm_value(vm)?;
+            let reject_message: String = reject_py_object_ref.try_from_vm_value(vm)?;
 
-            ic_cdk::println!("{:#?}", param_string)
+            ic_cdk::api::call::reject(reject_message.as_str())
                 .try_into_vm_value(vm)
                 .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
         }
     }
 }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 use proc_macro2::TokenStream;
 use quote::quote;
 
 pub fn generate() -> TokenStream {
     quote! {
         #[pymethod]
-        fn reject(
+        fn stable_read(
             &self,
-            reject_py_object_ref: rustpython_vm::PyObjectRef,
+            offset_py_object_ref: rustpython_vm::PyObjectRef,
+            length_py_object_ref: rustpython_vm::PyObjectRef,
             vm: &rustpython_vm::VirtualMachine,
         ) -> rustpython_vm::PyResult {
-            let reject_message: String = reject_py_object_ref.try_from_vm_value(vm)?;
+            let offset: u32 = offset_py_object_ref.try_from_vm_value(vm)?;
+            let length: u32 = length_py_object_ref.try_from_vm_value(vm)?;
+            let mut buf: Vec<u8> = vec![0; length as usize];
 
-            ic_cdk::api::call::reject(reject_message.as_str())
-                .try_into_vm_value(vm)
+            ic_cdk::api::stable::stable_read(offset, &mut buf);
+
+            buf.try_into_vm_value(vm)
                 .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
         }
     }
 }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/ic_object/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/ic_object/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/lib.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/main.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/main.rs`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     let py_file_names_string = fs::read_to_string(py_file_names_path).unwrap_or_else(|err| {
         eprintln!("Error reading {py_file_names_path}: {err}");
         process::exit(exit_codes::PY_FILE_NAMES_READ_ERROR);
     });
     let py_file_names: Vec<&str> = py_file_names_string.split(",").collect();
 
-    let lib_file = generate_canister(&py_file_names, &py_entry_module_name)
+    let lib_file = generate_canister(&py_file_names, py_entry_module_name)
         .unwrap_or_else(|errors| {
             eprintln!("Canister compilation failed:");
             for error in errors {
                 eprintln!("{}", error)
             }
             process::exit(exit_codes::CANISTER_COMPILATION_ERROR);
         })
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/params.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/method_utils/returns.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/method_utils/returns.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/py_ast/to_act.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/py_ast/to_act.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/source_map/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/source_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs`

 * *Files 20% similar despite different names*

```diff
@@ -24,35 +24,35 @@
                 self,
                 vm: &rustpython::vm::VirtualMachine,
             ) -> Result<bool, rustpython_vm::builtins::PyBaseExceptionRef> {
                 self.try_into_value(vm)
             }
         }
 
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Empty, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
+        impl CdkActTryFromVmValue<candid::Empty, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
             for rustpython::vm::PyObjectRef
         {
             fn try_from_vm_value(
                 self,
                 vm: &rustpython::vm::VirtualMachine,
-            ) -> Result<ic_cdk::export::candid::Empty, rustpython_vm::builtins::PyBaseExceptionRef>
+            ) -> Result<candid::Empty, rustpython_vm::builtins::PyBaseExceptionRef>
             {
                 Err(vm.new_type_error(
                     "value cannot be converted to Empty".to_string(),
                 ))
             }
         }
 
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Func, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
+        impl CdkActTryFromVmValue<candid::Func, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
             for rustpython::vm::PyObjectRef
         {
             fn try_from_vm_value(
                 self,
                 vm: &rustpython::vm::VirtualMachine,
-            ) -> Result<ic_cdk::export::candid::Func, rustpython_vm::builtins::PyBaseExceptionRef>
+            ) -> Result<candid::Func, rustpython_vm::builtins::PyBaseExceptionRef>
             {
                 let tuple_self: rustpython_vm::builtins::PyTupleRef = self.try_into_value(vm)?;
                 let principal = match tuple_self.get(0) {
                     Some(principal) => principal,
                     None => {
                         return Err(vm.new_type_error(
                             "could not convert value to Func, missing Principal"
@@ -66,51 +66,51 @@
                         return Err(vm.new_type_error(
                             "could not convert value to Func, missing method"
                                 .to_string(),
                         ))
                     }
                 };
 
-                Ok(ic_cdk::export::candid::Func {
+                Ok(candid::Func {
                     principal: principal.clone().try_from_vm_value(vm)?,
                     method: method.clone().try_from_vm_value(vm)?,
                 })
             }
         }
 
-        impl CdkActTryFromVmValue<ic_cdk::export::Principal, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
+        impl CdkActTryFromVmValue<candid::Principal, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
             for rustpython::vm::PyObjectRef
         {
             fn try_from_vm_value(
                 self,
                 vm: &rustpython::vm::VirtualMachine,
-            ) -> Result<ic_cdk::export::Principal, rustpython_vm::builtins::PyBaseExceptionRef>
+            ) -> Result<candid::Principal, rustpython_vm::builtins::PyBaseExceptionRef>
             {
                 let to_str = self.get_attr("to_str", vm)?;
                 let result = to_str.call((), vm)?;
                 let result_string: String = result.try_into_value(vm)?;
-                match ic_cdk::export::Principal::from_text(result_string) {
+                match candid::Principal::from_text(result_string) {
                     Ok(principal) => Ok(principal),
                     Err(err) => Err(vm.new_type_error(format!(
                         "could not convert value to Principal: {}",
                         err.to_string()
                     ))),
                 }
             }
         }
 
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Reserved, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
+        impl CdkActTryFromVmValue<candid::Reserved, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
             for rustpython::vm::PyObjectRef
         {
             fn try_from_vm_value(
                 self,
                 vm: &rustpython::vm::VirtualMachine,
-            ) -> Result<ic_cdk::export::candid::Reserved, rustpython_vm::builtins::PyBaseExceptionRef>
+            ) -> Result<candid::Reserved, rustpython_vm::builtins::PyBaseExceptionRef>
             {
-                Ok(ic_cdk::export::candid::Reserved)
+                Ok(candid::Reserved)
             }
         }
 
         impl CdkActTryFromVmValue<ic_cdk_timers::TimerId, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
             for rustpython::vm::PyObjectRef
         {
             fn try_from_vm_value(
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs`

 * *Files 3% similar despite different names*

```diff
@@ -38,27 +38,27 @@
                 self,
                 vm: &rustpython::vm::VirtualMachine,
             ) -> Result<_CdkFloat32, rustpython_vm::builtins::PyBaseExceptionRef> {
                 Ok(_CdkFloat32(self.try_into_value(vm)?))
             }
         }
 
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Int, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
+        impl CdkActTryFromVmValue<candid::Int, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
             for rustpython::vm::PyObjectRef
         {
             fn try_from_vm_value(
                 self,
                 vm: &rustpython::vm::VirtualMachine,
-            ) -> Result<ic_cdk::export::candid::Int, rustpython_vm::builtins::PyBaseExceptionRef>
+            ) -> Result<candid::Int, rustpython_vm::builtins::PyBaseExceptionRef>
             {
                 let int_result: Result<rustpython_vm::builtins::PyIntRef, _> =
                     self.try_into_value(vm);
 
                 match int_result {
-                    Ok(int) => Ok(ic_cdk::export::candid::Int(int.as_bigint().clone())),
+                    Ok(int) => Ok(candid::Int(int.as_bigint().clone())),
                     Err(_) => Err(vm.new_type_error("PyObjectRef is not a PyIntRef".to_string())),
                 }
             }
         }
 
         impl CdkActTryFromVmValue<i128, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(
@@ -101,25 +101,25 @@
                 self,
                 vm: &rustpython::vm::VirtualMachine,
             ) -> Result<i8, rustpython_vm::builtins::PyBaseExceptionRef> {
                 self.try_into_value(vm)
             }
         }
 
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Nat, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
+        impl CdkActTryFromVmValue<candid::Nat, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine>
             for rustpython::vm::PyObjectRef
         {
             fn try_from_vm_value(
                 self,
                 vm: &rustpython::vm::VirtualMachine,
-            ) -> Result<ic_cdk::export::candid::Nat, rustpython_vm::builtins::PyBaseExceptionRef>
+            ) -> Result<candid::Nat, rustpython_vm::builtins::PyBaseExceptionRef>
             {
                 let int: rustpython_vm::builtins::PyIntRef = self.try_into_value(vm)?;
 
-                match ic_cdk::export::candid::Nat::from_str(&int.as_bigint().to_string()) {
+                match candid::Nat::from_str(&int.as_bigint().to_string()) {
                     // TODO probably not the best conversion
                     Ok(nat) => Ok(nat),
                     Err(_) => {
                         Err(vm.new_type_error("Could not convert value to nat".to_string()))
                     }
                 }
             }
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs`

 * *Files 2% similar despite different names*

```diff
@@ -92,27 +92,27 @@
 
         impl<T> KybraTryFromVec for Box<T> {}
 
         impl KybraTryFromVec for () {}
 
         impl<T> KybraTryFromVec for Option<T> {}
 
-        impl KybraTryFromVec for ic_cdk::export::candid::Empty {}
+        impl KybraTryFromVec for candid::Empty {}
 
-        impl KybraTryFromVec for ic_cdk::export::candid::Reserved {}
+        impl KybraTryFromVec for candid::Reserved {}
 
-        impl KybraTryFromVec for ic_cdk::export::candid::Func {}
+        impl KybraTryFromVec for candid::Func {}
 
-        impl KybraTryFromVec for ic_cdk::export::Principal {}
+        impl KybraTryFromVec for candid::Principal {}
 
         impl KybraTryFromVec for ic_cdk_timers::TimerId {}
 
-        impl KybraTryFromVec for ic_cdk::export::candid::Int {}
+        impl KybraTryFromVec for candid::Int {}
 
-        impl KybraTryFromVec for ic_cdk::export::candid::Nat {}
+        impl KybraTryFromVec for candid::Nat {}
 
         impl KybraTryFromVec for _CdkFloat32 {}
 
         impl KybraTryFromVec for _CdkFloat64 {}
 
         impl<T> CdkActTryFromVmValue<Vec<T>, rustpython_vm::builtins::PyBaseExceptionRef, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
         where
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs`

 * *Files 5% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for bool {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.to_pyobject(vm))
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Empty {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for candid::Empty {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Err(CdkActTryIntoVmValueError("type \"empty\" cannot be represented in python".to_string()))
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Func {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for candid::Func {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 let principal = self.principal.try_into_vm_value(vm)?;
                 let method = self.method.try_into_vm_value(vm)?;
                 Ok(vm.ctx.new_tuple(vec![principal, method]).into())
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::Principal {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for candid::Principal {
             // TODO: In the future CdkActTryIntoVmValue needs to return rustpython_vm::object::PyResult
             // When it does all these map_err calls will be unnecessary and should be replaced with
             // question mark syntax.
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 let principal_class = vm.run_block_expr(
                     vm.new_scope_with_builtins(),
                     "from kybra import Principal; Principal"
@@ -63,15 +63,15 @@
 
                 let dict = vm.ctx.new_dict();
                 dict.set_item(attribute, vm.ctx.none(), vm);
                 Ok(dict.into())
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Reserved {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for candid::Reserved {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(vm.ctx.none())
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk_timers::TimerId {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for _CdkFloat32 {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.0.to_pyobject(vm))
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Int {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for candid::Int {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(vm.ctx.new_int(self.0).into())
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for i128 {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
@@ -58,15 +58,15 @@
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for i8 {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.to_pyobject(vm))
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Nat {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for candid::Nat {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(vm.ctx.new_int(self.0).into())
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for u128 {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs`

 * *Files 12% similar despite different names*

```diff
@@ -6,47 +6,47 @@
 
         impl KybraTryIntoVec for () {}
 
         impl KybraTryIntoVec for bool {}
 
         impl KybraTryIntoVec for String {}
 
-        impl KybraTryIntoVec for ic_cdk::export::candid::Empty {}
+        impl KybraTryIntoVec for candid::Empty {}
 
-        impl KybraTryIntoVec for ic_cdk::export::candid::Reserved {}
+        impl KybraTryIntoVec for candid::Reserved {}
 
-        impl KybraTryIntoVec for ic_cdk::export::candid::Func {}
+        impl KybraTryIntoVec for candid::Func {}
 
-        impl KybraTryIntoVec for ic_cdk::export::Principal {}
+        impl KybraTryIntoVec for candid::Principal {}
 
         impl KybraTryIntoVec for ic_cdk_timers::TimerId {}
 
         impl KybraTryIntoVec for ic_cdk::api::call::RejectionCode {}
 
         impl KybraTryIntoVec for f64 {}
 
         impl KybraTryIntoVec for f32 {}
 
         impl KybraTryIntoVec for _CdkFloat64 {}
 
         impl KybraTryIntoVec for _CdkFloat32 {}
 
-        impl KybraTryIntoVec for ic_cdk::export::candid::Int {}
+        impl KybraTryIntoVec for candid::Int {}
 
         impl KybraTryIntoVec for i128 {}
 
         impl KybraTryIntoVec for i64 {}
 
         impl KybraTryIntoVec for i32 {}
 
         impl KybraTryIntoVec for i16 {}
 
         impl KybraTryIntoVec for i8 {}
 
-        impl KybraTryIntoVec for ic_cdk::export::candid::Nat {}
+        impl KybraTryIntoVec for candid::Nat {}
 
         impl KybraTryIntoVec for u128 {}
 
         impl KybraTryIntoVec for u64 {}
 
         impl KybraTryIntoVec for usize {}
```

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs` & `kybra-0.6.0rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/module_bundler.py` & `kybra-0.6.0rc0/kybra/module_bundler.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/run_kybra_generate_or_exit.py` & `kybra-0.6.0rc0/kybra/run_kybra_generate_or_exit.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 ) -> subprocess.CompletedProcess[bytes]:
     return subprocess.run(
         [
             bin_path,
             paths["py_file_names_file"],
             paths["py_entry_module_name"],
             paths["lib"],
+            kybra.__version__,
         ],
         capture_output=not verbose,
         env=cargo_env,
     )
 
 
 def validate_process(
```

### Comparing `kybra-0.5.3rc0/kybra/timed.py` & `kybra-0.6.0rc0/kybra/timed.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.3rc0/kybra/types.py` & `kybra-0.6.0rc0/kybra/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,11 +22,12 @@
     did: str
     compiler: str
     lib: str
     generated_did: str
     wasm: str
     custom_modules: str
     global_kybra_config_dir: str
+    global_kybra_version_dir: str
     global_kybra_rust_dir: str
     global_kybra_rust_bin_dir: str
     global_kybra_bin_dir: str
     global_kybra_target_dir: str
```

### Comparing `kybra-0.5.3rc0/kybra.egg-info/PKG-INFO` & `kybra-0.6.0rc0/kybra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.5.3rc0
+Version: 0.6.0rc0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: NOTICE_PYTHON
 Requires-Dist: modulegraph==0.19.3
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kybra Version: 0.5.3rc0 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc0 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE License-File:
 NOTICE_PYTHON Requires-Dist: modulegraph==0.19.3
                                  _[_k_y_b_r_a_ _l_o_g_o_]
                         _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Kybra may have unknown security
 vulnerabilities due to the following: - Kybra does not yet have many live,
```

### Comparing `kybra-0.5.3rc0/kybra.egg-info/SOURCES.txt` & `kybra-0.6.0rc0/kybra.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,38 +22,38 @@
 kybra/canisters/ledger/NOTICE
 kybra/canisters/ledger/__init__.py
 kybra/canisters/management/__init__.py
 kybra/canisters/management/basic.py
 kybra/canisters/management/bitcoin.py
 kybra/canisters/management/http.py
 kybra/canisters/management/tecdsa.py
+kybra/compiler/LICENSE-RustPython
 kybra/compiler/__init__.py
 kybra/compiler/install_rust_dependencies.sh
+kybra/compiler/python_3_10_13_licenses.pdf
 kybra/compiler/__pycache__/__init__.cpython-310.pyc
 kybra/compiler/custom_modules/__init__.py
 kybra/compiler/custom_modules/principal.py
 kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
 kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
-kybra/compiler/kybra_deployer/Cargo.toml
-kybra/compiler/kybra_deployer/src/errors.rs
-kybra/compiler/kybra_deployer/src/lib.rs
+kybra/compiler/kybra_compile_python_stdlib/Cargo.toml
+kybra/compiler/kybra_compile_python_stdlib/src/main.rs
 kybra/compiler/kybra_generate/Cargo.toml
 kybra/compiler/kybra_generate/src/constants.rs
 kybra/compiler/kybra_generate/src/exit_codes.rs
 kybra/compiler/kybra_generate/src/get_child_class_of.rs
 kybra/compiler/kybra_generate/src/get_name.rs
 kybra/compiler/kybra_generate/src/get_subscript_slice.rs
 kybra/compiler/kybra_generate/src/keywords.rs
 kybra/compiler/kybra_generate/src/lib.rs
 kybra/compiler/kybra_generate/src/main.rs
 kybra/compiler/kybra_generate/src/tuple.rs
 kybra/compiler/kybra_generate/src/body/async_result_handler.rs
 kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
-kybra/compiler/kybra_generate/src/body/candid.rs
-kybra/compiler/kybra_generate/src/body/does_interpreter_exist.rs
+kybra/compiler/kybra_generate/src/body/guard_against_non_controllers.rs
 kybra/compiler/kybra_generate/src/body/mod.rs
 kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
 kybra/compiler/kybra_generate/src/body/utils.rs
 kybra/compiler/kybra_generate/src/candid_type/array.rs
 kybra/compiler/kybra_generate/src/candid_type/mod.rs
 kybra/compiler/kybra_generate/src/candid_type/opt.rs
 kybra/compiler/kybra_generate/src/candid_type/primitive.rs
@@ -127,15 +127,14 @@
 kybra/compiler/kybra_generate/src/errors/unreachable.rs
 kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
 kybra/compiler/kybra_generate/src/guard_function/mod.rs
 kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
 kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
 kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
 kybra/compiler/kybra_generate/src/header/mod.rs
-kybra/compiler/kybra_generate/src/header/ref_cells.rs
 kybra/compiler/kybra_generate/src/header/traits.rs
 kybra/compiler/kybra_generate/src/header/use_statements.rs
 kybra/compiler/kybra_generate/src/ic_object/mod.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
@@ -233,28 +232,14 @@
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
-kybra/compiler/kybra_post_install/Cargo.toml
-kybra/compiler/kybra_post_install/build.rs
-kybra/compiler/kybra_post_install/src/clear_chunks.rs
-kybra/compiler/kybra_post_install/src/dfx.rs
-kybra/compiler/kybra_post_install/src/error.rs
-kybra/compiler/kybra_post_install/src/generate_candid.rs
-kybra/compiler/kybra_post_install/src/install_app_canister.rs
-kybra/compiler/kybra_post_install/src/main.rs
-kybra/compiler/kybra_post_install/src/permissions.rs
-kybra/compiler/kybra_post_install/src/upload_app_canister.rs
-kybra/compiler/kybra_post_install/src/upload_chunk.rs
-kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs
 kybra/compiler/kybra_vm_value_derive/Cargo.toml
 kybra/compiler/kybra_vm_value_derive/src/lib.rs
 kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
 kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
 kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
 kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
-kybra/compiler/shared_utils/Cargo.toml
-kybra/compiler/shared_utils/src/lib.rs
 kybra/compiler/src/lib.rs
```

