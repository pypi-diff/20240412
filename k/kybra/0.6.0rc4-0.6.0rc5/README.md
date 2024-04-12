# Comparing `tmp/kybra-0.6.0rc4.tar.gz` & `tmp/kybra-0.6rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kybra-0.6.0rc4.tar", last modified: Fri Apr 12 15:11:22 2024, max compression
+gzip compressed data, was "kybra-0.6rc5.tar", last modified: Fri Apr 12 20:24:13 2024, max compression
```

## Comparing `kybra-0.6.0rc4.tar` & `kybra-0.6rc5.tar`

### file list

```diff
@@ -1,306 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.538684 kybra-0.6.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 15:09:33.000000 kybra-0.6.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 15:09:33.000000 kybra-0.6.0rc4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 15:09:33.000000 kybra-0.6.0rc4/NOTICE_PYTHON
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 15:11:22.538684 kybra-0.6.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-12 15:09:33.000000 kybra-0.6.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.494683 kybra-0.6.0rc4/kybra/
--rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-04-12 15:11:08.000000 kybra-0.6.0rc4/kybra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/build_wasm_binary_or_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.494683 kybra-0.6.0rc4/kybra/canisters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.494683 kybra-0.6.0rc4/kybra/canisters/ledger/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/ledger/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9521 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/ledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.494683 kybra-0.6.0rc4/kybra/canisters/management/
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/management/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/management/bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/management/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/canisters/management/tecdsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    85709 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/cargotoml.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.494683 kybra-0.6.0rc4/kybra/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/LICENSE-RustPython
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.498683 kybra-0.6.0rc4/kybra/compiler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra/compiler/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.498683 kybra-0.6.0rc4/kybra/compiler/custom_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/custom_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.498683 kybra-0.6.0rc4/kybra/compiler/custom_modules/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/custom_modules/principal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3370 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/install_rust_dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.498683 kybra-0.6.0rc4/kybra/compiler/kybra_compile_python_stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_compile_python_stdlib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.498683 kybra-0.6.0rc4/kybra/compiler/kybra_compile_python_stdlib/src/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_compile_python_stdlib/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.498683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.498683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.502683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/
--rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/guard_against_non_controllers.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.502683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/array.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.502683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.502683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.502683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/opt.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/record/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/tuple/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/variant/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/warnings/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.506683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.510683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.510683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/init_method/
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.510683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.510683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.510683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.510683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/constants.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.514683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/
--rw-r--r--   0 runner    (1001) docker     (127)    33809 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/analyze.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/display_string.rs
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/test_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.514683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/collect_results.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/unreachable.rs
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/exit_codes.rs
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/get_child_class_of.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/get_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.514683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.514683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.514683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/header/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/header/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/header/traits.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/header/use_statements.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.514683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.522683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.526683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/keywords.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.526683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.526683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/params.rs
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/returns.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.526683 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/errors.rs
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.530684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/source_map/
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/source_map/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.530684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/source_map/token_length/
--rw-r--r--   0 runner    (1001) docker     (127)    28330 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.530684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.530684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/tuple.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)   438859 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/python_3_10_13_licenses.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra/compiler/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/compiler/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/module_bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/run_kybra_generate_or_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/timed.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/kybra/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:11:22.534684 kybra-0.6.0rc4/kybra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 15:11:22.000000 kybra-0.6.0rc4/kybra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:11:22.538684 kybra-0.6.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 15:09:34.000000 kybra-0.6.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.014045 kybra-0.6rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 20:22:19.000000 kybra-0.6rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 20:22:19.000000 kybra-0.6rc5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 20:22:19.000000 kybra-0.6rc5/NOTICE_PYTHON
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 20:24:13.014045 kybra-0.6rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-12 20:22:19.000000 kybra-0.6rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.970045 kybra-0.6rc5/kybra/
+-rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-04-12 20:24:01.000000 kybra-0.6rc5/kybra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/build_wasm_binary_or_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.970045 kybra-0.6rc5/kybra/canisters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.970045 kybra-0.6rc5/kybra/canisters/ledger/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/ledger/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9521 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/ledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/canisters/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/management/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/management/bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/management/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/canisters/management/tecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60565 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/cargotoml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/LICENSE-RustPython
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/compiler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra/compiler/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/compiler/custom_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/custom_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/compiler/custom_modules/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/custom_modules/principal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3370 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/install_rust_dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/compiler/kybra_compile_python_stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_compile_python_stdlib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/compiler/kybra_compile_python_stdlib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_compile_python_stdlib/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.974045 kybra-0.6rc5/kybra/compiler/kybra_generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.978045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.978045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/
+-rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/guard_against_non_controllers.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.978045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/array.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/opt.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/record/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/tuple/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.982045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/variant/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/warnings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/init_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.986045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.990045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.990045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/constants.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.990045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)    33809 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/analyze.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/display_string.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/test_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.990045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/collect_results.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/unreachable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/exit_codes.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/get_child_class_of.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/get_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.990045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.994045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.994045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/header/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/header/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/header/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/header/use_statements.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:12.994045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.002045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.002045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/keywords.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.002045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.006045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/returns.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.006045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.006045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/source_map/
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/source_map/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.006045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/source_map/token_length/
+-rw-r--r--   0 runner    (1001) docker     (127)    28330 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.006045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.010045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.010045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/tuple.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.010045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.010045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.010045 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.010045 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.010045 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.014045 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.014045 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)   438859 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/python_3_10_13_licenses.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.014045 kybra-0.6rc5/kybra/compiler/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/compiler/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/module_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/run_kybra_generate_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 20:22:19.000000 kybra-0.6rc5/kybra/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:24:13.014045 kybra-0.6rc5/kybra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 20:24:12.000000 kybra-0.6rc5/kybra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:24:13.014045 kybra-0.6rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 20:22:19.000000 kybra-0.6rc5/setup.py
```

### Comparing `kybra-0.6.0rc4/LICENSE` & `kybra-0.6rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/NOTICE` & `kybra-0.6rc5/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/NOTICE_PYTHON` & `kybra-0.6rc5/NOTICE_PYTHON`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/PKG-INFO` & `kybra-0.6rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.6.0rc4
+Version: 0.6.0rc5
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
-Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc4 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc5 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE License-File:
 NOTICE_PYTHON Requires-Dist: modulegraph==0.19.3
                                  _[_k_y_b_r_a_ _l_o_g_o_]
                         _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Kybra may have unknown security
 vulnerabilities due to the following: - Kybra does not yet have many live,
```

### Comparing `kybra-0.6.0rc4/README.md` & `kybra-0.6rc5/README.md`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/__init__.py` & `kybra-0.6rc5/kybra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeAlias,
     Union,
 )
 
 # TODO I think we can simplify this just like we're doing with canisters
 from .compiler.custom_modules.principal import Principal as PrincipalRenamed
 
-__version__ = "0.6.0rc4"
+__version__ = "0.6.0rc5"
 __rust_version__ = "1.77.0"
 
 Principal = PrincipalRenamed
 
 int64 = int
 int32 = int
 int16 = int
```

### Comparing `kybra-0.6.0rc4/kybra/__main__.py` & `kybra-0.6rc5/kybra/__main__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/build_wasm_binary_or_exit.py` & `kybra-0.6rc5/kybra/build_wasm_binary_or_exit.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,96 +9,156 @@
 from kybra.types import Paths
 
 
 @timed_inline
 def build_wasm_binary_or_exit(
     paths: Paths, canister_name: str, cargo_env: dict[str, str], verbose: bool = False
 ):
-    compile_python_stdlib(paths, cargo_env, verbose)
+    compile_or_download_rust_python_stdlib(paths, cargo_env, verbose)
     compile_generated_rust_code(paths, canister_name, cargo_env, verbose)
     copy_wasm_to_dev_location(paths, canister_name)
     run_wasi2ic_on_wasm(paths, canister_name, cargo_env, verbose)
     generate_and_create_candid_file(paths, canister_name, cargo_env, verbose)
 
 
-def compile_python_stdlib(paths: Paths, cargo_env: dict[str, str], verbose: bool):
+def compile_or_download_rust_python_stdlib(
+    paths: Paths, cargo_env: dict[str, str], verbose: bool
+):
     if os.environ.get("KYBRA_COMPILE_RUST_PYTHON_STDLIB") == "true":
