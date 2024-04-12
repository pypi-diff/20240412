# Comparing `tmp/kybra-0.6.0rc2.tar.gz` & `tmp/kybra-0.6.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kybra-0.6.0rc2.tar", last modified: Fri Apr 12 14:05:14 2024, max compression
+gzip compressed data, was "kybra-0.6.0rc3.tar", last modified: Fri Apr 12 14:16:35 2024, max compression
```

## Comparing `kybra-0.6.0rc2.tar` & `kybra-0.6.0rc3.tar`

### file list

```diff
@@ -1,306 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/NOTICE_PYTHON
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.663403 kybra-0.6.0rc2/kybra/
--rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-04-12 14:05:00.000000 kybra-0.6.0rc2/kybra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/build_wasm_binary_or_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.663403 kybra-0.6.0rc2/kybra/canisters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.663403 kybra-0.6.0rc2/kybra/canisters/ledger/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/ledger/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9521 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/ledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.667403 kybra-0.6.0rc2/kybra/canisters/management/
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/management/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/management/bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/management/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/canisters/management/tecdsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    85709 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/cargotoml.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.667403 kybra-0.6.0rc2/kybra/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/LICENSE-RustPython
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.667403 kybra-0.6.0rc2/kybra/compiler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra/compiler/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.667403 kybra-0.6.0rc2/kybra/compiler/custom_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/custom_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.667403 kybra-0.6.0rc2/kybra/compiler/custom_modules/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/custom_modules/principal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3370 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/install_rust_dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.667403 kybra-0.6.0rc2/kybra/compiler/kybra_compile_python_stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_compile_python_stdlib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.667403 kybra-0.6.0rc2/kybra/compiler/kybra_compile_python_stdlib/src/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_compile_python_stdlib/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.671404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.671404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.671404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/
--rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/guard_against_non_controllers.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.675403 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/array.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.675403 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.675403 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.675403 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/opt.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.675403 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/record/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.675403 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/tuple/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/variant/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/warnings/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.679404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.683404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.683404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/init_method/
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.683404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.683404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.683404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.683404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/constants.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.687404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/
--rw-r--r--   0 runner    (1001) docker     (127)    33809 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/analyze.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/display_string.rs
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/test_error.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.687404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/collect_results.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/unreachable.rs
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/exit_codes.rs
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/get_child_class_of.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/get_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.687404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.687404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.687404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/header/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/header/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/header/traits.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/header/use_statements.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.687404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.699404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.699404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/keywords.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.699404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.703404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/params.rs
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/returns.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.703404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/errors.rs
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.703404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/source_map/
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/source_map/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.703404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/source_map/token_length/
--rw-r--r--   0 runner    (1001) docker     (127)    28330 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.703404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.707404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.707404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/tuple.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.707404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.707404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)   438859 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/python_3_10_13_licenses.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/kybra/compiler/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/compiler/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/module_bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/run_kybra_generate_or_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/timed.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/kybra/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/kybra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 14:05:14.000000 kybra-0.6.0rc2/kybra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:05:14.711404 kybra-0.6.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 14:03:12.000000 kybra-0.6.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.395631 kybra-0.6.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/NOTICE_PYTHON
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 14:16:35.395631 kybra-0.6.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.347631 kybra-0.6.0rc3/kybra/
+-rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-04-12 14:16:23.000000 kybra-0.6.0rc3/kybra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/build_wasm_binary_or_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.351631 kybra-0.6.0rc3/kybra/canisters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.351631 kybra-0.6.0rc3/kybra/canisters/ledger/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/ledger/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9521 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/ledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.351631 kybra-0.6.0rc3/kybra/canisters/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/management/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/management/bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/management/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/canisters/management/tecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85709 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/cargotoml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.351631 kybra-0.6.0rc3/kybra/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/LICENSE-RustPython
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.351631 kybra-0.6.0rc3/kybra/compiler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra/compiler/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.351631 kybra-0.6.0rc3/kybra/compiler/custom_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/custom_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.355631 kybra-0.6.0rc3/kybra/compiler/custom_modules/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/custom_modules/principal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3370 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/install_rust_dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.355631 kybra-0.6.0rc3/kybra/compiler/kybra_compile_python_stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_compile_python_stdlib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.355631 kybra-0.6.0rc3/kybra/compiler/kybra_compile_python_stdlib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_compile_python_stdlib/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.355631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.355631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.355631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/
+-rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/guard_against_non_controllers.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.359631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/array.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.359631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.359631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.359631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/opt.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.359631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/record/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.359631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/tuple/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/variant/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/warnings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.363631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.367631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.367631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/init_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.367631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.367631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.367631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.367631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/constants.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.371631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)    33809 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/analyze.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/display_string.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/test_error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.371631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/collect_results.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/unreachable.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/exit_codes.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/get_child_class_of.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/get_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.371631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.371631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.371631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/header/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/header/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/header/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/header/use_statements.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.371631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.379631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.383631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/keywords.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.383631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.383631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/params.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/returns.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.387631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.387631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/source_map/
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/source_map/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.387631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/source_map/token_length/
+-rw-r--r--   0 runner    (1001) docker     (127)    28330 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.387631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.387631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/tuple.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)   438859 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/python_3_10_13_licenses.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.391631 kybra-0.6.0rc3/kybra/compiler/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/compiler/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/module_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/run_kybra_generate_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/kybra/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:16:35.395631 kybra-0.6.0rc3/kybra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 14:16:35.000000 kybra-0.6.0rc3/kybra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:16:35.395631 kybra-0.6.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 14:14:49.000000 kybra-0.6.0rc3/setup.py
```

### Comparing `kybra-0.6.0rc2/LICENSE` & `kybra-0.6.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/NOTICE` & `kybra-0.6.0rc3/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/NOTICE_PYTHON` & `kybra-0.6.0rc3/NOTICE_PYTHON`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/PKG-INFO` & `kybra-0.6.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.6.0rc2
+Version: 0.6.0rc3
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
-Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc2 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc3 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE License-File:
 NOTICE_PYTHON Requires-Dist: modulegraph==0.19.3
                                  _[_k_y_b_r_a_ _l_o_g_o_]
                         _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Kybra may have unknown security
 vulnerabilities due to the following: - Kybra does not yet have many live,
```

