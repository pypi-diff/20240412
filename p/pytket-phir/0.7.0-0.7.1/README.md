# Comparing `tmp/pytket-phir-0.7.0.tar.gz` & `tmp/pytket_phir-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-phir-0.7.0.tar", last modified: Wed Apr 10 15:52:49 2024, max compression
+gzip compressed data, was "pytket_phir-0.7.1.tar", last modified: Fri Apr 12 17:26:14 2024, max compression
```

## Comparing `pytket-phir-0.7.0.tar` & `pytket_phir-0.7.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/workflows/pre-commit-au.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/pytket.phir.rebasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/pytket.phir.rst
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/docs/source/pytket.phir.sharding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.898992 pytket-phir-0.7.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.906992 pytket-phir-0.7.0/pytket/phir/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/phirgen_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/place_and_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/qtm_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.906992 pytket-phir-0.7.0/pytket/phir/rebasing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/rebasing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/rebasing/rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.906992 pytket-phir-0.7.0/pytket/phir/sharding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/shard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/pytket/phir/sharding/shards2ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/pytket_phir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 15:52:49.000000 pytket-phir-0.7.0/pytket_phir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.910992 pytket-phir-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.902992 pytket-phir-0.7.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/tests/data/qasm/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/arbitrary_qreg_names.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/baby.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/baby_with_rollup.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/barrier_complex.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/big_gate.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/bv_n10.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/classical_hazards.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/classical_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/cond_1.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/cond_barrier.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/cond_classical.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/exec_order_two_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/eztest.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/group_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/n10_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/oned_brickwork_circuit_n20.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/parallelization_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/qv20_0.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/rxrz.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/rz_exec_order_three_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/simple.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/simple_cond.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/single_qubit_parallel_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/sleep.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/tk2_diff_angles.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/qasm/tk2_same_angle.qasm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 15:52:49.914992 pytket-phir-0.7.0/tests/data/wasm/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/wasm/add.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/data/wasm/testfile.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/e2e_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_parallel_tk2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_parallelization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-10 15:52:44.000000 pytket-phir-0.7.0/tests/test_wasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/workflows/pre-commit-au.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/pytket.phir.rebasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/pytket.phir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/docs/source/pytket.phir.sharding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.669458 pytket_phir-0.7.1/pytket/phir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/phirgen_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/place_and_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/qtm_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.673458 pytket_phir-0.7.1/pytket/phir/rebasing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/rebasing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/rebasing/rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.673458 pytket_phir-0.7.1/pytket/phir/sharding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/shard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/pytket/phir/sharding/shards2ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/pytket_phir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 17:26:14.000000 pytket_phir-0.7.1/pytket_phir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.673458 pytket_phir-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.665458 pytket_phir-0.7.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/tests/data/qasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/arbitrary_qreg_names.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/baby.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/baby_with_rollup.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/barrier_complex.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/big_gate.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/bv_n10.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/classical_hazards.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/classical_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/cond_1.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/cond_barrier.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/cond_classical.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/exec_order_two_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/eztest.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/group_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/n10_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/oned_brickwork_circuit_n20.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/parallelization_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/qv20_0.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/rxrz.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/rz_exec_order_three_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/simple.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/simple_cond.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/single_qubit_parallel_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/sleep.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/tk2_diff_angles.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/qasm/tk2_same_angle.qasm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:14.681458 pytket_phir-0.7.1/tests/data/wasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/wasm/add.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/data/wasm/testfile.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_parallel_tk2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_parallelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-12 17:26:09.000000 pytket_phir-0.7.1/tests/test_wasm.py
```

### Comparing `pytket-phir-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pytket_phir-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/.github/pull_request_template.md` & `pytket_phir-0.7.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/.github/workflows/pre-commit-au.yml` & `pytket_phir-0.7.1/.github/workflows/pre-commit-au.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/.github/workflows/python-app.yml` & `pytket_phir-0.7.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/.github/workflows/python-publish.yml` & `pytket_phir-0.7.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/.gitignore` & `pytket_phir-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/CHANGELOG.md` & `pytket_phir-0.7.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/LICENSE` & `pytket_phir-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/PKG-INFO` & `pytket_phir-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.7.0
+Version: 0.7.1
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket-phir-0.7.0/README.md` & `pytket_phir-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/docs/Makefile` & `pytket_phir-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/docs/source/conf.py` & `pytket_phir-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/docs/source/index.rst` & `pytket_phir-0.7.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/docs/source/pytket.phir.rst` & `pytket_phir-0.7.1/docs/source/pytket.phir.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/docs/source/pytket.phir.sharding.rst` & `pytket_phir-0.7.1/docs/source/pytket.phir.sharding.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pyproject.toml` & `pytket_phir-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/api.py` & `pytket_phir-0.7.1/pytket/phir/api.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/cli.py` & `pytket_phir-0.7.1/pytket/phir/cli.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/machine.py` & `pytket_phir-0.7.1/pytket/phir/machine.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/phirgen.py` & `pytket_phir-0.7.1/pytket/phir/phirgen.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/phirgen_parallel.py` & `pytket_phir-0.7.1/pytket/phir/phirgen_parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,41 +276,39 @@
         else:
             fmt_g2q: dict[int, list[tk.Command]] = {0: []}
             for shard in group:
                 fmt_g2q[0].append(shard.primary_command)
             groups2qops(fmt_g2q, ops)
 
 