-        rust_python_path = f"{paths['global_kybra_version_dir']}/RustPython"
-
-        if not os.path.exists(rust_python_path):
-            run_subprocess(
-                ["git", "clone", "https://github.com/RustPython/RustPython.git"],
-                cargo_env,
-                verbose,
-                cwd=paths["global_kybra_version_dir"],
-            )
-
-            run_subprocess(
-                ["git", "checkout", "f12875027ce425297c07cbccb9be77514ed46157"],
-                cargo_env,
-                verbose,
-                cwd=f"{paths['global_kybra_version_dir']}/RustPython",
-            )
-
-        shutil.copytree(
-            f"{rust_python_path}/Lib",
-            f"{paths['canister']}/Lib",
-        )
-
-        os.makedirs(f"{paths['canister']}/rust_python_stdlib")
-        shutil.copy(
-            os.path.dirname(kybra.__file__) + "/compiler/LICENSE-RustPython",
-            f"{paths['canister']}/rust_python_stdlib/LICENSE-RustPython",
-        )
-        shutil.copy(
-            os.path.dirname(kybra.__file__) + "/compiler/python_3_10_13_licenses.pdf",
-            f"{paths['canister']}/rust_python_stdlib/python_3_10_13_licenses.pdf",
-        )
-
-        run_subprocess(
-            [
-                f"{paths['global_kybra_rust_bin_dir']}/cargo",
-                "run",
-                f"--manifest-path={paths['canister']}/kybra_compile_python_stdlib/Cargo.toml",
-                f"--package=kybra_compile_python_stdlib",
-                f"{paths['canister']}/rust_python_stdlib/stdlib",
-            ],
-            cargo_env,
-            verbose,
-        )
+        compile_rust_python_stdlib(paths, cargo_env, verbose)
     else:
