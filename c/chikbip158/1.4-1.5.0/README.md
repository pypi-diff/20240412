# Comparing `tmp/chikbip158-1.4.tar.gz` & `tmp/chikbip158-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chikbip158-1.4.tar", last modified: Fri Apr 12 00:30:42 2024, max compression
+gzip compressed data, was "chikbip158-1.5.0.tar", last modified: Fri Apr 12 05:44:36 2024, max compression
```

## Comparing `chikbip158-1.4.tar` & `chikbip158-1.5.0.tar`

### file list

```diff
@@ -1,95 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.845832 chikbip158-1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.849832 chikbip158-1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-12 00:30:37.000000 chikbip158-1.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 00:30:37.000000 chikbip158-1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 00:30:37.000000 chikbip158-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-12 00:30:42.861832 chikbip158-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-12 00:30:37.000000 chikbip158-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/chikbip158.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-12 00:30:42.000000 chikbip158-1.4/chikbip158.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-12 00:30:42.000000 chikbip158-1.4/chikbip158.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:30:42.000000 chikbip158-1.4/chikbip158.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:30:42.000000 chikbip158-1.4/chikbip158.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 00:30:42.000000 chikbip158-1.4/chikbip158.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-12 00:30:37.000000 chikbip158-1.4/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 00:30:37.000000 chikbip158-1.4/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-12 00:30:37.000000 chikbip158-1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.849832 chikbip158-1.4/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-12 00:30:37.000000 chikbip158-1.4/python-bindings/PyBIP158.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 00:30:37.000000 chikbip158-1.4/python-bindings/PyBIP158.h
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-12 00:30:37.000000 chikbip158-1.4/python-bindings/chikbip158.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:30:42.861832 chikbip158-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-12 00:30:37.000000 chikbip158-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.857832 chikbip158-1.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 00:30:37.000000 chikbip158-1.4/src/amount.h
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 00:30:37.000000 chikbip158-1.4/src/attributes.h
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-12 00:30:37.000000 chikbip158-1.4/src/blockfilter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-12 00:30:37.000000 chikbip158-1.4/src/blockfilter.h
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-12 00:30:37.000000 chikbip158-1.4/src/coins.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.857832 chikbip158-1.4/src/compat/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-12 00:30:37.000000 chikbip158-1.4/src/compat/byteswap.h
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-12 00:30:37.000000 chikbip158-1.4/src/compat/endian.h
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-12 00:30:37.000000 chikbip158-1.4/src/compressor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.857832 chikbip158-1.4/src/consensus/
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-12 00:30:37.000000 chikbip158-1.4/src/consensus/consensus.h
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-12 00:30:37.000000 chikbip158-1.4/src/core_memusage.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.857832 chikbip158-1.4/src/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/chacha20.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/chacha20.h
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/common.h
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/ripemd160.h
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/sha256.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/sha256.h
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/sha512.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/sha512.h
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/siphash.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 00:30:37.000000 chikbip158-1.4/src/crypto/siphash.h
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-12 00:30:37.000000 chikbip158-1.4/src/fs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-12 00:30:37.000000 chikbip158-1.4/src/fs.h
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-12 00:30:37.000000 chikbip158-1.4/src/hash.h
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-12 00:30:37.000000 chikbip158-1.4/src/indirectmap.h
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-12 00:30:37.000000 chikbip158-1.4/src/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-12 00:30:37.000000 chikbip158-1.4/src/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-12 00:30:37.000000 chikbip158-1.4/src/memusage.h
--rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-04-12 00:30:37.000000 chikbip158-1.4/src/prevector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/src/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-12 00:30:37.000000 chikbip158-1.4/src/primitives/block.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-12 00:30:37.000000 chikbip158-1.4/src/primitives/block.h
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-12 00:30:37.000000 chikbip158-1.4/src/primitives/transaction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12213 2024-04-12 00:30:37.000000 chikbip158-1.4/src/primitives/transaction.h
--rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-12 00:30:37.000000 chikbip158-1.4/src/random.cpp.orig
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-12 00:30:37.000000 chikbip158-1.4/src/random.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/src/script/
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-04-12 00:30:37.000000 chikbip158-1.4/src/script/script.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-04-12 00:30:37.000000 chikbip158-1.4/src/script/script.h
--rw-r--r--   0 runner    (1001) docker     (127)    30247 2024-04-12 00:30:37.000000 chikbip158-1.4/src/serialize.h
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-12 00:30:37.000000 chikbip158-1.4/src/span.h
--rw-r--r--   0 runner    (1001) docker     (127)    25702 2024-04-12 00:30:37.000000 chikbip158-1.4/src/streams.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/src/support/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/src/support/allocators/
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-12 00:30:37.000000 chikbip158-1.4/src/support/allocators/secure.h
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 00:30:37.000000 chikbip158-1.4/src/support/allocators/zeroafterfree.h
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 00:30:37.000000 chikbip158-1.4/src/support/cleanse.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 00:30:37.000000 chikbip158-1.4/src/support/cleanse.h
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-04-12 00:30:37.000000 chikbip158-1.4/src/support/lockedpool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-12 00:30:37.000000 chikbip158-1.4/src/support/lockedpool.h
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-12 00:30:37.000000 chikbip158-1.4/src/sync.h
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-12 00:30:37.000000 chikbip158-1.4/src/threadsafety.h
--rw-r--r--   0 runner    (1001) docker     (127)    43685 2024-04-12 00:30:37.000000 chikbip158-1.4/src/tinyformat.h
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-12 00:30:37.000000 chikbip158-1.4/src/uint256.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-12 00:30:37.000000 chikbip158-1.4/src/uint256.h
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-12 00:30:37.000000 chikbip158-1.4/src/undo.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/bytevectorhash.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/bytevectorhash.h
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/strencodings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/strencodings.h
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/threadnames.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/threadnames.h
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/time.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-12 00:30:37.000000 chikbip158-1.4/src/util/time.h
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-12 00:30:37.000000 chikbip158-1.4/src/version.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:42.861832 chikbip158-1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:30:37.000000 chikbip158-1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-12 00:30:37.000000 chikbip158-1.4/tests/simple_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.837514 chikbip158-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.813515 chikbip158-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.817515 chikbip158-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-12 05:44:30.000000 chikbip158-1.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-12 05:44:30.000000 chikbip158-1.5.0/.github/workflows/rust.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 05:44:30.000000 chikbip158-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 05:44:30.000000 chikbip158-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-12 05:44:36.833515 chikbip158-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-12 05:44:30.000000 chikbip158-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.833515 chikbip158-1.5.0/chikbip158.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-12 05:44:36.000000 chikbip158-1.5.0/chikbip158.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-12 05:44:36.000000 chikbip158-1.5.0/chikbip158.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:44:36.000000 chikbip158-1.5.0/chikbip158.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:44:36.000000 chikbip158-1.5.0/chikbip158.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 05:44:36.000000 chikbip158-1.5.0/chikbip158.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-12 05:44:30.000000 chikbip158-1.5.0/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 05:44:30.000000 chikbip158-1.5.0/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-12 05:44:30.000000 chikbip158-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.821514 chikbip158-1.5.0/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-12 05:44:30.000000 chikbip158-1.5.0/python-bindings/PyBIP158.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 05:44:30.000000 chikbip158-1.5.0/python-bindings/PyBIP158.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-12 05:44:30.000000 chikbip158-1.5.0/python-bindings/chikbip158.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.821514 chikbip158-1.5.0/rust-bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    14099 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.821514 chikbip158-1.5.0/rust-bindings/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.821514 chikbip158-1.5.0/rust-bindings/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/fuzz/fuzz_targets/fuzz_filter.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.821514 chikbip158-1.5.0/rust-bindings/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-12 05:44:30.000000 chikbip158-1.5.0/rust-bindings/wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:44:36.837514 chikbip158-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-12 05:44:30.000000 chikbip158-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.829515 chikbip158-1.5.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/amount.h
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/attributes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/blockfilter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/blockfilter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/coins.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.829515 chikbip158-1.5.0/src/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/compat/byteswap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/compat/endian.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/compressor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.829515 chikbip158-1.5.0/src/consensus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/consensus/consensus.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/core_memusage.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.829515 chikbip158-1.5.0/src/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/chacha20.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/chacha20.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/ripemd160.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/sha256.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/sha256.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/sha512.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/sha512.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/siphash.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/crypto/siphash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/fs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/fs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/hash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/indirectmap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/memusage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/prevector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.829515 chikbip158-1.5.0/src/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/primitives/block.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/primitives/block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/primitives/transaction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12213 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/primitives/transaction.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/random.cpp.orig
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/random.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.833515 chikbip158-1.5.0/src/script/
+-rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/script/script.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/script/script.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30247 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/serialize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/span.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25702 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/streams.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.833515 chikbip158-1.5.0/src/support/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.833515 chikbip158-1.5.0/src/support/allocators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/support/allocators/secure.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/support/allocators/zeroafterfree.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/support/cleanse.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/support/cleanse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/support/lockedpool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/support/lockedpool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/sync.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/threadsafety.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43685 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/tinyformat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/uint256.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/uint256.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/undo.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.833515 chikbip158-1.5.0/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/bytevectorhash.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/bytevectorhash.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/strencodings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/strencodings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/threadnames.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/threadnames.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/time.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/util/time.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-12 05:44:30.000000 chikbip158-1.5.0/src/version.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:36.833515 chikbip158-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:44:30.000000 chikbip158-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-12 05:44:30.000000 chikbip158-1.5.0/tests/simple_test.py
```

### Comparing `chikbip158-1.4/.github/workflows/build.yml` & `chikbip158-1.5.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/LICENSE` & `chikbip158-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/PKG-INFO` & `chikbip158-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chikbip158
-Version: 1.4
+Version: 1.5.0
 Summary: Chik BIP158 (wraps C++)
 Home-page: https://github.com/Chik-Network/chikbip158
 Author: Mariano Sorgente
 Author-email: admin@chiknetwork.com
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chikbip158-1.4/README.md` & `chikbip158-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/chikbip158.egg-info/PKG-INFO` & `chikbip158-1.5.0/chikbip158.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chikbip158
-Version: 1.4
+Version: 1.5.0
 Summary: Chik BIP158 (wraps C++)
 Home-page: https://github.com/Chik-Network/chikbip158
 Author: Mariano Sorgente
 Author-email: admin@chiknetwork.com
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chikbip158-1.4/chikbip158.egg-info/SOURCES.txt` & `chikbip158-1.5.0/chikbip158.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,33 @@
 LICENSE
 README.md
 main.cpp
 mypi.ini
 pyproject.toml
 setup.py
 .github/workflows/build.yml