### Comparing `kybra-0.6.0rc2/README.md` & `kybra-0.6.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/__init__.py` & `kybra-0.6.0rc3/kybra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeAlias,
     Union,
 )
 
 # TODO I think we can simplify this just like we're doing with canisters
 from .compiler.custom_modules.principal import Principal as PrincipalRenamed
 
-__version__ = "0.6.0rc2"
+__version__ = "0.6.0rc3"
 __rust_version__ = "1.77.0"
 
 Principal = PrincipalRenamed
 
 int64 = int
 int32 = int
 int16 = int
```

### Comparing `kybra-0.6.0rc2/kybra/__main__.py` & `kybra-0.6.0rc3/kybra/__main__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/build_wasm_binary_or_exit.py` & `kybra-0.6.0rc3/kybra/build_wasm_binary_or_exit.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/canisters/ledger/NOTICE` & `kybra-0.6.0rc3/kybra/canisters/ledger/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/canisters/ledger/__init__.py` & `kybra-0.6.0rc3/kybra/canisters/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/canisters/management/__init__.py` & `kybra-0.6.0rc3/kybra/canisters/management/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/canisters/management/basic.py` & `kybra-0.6.0rc3/kybra/canisters/management/basic.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/canisters/management/bitcoin.py` & `kybra-0.6.0rc3/kybra/canisters/management/bitcoin.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/canisters/management/http.py` & `kybra-0.6.0rc3/kybra/canisters/management/http.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/canisters/management/tecdsa.py` & `kybra-0.6.0rc3/kybra/canisters/management/tecdsa.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/cargotoml.py` & `kybra-0.6.0rc3/kybra/cargotoml.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/LICENSE-RustPython` & `kybra-0.6.0rc3/kybra/compiler/LICENSE-RustPython`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc` & `kybra-0.6.0rc3/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 12 14:03:12 2024 UTC, .py size: 4555 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 203f 1966 cb11 0000  o....... ?.f....
+00000000: 6f0d 0d0a 0000 0000 d941 1966 cb11 0000  o........A.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6404 5a08 6405 5a09 6406  m.Z...d.Z.d.Z.d.
 00000070: 5a0a 4700 6407 6408 8400 6408 6505 8303  Z.G.d.d...d.e...
```

### Comparing `kybra-0.6.0rc2/kybra/compiler/custom_modules/principal.py` & `kybra-0.6.0rc3/kybra/compiler/custom_modules/principal.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/install_rust_dependencies.sh` & `kybra-0.6.0rc3/kybra/compiler/install_rust_dependencies.sh`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/Cargo.toml` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/async_result_handler.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/async_result_handler.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/body/utils.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/body/utils.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/array.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/array.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/opt.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/opt.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/primitive.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/primitive.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/canister_method/rust.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/canister_method/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/constants.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/constants.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/analyze.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/analyze.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/display_string.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/display_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/test_error.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/test_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/debug/what_is_it.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/debug/what_is_it.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/collect_results.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/collect_results.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/compiler_output.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/compiler_output.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/errors/unreachable.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/errors/unreachable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/get_child_class_of.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/get_child_class_of.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/get_name.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/get_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/guard_function/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/guard_function/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/header/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/header/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/header/traits.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/header/traits.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/header/use_statements.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/header/use_statements.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/ic_object/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/ic_object/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/lib.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/main.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/main.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/params.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/method_utils/returns.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/method_utils/returns.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/py_ast/to_act.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/py_ast/to_act.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/source_map/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/source_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/kybra_vm_value_derive/src/lib.rs` & `kybra-0.6.0rc3/kybra/compiler/kybra_vm_value_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/compiler/python_3_10_13_licenses.pdf` & `kybra-0.6.0rc3/kybra/compiler/python_3_10_13_licenses.pdf`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/module_bundler.py` & `kybra-0.6.0rc3/kybra/module_bundler.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/run_kybra_generate_or_exit.py` & `kybra-0.6.0rc3/kybra/run_kybra_generate_or_exit.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/timed.py` & `kybra-0.6.0rc3/kybra/timed.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra/types.py` & `kybra-0.6.0rc3/kybra/types.py`

 * *Files identical despite different names*

### Comparing `kybra-0.6.0rc2/kybra.egg-info/PKG-INFO` & `kybra-0.6.0rc3/kybra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.6.0rc2
+Version: 0.6.0rc3
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
-Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc2 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.6.0rc3 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE License-File:
 NOTICE_PYTHON Requires-Dist: modulegraph==0.19.3
                                  _[_k_y_b_r_a_ _l_o_g_o_]
                         _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Kybra may have unknown security
 vulnerabilities due to the following: - Kybra does not yet have many live,
```

### Comparing `kybra-0.6.0rc2/kybra.egg-info/SOURCES.txt` & `kybra-0.6.0rc3/kybra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