+def get_transport_time_for_gate(gate: str, machine: "Machine") -> float:
+    """Return the transport time on the machine for the given gate type."""
+    match gate:
+        case "RZ" | "R1XY":
+            return machine.sq_time
+        case "RZZ":
+            return machine.tq_time
+        case "Measure":
+            return machine.meas_prep_time
+        case "Init":
+            return 0
+        case _:
+            logger.warning("Gate type %s not assigned a transport duration", gate)
+            return 0
+
+
 def adjust_phir_transport_time(ops: list["JsonDict"], machine: "Machine") -> None:
     """Analyze the generated phir and adjust the transport time."""
     adjustment = 0.0
     for op in ops:
         if "qop" in op:
-            match op["qop"]:
-                case "RZ" | "R1XY":
-                    adjustment += machine.sq_time
-                case "RZZ":
-                    adjustment += machine.tq_time
-                case "Measure":
-                    adjustment += machine.meas_prep_time
-                case _:
-                    logger.warning(
-                        "Gate type %s not assigned a transport duration", op["qop"]
-                    )
+            adjustment += get_transport_time_for_gate(op["qop"], machine)
         if "block" in op and op["block"] == "qparallel":
             first_op = op["ops"][0]["qop"]
-            match first_op:
-                case "RZ" | "R1XY":
-                    adjustment += machine.sq_time
-                case "RZZ":
-                    adjustment += machine.tq_time
-                case _:
-                    logger.warning(
-                        "Gate type %s not assigned a transport duration", first_op
-                    )
+            adjustment += get_transport_time_for_gate(first_op, machine)
         if "mop" in op and op["mop"] == "Transport":
             cost, units = op["duration"]
             op["duration"] = cost + adjustment, units
             adjustment = 0.0
 
 
 def genphir_parallel(
```

### Comparing `pytket-phir-0.7.0/pytket/phir/place_and_route.py` & `pytket_phir-0.7.1/pytket/phir/place_and_route.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/placement.py` & `pytket_phir-0.7.1/pytket/phir/placement.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/qtm_machine.py` & `pytket_phir-0.7.1/pytket/phir/qtm_machine.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/rebasing/rebaser.py` & `pytket_phir-0.7.1/pytket/phir/rebasing/rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/routing.py` & `pytket_phir-0.7.1/pytket/phir/routing.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/sharding/shard.py` & `pytket_phir-0.7.1/pytket/phir/sharding/shard.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/sharding/sharder.py` & `pytket_phir-0.7.1/pytket/phir/sharding/sharder.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket/phir/sharding/shards2ops.py` & `pytket_phir-0.7.1/pytket/phir/sharding/shards2ops.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/pytket_phir.egg-info/PKG-INFO` & `pytket_phir-0.7.1/pytket_phir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.7.0
+Version: 0.7.1
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket-phir-0.7.0/pytket_phir.egg-info/SOURCES.txt` & `pytket_phir-0.7.1/pytket_phir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/data/qasm/arbitrary_qreg_names.qasm` & `pytket_phir-0.7.1/tests/data/qasm/arbitrary_qreg_names.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/data/qasm/bv_n10.qasm` & `pytket_phir-0.7.1/tests/data/qasm/bv_n10.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/data/qasm/oned_brickwork_circuit_n20.qasm` & `pytket_phir-0.7.1/tests/data/qasm/oned_brickwork_circuit_n20.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/data/qasm/qv20_0.qasm` & `pytket_phir-0.7.1/tests/data/qasm/qv20_0.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/data/wasm/add.wat` & `pytket_phir-0.7.1/tests/data/wasm/add.wat`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/data/wasm/testfile.wat` & `pytket_phir-0.7.1/tests/data/wasm/testfile.wat`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/e2e_test.py` & `pytket_phir-0.7.1/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_api.py` & `pytket_phir-0.7.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_parallel_tk2.py` & `pytket_phir-0.7.1/tests/test_parallel_tk2.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_parallelization.py` & `pytket_phir-0.7.1/tests/test_parallelization.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_phirgen.py` & `pytket_phir-0.7.1/tests/test_phirgen.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_placement.py` & `pytket_phir-0.7.1/tests/test_placement.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_rebaser.py` & `pytket_phir-0.7.1/tests/test_rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_sharder.py` & `pytket_phir-0.7.1/tests/test_sharder.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_utils.py` & `pytket_phir-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.7.0/tests/test_wasm.py` & `pytket_phir-0.7.1/tests/test_wasm.py`

 * *Files identical despite different names*