+.github/workflows/rust.yml
 chikbip158.egg-info/PKG-INFO
 chikbip158.egg-info/SOURCES.txt
 chikbip158.egg-info/dependency_links.txt
 chikbip158.egg-info/not-zip-safe
 chikbip158.egg-info/top_level.txt
 python-bindings/PyBIP158.cpp
 python-bindings/PyBIP158.h
 python-bindings/chikbip158.cpp
+rust-bindings/.gitignore
+rust-bindings/Cargo.lock
+rust-bindings/Cargo.toml
+rust-bindings/build.rs
+rust-bindings/wrapper.cpp
+rust-bindings/wrapper.h
+rust-bindings/fuzz/.gitignore
+rust-bindings/fuzz/Cargo.toml
+rust-bindings/fuzz/fuzz_targets/fuzz_filter.rs
+rust-bindings/src/lib.rs
 src/amount.h
 src/attributes.h
 src/blockfilter.cpp
 src/blockfilter.h
 src/coins.h
 src/compressor.h
 src/core_memusage.h
```

### Comparing `chikbip158-1.4/main.cpp` & `chikbip158-1.5.0/main.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/python-bindings/PyBIP158.cpp` & `chikbip158-1.5.0/python-bindings/PyBIP158.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/python-bindings/PyBIP158.h` & `chikbip158-1.5.0/python-bindings/PyBIP158.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/python-bindings/chikbip158.cpp` & `chikbip158-1.5.0/python-bindings/chikbip158.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/setup.py` & `chikbip158-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/amount.h` & `chikbip158-1.5.0/src/amount.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/attributes.h` & `chikbip158-1.5.0/src/attributes.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/blockfilter.cpp` & `chikbip158-1.5.0/src/blockfilter.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/blockfilter.h` & `chikbip158-1.5.0/src/blockfilter.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/coins.h` & `chikbip158-1.5.0/src/coins.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/compat/byteswap.h` & `chikbip158-1.5.0/src/compat/byteswap.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/compat/endian.h` & `chikbip158-1.5.0/src/compat/endian.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/compressor.h` & `chikbip158-1.5.0/src/compressor.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/consensus/consensus.h` & `chikbip158-1.5.0/src/consensus/consensus.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/core_memusage.h` & `chikbip158-1.5.0/src/core_memusage.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/chacha20.cpp` & `chikbip158-1.5.0/src/crypto/chacha20.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/chacha20.h` & `chikbip158-1.5.0/src/crypto/chacha20.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/common.h` & `chikbip158-1.5.0/src/crypto/common.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/ripemd160.h` & `chikbip158-1.5.0/src/crypto/ripemd160.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/sha256.cpp` & `chikbip158-1.5.0/src/crypto/sha256.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/sha256.h` & `chikbip158-1.5.0/src/crypto/sha256.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/sha512.cpp` & `chikbip158-1.5.0/src/crypto/sha512.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/sha512.h` & `chikbip158-1.5.0/src/crypto/sha512.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/siphash.cpp` & `chikbip158-1.5.0/src/crypto/siphash.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/crypto/siphash.h` & `chikbip158-1.5.0/src/crypto/siphash.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/fs.cpp` & `chikbip158-1.5.0/src/fs.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/fs.h` & `chikbip158-1.5.0/src/fs.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/hash.h` & `chikbip158-1.5.0/src/hash.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/indirectmap.h` & `chikbip158-1.5.0/src/indirectmap.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/logging.cpp` & `chikbip158-1.5.0/src/logging.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/logging.h` & `chikbip158-1.5.0/src/logging.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/memusage.h` & `chikbip158-1.5.0/src/memusage.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/prevector.h` & `chikbip158-1.5.0/src/prevector.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/primitives/block.cpp` & `chikbip158-1.5.0/src/primitives/block.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/primitives/block.h` & `chikbip158-1.5.0/src/primitives/block.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/primitives/transaction.cpp` & `chikbip158-1.5.0/src/primitives/transaction.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/primitives/transaction.h` & `chikbip158-1.5.0/src/primitives/transaction.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/random.cpp.orig` & `chikbip158-1.5.0/src/random.cpp.orig`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/random.h` & `chikbip158-1.5.0/src/random.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/script/script.cpp` & `chikbip158-1.5.0/src/script/script.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/script/script.h` & `chikbip158-1.5.0/src/script/script.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/serialize.h` & `chikbip158-1.5.0/src/serialize.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/span.h` & `chikbip158-1.5.0/src/span.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/streams.h` & `chikbip158-1.5.0/src/streams.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/support/allocators/secure.h` & `chikbip158-1.5.0/src/support/allocators/secure.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/support/allocators/zeroafterfree.h` & `chikbip158-1.5.0/src/support/allocators/zeroafterfree.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/support/cleanse.cpp` & `chikbip158-1.5.0/src/support/cleanse.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/support/cleanse.h` & `chikbip158-1.5.0/src/support/cleanse.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/support/lockedpool.cpp` & `chikbip158-1.5.0/src/support/lockedpool.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/support/lockedpool.h` & `chikbip158-1.5.0/src/support/lockedpool.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/sync.h` & `chikbip158-1.5.0/src/sync.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/threadsafety.h` & `chikbip158-1.5.0/src/threadsafety.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/tinyformat.h` & `chikbip158-1.5.0/src/tinyformat.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/uint256.cpp` & `chikbip158-1.5.0/src/uint256.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/uint256.h` & `chikbip158-1.5.0/src/uint256.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/undo.h` & `chikbip158-1.5.0/src/undo.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/bytevectorhash.cpp` & `chikbip158-1.5.0/src/util/bytevectorhash.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/bytevectorhash.h` & `chikbip158-1.5.0/src/util/bytevectorhash.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/strencodings.cpp` & `chikbip158-1.5.0/src/util/strencodings.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/strencodings.h` & `chikbip158-1.5.0/src/util/strencodings.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/threadnames.cpp` & `chikbip158-1.5.0/src/util/threadnames.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/threadnames.h` & `chikbip158-1.5.0/src/util/threadnames.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/time.cpp` & `chikbip158-1.5.0/src/util/time.cpp`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/util/time.h` & `chikbip158-1.5.0/src/util/time.h`

 * *Files identical despite different names*

### Comparing `chikbip158-1.4/src/version.h` & `chikbip158-1.5.0/src/version.h`

 * *Files identical despite different names*