-        rust_python_stdlib_path = (
+        rust_python_stdlib_global_path = (
             f"{paths['global_kybra_version_dir']}/rust_python_stdlib"
         )
-
-        if not os.path.exists(rust_python_stdlib_path):
-            run_subprocess(
-                [
-                    "curl",
-                    "-Lf",
-                    f"https://github.com/demergent-labs/kybra/releases/download/{kybra.__version__}/rust_python_stdlib.tar.gz",
-                    "-o",
-                    "rust_python_stdlib.tar.gz",
-                ],
-                cargo_env,
-                verbose,
-                cwd=paths["global_kybra_version_dir"],
-            )
-
-            run_subprocess(
-                ["tar", "-xvf", "rust_python_stdlib.tar.gz"],
-                cargo_env,
-                verbose,
-                cwd=paths["global_kybra_version_dir"],
-            )
-
-        shutil.copytree(
-            rust_python_stdlib_path,
-            f"{paths['canister']}/rust_python_stdlib",
+        download_rust_python_stdlib(
+            rust_python_stdlib_global_path, paths, cargo_env, verbose
         )
+        copy_rust_python_stdlib_global_to_staging(rust_python_stdlib_global_path, paths)
+
+
+def compile_rust_python_stdlib(paths: Paths, cargo_env: dict[str, str], verbose: bool):
+    rust_python_global_path = f"{paths['global_kybra_version_dir']}/RustPython"
+
+    if not os.path.exists(rust_python_global_path):
+        clone_and_checkout_rust_python(paths, cargo_env, verbose)
+
+    copy_rust_python_lib_global_to_staging(rust_python_global_path, paths)
+
+    rust_python_stdlib_staging_path = f"{paths['canister']}/rust_python_stdlib"
+
+    create_rust_python_stdlib_staging_directory(rust_python_stdlib_staging_path)
+    compile_and_write_rust_python_stdlib_to_staging(
+        rust_python_stdlib_staging_path, paths, cargo_env, verbose
+    )
+
+
+def clone_and_checkout_rust_python(
+    paths: Paths, cargo_env: dict[str, str], verbose: bool
+):
+    run_subprocess(
+        ["git", "clone", "https://github.com/RustPython/RustPython.git"],
+        cargo_env,
+        verbose,
+        cwd=paths["global_kybra_version_dir"],
+    )
+
+    run_subprocess(
+        ["git", "checkout", "f12875027ce425297c07cbccb9be77514ed46157"],
+        cargo_env,
+        verbose,
+        cwd=f"{paths['global_kybra_version_dir']}/RustPython",
+    )
+
+
+def copy_rust_python_lib_global_to_staging(rust_python_global_path: str, paths: Paths):
+    shutil.copytree(
+        f"{rust_python_global_path}/Lib",
+        f"{paths['canister']}/Lib",
+    )
+
+
+def create_rust_python_stdlib_staging_directory(rust_python_stdlib_staging_path: str):
+    os.makedirs(rust_python_stdlib_staging_path)
+
+    shutil.copy(
+        os.path.dirname(kybra.__file__) + "/compiler/LICENSE-RustPython",
+        f"{rust_python_stdlib_staging_path}/LICENSE-RustPython",
+    )
+
+    shutil.copy(
+        os.path.dirname(kybra.__file__) + "/compiler/python_3_10_13_licenses.pdf",
+        f"{rust_python_stdlib_staging_path}/python_3_10_13_licenses.pdf",
+    )
+
+
+def compile_and_write_rust_python_stdlib_to_staging(
+    rust_python_stdlib_staging_path: str,
+    paths: Paths,
+    cargo_env: dict[str, str],
+    verbose: bool,
+):
+    run_subprocess(
+        [
+            f"{paths['global_kybra_rust_bin_dir']}/cargo",
+            "run",
+            f"--manifest-path={paths['canister']}/kybra_compile_python_stdlib/Cargo.toml",
+            f"--package=kybra_compile_python_stdlib",
+            f"{rust_python_stdlib_staging_path}/stdlib",
+        ],
+        cargo_env,
+        verbose,
+    )
+
+
+def download_rust_python_stdlib(
+    rust_python_stdlib_global_path: str,
+    paths: Paths,
+    cargo_env: dict[str, str],
+    verbose: bool,
+):
+    if not os.path.exists(rust_python_stdlib_global_path):
+        download_rust_python_stdlib_tar_gz(paths, cargo_env, verbose)
+        extract_and_decompress_rust_python_stdlib_tar_gz(paths, cargo_env, verbose)
+
+
+def download_rust_python_stdlib_tar_gz(
+    paths: Paths, cargo_env: dict[str, str], verbose: bool
+):
+    run_subprocess(
+        [
+            "curl",
+            "-Lf",
+            f"https://github.com/demergent-labs/kybra/releases/download/{kybra.__version__}/rust_python_stdlib.tar.gz",
+            "-o",
+            "rust_python_stdlib.tar.gz",
+        ],
+        cargo_env,
+        verbose,
+        cwd=paths["global_kybra_version_dir"],
+    )
+
+
+def copy_rust_python_stdlib_global_to_staging(
+    rust_python_stdlib_global_path: str, paths: Paths
+):
+    shutil.copytree(
+        rust_python_stdlib_global_path,
+        f"{paths['canister']}/rust_python_stdlib",
+    )
+
+
+def extract_and_decompress_rust_python_stdlib_tar_gz(
+    paths: Paths, cargo_env: dict[str, str], verbose: bool
+):
+    run_subprocess(
+        ["tar", "-xvf", "rust_python_stdlib.tar.gz"],
+        cargo_env,
+        verbose,
+        cwd=paths["global_kybra_version_dir"],
+    )
 
 
 def compile_generated_rust_code(
     paths: Paths, canister_name: str, cargo_env: dict[str, str], verbose: bool
 ):
     run_subprocess(
         [
```

### Comparing `kybra-0.6.0rc4/kybra/canisters/ledger/NOTICE` & `kybra-0.6rc5/kybra/canisters/ledger/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/canisters/ledger/__init__.py` & `kybra-0.6rc5/kybra/canisters/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/canisters/management/__init__.py` & `kybra-0.6rc5/kybra/canisters/management/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/canisters/management/basic.py` & `kybra-0.6rc5/kybra/canisters/management/basic.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/canisters/management/bitcoin.py` & `kybra-0.6rc5/kybra/canisters/management/bitcoin.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/canisters/management/http.py` & `kybra-0.6rc5/kybra/canisters/management/http.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/canisters/management/tecdsa.py` & `kybra-0.6rc5/kybra/canisters/management/tecdsa.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/cargotoml.py` & `kybra-0.6rc5/kybra/cargotoml.py`

 * *Files 17% similar despite different names*

```diff
@@ -68,71 +68,71 @@
 [[package]]
 name = "Inflector"
 version = "0.11.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe438c63458706e03479442743baae6c88256498e6431708f6dfc520a26515d3"
 
 [[package]]
-name = "adler"
-version = "1.0.2"
+name = "addr2line"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+checksum = "a76fd60b23679b7d19bd066031410fb7e458ccc5e958eb5c325888ce4baedc97"
+dependencies = [
+ "gimli",
+]
 
 [[package]]
-name = "adler32"
-version = "1.2.0"
+name = "adler"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aae1277d39aeec15cb388266ecc24b11c80469deae6067e17a1a7aa9e5c1f234"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.2"
+version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "annotate-snippets"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3b9d411ecbaf79885c6df4d75fff75858d5995ff25385657a28af47e82f9c36"
+dependencies = [
+ "unicode-width",
+]
+
+[[package]]
 name = "ansi_term"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
-
-[[package]]
-name = "arbitrary"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
-
-[[package]]
-name = "arrayvec"
-version = "0.5.2"
+version = "1.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
+checksum = "98161a4e3e2184da77bb14f02184cdd111e83bbbcc9979dfee3c44b9a85f5602"
 
 [[package]]
 name = "ascii"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d92bec98840b8f03a5ff5413de5293bfcd8bf96467cf5452609f939ec6f5de16"
 
@@ -142,31 +142,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8824ecca2e851cec16968d54a01dd372ef8f95b244fb84b84e70128be347c3c6"
 dependencies = [
  "term",
 ]
 
 [[package]]
-name = "async-recursion"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
-
-[[package]]
-name = "atomic"
-version = "0.5.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c59bdb34bc650a32731b31bd8f0829cc15d24a708ee31559e0bb34f2bc320cba"
-
-[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi 0.1.19",
  "libc",
@@ -176,46 +159,35 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
-name = "base64"
-version = "0.13.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
-
-[[package]]
-name = "beef"
-version = "0.5.2"
+name = "backtrace"
+version = "0.3.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a8241f3ebb85c056b509d4327ad0358fbbba6ffb340bf388f26350aeda225b1"
-
-[[package]]
-name = "binread"
-version = "2.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16598dfc8e6578e9b597d9910ba2e73618385dc9f4b1d43dd92c349d6be6418f"
+checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
 dependencies = [
- "binread_derive",
- "lazy_static",
- "rustversion",
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
 ]
 
 [[package]]
-name = "binread_derive"
-version = "2.1.0"
+name = "bincode"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d9672209df1714ee804b1f4d4f68c8eb2a90b1f7a07acf472f88ce198ef1fed"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
- "either",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
+ "serde",
 ]
 
 [[package]]
 name = "bit-set"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
@@ -233,153 +205,34 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6dbe3c979c178231552ecba20214a8272df4e09f232a87aef4320cf06539aded"
-
-[[package]]
-name = "blake2"
-version = "0.10.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
-dependencies = [
- "digest",
-]
-
-[[package]]
-name = "block-buffer"
-version = "0.10.4"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
-dependencies = [
- "generic-array",
-]
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bstr"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
 dependencies = [
  "lazy_static",
  "memchr",
- "regex-automata 0.1.10",
+ "regex-automata",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.13.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
-
-[[package]]
-name = "byteorder"
-version = "1.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
-
-[[package]]
-name = "candid"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "244005a1917bb7614cd775ca8a5d59efeb5ac74397bb14ba29a19347ebd78591"
-dependencies = [
- "anyhow",
- "binread",
- "byteorder",
- "candid_derive 0.5.0",
- "codespan-reporting",
- "crc32fast",
- "data-encoding",
- "hex",
- "lalrpop 0.19.12",
- "lalrpop-util 0.19.12",
- "leb128",
- "logos 0.12.1",
- "num-bigint",
- "num-traits",
- "num_enum",
- "paste",
- "pretty 0.10.0",
- "serde",
- "serde_bytes",
- "sha2",
- "thiserror",
-]
-
-[[package]]
-name = "candid"
-version = "0.10.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "965e86b1bd1c0c26df70cf0c92ae16c56204ab402eb915c26a541cf949d841cf"
-dependencies = [
- "anyhow",
- "binread",
- "byteorder",
- "candid_derive 0.6.6",
- "hex",
- "ic_principal",
- "leb128",
- "num-bigint",
- "num-traits",
- "paste",
- "pretty 0.12.3",
- "serde",
- "serde_bytes",
- "stacker",
- "thiserror",
-]
-
-[[package]]
-name = "candid_derive"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58f1f4db7c7d04b87b70b3a35c5dc5c2c9dd73cef8bdf6760e2f18a0d45350dd"
-dependencies = [
- "lazy_static",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "candid_derive"
-version = "0.6.6"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3de398570c386726e7a59d9887b68763c481477f9a043fb998a2e09d428df1a9"
-dependencies = [
- "lazy_static",
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
-
-[[package]]
-name = "candid_parser"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48a3da76f989cd350b7342c64c6c6008341bb6186f6832ef04e56dc50ba0fd76"
-dependencies = [
- "anyhow",
- "candid 0.10.6",
- "codespan-reporting",
- "convert_case",
- "hex",
- "lalrpop 0.20.2",
- "lalrpop-util 0.20.2",
- "logos 0.13.0",
- "num-bigint",
- "pretty 0.12.3",
- "thiserror",
-]
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "caseless"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "808dab3318747be122cb31d36de18d4d1c81277a76f8332a02b81a3d73463d7f"
 dependencies = [
@@ -392,15 +245,15 @@
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cdk_framework"
 version = "0.0.0"
-source = "git+https://github.com/demergent-labs/cdk_framework?rev=b006618358f455e4a378552cfe821c934eb2fd3d#b006618358f455e4a378552cfe821c934eb2fd3d"
+source = "git+https://github.com/demergent-labs/cdk_framework?rev=86b5acf42f2eba83728328b64112f446a3f8f4cb#86b5acf42f2eba83728328b64112f446a3f8f4cb"
 dependencies = [
  "proc-macro2",
  "quote",
  "regex",
 ]
 
 [[package]]
@@ -419,41 +272,14 @@
  "num-integer",
  "num-traits",
  "time",
  "winapi",
 ]
 
 [[package]]
-name = "ciborium"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
-dependencies = [
- "ciborium-io",
- "ciborium-ll",
- "serde",
-]
-
-[[package]]
-name = "ciborium-io"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
-
-[[package]]
-name = "ciborium-ll"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
-dependencies = [
- "ciborium-io",
- "half",
-]
-
-[[package]]
 name = "clap"
 version = "2.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
 dependencies = [
  "ansi_term",
  "atty",
@@ -472,124 +298,32 @@
 dependencies = [
  "error-code",
  "str-buf",
  "winapi",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
-name = "convert_case"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
-dependencies = [
- "unicode-segmentation",
-]
-
-[[package]]
-name = "core-foundation"
-version = "0.9.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
-name = "core-foundation-sys"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
-
-[[package]]
-name = "cpufeatures"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "crc32fast"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
 name = "crossbeam-utils"
-version = "0.8.16"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
-dependencies = [
- "cfg-if",
-]
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
-name = "crypto-common"
-version = "0.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
-dependencies = [
- "generic-array",
- "typenum",
-]
-
-[[package]]
-name = "csv-core"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
-dependencies = [
- "memchr",
-]
-
-[[package]]
-name = "data-encoding"
-version = "2.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
-
-[[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
 
 [[package]]
-name = "digest"
-version = "0.10.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
-dependencies = [
- "block-buffer",
- "crypto-common",
- "subtle",
-]
-
-[[package]]
 name = "dirs-next"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b98cf8ebf19c3d1b223e151f99a4f9f0690dca41414773390fc824184ac833e1"
 dependencies = [
  "cfg-if",
  "dirs-sys-next",
@@ -603,36 +337,18 @@
 dependencies = [
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
-name = "dns-lookup"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53ecafc952c4528d9b51a458d1a8904b81783feff9fde08ab6ed2545ff396872"
-dependencies = [
- "cfg-if",
- "libc",
- "socket2",
- "winapi",
-]
-
-[[package]]
-name = "dyn-clone"
-version = "1.0.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
-
-[[package]]
 name = "either"
-version = "1.8.1"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
 
 [[package]]
 name = "ena"
 version = "0.14.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c533630cf40e9caa44bd91aadc88a75d75a4c3a12b4cfde353cbed41daa1e1f1"
 dependencies = [
@@ -653,32 +369,27 @@
 dependencies = [
  "atty",
  "log",
  "termcolor",
 ]
 
 [[package]]
-name = "errno"
-version = "0.3.1"
+name = "equivalent"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "windows-sys 0.48.0",
-]
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
+name = "errno"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
- "cc",
  "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "error-code"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64f18991e7bf11e7ffee451b5318b5c1a73c52d0d0ada6e5a3017c8c1ced6a21"
@@ -707,183 +418,55 @@
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
-name = "flate2"
-version = "1.0.26"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
-dependencies = [
- "crc32fast",
- "miniz_oxide",
-]
-
-[[package]]
-name = "fnv"
-version = "1.0.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
-
-[[package]]
-name = "function_name"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1ab577a896d09940b5fe12ec5ae71f9d8211fff62c919c03a3750a9901e98a7"
-dependencies = [
- "function_name-proc-macro",
-]
-
-[[package]]
-name = "function_name-proc-macro"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "673464e1e314dd67a0fd9544abc99e8eb28d0c7e3b69b033bcff9b2d00b87333"
-
-[[package]]
-name = "futures"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
-dependencies = [
- "futures-channel",
- "futures-core",
- "futures-executor",
- "futures-io",
- "futures-sink",
- "futures-task",
- "futures-util",
-]
-
-[[package]]
-name = "futures-channel"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
-dependencies = [
- "futures-core",
- "futures-sink",
-]
-
-[[package]]
-name = "futures-core"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
-
-[[package]]
-name = "futures-executor"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
-dependencies = [
- "futures-core",
- "futures-task",
- "futures-util",
-]
-
-[[package]]
-name = "futures-io"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
-
-[[package]]
-name = "futures-macro"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
-
-[[package]]
-name = "futures-sink"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
-
-[[package]]
-name = "futures-task"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
-
-[[package]]
-name = "futures-util"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
-dependencies = [
- "futures-channel",
- "futures-core",
- "futures-io",
- "futures-macro",
- "futures-sink",
- "futures-task",
- "memchr",
- "pin-project-lite",
- "pin-utils",
- "slab",
-]
-
-[[package]]
-name = "generic-array"
-version = "0.14.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
-dependencies = [
- "typenum",
- "version_check",
-]
-
-[[package]]
-name = "gethostname"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1ebd34e35c46e00bb73e81363248d627782724609fe1b6396f553f68fe3862e"
-dependencies = [
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "4eb1a864a501629691edf6c15a593b7a51eebaa1e8468e9ddc623de7c9b58ec6"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "half"
-version = "1.8.2"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
+checksum = "1b43ede17f21864e81be2fa654110bf1e793774238d86ef8555c37e6519c0403"
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+
+[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
@@ -892,345 +475,166 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "hexf-parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfa686283ad6dd069f105e5ab091b04c62850d3e4cf5d67debad1933f55023df"
 
 [[package]]
-name = "ic-cdk"
-version = "0.7.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9beb0bf1dcd0639c313630e34aa547a2b19450ddf1969c176e13225ef3b29048"
-dependencies = [
- "candid 0.8.4",
- "ic-cdk-macros 0.6.10",
- "ic0 0.18.10",
- "serde",
- "serde_bytes",
-]
-
-[[package]]
-name = "ic-cdk"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f3d204af0b11c45715169c997858edb58fa8407d08f4fae78a6b415dd39a362"
-dependencies = [
- "candid 0.10.6",
- "ic-cdk-macros 0.8.4",
- "ic0 0.21.1",
- "serde",
- "serde_bytes",
-]
-
-[[package]]
-name = "ic-cdk"
-version = "0.13.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c63a6fceb94127bda86bd6d05f859a0e2a67d128a8ffb5ddab17e1f15ac8f555"
-dependencies = [
- "candid 0.10.6",
- "ic-cdk-macros 0.9.0",
- "ic0 0.21.1",
- "serde",
- "serde_bytes",
-]
-
-[[package]]
-name = "ic-cdk-macros"
-version = "0.6.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebf50458685a0fc6b0e414cdba487610aeb199ac94db52d9fd76270565debee7"
-dependencies = [
- "candid 0.8.4",
- "proc-macro2",
- "quote",
- "serde",
- "serde_tokenstream",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "ic-cdk-macros"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5a618e4020cea88e933d8d2f8c7f86d570ec06213506a80d4f2c520a9bba512"
-dependencies = [
- "candid 0.10.6",
- "proc-macro2",
- "quote",
- "serde",
- "serde_tokenstream",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "ic-cdk-macros"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fde5ca6ef1e69825c68916ff1bf7256b8f7ed69ac5ea3f1756f6e57f1503e27"
-dependencies = [
- "candid 0.10.6",
- "proc-macro2",
- "quote",
- "serde",
- "serde_tokenstream",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "ic-cdk-timers"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "054727a3a1c486528b96349817d54290ff70df6addf417def456ea708a16f7fb"
-dependencies = [
- "futures",
- "ic-cdk 0.13.1",
- "ic0 0.21.1",
- "serde",
- "serde_bytes",
- "slotmap",
-]
-
-[[package]]
-name = "ic-stable-structures"
-version = "0.5.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4e026318236de13568edafd85534ad29910908bf08cdcf177d4403fd4a5f6c4"
-
-[[package]]
-name = "ic-stable-structures"
-version = "0.6.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a314297eb9edb4bbcc2e04d2e634e38d5900b68eadae661e927946d1aba3f9f7"
-dependencies = [
- "ic_principal",
-]
-
-[[package]]
-name = "ic-wasi-polyfill"
-version = "0.3.14"
-source = "git+https://github.com/wasm-forge/ic-wasi-polyfill?rev=2d2edb382816e12da9bc81b786b7cd1a00d36735#2d2edb382816e12da9bc81b786b7cd1a00d36735"
-dependencies = [
- "function_name",
- "ic-cdk 0.12.1",
- "ic-stable-structures 0.6.3",
- "rand",
- "stable-fs",
-]
-
-[[package]]
-name = "ic0"
-version = "0.18.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "187fa0cecf46628330b7a390a1a65fb0637ea00d3a1121aa847ecbebc0f3ff79"
-
-[[package]]
-name = "ic0"
-version = "0.21.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a54b5297861c651551676e8c43df805dad175cc33bc97dbd992edbbb85dcbcdf"
-
-[[package]]
-name = "ic_principal"
-version = "0.1.1"
+name = "indexmap"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1762deb6f7c8d8c2bdee4b6c5a47b60195b74e9b5280faa5ba29692f8e17429c"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
- "arbitrary",
- "crc32fast",
- "data-encoding",
- "serde",
- "sha2",
- "thiserror",
+ "autocfg",
+ "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.3"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
- "autocfg",
- "hashbrown",
+ "equivalent",
+ "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
- "hermit-abi 0.3.1",
+ "hermit-abi 0.3.9",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "is-macro"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a7d079e129b77477a49c5c4f1cfe9ce6c2c909ef52520693e8e811a714c7b20"
 dependencies = [
  "Inflector",
  "pmutil",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 1.0.99",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
- "rustix",
- "windows-sys 0.48.0",
+ "hermit-abi 0.3.9",
+ "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
-name = "itertools"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+name = "kybra-vm-value-derive"
+version = "0.0.0"
 dependencies = [
- "either",
+ "cdk_framework",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.99",
 ]
 
 [[package]]
-name = "keccak"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f6d5ed8676d904364de097082f4e7d240b571b67989ced0240f08b7f966f940"
+name = "kybra_compile_python_stdlib"
+version = "0.0.0"
 dependencies = [
- "cpufeatures",
+ "rustpython",
+ "rustpython-vm",
 ]
 
 [[package]]
-name = "kybra-vm-value-derive"
+name = "kybra_generate"
 version = "0.0.0"
 dependencies = [
+ "annotate-snippets",
+ "backtrace",
  "cdk_framework",
+ "num-bigint",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "regex",
+ "rustpython-parser 0.1.2",
+ "syn 1.0.99",
 ]
 
 [[package]]
 name = "lalrpop"
-version = "0.19.12"
+version = "0.19.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a1cbf952127589f2851ab2046af368fd20645491bb4b376f04b7f94d7a9837b"
+checksum = "f34313ec00c2eb5c3c87ca6732ea02dcf3af99c3ff7a8fb622ffb99c9d860a87"
 dependencies = [
  "ascii-canvas",
  "bit-set",
  "diff",
  "ena",
  "is-terminal",
- "itertools 0.10.5",
- "lalrpop-util 0.19.12",
- "petgraph",
- "regex",
- "regex-syntax 0.6.29",
- "string_cache",
- "term",
- "tiny-keccak",
- "unicode-xid",
-]
-
-[[package]]
-name = "lalrpop"
-version = "0.20.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55cb077ad656299f160924eb2912aa147d7339ea7d69e1b5517326fdcec3c1ca"
-dependencies = [
- "ascii-canvas",
- "bit-set",
- "ena",
- "itertools 0.11.0",
- "lalrpop-util 0.20.2",
+ "itertools",
+ "lalrpop-util",
  "petgraph",
  "pico-args",
  "regex",
- "regex-syntax 0.8.3",
+ "regex-syntax",
  "string_cache",
  "term",
  "tiny-keccak",
  "unicode-xid",
- "walkdir",
 ]
 
 [[package]]
 name = "lalrpop-util"
-version = "0.19.12"
+version = "0.19.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3c48237b9604c5a4702de6b824e02006c3214327564636aef27c1028a8fa0ed"
+checksum = "3d3b45d694c8074f77bc24fc26e47633c862a9cd3b48dd51209c02ba4c434d68"
 dependencies = [
  "regex",
 ]
 
 [[package]]
-name = "lalrpop-util"
-version = "0.20.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "507460a910eb7b32ee961886ff48539633b788a36b65692b95f225b844c82553"
-dependencies = [
- "regex-automata 0.4.6",
-]
-
-[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
-name = "leb128"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "884e2677b40cc8c339eaefcb701c32ef1fd2493d71118dc0ca4b6a736c93bd67"
-
-[[package]]
 name = "lexical-parse-float"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "683b3a5ebd0130b8fb52ba0bdc718cc56815b6a097e28ae5a6997d0ad17dc05f"
 dependencies = [
  "lexical-parse-integer",
  "lexical-util",
@@ -1254,160 +658,79 @@
 checksum = "5255b9ff16ff898710eb9eb63cb39248ea8a5bb036bea8085b1a767ff6c4e3fc"
 dependencies = [
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
-name = "libsqlite3-sys"
-version = "0.25.2"
+name = "libredox"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "29f835d03d717946d28b1d1ed632eb6f0e24a299388ee623d0c23118d3e8a7fa"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
- "cc",
- "pkg-config",
- "vcpkg",
+ "bitflags 2.5.0",
+ "libc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
-
-[[package]]
-name = "logos"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf8b031682c67a8e3d5446840f9573eb7fe26efe7ec8d195c9ac4c0647c502f1"
-dependencies = [
- "logos-derive 0.12.1",
-]
-
-[[package]]
-name = "logos"
-version = "0.13.0"
+version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c000ca4d908ff18ac99b93a062cb8958d331c3220719c52e77cb19cc6ac5d2c1"
+checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
- "logos-derive 0.13.0",
-]
-
-[[package]]
-name = "logos-codegen"
-version = "0.13.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc487311295e0002e452025d6b580b77bb17286de87b57138f3b5db711cded68"
-dependencies = [
- "beef",
- "fnv",
- "proc-macro2",
- "quote",
- "regex-syntax 0.6.29",
- "syn 2.0.18",
-]
-
-[[package]]
-name = "logos-derive"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1d849148dbaf9661a6151d1ca82b13bb4c4c128146a88d05253b38d4e2f496c"
-dependencies = [
- "beef",
- "fnv",
- "proc-macro2",
- "quote",
- "regex-syntax 0.6.29",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "logos-derive"
-version = "0.13.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbfc0d229f1f42d790440136d941afd806bc9e949e2bcb8faa813b0f00d1267e"
-dependencies = [
- "logos-codegen",
+ "cfg-if",
 ]
 
 [[package]]
 name = "lz4_flex"
 version = "0.9.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a8cbbb2831780bc3b9c15a41f5b49222ef756b6730a95f3decfdd15903eb5a3"
 dependencies = [
  "twox-hash",
 ]
 
 [[package]]
-name = "mac_address"
-version = "1.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4863ee94f19ed315bf3bc00299338d857d4b5bc856af375cc97d237382ad3856"
-dependencies = [
- "nix 0.23.2",
- "winapi",
-]
-
-[[package]]
 name = "maplit"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e2e65a1a2e43cfcb47a895c4c8b10d1f4a61097f9f254f183aee60cad9c651d"
 
 [[package]]
 name = "matches"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2532096657941c2fea9c289d370a250971c689d4f143798ff67113ec042024a5"
 
 [[package]]
-name = "md-5"
-version = "0.10.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6365506850d44bff6e2fbcb5176cf63650e48bd45ef2fe2665ae1570e0f4b9ca"
-dependencies = [
- "digest",
-]
-
-[[package]]
 name = "memchr"
-version = "2.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
-
-[[package]]
-name = "memmap2"
-version = "0.5.10"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
-dependencies = [
- "libc",
-]
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
@@ -1421,90 +744,69 @@
 checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
-name = "mt19937"
-version = "2.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12ca7f22ed370d5991a9caec16a83187e865bc8a532f889670337d5a5689e3a1"
-dependencies = [
- "rand_core",
-]
-
-[[package]]
 name = "new_debug_unreachable"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
+checksum = "650eef8c711430f1a879fdd01d4745a7deea475becfb90269c06775983bbf086"
 
 [[package]]
 name = "nibble_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77a5d83df9f36fe23f0c3648c6bbb8b0298bb5f1939c8f2704431371f4b84d43"
 dependencies = [
  "smallvec",
 ]
 
 [[package]]
 name = "nix"
-version = "0.23.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3790c00a0150112de0f4cd161e3d7fc4b2d8a5542ffc35f099a2562aecb35c"
-dependencies = [
- "bitflags 1.3.2",
- "cc",
- "cfg-if",
- "libc",
- "memoffset 0.6.5",
-]
-
-[[package]]
-name = "nix"
-version = "0.26.2"
+version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
+checksum = "598beaf3cc6fdd9a5dfb1630c2800c7acd31df7aaf0f565796fba2b53ca1af1b"
 dependencies = [
  "bitflags 1.3.2",
  "cfg-if",
  "libc",
  "memoffset 0.7.1",
  "pin-utils",
- "static_assertions",
 ]
 
 [[package]]
 name = "num-bigint"
 version = "0.4.3"
-source = "git+https://github.com/rust-num/num-bigint#6f2b8e0fc218dbd0f49bebb8db2d1a771fe6bafa"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.3"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
+checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
 dependencies = [
  "num-traits",
+ "serde",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
@@ -1532,19 +834,19 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi 0.3.9",
  "libc",
 ]
 
 [[package]]
 name = "num_enum"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1558,254 +860,212 @@
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dcbff9bc912032c62bf65ef1d5aea88983b420f4f839db1e9b0c281a25c9c799"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 1.0.99",
+]
+
+[[package]]
+name = "object"
+version = "0.30.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
+dependencies = [
+ "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "e82dad04139b71a90c080c8463fe0dc7902db5192d939bd0950f074d014339e1"
 
 [[package]]
 name = "optional"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978aa494585d3ca4ad74929863093e87cac9790d81fe7aba2b3dc2890643a0fc"
 
 [[package]]
-name = "page_size"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eebde548fbbf1ea81a99b128872779c437752fb99f217c45245e1a61dcd9edcd"
-dependencies = [
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.3.5",
+ "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "petgraph"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
+checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
 dependencies = [
  "fixedbitset",
- "indexmap",
+ "indexmap 2.2.6",
+]
+
+[[package]]
+name = "phf"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fabbf1ead8a5bcbc20f5f8b939ee3f5b0f6f281b6ad3468b84656b658b455259"
+dependencies = [
+ "phf_shared 0.10.0",
 ]
 
 [[package]]
 name = "phf"
-version = "0.11.1"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
+dependencies = [
+ "phf_shared 0.11.2",
+]
+
+[[package]]
+name = "phf_codegen"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+checksum = "4fb1c3a8bc4dd4e5cfce29b44ffc14bedd2ee294559a294e2a4d4c9e9a6a13cd"
 dependencies = [
- "phf_shared 0.11.1",
+ "phf_generator 0.10.0",
+ "phf_shared 0.10.0",
 ]
 
 [[package]]
 name = "phf_codegen"
-version = "0.11.1"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8d39688d359e6b34654d328e262234662d16cc0f60ec8dcbe5e718709342a5a"
+dependencies = [
+ "phf_generator 0.11.2",
+ "phf_shared 0.11.2",
+]
+
+[[package]]
+name = "phf_generator"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56ac890c5e3ca598bbdeaa99964edb5b0258a583a9eb6ef4e89fc85d9224770"
+checksum = "5d5285893bb5eb82e6aaf5d59ee909a06a16737a8970984dd7746ba9283498d6"
 dependencies = [
- "phf_generator",
- "phf_shared 0.11.1",
+ "phf_shared 0.10.0",
+ "rand",
 ]
 
 [[package]]
 name = "phf_generator"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+checksum = "48e4cc64c2ad9ebe670cb8fd69dd50ae301650392e81c05f9bfcb2d5bdbc24b0"
 dependencies = [
- "phf_shared 0.11.1",
+ "phf_shared 0.11.2",
  "rand",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6796ad771acdc0123d2a88dc428b5e38ef24456743ddb1744ed628f9815c096"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "phf_shared"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pico-args"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5be167a7af36ee22fe3115051bc51f6e6c7054c9348e28deb4f49bd6f705a315"
-
-[[package]]
-name = "pin-project-lite"
-version = "0.2.9"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "db8bcd96cb740d03149cbad5518db9fd87126a10ab519c011893b1754134c468"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
-name = "pkg-config"
-version = "0.3.27"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
-
-[[package]]
 name = "pmutil"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3894e5d549cccbe44afecf72922f277f603cd4bb0219c8342631ef18fffbe004"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 1.0.99",
 ]
 
 [[package]]
 name = "ppv-lite86"
-version = "0.2.17"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
-
-[[package]]
-name = "pre_and_post_upgrade"
-version = "0.0.0"
-dependencies = [
- "async-recursion",
- "candid 0.10.6",
- "candid_parser",
- "ic-cdk 0.13.1",
- "ic-cdk-macros 0.9.0",
- "ic-cdk-timers",
- "ic-stable-structures 0.5.4",
- "ic-wasi-polyfill",
- "kybra-vm-value-derive",
- "rustpython",
- "rustpython-compiler-core",
- "rustpython-derive",
- "rustpython-stdlib",
- "rustpython-vm",
- "serde",
- "slotmap",
-]
+checksum = "eb9f9e6e233e5c4a35559a617bf40a4ec447db2e84c20b55a6f83167b7e57872"
 
 [[package]]
 name = "precomputed-hash"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
-name = "pretty"
-version = "0.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad9940b913ee56ddd94aec2d3cd179dd47068236f42a1a6415ccf9d880ce2a61"
-dependencies = [
- "arrayvec",
- "typed-arena",
-]
-
-[[package]]
-name = "pretty"
-version = "0.12.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b55c4d17d994b637e2f4daf6e5dc5d660d209d5642377d675d7a1c3ab69fa579"
-dependencies = [
- "arrayvec",
- "typed-arena",
- "unicode-width",
-]
-
-[[package]]
 name = "proc-macro-crate"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
 dependencies = [
  "once_cell",
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
-name = "psm"
-version = "0.1.21"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
-dependencies = [
- "cc",
-]
-
-[[package]]
-name = "puruspe"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b7e158a385023d209d6d5f2585c4b468f6dcb3dd5aca9b75c4f1678c05bb375"
-
-[[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -1850,86 +1110,54 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
-dependencies = [
- "bitflags 1.3.2",
-]
-
-[[package]]
-name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.3"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
- "redox_syscall 0.2.16",
+ "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.7.2",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
-name = "regex-automata"
-version = "0.4.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-syntax 0.8.3",
-]
-
-[[package]]
-name = "regex-syntax"
-version = "0.6.29"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
-
-[[package]]
-name = "regex-syntax"
-version = "0.7.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
-
-[[package]]
 name = "regex-syntax"
-version = "0.8.3"
+version = "0.6.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
+checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
 
 [[package]]
 name = "result-like"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccc7ce6435c33898517a30e85578cd204cbb696875efb93dec19a2d31294f810"
 dependencies = [
@@ -1941,19 +1169,25 @@
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fabf0a2e54f711c68c50d49f648a1a8a37adcb57353f518ac4df374f0788f42"
 dependencies = [
  "pmutil",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 1.0.99",
  "syn-ext",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustc_version"
@@ -1962,17 +1196,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -1987,58 +1221,65 @@
  "cfg-if",
  "clap",
  "dirs-next",
  "env_logger",
  "libc",
  "log",
  "rustpython-compiler",
- "rustpython-parser",
- "rustpython-pylib",
- "rustpython-stdlib",
+ "rustpython-parser 0.2.0",
  "rustpython-vm",
  "rustyline",
 ]
 
 [[package]]
 name = "rustpython-ast"
+version = "0.1.0"
+source = "git+https://github.com/demergent-labs/RustPython?branch=kybra_initial#7527234365da52f5f4bca11ac84d403627ca6338"
+dependencies = [
+ "num-bigint",
+ "rustpython-compiler-core 0.1.2",
+]
+
+[[package]]
+name = "rustpython-ast"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "num-bigint",
  "rustpython-common",
- "rustpython-compiler-core",
+ "rustpython-compiler-core 0.2.0",
 ]
 
 [[package]]
 name = "rustpython-codegen"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "ahash",
  "bitflags 1.3.2",
- "indexmap",
- "itertools 0.10.5",
+ "indexmap 1.9.3",
+ "itertools",
  "log",
  "num-complex",
  "num-traits",
- "rustpython-ast",
- "rustpython-compiler-core",
+ "rustpython-ast 0.2.0",
+ "rustpython-compiler-core 0.2.0",
 ]
 
 [[package]]
 name = "rustpython-common"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "ascii",
  "bitflags 1.3.2",
  "bstr",
  "cfg-if",
  "hexf-parse",
- "itertools 0.10.5",
+ "itertools",
  "lexical-parse-float",
  "libc",
  "lock_api",
  "num-bigint",
  "num-complex",
  "num-traits",
  "once_cell",
@@ -2052,166 +1293,129 @@
 
 [[package]]
 name = "rustpython-compiler"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "rustpython-codegen",
- "rustpython-compiler-core",
- "rustpython-parser",
+ "rustpython-compiler-core 0.2.0",
+ "rustpython-parser 0.2.0",
+]
+
+[[package]]
+name = "rustpython-compiler-core"
+version = "0.1.2"
+source = "git+https://github.com/demergent-labs/RustPython?branch=kybra_initial#7527234365da52f5f4bca11ac84d403627ca6338"
+dependencies = [
+ "bincode",
+ "bitflags 1.3.2",
+ "bstr",
+ "itertools",
+ "lz4_flex",
+ "num-bigint",
+ "num-complex",
+ "serde",
+ "static_assertions",
+ "thiserror",
 ]
 
 [[package]]
 name = "rustpython-compiler-core"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "bitflags 1.3.2",
  "bstr",
- "itertools 0.10.5",
+ "itertools",
  "lz4_flex",
  "num-bigint",
  "num-complex",
 ]
 
 [[package]]
 name = "rustpython-derive"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
  "rustpython-compiler",
  "rustpython-derive-impl",
- "syn 1.0.109",
+ "syn 1.0.99",
 ]
 
 [[package]]
 name = "rustpython-derive-impl"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
- "indexmap",
- "itertools 0.10.5",
+ "indexmap 1.9.3",
+ "itertools",
  "maplit",
  "once_cell",
  "proc-macro2",
  "quote",
- "rustpython-compiler-core",
+ "rustpython-compiler-core 0.2.0",
  "rustpython-doc",
- "syn 1.0.109",
+ "syn 1.0.99",
  "syn-ext",
  "textwrap 0.15.2",
 ]
 
 [[package]]
 name = "rustpython-doc"
-version = "0.1.0"
-source = "git+https://github.com/RustPython/__doc__?branch=main#d927debd491e4c45b88e953e6e50e4718e0f2965"
+version = "0.3.0"
+source = "git+https://github.com/RustPython/__doc__?branch=main#8b62ce5d796d68a091969c9fa5406276cb483f79"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "rustpython-parser"
-version = "0.2.0"
-source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
+version = "0.1.2"
+source = "git+https://github.com/demergent-labs/RustPython?branch=kybra_initial#7527234365da52f5f4bca11ac84d403627ca6338"
 dependencies = [
  "ahash",
  "anyhow",
- "itertools 0.10.5",
- "lalrpop 0.19.12",
- "lalrpop-util 0.19.12",
+ "itertools",
+ "lalrpop-util",
  "log",
  "num-bigint",
  "num-traits",
- "phf",
- "phf_codegen",
- "rustc-hash",
- "rustpython-ast",
- "rustpython-compiler-core",
+ "phf 0.10.1",
+ "phf_codegen 0.10.0",
+ "rustpython-ast 0.1.0",
+ "rustpython-compiler-core 0.1.2",
+ "thiserror",
  "tiny-keccak",
  "unic-emoji-char",
  "unic-ucd-ident",
- "unicode_names2",
-]
-
-[[package]]
-name = "rustpython-pylib"
-version = "0.2.0"
-source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
-dependencies = [
- "glob",
- "rustpython-compiler-core",
- "rustpython-derive",
+ "unicode_names2 0.5.1",
 ]
 
 [[package]]
-name = "rustpython-stdlib"
+name = "rustpython-parser"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
- "adler32",
  "ahash",
- "ascii",
- "base64",
- "blake2",
- "cfg-if",
- "crc32fast",
- "crossbeam-utils",
- "csv-core",
- "digest",
- "dns-lookup",
- "dyn-clone",
- "flate2",
- "gethostname",
- "hex",
- "itertools 0.10.5",
- "libc",
- "libsqlite3-sys",
- "mac_address",
- "md-5",
- "memchr",
- "memmap2",
- "mt19937",
- "nix 0.26.2",
+ "anyhow",
+ "itertools",
+ "lalrpop",
+ "lalrpop-util",
+ "log",
  "num-bigint",
- "num-complex",
- "num-integer",
- "num-rational",
  "num-traits",
- "num_enum",
- "once_cell",
- "page_size",
- "parking_lot",
- "paste",
- "puruspe",
- "rand",
- "rand_core",
- "rustpython-common",
- "rustpython-derive",
- "rustpython-vm",
- "schannel",
- "sha-1",
- "sha2",
- "sha3",
- "socket2",
- "system-configuration",
- "termios",
- "ucd",
- "unic-char-property",
- "unic-normal",
- "unic-ucd-age",
- "unic-ucd-bidi",
- "unic-ucd-category",
+ "phf 0.11.2",
+ "phf_codegen 0.11.2",
+ "rustc-hash",
+ "rustpython-ast 0.2.0",
+ "rustpython-compiler-core 0.2.0",
+ "tiny-keccak",
+ "unic-emoji-char",
  "unic-ucd-ident",
- "unicode-casing",
- "unicode_names2",
- "uuid",
- "widestring",
- "winapi",
- "xml-rs",
+ "unicode_names2 0.6.0",
 ]
 
 [[package]]
 name = "rustpython-vm"
 version = "0.2.0"
 source = "git+https://github.com/demergent-labs/RustPython?rev=b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874#b7b0a4994d7871bf1e21fedb6bd0f0e5639fa874"
 dependencies = [
@@ -2225,72 +1429,71 @@
  "chrono",
  "crossbeam-utils",
  "exitcode",
  "getrandom",
  "glob",
  "half",
  "hex",
- "ic-cdk 0.7.4",
- "indexmap",
+ "indexmap 1.9.3",
  "is-macro",
- "itertools 0.10.5",
+ "itertools",
  "libc",
  "log",
  "memchr",
  "memoffset 0.6.5",
- "nix 0.26.2",
+ "nix",
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-rational",
  "num-traits",
  "num_cpus",
  "num_enum",
  "once_cell",
  "optional",
  "parking_lot",
  "paste",
  "rand",
  "result-like",
  "rustc_version",
- "rustpython-ast",
+ "rustpython-ast 0.2.0",
  "rustpython-codegen",
  "rustpython-common",
  "rustpython-compiler",
- "rustpython-compiler-core",
+ "rustpython-compiler-core 0.2.0",
  "rustpython-derive",
- "rustpython-parser",
+ "rustpython-parser 0.2.0",
  "rustyline",
  "schannel",
  "sre-engine",
  "static_assertions",
  "strum",
  "strum_macros",
  "thiserror",
  "thread_local",
  "timsort",
  "uname",
  "unic-ucd-bidi",
  "unic-ucd-category",
  "unic-ucd-ident",
  "unicode-casing",
- "unicode_names2",
+ "unicode_names2 0.6.0",
  "wasm-bindgen",
  "which",
  "widestring",
  "winapi",
  "windows",
  "winreg",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "rustyline"
 version = "11.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5dfc8644681285d1fb67a467fb3021bfea306b99b4146b166a1fe3ada965eece"
 dependencies = [
@@ -2298,204 +1501,88 @@
  "cfg-if",
  "clipboard-win",
  "dirs-next",
  "fd-lock",
  "libc",
  "log",
  "memchr",
- "nix 0.26.2",
+ "nix",
  "radix_trie",
  "scopeguard",
  "unicode-segmentation",
  "unicode-width",
  "utf8parse",
  "winapi",
 ]
 
 [[package]]
-name = "same-file"
-version = "1.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
- "windows-sys 0.42.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
-name = "serde_bytes"
-version = "0.11.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "416bda436f9aab92e02c8e10d49a15ddd339cea90b6e340fe51ed97abb548294"
-dependencies = [
- "serde",
-]
-
-[[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
-]
-
-[[package]]
-name = "serde_tokenstream"
-version = "0.1.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "797ba1d80299b264f3aac68ab5d12e5825a561749db4df7cd7c8083900c5d4e9"
-dependencies = [
- "proc-macro2",
- "serde",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "sha-1"
-version = "0.10.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5058ada175748e33390e40e872bd0fe59a19f265d0158daa551c5a88a76009c"
-dependencies = [
- "cfg-if",
- "cpufeatures",
- "digest",
-]
-
-[[package]]
-name = "sha2"
-version = "0.10.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
-dependencies = [
- "cfg-if",
- "cpufeatures",
- "digest",
-]
-
-[[package]]
-name = "sha3"
-version = "0.10.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75872d278a8f37ef87fa0ddbda7802605cb18344497949862c0d4dcb291eba60"
-dependencies = [
- "digest",
- "keccak",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
-name = "slab"
-version = "0.4.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "slotmap"
-version = "1.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1e08e261d0e8f5c43123b7adf3e4ca1690d655377ac93a03b2c9d3e98de1342"
-dependencies = [
- "version_check",
-]
-
-[[package]]
 name = "smallvec"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
-
-[[package]]
-name = "socket2"
-version = "0.4.9"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
-dependencies = [
- "libc",
- "winapi",
-]
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "sre-engine"
-version = "0.4.1"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a490c5c46c35dba9a6f5e7ee8e4d67e775eb2d2da0f115750b8d10e1c1ac2d28"
+checksum = "1120e6a8cbd4d85d5532d2e8a245aef2128e1853981f8b6d9943264184843102"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "num_enum",
  "optional",
 ]
 
 [[package]]
-name = "stable-fs"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85e88946666828308003420895ebdca375b0aa8e9b06503cb366aedb4cc0020a"
-dependencies = [
- "bitflags 2.3.2",
- "ciborium",
- "ic-cdk 0.12.1",
- "ic-stable-structures 0.6.3",
- "serde",
- "serde_bytes",
-]
-
-[[package]]
-name = "stacker"
-version = "0.1.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
-dependencies = [
- "cc",
- "cfg-if",
- "libc",
- "psm",
- "winapi",
-]
-
-[[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "str-buf"
@@ -2534,73 +1621,46 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 1.0.109",
+ "syn 1.0.99",
 ]
 
 [[package]]
-name = "subtle"
-version = "2.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
-
-[[package]]
 name = "syn"
-version = "1.0.109"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+checksum = "58dbef6ec655055e20b86b15a8cc6d439cca19b667537ac6a1369572d151ab13"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn-ext"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b86cb2b68c5b3c078cac02588bc23f3c04bb828c5d3aedd17980876ec6a7be6"
 dependencies = [
- "syn 1.0.109",
-]
-
-[[package]]
-name = "system-configuration"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
-dependencies = [
- "bitflags 1.3.2",
- "core-foundation",
- "system-configuration-sys",
-]
-
-[[package]]
-name = "system-configuration-sys"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
-dependencies = [
- "core-foundation-sys",
- "libc",
+ "syn 1.0.99",
 ]
 
 [[package]]
 name = "term"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c59df8ac95d96ff9bede18eb7300b0fda5e5d8d90960e76f8e14ae765eedbf1f"
@@ -2608,31 +1668,22 @@
  "dirs-next",
  "rustversion",
  "winapi",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.2.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "termios"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "411c5bf740737c7918b8b1fe232dca4dc9f8e754b8ad5e20966814001ed0ac6b"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "textwrap"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
@@ -2656,22 +1707,22 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
@@ -2682,17 +1733,17 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "timsort"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3cb4fa83bb73adf1c7219f4fe4bf3c0ac5635e4e51e070fad5df745a41bedfb8"
+checksum = "639ce8ef6d2ba56be0383a94dd13b92138d58de44c62618303bb798fa92bdc00"
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
@@ -2712,25 +1763,25 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.2"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 
 [[package]]
 name = "toml_edit"
-version = "0.19.10"
+version = "0.19.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
+checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
 dependencies = [
- "indexmap",
+ "indexmap 2.2.6",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "twox-hash"
 version = "1.6.3"
@@ -2738,32 +1789,14 @@
 checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
 dependencies = [
  "cfg-if",
  "static_assertions",
 ]
 
 [[package]]
-name = "typed-arena"
-version = "2.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
-
-[[package]]
-name = "typenum"
-version = "1.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
-
-[[package]]
-name = "ucd"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe4fa6e588762366f1eb4991ce59ad1b93651d0b769dfb4e4d1c5c4b943d1159"
-
-[[package]]
 name = "uname"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b72f89f0ca32e4db1c04e2a72f5345d59796d4866a1ee0609084569f73683dc8"
 dependencies = [
  "libc",
 ]
@@ -2797,34 +1830,14 @@
 dependencies = [
  "unic-char-property",
  "unic-char-range",
  "unic-ucd-version",
 ]
 
 [[package]]
-name = "unic-normal"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f09d64d33589a94628bc2aeb037f35c2e25f3f049c7348b5aa5580b48e6bba62"
-dependencies = [
- "unic-ucd-normal",
-]
-
-[[package]]
-name = "unic-ucd-age"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c8cfdfe71af46b871dc6af2c24fcd360e2f3392ee4c5111877f2947f311671c"
-dependencies = [
- "unic-char-property",
- "unic-char-range",
- "unic-ucd-version",
-]
-
-[[package]]
 name = "unic-ucd-bidi"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d1d568b51222484e1f8209ce48caa6b430bf352962b877d592c29ab31fb53d8c"
 dependencies = [
  "unic-char-property",
  "unic-char-range",
@@ -2840,46 +1853,25 @@
  "matches",
  "unic-char-property",
  "unic-char-range",
  "unic-ucd-version",
 ]
 
 [[package]]
-name = "unic-ucd-hangul"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb1dc690e19010e1523edb9713224cba5ef55b54894fe33424439ec9a40c0054"
-dependencies = [
- "unic-ucd-version",
-]
-
-[[package]]
 name = "unic-ucd-ident"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e230a37c0381caa9219d67cf063aa3a375ffed5bf541a452db16e744bdab6987"
 dependencies = [
  "unic-char-property",
  "unic-char-range",
  "unic-ucd-version",
 ]
 
 [[package]]
-name = "unic-ucd-normal"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86aed873b8202d22b13859dda5fe7c001d271412c31d411fd9b827e030569410"
-dependencies = [
- "unic-char-property",
- "unic-char-range",
- "unic-ucd-hangul",
- "unic-ucd-version",
-]
-
-[[package]]
 name = "unic-ucd-version"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96bd2f2237fe450fcd0a1d2f5f4e91711124f7857ba2e964247776ebeeb7b0c4"
 dependencies = [
  "unic-common",
 ]
@@ -2888,32 +1880,32 @@
 name = "unicode-casing"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "623f59e6af2a98bdafeb93fa277ac8e1e40440973001ca15cf4ae1541cd16d56"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "dcc811dc4066ac62f84f11307873c4850cb653bfa9b1719cee2bd2204a4bc5dd"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
@@ -2921,56 +1913,33 @@
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unicode_names2"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "029df4cc8238cefc911704ff8fa210853a0f3bce2694d8f51181dd41ee0f3301"
+
+[[package]]
+name = "unicode_names2"
 version = "0.6.0"
 source = "git+https://github.com/youknowone/unicode_names2.git?rev=4ce16aa85cbcdd9cc830410f1a72ef9a235f2fde#4ce16aa85cbcdd9cc830410f1a72ef9a235f2fde"
 dependencies = [
- "phf",
+ "phf 0.11.2",
 ]
 
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
-name = "uuid"
-version = "1.3.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
-dependencies = [
- "atomic",
- "getrandom",
- "rand",
- "uuid-macro-internal",
-]
-
-[[package]]
-name = "uuid-macro-internal"
-version = "1.3.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7da8500be15217da76379f13cfb1a9e351ccc2b0959c7bc8ea64ac4302ba4de4"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
-
-[[package]]
-name = "vcpkg"
-version = "0.2.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
-
-[[package]]
 name = "vec_map"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
 
 [[package]]
 name = "version_check"
@@ -2981,88 +1950,78 @@
 [[package]]
 name = "volatile"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8e76fae08f03f96e166d2dfda232190638c10e0383841252416f9cfe2ae60e6"
 
 [[package]]
-name = "walkdir"
-version = "2.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
-dependencies = [
- "same-file",
- "winapi-util",
-]
-
-[[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.15",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.15",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "which"
 version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
 dependencies = [
@@ -3091,17 +2050,17 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
@@ -3119,182 +2078,185 @@
  "windows_i686_msvc 0.39.0",
  "windows_x86_64_gnu 0.39.0",
  "windows_x86_64_msvc 0.39.0",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.48.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.39.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec7711666096bd4096ffa835238905bb33fb87267910e154b18b44eaabb340f2"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.39.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "763fc57100a5f7042e3057e7e8d9bdd7860d330070251a73d003563a3bb49e1b"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.39.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bc7cbfe58828921e10a9f446fcaaf649204dcfe6c1ddd712c5eebae6bda1106"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.39.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6868c165637d653ae1e8dc4d82c25d4f97dd6605eaa8d784b5c6e0ab2a252b65"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.39.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e4d40883ae9cae962787ca76ba76390ffa29214667a111db9e0a1ad8377e809"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
 
 [[package]]
 name = "winnow"
-version = "0.4.7"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca0ace3845f0d96209f0375e6d367e3eb87eb65d27d445bdc9f1843a26f39448"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
  "winapi",
 ]
-
-[[package]]
-name = "xml-rs"
-version = "0.8.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52839dc911083a8ef63efa4d039d1f58b5e409f923e44c80828f206f66e5541c"
     """
```

### Comparing `kybra-0.6.0rc4/kybra/compiler/LICENSE-RustPython` & `kybra-0.6rc5/kybra/compiler/LICENSE-RustPython`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc` & `kybra-0.6rc5/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 12 15:09:34 2024 UTC, .py size: 4555 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ae4e 1966 cb11 0000  o........N.f....
+00000000: 6f0d 0d0a 0000 0000 fb97 1966 cb11 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6404 5a08 6405 5a09 6406  m.Z...d.Z.d.Z.d.
 00000070: 5a0a 4700 6407 6408 8400 6408 6505 8303  Z.G.d.d...d.e...
```

### Comparing `kybra-0.6.0rc4/kybra/compiler/custom_modules/principal.py` & `kybra-0.6rc5/kybra/compiler/custom_modules/principal.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/install_rust_dependencies.sh` & `kybra-0.6rc5/kybra/compiler/install_rust_dependencies.sh`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/Cargo.toml` & `kybra-0.6rc5/kybra/compiler/kybra_generate/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/async_result_handler.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/async_result_handler.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/body/utils.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/body/utils.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/array.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/array.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/opt.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/opt.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/primitive.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/primitive.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/canister_method/rust.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/canister_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/constants.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/constants.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/analyze.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/analyze.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/display_string.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/display_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/test_error.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/test_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/debug/what_is_it.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/debug/what_is_it.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/collect_results.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/collect_results.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/compiler_output.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/compiler_output.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/errors/unreachable.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/errors/unreachable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/get_child_class_of.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/get_child_class_of.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/get_name.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/get_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/guard_function/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/guard_function/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/header/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/header/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/header/traits.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/header/traits.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/header/use_statements.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/header/use_statements.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/ic_object/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/ic_object/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/lib.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/main.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/main.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/params.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/method_utils/returns.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/method_utils/returns.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/py_ast/to_act.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/py_ast/to_act.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/source_map/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/source_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs` & `kybra-0.6rc5/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs` & `kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs` & `kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs` & `kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs` & `kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/kybra_vm_value_derive/src/lib.rs` & `kybra-0.6rc5/kybra/compiler/kybra_vm_value_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/compiler/python_3_10_13_licenses.pdf` & `kybra-0.6rc5/kybra/compiler/python_3_10_13_licenses.pdf`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/module_bundler.py` & `kybra-0.6rc5/kybra/module_bundler.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/run_kybra_generate_or_exit.py` & `kybra-0.6rc5/kybra/run_kybra_generate_or_exit.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/timed.py` & `kybra-0.6rc5/kybra/timed.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra/types.py` & `kybra-0.6rc5/kybra/types.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc4/kybra.egg-info/PKG-INFO` & `kybra-0.6rc5/kybra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.6.0rc4
+Version: 0.6.0rc5
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
-Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc4 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc5 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE License-File:
 NOTICE_PYTHON Requires-Dist: modulegraph==0.19.3
                                  _[_k_y_b_r_a_ _l_o_g_o_]
                         _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Kybra may have unknown security
 vulnerabilities due to the following: - Kybra does not yet have many live,
```

### Comparing `kybra-0.6.0rc4/kybra.egg-info/SOURCES.txt` & `kybra-0.6rc5/kybra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

