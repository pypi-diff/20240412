# Comparing `tmp/cmeel_mim_solvers-0.0.2.tar.gz` & `tmp/cmeel_mim_solvers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmeel_mim_solvers-0.0.2.tar", last modified: Sun Dec 10 15:06:38 2023, max compression
+gzip compressed data, was "cmeel_mim_solvers-0.0.4.tar", last modified: Fri Apr 12 08:53:49 2024, max compression
```

## Comparing `cmeel_mim_solvers-0.0.2.tar` & `cmeel_mim_solvers-0.0.4.tar`

### file list

```diff
@@ -1,411 +1,427 @@
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/examples/humanoid_taichi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/examples/solo12.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/examples/ur5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/examples/utils_solo12.py
--rw-r--r--   0 runner    (1001) docker     (127)    13365 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/include/mim_solvers/csqp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/include/mim_solvers/csqp_proxqp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15056 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/include/mim_solvers/ddp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/include/mim_solvers/fddp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/include/mim_solvers/kkt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/include/mim_solvers/python.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/include/mim_solvers/sqp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/package.xml
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2023-12-10 15:06:14.238013 cmeel_mim_solvers-0.0.2/python/csqp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/csqp_proxqp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/ddp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/fddp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/mim_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/py_mim_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/py_mim_solvers/sqp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/python/sqp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    35325 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/src/csqp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17079 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/src/csqp_proxqp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19115 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/src/ddp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12581 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/src/fddp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11814 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/src/kkt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/src/sqp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/action.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/action.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/activation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/activation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/cost.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/cost.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/impulse.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/impulse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/pinocchio_model.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/pinocchio_model.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/state.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/state.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/factory/solver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/python/problems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/python/sqp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/random_generator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8326 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/test_solvers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/test_sqp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2023-12-10 15:06:14.242013 cmeel_mim_solvers-0.0.2/tests/unittest_common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.cmake-format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/_static/css/cmake.css
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/cmake.py
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/examples/minimal-hpp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/examples/minimal-with-packages.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/examples/minimal.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/pages/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/pages/cmake-packages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/pages/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/pages/developers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/pages/internal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/pages/other.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.docs/pages/projects.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-10 15:06:14.926027 cmeel_mim_solvers-0.0.2/cmake/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    14705 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/GNUInstallDirs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/catkin/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/cpp/include/jrl_cmakemodule/lib.hh
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/cpp/src/lib.cc
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/cpp/src/main.cc
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/dependency/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/macros.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/python/jrl_cmakemodule/python.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1583 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/run_unit_tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/_unittests/test_pkg-config.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)    15895 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/announce-gen
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/apple.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    13301 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/base.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/boost.cmake
--rw-r--r--   0 runner    (1001) docker     (127)   116712 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/boost/FindBoost.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/catkin.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cmake_reinstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/compiler.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/componentConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/config.h.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/config.hh.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/coverage.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cpack.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/createshexe.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cxx-standard.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cxx11.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    32130 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/cython.cmake
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/dummy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    67009 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython/Support.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython2.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython3.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/python/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/cython/setup.in.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/debian.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/deprecated.hh.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/dist.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/distcheck.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    26500 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/doxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    60572 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/MathJax.js
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2023-12-10 15:06:14.930027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/CHTML-preview.js
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/FontWarnings.js
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/HelpDialog.js
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MatchWebFonts.js
--rw-r--r--   0 runner    (1001) docker     (127)    10346 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MathEvents.js
--rw-r--r--   0 runner    (1001) docker     (127)    30140 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MathMenu.js
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MathZoom.js
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/Safe.js
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/AMScd.js
--rw-r--r--   0 runner    (1001) docker     (127)    13886 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/AMSmath.js
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/AMSsymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/HTML.js
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/action.js
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/autobold.js
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/autoload-all.js
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/bbox.js
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/begingroup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/boldsymbol.js
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/cancel.js
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/color.js
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/enclose.js
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/extpfeil.js
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/mathchoice.js
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/mediawiki-texvc.js
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/mhchem.js
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/newcommand.js
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/noErrors.js
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/noUndefined.js
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/unicode.js
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/verb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/jsMath2jax.js
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/tex2jax.js
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/toMathML.js
--rw-r--r--   0 runner    (1001) docker     (127)    38722 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/jax.js
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/Arrows.js
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiactForSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/Dingbats.js
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/GeneralPunctuation.js
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/GeometricShapes.js
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/GreekAndCoptic.js
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/Latin1Supplement.js
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/LetterlikeSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsA.js
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsB.js
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscSymbolsAndArrows.js
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscTechnical.js
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SpacingModLetters.js
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SuppMathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsA.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsB.js
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/AsciiMath/config.js
--rw-r--r--   0 runner    (1001) docker     (127)    32187 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/AsciiMath/jax.js
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/config.js
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/a.js
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/fr.js
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/g.js
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/h.js
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/i.js
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/j.js
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/k.js
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/l.js
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/m.js
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2023-12-10 15:06:14.934027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/n.js
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/o.js
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/opf.js
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/p.js
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/q.js
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/r.js
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/s.js
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/scr.js
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/t.js
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/u.js
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/v.js
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/w.js
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/x.js
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/y.js
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/z.js
--rw-r--r--   0 runner    (1001) docker     (127)    16140 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/jax.js
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/TeX/config.js
--rw-r--r--   0 runner    (1001) docker     (127)    51329 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/TeX/jax.js
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/CommonHTML/config.js
--rw-r--r--   0 runner    (1001) docker     (127)    25209 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/CommonHTML/jax.js
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/annotation-xml.js
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/maction.js
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/menclose.js
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/mglyph.js
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/mmultiscripts.js
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/ms.js
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/mtable.js
--rw-r--r--   0 runner    (1001) docker     (127)    11876 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/multiline.js
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/config.js
--rw-r--r--   0 runner    (1001) docker     (127)    19232 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Arrows.js
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/BoxDrawing.js
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Dingbats.js
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/EnclosedAlphanum.js
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeneralPunctuation.js
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeometricShapes.js
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GreekAndCoptic.js
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Latin1Supplement.js
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LatinExtendedA.js
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LetterlikeSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)    24217 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    55608 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscMathSymbolsB.js
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscTechnical.js
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/PUA.js
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SpacingModLetters.js
--rw-r--r--   0 runner    (1001) docker     (127)    18287 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SuppMathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)    22630 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Bold/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2023-12-10 15:06:14.938027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    50076 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Other.js
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/PUA.js
--rw-r--r--   0 runner    (1001) docker     (127)    48363 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Other.js
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/PUA.js
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Arrows.js
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiactForSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeneralPunctuation.js
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeometricShapes.js
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GreekAndCoptic.js
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Latin1Supplement.js
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedA.js
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedB.js
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LetterlikeSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)    21842 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    27365 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscMathSymbolsA.js
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscTechnical.js
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SpacingModLetters.js
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SuppMathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SupplementalArrowsA.js
--rw-r--r--   0 runner    (1001) docker     (127)    49033 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GeneralPunctuation.js
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GreekAndCoptic.js
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedA.js
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedB.js
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LetterlikeSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/MathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)    19906 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GeometricShapes.js
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GreekAndCoptic.js
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedA.js
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedB.js
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LetterlikeSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)    73127 2023-12-10 15:06:14.942027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MiscSymbols.js
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SpacingModLetters.js
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SuppMathOperators.js
--rw-r--r--   0 runner    (1001) docker     (127)    58711 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/BoldItalic/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    58962 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/Italic/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    36852 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Other.js
--rw-r--r--   0 runner    (1001) docker     (127)    30362 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Other.js
--rw-r--r--   0 runner    (1001) docker     (127)    24036 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Other.js
--rw-r--r--   0 runner    (1001) docker     (127)    28343 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    17011 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size1/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    15579 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size2/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size3/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size4/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)    43719 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/BasicLatin.js
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/CombDiacritMarks.js
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Main.js
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Other.js
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2023-12-10 15:06:14.946027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata-extra.js
--rw-r--r--   0 runner    (1001) docker     (127)   143390 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata.js
--rw-r--r--   0 runner    (1001) docker     (127)    51498 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/jax.js
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/doxyfile.awk
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/doxygen.css
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/header-mathjax.html
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/header.tex
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/style.rtf
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/style.tex
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/doxygen/tabs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/dynamic_graph/python-module-py.cc.in
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/dynamic_graph/submodule/__init__.py.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/filefilter.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/CDD/FindCDD.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/CLP/FindCLP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/CoinUtils/FindCoinUtils.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/CppAD/Findcppad.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/CppAD/Findcppadcg.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/GMP/FindGMP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/Julia/FindJulia.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/MPFR/FindMPFR.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    29304 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/OpenMP/FindOpenMP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/OpenRTM/FindOpenRTM.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/Qhull/FindQhull.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/Simde/FindSimde.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/TinyXML/FindTinyXML.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/assimp/Findassimp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/glpk/Findglpk.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/find-external/qpOASES/FindqpOASES.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/fix-license.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/geometric-tools.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)    20530 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/git-archive-all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8237 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/git-archive-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     9164 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/github/update-doxygen-doc.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    13416 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/gitlog-to-changelog
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/gtest.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/gtest/CMakeLists.txt.in
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/header.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/hpp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/hpp/doc.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/hpp/doc/layout.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/hpp/idl/omniidl_be_python_with_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/ide.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/idl.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/idlrtc.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/image/visp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-10 15:06:14.950027 cmeel_mim_solvers-0.0.2/cmake/install-data.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/julia.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/kineo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/lapack.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/logging.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/man.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/memorycheck_unit_test.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/metapodfromurdf.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/modernize-links.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/msvc-specific.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/msvc.vcxproj.user.in
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/openhrp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/openhrpcontroller.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/openrtm.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/oscheck.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/package-config.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    41205 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/pkg-config.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/pkg-config.pc.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/portability.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/post-project.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/pthread.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)      826 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/python-helpers.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    19271 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/python.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/qhull.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/release.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/relpath.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/ros.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/sdformat.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/shared-library.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/sphinx.cmake
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/sphinx/conf.py.in
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/sphinx/index.rst.in
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/stubgen/CMakeLists.txt.in
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/stubs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/swig.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/test.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/uninstall.cmake
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/version-script-test.lds
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/version-script.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    10185 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/version.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/warning.hh.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2023-12-10 15:06:14.954028 cmeel_mim_solvers-0.0.2/cmake/xacro.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2023-12-10 15:06:38.134354 cmeel_mim_solvers-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/benchmarks/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/benchmarks/solo12.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/benchmarks/timings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-12 08:53:22.851685 cmeel_mim_solvers-0.0.4/benchmarks/timings.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/benchmarks/ur5.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/csqp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/csqp_proxqp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/ddp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/fddp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/mim_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/bindings/sqp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/examples/humanoid_taichi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/examples/solo12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/examples/ur5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/examples/utils_solo12.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/include/mim_solvers/csqp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/include/mim_solvers/csqp_proxqp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/include/mim_solvers/ddp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/include/mim_solvers/fddp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/include/mim_solvers/kkt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/include/mim_solvers/python.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/include/mim_solvers/sqp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/package.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/csqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/qp_solvers/py_osqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/qp_solvers/qpsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20063 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/qp_solvers/stagewise_qp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/qp_solvers/stagewise_qp_kkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/sqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/python/sqp_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39636 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/src/csqp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17969 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/src/csqp_proxqp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/src/ddp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/src/fddp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/src/kkt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 08:53:22.855685 cmeel_mim_solvers-0.0.4/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/src/sqp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/constraints.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/constraints.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/model.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/point-mass.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/point-mass.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/problem.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/factory/solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/Testing/Temporary/CTestCostData.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_clqr_convergence_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_clqr_osqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_clqr_stagewise_admm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_lqr_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_sqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_sqp_taichi_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_sqp_ur5_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/python/test_ur5_csqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/random_generator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/test_solvers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 08:53:22.859685 cmeel_mim_solvers-0.0.4/tests/unittest_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.cmake-format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/_static/css/cmake.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/cmake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/examples/minimal-hpp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/examples/minimal-with-packages.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/examples/minimal.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/pages/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/pages/cmake-packages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/pages/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/pages/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/pages/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/pages/other.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.docs/pages/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-12 08:53:24.827683 cmeel_mim_solvers-0.0.4/cmake/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/GNUInstallDirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/catkin/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/cpp/include/jrl_cmakemodule/lib.hh
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/cpp/src/lib.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/cpp/src/main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/dependency/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/macros.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/python/jrl_cmakemodule/python.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1583 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/run_unit_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/_unittests/test_pkg-config.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15895 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/announce-gen
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/apple.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/base.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/boost.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)   116712 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/boost/FindBoost.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/catkin.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cmake_reinstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/compiler.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/componentConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/config.h.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/config.hh.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/coverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cpack.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/createshexe.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cxx-standard.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cxx11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    32130 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/cython.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/dummy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    67009 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython/Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython2.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython3.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/python/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/cython/setup.in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/debian.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/deprecated.hh.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/dist.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/distcheck.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    26500 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/doxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    60572 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/MathJax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-12 08:53:24.831683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/CHTML-preview.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/FontWarnings.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/HelpDialog.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MatchWebFonts.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MathEvents.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MathMenu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MathZoom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/Safe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/AMScd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13886 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/AMSmath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/AMSsymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/HTML.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/action.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/autobold.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/autoload-all.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/bbox.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/begingroup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/boldsymbol.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/cancel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/color.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/enclose.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/extpfeil.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/mathchoice.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/mediawiki-texvc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/mhchem.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/newcommand.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/noErrors.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/noUndefined.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/unicode.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/verb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/jsMath2jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/tex2jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/toMathML.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38722 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/Arrows.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiactForSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/Dingbats.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/GeneralPunctuation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/GeometricShapes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/GreekAndCoptic.js
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/Latin1Supplement.js
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/LetterlikeSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsB.js
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscSymbolsAndArrows.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscTechnical.js
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SpacingModLetters.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SuppMathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/AsciiMath/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32187 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/AsciiMath/jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/g.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/h.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/i.js
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/j.js
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/k.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/l.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/m.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/n.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 08:53:24.835683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/o.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/opf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/p.js
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/q.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/r.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/s.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/scr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/t.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/u.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/v.js
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/w.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/x.js
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/y.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/z.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/TeX/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51329 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/TeX/jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/CommonHTML/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25209 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/CommonHTML/jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/annotation-xml.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/maction.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/menclose.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/mglyph.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/mmultiscripts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/ms.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/mtable.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/multiline.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/config.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19232 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Arrows.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/BoxDrawing.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Dingbats.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/EnclosedAlphanum.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeneralPunctuation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeometricShapes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GreekAndCoptic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Latin1Supplement.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LatinExtendedA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LetterlikeSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24217 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscMathSymbolsB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscTechnical.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/PUA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SpacingModLetters.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18287 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SuppMathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22630 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Bold/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-12 08:53:24.839683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50076 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Other.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/PUA.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48363 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Other.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/PUA.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Arrows.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiactForSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeneralPunctuation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeometricShapes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GreekAndCoptic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Latin1Supplement.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LetterlikeSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21842 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27365 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscMathSymbolsA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscTechnical.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SpacingModLetters.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SuppMathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SupplementalArrowsA.js
+-rw-r--r--   0 runner    (1001) docker     (127)    49033 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GeneralPunctuation.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GreekAndCoptic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LetterlikeSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/MathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19906 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GeometricShapes.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GreekAndCoptic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedA.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedB.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LetterlikeSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73127 2024-04-12 08:53:24.843683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MiscSymbols.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SpacingModLetters.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SuppMathOperators.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58711 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/BoldItalic/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58962 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/Italic/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36852 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Other.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30362 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Other.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Other.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28343 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size1/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15579 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size2/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size3/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size4/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    43719 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/BasicLatin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/CombDiacritMarks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Other.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-12 08:53:24.847683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata-extra.js
+-rw-r--r--   0 runner    (1001) docker     (127)   143390 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51498 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/jax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/doxyfile.awk
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/doxygen.css
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/header-mathjax.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/header.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/style.rtf
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/style.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/doxygen/tabs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/dynamic_graph/python-module-py.cc.in
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/dynamic_graph/submodule/__init__.py.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/filefilter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/CDD/FindCDD.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/CLP/FindCLP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/CoinUtils/FindCoinUtils.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/CppAD/Findcppad.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/CppAD/Findcppadcg.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/GMP/FindGMP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/Julia/FindJulia.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/MPFR/FindMPFR.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    29304 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/OpenMP/FindOpenMP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/OpenRTM/FindOpenRTM.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/Qhull/FindQhull.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/Simde/FindSimde.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/TinyXML/FindTinyXML.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/assimp/Findassimp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/glpk/Findglpk.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/find-external/qpOASES/FindqpOASES.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1394 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/fix-license.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/geometric-tools.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20530 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/git-archive-all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8237 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/git-archive-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9164 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/github/update-doxygen-doc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13416 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/gitlog-to-changelog
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/gtest.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/gtest/CMakeLists.txt.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/header.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/hpp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/hpp/doc.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/hpp/doc/layout.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/hpp/idl/omniidl_be_python_with_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/ide.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/idl.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/idlrtc.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/image/visp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/install-data.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/julia.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/kineo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/lapack.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-12 08:53:24.851683 cmeel_mim_solvers-0.0.4/cmake/logging.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/man.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/memorycheck_unit_test.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/metapodfromurdf.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/modernize-links.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/msvc-specific.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/msvc.vcxproj.user.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/openhrp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/openhrpcontroller.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/openrtm.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/oscheck.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/package-config.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    41205 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/pkg-config.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/pkg-config.pc.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/portability.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/post-project.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/pthread.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/python-helpers.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    19271 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/python.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/qhull.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/release.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/relpath.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/ros.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/sdformat.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/shared-library.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/sphinx.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/sphinx/conf.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/sphinx/index.rst.in
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/stubgen/CMakeLists.txt.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/stubs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/swig.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/test.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/uninstall.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/version-script-test.lds
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/version-script.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/version.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/warning.hh.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-12 08:53:24.855683 cmeel_mim_solvers-0.0.4/cmake/xacro.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-12 08:53:49.311652 cmeel_mim_solvers-0.0.4/PKG-INFO
```

### Comparing `cmeel_mim_solvers-0.0.2/.github/workflows/release.yml` & `cmeel_mim_solvers-0.0.4/.github/workflows/release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,75 +12,82 @@
 
 env:
   CMEEL_LOG_LEVEL: DEBUG
 
 jobs:
   wheel:
     name: "${{ matrix.build }} ${{ matrix.os }} ${{ matrix.arch }}"
-    runs-on: "${{ matrix.os }}"
+    runs-on: "${{ matrix.os }}-latest"
     strategy:
       matrix:
-        os: ["ubuntu-latest"] # no OpenMP yet, "macos-latest"]
+        os: ["ubuntu"] # no OpenMP yet, "macos"]
         arch: ["x86_64", "aarch64"]
-        build: ["cp38-*", "cp39-*", "cp310-*", "cp311-*"] # proxsuite is not ready for 3.12
+        build: ["cp38", "cp39", "cp310", "cp311"] # proxsuite is not ready for 3.12
         exclude:
-          - os: "macos-latest"
+          - os: "macos"
             arch: "aarch64"
     steps:
       - uses: actions/checkout@v4
         with:
           submodules: 'true'
       - name: Set up QEMU
         if: matrix.arch == 'aarch64'
         uses: docker/setup-qemu-action@v3
         with:
           platforms: all
       - run: pipx install cibuildwheel
       - run: cibuildwheel --output-dir wh
         env:
-          CIBW_BUILD: ${{ matrix.build }}
-          CIBW_ARCHS: ${{ matrix.arch }}
+          CIBW_BUILD: "${{ matrix.build }}-*"
+          CIBW_ARCHS: "${{ matrix.arch }}"
           CIBW_SKIP: "*musllinux*"
           CIBW_MANYLINUX_X86_64_IMAGE: "quay.io/pypa/manylinux_2_28_x86_64"
           CIBW_MANYLINUX_AARCH64_IMAGE: "quay.io/pypa/manylinux_2_28_aarch64"
           CIBW_REPAIR_WHEEL_COMMAND: ""
-          CIBW_ENVIRONMENT: CMEEL_LOG_LEVEL="DEBUG" CMEEL_JOBS="1" CMEEL_TEST_JOBS="1" CMEEL_RUN_TESTS="false"
-      - uses: actions/upload-artifact@v3
+          CIBW_ENVIRONMENT: CMEEL_LOG_LEVEL="DEBUG" CMEEL_JOBS="1" CMEEL_RUN_TESTS="false"
+      - uses: actions/upload-artifact@v4
         with:
-          path: wh
+          name: "artifact-${{ matrix.os }}-${{ matrix.arch }}-${{ matrix.build }}"
+          path: wh/cmeel_mim_solvers*
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           submodules: 'true'
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.11
       - name: setup
         run: |
           python -m pip install -U pip
           python -m pip install build cmeel[build] crocoddyl[build] proxsuite[build] cmeel-boost
       - name: build sdist
         run: python -m build -nso dist .
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           path: dist
 
   release:
     needs: ["wheel", "sdist"]
     if: ${{ startsWith(github.ref, 'refs/tags/v') }}
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
+      contents: write
     steps:
       - uses: actions/checkout@v4
         with:
           ref: ${{ github.ref_name }}
       - run: curl https://github.com/nim65s.gpg | gpg --import
       - name: validate signature
         run: >
           git verify-tag --raw ${{ github.ref_name }} 2>&1
           | grep -q 'VALIDSIG 9B1A79065D2F2B806C8A5A1C7D2ACDAF4653CF28'
-      - uses: actions/download-artifact@v3
-      - run: pipx install twine
-      - run: twine upload -u __token__ -p "${{ secrets.PYPI_TOKEN }}" artifact/cmeel_mim_solvers*.whl
-      - run: twine upload -u __token__ -p "${{ secrets.PYPI_TOKEN }}" artifact/cmeel_mim_solvers*.tar.gz || true
+      - uses: actions/download-artifact@v4
+      - run: mkdir dist && mv artifact*/* dist
+      - name: Publish package distributions to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          skip-existing: true
```

### Comparing `cmeel_mim_solvers-0.0.2/.gitignore` & `cmeel_mim_solvers-0.0.4/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+*.data
 *.vscode
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `cmeel_mim_solvers-0.0.2/LICENSE` & `cmeel_mim_solvers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/README.md` & `cmeel_mim_solvers-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # mim_solvers
-Implementation of numerical solvers used in the Machines in Motion Laboratory. 
-In particular, the Sequential Quadratic Programming (SQP) solver described in [this paper](https://laas.hal.science/hal-04330251) solves nonlinear constrained OCPs efficiently.
+Implementation of efficient numerical optimal control solvers. 
+In particular, the Sequential Quadratic Programming (SQP) solver described in [this paper](https://laas.hal.science/hal-04330251) solves nonlinear constrained OCPs efficiently by leveraging sparsity.
 
-All solvers are implemented by using [Crocoddyl](https://github.com/loco-3d/crocoddyl/tree/devel) (v2.0) as the base software. 
-Consequently, Crocoddyl users can use our efficient solvers while constructing their OCPs using the same API they are used to. 
-The default solvers of Crocoddyl are also re-implemented for benchmarking purposes (namely DDP and FDDP) but with modified termination criteria and line-search.
+All the solvers are implemented based on the API of [Crocoddyl](https://github.com/loco-3d/crocoddyl/tree/devel) (v2). 
+In other words, our solvers take as input a `crocoddyl.ShootingProblem`.
 
 Examples on how to use the solvers can be found in the `examples` directory.
 
 # Dependencies
 - [Pinocchio](https://github.com/stack-of-tasks/pinocchio) (rigid-body dynamics computations)
 - [Crocoddyl](https://github.com/loco-3d/crocoddyl) (optimal control library)
-- [ProxSuite](https://github.com/Simple-Robotics/proxsuite) (quadratic programming) [OPTIONAL]
+- [ProxSuite](https://github.com/Simple-Robotics/proxsuite) (quadratic programming) (optional)
 
 # Installation
 
   ## Using conda
 
 `conda install mim-solvers --channel conda-forge`
 
@@ -25,18 +24,21 @@
 
 `cd mim_solvers && mkdir build && cd build`
 
 `cmake .. [-DCMAKE_BUILD_TYPE=Release] [-DCMAKE_INSTALL_PREFIX=...]`
 
 `make [-j6] && make install`
 
+You can also run unittests using `ctest -v` and benchmarks using `./benchmarks/ur5` or `./benchmarks/solo12` from the build directory.
+
 
 # Contributors
 
 -   [Armand Jordana](https://github.com/ajordana) (NYU): main developer and manager of the project
 -   [Sébastien Kleff](https://github.com/skleff1994) (NYU): main developer and manager of the project
 -   [Avadesh Meduri](https://github.com/avadesh02) (NYU): main developer and manager of the project
 -   [Ludovic Righetti](https://engineering.nyu.edu/faculty/ludovic-righetti) (NYU): project instructor
 -   [Justin Carpentier](https://jcarpent.github.io) (INRIA): project instructor
 -   [Nicolas Mansard](http://projects.laas.fr/gepetto/index.php/Members/NicolasMansard) (LAAS-CNRS): project instructor
 -   [Yann de Mont-Marin](https://github.com/ymontmarin) (INRIA): Conda integration and support
-
+-   [Louis Montaut](https://github.com/lmontaut) (INRIA): CMake support
+-   [Guilhem Saurel](https://github.com/nim65s) (LAAS-CNRS): CMake & pip packaging support
```

### Comparing `cmeel_mim_solvers-0.0.2/examples/humanoid_taichi.py` & `cmeel_mim_solvers-0.0.4/examples/humanoid_taichi.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/examples/solo12.py` & `cmeel_mim_solvers-0.0.4/examples/solo12.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/examples/ur5.py` & `cmeel_mim_solvers-0.0.4/examples/ur5.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/examples/utils_solo12.py` & `cmeel_mim_solvers-0.0.4/examples/utils_solo12.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/include/mim_solvers/csqp.hpp` & `cmeel_mim_solvers-0.0.4/include/mim_solvers/csqp.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -59,15 +59,15 @@
    * @param[in] problem  shooting problem
    */
   explicit SolverCSQP(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
   virtual ~SolverCSQP();
 
   virtual bool solve(const std::vector<Eigen::VectorXd>& init_xs = crocoddyl::DEFAULT_VECTOR,
                      const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR, const std::size_t maxiter = 100,
-                     const bool is_feasible = false, const double regInit = 1e-9);
+                     const bool is_feasible = false, const double regInit = NAN);
 
   /**
    * @copybrief SolverAbstract::expectedImprovement
    *
    * This function requires to first run `updateExpectedImprovement()`. The expected improvement computation considers
    * the gaps in the dynamics: \f{equation} \Delta J(\alpha) = \Delta_1\alpha + \frac{1}{2}\Delta_2\alpha^2, \f} with
    * \f{eqnarray}
@@ -80,15 +80,16 @@
   // virtual const Eigen::Vector2d& expectedImprovement();
 
   /**
    * @brief Update internal values for computing the expected improvement
    */
   void updateExpectedImprovement();
 
-  virtual void forwardPass();
+  virtual void forwardPass(const double stepLength=0);
+  virtual void forwardPass_without_constraints();
   virtual void backwardPass();
   virtual void backwardPass_without_rho_update();
   virtual void backwardPass_without_constraints();
 
   /**
    * @brief Computes the merit function, gaps at the given xs, us along with delta x and delta u
    */
@@ -96,14 +97,16 @@
 
   virtual double tryStep(const double stepLength);
 
   virtual void calc(const bool recalc = true);
 
   virtual void reset_params();
 
+  virtual void reset_rho_vec();
+
   // virtual void set_constraints(const std::vector<boost::shared_ptr<ConstraintModelAbstract>>& constraint_models){
   //   constraint_models_ = constraint_models;
   // };
 
   /**
    * @brief Compute the KKT conditions residual
    */
@@ -128,62 +131,78 @@
   double get_KKT() const { return KKT_; };
   double get_gap_norm() const { return gap_norm_; };
   double get_constraint_norm() const { return constraint_norm_; };
   double get_qp_iters() const { return qp_iters_; };
   double get_xgrad_norm() const { return x_grad_norm_; };
   double get_ugrad_norm() const { return u_grad_norm_; };
   double get_merit() const { return merit_; };
-  bool get_use_kkt_criteria() const { return use_kkt_criteria_; };
+  bool get_extra_iteration_for_last_kkt() const { return extra_iteration_for_last_kkt_; };
   bool get_use_filter_line_search() const { return use_filter_line_search_; };
   double get_mu() const { return mu_; };
+  double get_mu2() const { return mu2_; };
   double get_termination_tolerance() const { return termination_tol_; };
   std::size_t get_max_qp_iters(){ return max_qp_iters_; };
-  double get_cost(){ return cost_;};
-  bool get_warm_start() { return warm_start_; };
+  bool get_equality_qp_initial_guess() { return equality_qp_initial_guess_; };
   std::size_t get_filter_size() const { return filter_size_; };
 
 
   std::size_t get_rho_update_interval() { return rho_update_interval_; };
   std::size_t get_adaptive_rho_tolerance() { return adaptive_rho_tolerance_; };
   double get_alpha() { return alpha_; };
   double get_sigma() { return sigma_; };
   double get_rho_sparse() { return rho_sparse_;};
 
   double get_eps_abs() { return eps_abs_;};
   double get_eps_rel() { return eps_rel_;};
+  double get_norm_primal() { return norm_primal_;};
+  double get_norm_primal_tolerance() { return norm_primal_tolerance_;};
+  double get_norm_dual() { return norm_dual_;};
+  double get_norm_dual_tolerance() { return norm_dual_tolerance_;};
+
+  double get_reset_y() { return reset_y_;};
+  double get_reset_rho() { return reset_rho_;};
+  double get_rho_min() { return rho_min_;};
+  double get_rho_max() { return rho_max_;};
 
 
-  void printCallbacks();
+  void printCallbacks(bool isLastIteration = false);
+  void printQPCallbacks(int iter);
   void setCallbacks(bool inCallbacks);
   bool getCallbacks();
+  void setQPCallbacks(bool inCallbacks);
+  bool getQPCallbacks();
+
 
 
 
   void set_rho_update_interval(std::size_t interval) { rho_update_interval_ = interval; };
   void set_adaptive_rho_tolerance(std::size_t tolerance) { adaptive_rho_tolerance_ = tolerance; };
 
   void set_mu(double mu) { mu_ = mu; };
+  void set_mu2(double mu2) { mu2_ = mu2; };
   void set_alpha(double alpha) { alpha_ = alpha; };
   void set_sigma(double sigma) { sigma_ = sigma; };
 
-  void set_warm_start(bool warm_start) { warm_start_ = warm_start; };
+  void set_equality_qp_initial_guess(bool equality_qp_initial_guess) { equality_qp_initial_guess_ = equality_qp_initial_guess; };
+
 
   void set_termination_tolerance(double tol) { termination_tol_ = tol; };
-  void set_use_kkt_criteria(bool inBool) { use_kkt_criteria_ = inBool; };
+  void set_extra_iteration_for_last_kkt(bool inBool) { extra_iteration_for_last_kkt_ = inBool; };
   void set_use_filter_line_search(bool inBool) { use_filter_line_search_ = inBool; };
   void set_filter_size(const std::size_t inFilterSize) { filter_size_ = inFilterSize; 
                                                         gap_list_.resize(filter_size_); 
                                                         constraint_list_.resize(filter_size_); 
                                                         cost_list_.resize(filter_size_); };
 
 
 
-  void update_lagrangian_parameters(bool update_y);
+  void update_lagrangian_parameters();
   void set_rho_sparse(double rho_sparse) {rho_sparse_ = rho_sparse;};
-  void update_rho_sparse(int iter);
+  void update_rho_vec(int iter);
+  void apply_rho_update(double rho_sparse_);
 
   void set_max_qp_iters(int iters){ max_qp_iters_ = iters; };
   void set_eps_abs(double eps_abs) { eps_abs_ = eps_abs;};
   void set_eps_rel(double eps_rel) { eps_rel_ = eps_rel;};
 
  public:
   boost::circular_buffer<double> constraint_list_;             //!< memory buffer of constraint norms (used in filter line-search)
@@ -210,59 +229,64 @@
   std::vector<Eigen::VectorXd> rho_vec_;                       //!< rho vector
   std::vector<Eigen::VectorXd> inv_rho_vec_;                   //!< rho vector
 
   double norm_primal_ = 0.0;                                   //!< norm primal residual
   double norm_dual_ = 0.0;                                     //!< norm dual residual
   double norm_primal_rel_ = 0.0;                               //!< norm primal relative residual
   double norm_dual_rel_ = 0.0;                                 //!< norm dual relative residual
-
-  bool warm_start_y_ = false;
+  double norm_primal_tolerance_ = 0.0;                         //!< tolerance of the primal residual norm
+  double norm_dual_tolerance_ = 0.0;                           //!< tolerance of the primal residual norm
+  bool reset_y_ = false;
   bool reset_rho_ = false;
+  bool update_rho_with_heuristic_ = false;
+  bool remove_reg_ = false;                                    //!< Removes Crocoddyl's regularization (preg,dreg)
 
  protected:
   double merit_ = 0;                                           //!< merit function at nominal traj
   double merit_try_ = 0;                                       //!< merit function for the step length tried
   double x_grad_norm_ = 0;                                     //!< 1 norm of the delta x
   double u_grad_norm_ = 0;                                     //!< 1 norm of the delta u
   double gap_norm_ = 0;                                        //!< 1 norm of the gaps
   double constraint_norm_ = 0;                                 //!< 1 norm of constraint violation
   double constraint_norm_try_ = 0;                             //!< 1 norm of constraint violation try
   double gap_norm_try_ = 0;                                    //!< 1 norm of the gaps
-  double cost_ = 0.0;                                          //!< cost function
   double mu_ = 1e1;                                            //!< penalty no constraint violation
   double mu2_ = 1e1;                                           //!< penalty no constraint violation
   double termination_tol_ = 1e-6;                              //!< Termination tolerance
   bool with_callbacks_ = false;                                //!< With callbacks
-  bool use_kkt_criteria_ = true;                               //!< Use KKT conditions as termination criteria 
+  bool with_qp_callbacks_ = false;                         //!< With QP callbacks
+  bool extra_iteration_for_last_kkt_ = false;                  //!< Additional iteration if SQP max. iter reached
   double sigma_ = 1e-6;                                        //!< proximal term
   double alpha_ = 1.6;                                         //!< relaxed step size
   std::size_t max_qp_iters_ = 1000;                            //!< max qp iters
   std::size_t qp_iters_ = 0;
 
   double rho_estimate_sparse_ = 0.0;                          //!< rho estimate
-  double rho_sparse_ = 1e-1;                                  //!< rho
-  double rho_sparse_base_;
+  double rho_sparse_;                                  //!< rho
+  double rho_sparse_base_ = 1e-1;
   double rho_min_ = 1e-6;                                     //!< rho min
   double rho_max_ = 1e3;                                      //!< rho max 
   std::size_t rho_update_interval_ = 25;                      //!< frequency of update of rho
   double adaptive_rho_tolerance_ = 5; 
   double eps_abs_ = 1e-4;                                     //!< absolute termination criteria
   double eps_rel_ = 1e-4;                                     //!< relative termination criteria
-  double warm_start_ = true;
+  double equality_qp_initial_guess_ = true;
   std::size_t filter_size_ = 1;                               //!< Filter size for line-search (do not change the default value !)
   double KKT_ = std::numeric_limits<double>::infinity();      //!< KKT conditions residual
 
  private:
   double th_acceptnegstep_;                                   //!< Threshold used for accepting step along ascent direction
-  Eigen::VectorXd dual_vecx;
-  Eigen::VectorXd dual_vecu;
-
-  Eigen::MatrixXd sigma_diag_x;                // This is the sigma * eye(ndx)
-  std::vector<Eigen::MatrixXd> sigma_diag_u;   // This is the sigma * eye(nu)
-  std::vector<Eigen::VectorXd> Cdx_Cdu;
-  bool is_worse_than_memory_ = false;          //!< Boolean for filter line-search criteria 
+  bool is_worse_than_memory_ = false;                         //!< Boolean for filter line-search criteria 
 
+  Eigen::VectorXd tmp_vec_x_;                                 //!< Temporary variable
+  std::vector<Eigen::VectorXd> tmp_vec_u_;                    //!< Temporary variable
+  std::vector<Eigen::VectorXd> tmp_dual_cwise_;               //!< Temporary variable
+  Eigen::VectorXd tmp_Vx_;                                    //!< Temporary variable
+  std::vector<Eigen::VectorXd> tmp_Cdx_Cdu_;                       //!< Temporary variable
+  std::vector<Eigen::MatrixXd> tmp_rhoGx_mat_;                //!< Temporary variable
+  std::vector<Eigen::MatrixXd> tmp_rhoGu_mat_;                //!< Temporary variable
+  std::vector<Eigen::VectorXd> Vxx_fs_;                       //!< Temporary variable
 };
 
 }  // namespace mim_solvers
 
 #endif  // MIM_SOLVERS_CSQP_HPP_
```

### Comparing `cmeel_mim_solvers-0.0.2/include/mim_solvers/csqp_proxqp.hpp` & `cmeel_mim_solvers-0.0.4/include/mim_solvers/csqp_proxqp.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
    * @param[in] problem  shooting problem
    */
   explicit SolverPROXQP(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
   virtual ~SolverPROXQP();
 
   virtual bool solve(const std::vector<Eigen::VectorXd>& init_xs = crocoddyl::DEFAULT_VECTOR,
                      const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR, const std::size_t maxiter = 100,
-                     const bool is_feasible = false, const double regInit = 1e-9);
+                     const bool is_feasible = false, const double regInit = NAN);
 
   /**
    * @copybrief SolverAbstract::expectedImprovement
    *
    * This function requires to first run `updateExpectedImprovement()`. The expected improvement computation considers
    * the gaps in the dynamics: \f{equation} \Delta J(\alpha) = \Delta_1\alpha + \frac{1}{2}\Delta_2\alpha^2, \f} with
    * \f{eqnarray}
@@ -116,37 +116,42 @@
 
   const std::vector<Eigen::VectorXd>& get_dx() const { return dx_; };
   const std::vector<Eigen::VectorXd>& get_du() const { return du_; };
 
   const std::vector<Eigen::VectorXd>& get_y() const { return y_; };
   const std::vector<Eigen::VectorXd>& get_lag_mul() const { return lag_mul_; };
 
-  double get_KKT_norm() const { return KKT_; };
+  double get_KKT() const { return KKT_; };
   double get_gap_norm() const { return gap_norm_; };
   double get_constraint_norm() const { return constraint_norm_; };
   double get_qp_iters() const { return qp_iters_; };
   double get_xgrad_norm() const { return x_grad_norm_; };
   double get_ugrad_norm() const { return u_grad_norm_; };
   double get_merit() const { return merit_; };
-  bool get_use_kkt_criteria() const { return use_kkt_criteria_; };
   bool get_use_filter_line_search() const { return use_filter_line_search_; };
   double get_mu() const { return mu_; };
+  double get_mu2() const { return mu2_; };
   double get_termination_tolerance() const { return termination_tol_; };
   int get_max_qp_iters(){ return max_qp_iters_; };
   double get_cost(){ return cost_;};
   std::size_t get_filter_size() const { return filter_size_; };
 
   double get_eps_abs() { return eps_abs_;};
+  double get_eps_rel() { return eps_rel_;};
+  double get_norm_primal() { return norm_primal_;};
+  double get_norm_dual() { return norm_dual_;};
 
   void printCallbacks();
   void setCallbacks(bool inCallbacks);
   bool getCallbacks();
 
+  void set_mu(double mu) { mu_ = mu; };
+  void set_mu2(double mu2) { mu2_ = mu2; };
+  
   void set_termination_tolerance(double tol) { termination_tol_ = tol; };
-  void set_use_kkt_criteria(bool inBool) { use_kkt_criteria_ = inBool; };
   void set_use_filter_line_search(bool inBool) { use_filter_line_search_ = inBool; };
   void set_filter_size(const std::size_t inFilterSize) { filter_size_ = inFilterSize; 
                                                         gap_list_.resize(filter_size_); 
                                                         constraint_list_.resize(filter_size_); 
                                                         cost_list_.resize(filter_size_); };
 
 
@@ -157,61 +162,57 @@
   const Eigen::MatrixXd& get_C() const {return C_;};
   const Eigen::VectorXd& get_q() const {return q_;};
   const Eigen::VectorXd& get_b() const {return b_;};
   const Eigen::VectorXd& get_l() const {return l_;};
   const Eigen::VectorXd& get_u() const {return u_;};
 
   void set_eps_abs(double eps_abs) { eps_abs_ = eps_abs;};
-
+  void set_eps_rel(double eps_rel) { eps_rel_ = eps_rel;};
 
  public:  
   boost::circular_buffer<double> constraint_list_;             //!< memory buffer of constraint norms (used in filter line-search)
   boost::circular_buffer<double> gap_list_;                    //!< memory buffer of gap norms (used in filter line-search)
   boost::circular_buffer<double> cost_list_;                   //!< memory buffer of gap norms (used in filter line-search)
   
   using SolverDDP::xs_try_;
   using SolverDDP::us_try_;
   using SolverDDP::cost_try_;
-  std::vector<Eigen::VectorXd> fs_try_;                                //!< Gaps/defects between shooting nodes
-  std::vector<Eigen::VectorXd> dx_;                                    //!< the descent direction for x
-  std::vector<Eigen::VectorXd> du_;                                    //!< the descent direction for u
-  std::vector<Eigen::VectorXd> lag_mul_;                               //!< the Lagrange multiplier of the dynamics constraint
-  std::vector<Eigen::VectorXd> y_;                                    //!< lagrangian dual variable
+  std::vector<Eigen::VectorXd> fs_try_;                        //!< Gaps/defects between shooting nodes
+  std::vector<Eigen::VectorXd> dx_;                            //!< the descent direction for x
+  std::vector<Eigen::VectorXd> du_;                            //!< the descent direction for u
+  std::vector<Eigen::VectorXd> lag_mul_;                       //!< the Lagrange multiplier of the dynamics constraint
+  std::vector<Eigen::VectorXd> y_;                             //!< lagrangian dual variable
   
-  Eigen::VectorXd fs_flat_;                                            //!< Gaps/defects between shooting nodes (1D array)
-  double KKT_ = std::numeric_limits<double>::infinity();               //!< KKT conditions residual
+  Eigen::VectorXd fs_flat_;                                    //!< Gaps/defects between shooting nodes (1D array)
+  double KKT_ = std::numeric_limits<double>::infinity();       //!< KKT conditions residual
   bool use_filter_line_search_ = true;                         //!< Use filter line search
 
  protected:
   double merit_ = 0;                                           //!< merit function at nominal traj
   double merit_try_ = 0;                                       //!< merit function for the step length tried
   double x_grad_norm_ = 0;                                     //!< 1 norm of the delta x
   double u_grad_norm_ = 0;                                     //!< 1 norm of the delta u
   double gap_norm_ = 0;                                        //!< 1 norm of the gaps
   double constraint_norm_ = 0;                                 //!< 1 norm of constraint violation
-  double constraint_norm_try_ = 0;                                 //!< 1 norm of constraint violation try
+  double constraint_norm_try_ = 0;                             //!< 1 norm of constraint violation try
   double gap_norm_try_ = 0;                                    //!< 1 norm of the gaps
-  double cost_ = 0.0;                                            //!< cost function
+  double cost_ = 0.0;                                          //!< cost function
   double mu_ = 1e1;                                            //!< penalty no constraint violation
-  double mu2_ = 1e1;                                            //!< penalty no constraint violation
+  double mu2_ = 1e1;                                           //!< penalty no constraint violation
   double termination_tol_ = 1e-8;                              //!< Termination tolerance
   bool with_callbacks_ = false;                                //!< With callbacks
-  bool use_kkt_criteria_ = true;                               //!< Use KKT conditions as termination criteria 
-  double sigma_ = 1e-6; // proximal term
-  double alpha_ = 1.6; // relaxed step size
-  int max_qp_iters_ = 1000; // max qp iters
-  int qp_iters_ = 0;
-
-  double eps_abs_ = 1e-4; // absolute termination criteria
-  std::size_t filter_size_ = 1;                               //!< Filter size for line-search (do not change the default value !)
-
-  double norm_primal_ = 0.0; // norm primal residual
-  double norm_dual_ = 0.0; // norm dual residual
-  double norm_primal_rel_ = 0.0; // norm primal relative residual
-  double norm_dual_rel_ = 0.0; // norm dual relative residual
+  int max_qp_iters_ = 1000;                                    //!< maximum number of QP iterations
+  int qp_iters_ = 0;                                           //!< current number of QP iterations
+
+  double eps_abs_ = 1e-4;                                      //!< absolute termination criteria
+  double eps_rel_ = 1e-4;                                      //!< relative termination criteria
+  std::size_t filter_size_ = 1;                                //!< Filter size for line-search (do not change the default value !)
+
+  double norm_primal_ = 0.0;                                   //!< norm primal residual
+  double norm_dual_ = 0.0;                                     //!< norm dual residual
 
 
   // PROX QP STUFF
   Eigen::MatrixXd P_;
   Eigen::MatrixXd A_;
   Eigen::MatrixXd C_;
 
@@ -223,15 +224,15 @@
   Eigen::VectorXd b_;
   Eigen::VectorXd l_;
   Eigen::VectorXd u_;
 
   int n_in = 0;
   int n_eq = 0;
   int n_vars = 0;
-  
+  // 
  private:
   double th_acceptnegstep_;  //!< Threshold used for accepting step along ascent direction
   Eigen::VectorXd dual_vecx;
   Eigen::VectorXd dual_vecu;
   bool is_worse_than_memory_ = false;          //!< Boolean for filter line-search criteria 
 
 };
```

### Comparing `cmeel_mim_solvers-0.0.2/include/mim_solvers/ddp.hpp` & `cmeel_mim_solvers-0.0.4/include/mim_solvers/ddp.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #ifndef MIM_SOLVERS_DDP_HPP_
 #define MIM_SOLVERS_DDP_HPP_
 
 #include <vector>
 #include <Eigen/Cholesky>
 #include <crocoddyl/core/solver-base.hpp>
 #include <crocoddyl/core/mathbase.hpp>
-#include <crocoddyl/core/utils/deprecate.hpp>
 
 namespace mim_solvers {
 
 /**
  * @brief Differential Dynamic Programming (DDP) solver
  *
  * The DDP solver computes an optimal trajectory and control commands by iterates running `backwardPass()` and
@@ -63,15 +62,15 @@
    * @param[in] problem  shooting problem
    */
   explicit SolverDDP(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
   virtual ~SolverDDP();
 
   virtual bool solve(const std::vector<Eigen::VectorXd>& init_xs = crocoddyl::DEFAULT_VECTOR,
                      const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR, const std::size_t maxiter = 100,
-                     const bool is_feasible = false, const double regInit = 1e-9);
+                     const bool is_feasible = false, const double regInit = NAN);
   virtual void computeDirection(const bool recalc = true);
   virtual double tryStep(const double steplength = 1);
   virtual double stoppingCriteria();
   virtual const Eigen::Vector2d& expectedImprovement();
   virtual void resizeData();
 
   /**
@@ -300,18 +299,16 @@
 
   /**
    * @brief Compute the KKT conditions residual
    */
   virtual void checkKKTConditions();
   
   void set_termination_tolerance(double tol) { termination_tol_ = tol; };
-  void set_use_kkt_criteria(bool inBool) { use_kkt_criteria_ = inBool; };
 
   double get_termination_tolerance() const { return termination_tol_; };
-  bool get_use_kkt_criteria() const { return use_kkt_criteria_; }
 
   double get_KKT() const { return KKT_; };
 
  protected:
   double reg_incfactor_;  //!< Regularization factor used to increase the damping value
   double reg_decfactor_;  //!< Regularization factor used to decrease the damping value
   double reg_min_;        //!< Minimum allowed regularization value
@@ -345,15 +342,14 @@
   double th_grad_;                                         //!< Tolerance of the expected gradient used for testing the step
   double th_stepdec_;                                      //!< Step-length threshold used to decrease regularization
   double th_stepinc_;                                      //!< Step-length threshold used to increase regularization
   double KKT_ = std::numeric_limits<double>::infinity();   //!< KKT conditions residual
 
  public:
   std::vector<Eigen::VectorXd> lag_mul_;                   //!< the Lagrange multiplier of the dynamics constraint
-  bool use_kkt_criteria_ = true;                           //!< Use KKT conditions as termination criteria 
   Eigen::VectorXd fs_flat_;                                //!< Gaps/defects between shooting nodes (1D array)
   double termination_tol_ = 1e-6;                          //!< Termination tolerance
 };
 
 }  // namespace mim_solvers
 
 #endif  // MIM_SOLVERS_DDP_HPP_
```

### Comparing `cmeel_mim_solvers-0.0.2/include/mim_solvers/fddp.hpp` & `cmeel_mim_solvers-0.0.4/include/mim_solvers/sqp.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 ///////////////////////////////////////////////////////////////////////////////
-// 
-// This file is a modified version of SolverDDP from the Crocoddyl library
-// This modified version is used for benchmarking purposes only
-// Original file : https://github.com/loco-3d/crocoddyl/blob/devel/include/crocoddyl/core/solvers/fddp.hpp
-// 
 // BSD 3-Clause License
 // Copyright (C) 2023, New York University
 //
 // Copyright note valid unless otherwise stated in individual files.
 // All rights reserved.
 ///////////////////////////////////////////////////////////////////////////////
 
-#ifndef MIM_SOLVERS_FDDP_HPP_
-#define MIM_SOLVERS_FDDP_HPP_
+#ifndef MIM_SOLVERS_SQP_HPP_
+#define MIM_SOLVERS_SQP_HPP_
 
 #include <Eigen/Cholesky>
 #include <vector>
 #include <boost/circular_buffer.hpp>
 
 #include "mim_solvers/ddp.hpp"
 
 namespace mim_solvers {
 
 /**
- * @brief Feasibility-driven Differential Dynamic Programming (FDDP) solver
+ * @brief SQP solver
  *
- * The FDDP solver computes an optimal trajectory and control commands by iterates running `backwardPass()` and
- * `forwardPass()`. The backward pass accepts infeasible guess as described in the `SolverDDP::backwardPass()`.
+ * The SQP solver computes an optimal trajectory and control commands by iterates running `backwardPass()` and
+ * `forwardPass()`. The backward pass accepts infeasible guess as described in the `crocoddyl::SolverDDP::backwardPass()`.
  * Additionally, the forward pass handles infeasibility simulations that resembles the numerical behaviour of
  * a multiple-shooting formulation, i.e.:
  * \f{eqnarray}
  *   \mathbf{\hat{x}}_0 &=& \mathbf{\tilde{x}}_0 - (1 - \alpha)\mathbf{\bar{f}}_0,\\
  *   \mathbf{\hat{u}}_k &=& \mathbf{u}_k + \alpha\mathbf{k}_k + \mathbf{K}_k(\mathbf{\hat{x}}_k-\mathbf{x}_k),\\
  *   \mathbf{\hat{x}}_{k+1} &=& \mathbf{f}_k(\mathbf{\hat{x}}_k,\mathbf{\hat{u}}_k) - (1 -
  * \alpha)\mathbf{\bar{f}}_{k+1}.
@@ -47,109 +42,123 @@
  *   V_{\mathbf{xx}_k}\mathbf{x}_k),\nonumber\\ \Delta_2 = \sum_{k=0}^{N-1}
  *   \mathbf{k}_k^\top\mathbf{Q}_{\mathbf{uu}_k}\mathbf{k}_k + \mathbf{\bar{f}}_k^\top(2 V_{\mathbf{xx}_k}\mathbf{x}_k
  * - V_{\mathbf{xx}_k}\mathbf{\bar{f}}_k). \f}
  *
  * For more details about the feasibility-driven differential dynamic programming algorithm see:
  * \include mastalli-icra20.bib
  *
- * \sa `SolverDDP()`, `backwardPass()`, `forwardPass()`, `expectedImprovement()` and `updateExpectedImprovement()`
+ * \sa `crocoddyl::SolverDDP()`, `backwardPass()`, `forwardPass()`, `expectedImprovement()` and `updateExpectedImprovement()`
  */
-class SolverFDDP : public SolverDDP {
+class SolverSQP : public SolverDDP {
  public:
   EIGEN_MAKE_ALIGNED_OPERATOR_NEW
 
   /**
-   * @brief Initialize the FDDP solver
+   * @brief Initialize the SQP solver
    *
    * @param[in] problem  shooting problem
    */
-  explicit SolverFDDP(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
-  virtual ~SolverFDDP();
+  explicit SolverSQP(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
+  virtual ~SolverSQP();
 
   virtual bool solve(const std::vector<Eigen::VectorXd>& init_xs = crocoddyl::DEFAULT_VECTOR,
-                     const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR, const std::size_t maxiter = 100,
-                     const bool is_feasible = false, const double regInit = 1e-9);
+                     const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR, 
+                     const std::size_t maxiter = 100,
+                     const bool is_feasible = false, 
+                     const double regInit = NAN);
 
   /**
    * @copybrief SolverAbstract::expectedImprovement
    *
    * This function requires to first run `updateExpectedImprovement()`. The expected improvement computation considers
    * the gaps in the dynamics: \f{equation} \Delta J(\alpha) = \Delta_1\alpha + \frac{1}{2}\Delta_2\alpha^2, \f} with
    * \f{eqnarray}
    *   \Delta_1 = \sum_{k=0}^{N-1} \mathbf{k}_k^\top\mathbf{Q}_{\mathbf{u}_k} +\mathbf{\bar{f}}_k^\top(V_{\mathbf{x}_k}
    * - V_{\mathbf{xx}_k}\mathbf{x}_k),\nonumber\\ \Delta_2 = \sum_{k=0}^{N-1}
    *   \mathbf{k}_k^\top\mathbf{Q}_{\mathbf{uu}_k}\mathbf{k}_k + \mathbf{\bar{f}}_k^\top(2
    * V_{\mathbf{xx}_k}\mathbf{x}_k
    * - V_{\mathbf{xx}_k}\mathbf{\bar{f}}_k). \f}
    */
-  virtual const Eigen::Vector2d& expectedImprovement();
+  // virtual const Eigen::Vector2d& expectedImprovement();
 
   /**
    * @brief Update internal values for computing the expected improvement
    */
   void updateExpectedImprovement();
-  virtual void forwardPass(const double stepLength);
 
+  virtual void forwardPass(const double stepLength=0);
   /**
    * @brief Computes the merit function, gaps at the given xs, us along with delta x and delta u
    */
   virtual void computeDirection(const bool recalcDiff);
-  
-  /**
-   * @brief Return the threshold used for accepting step along ascent direction
-   */
-  double get_th_acceptnegstep() const;
 
-  /**
-   * @brief Modify the threshold used for accepting step along ascent direction
-   */
-  void set_th_acceptnegstep(const double th_acceptnegstep);
+  virtual double tryStep(const double stepLength);
 
   /**
    * @brief Compute the KKT conditions residual
    */
   virtual void checkKKTConditions();
-    
-  void set_termination_tolerance(double tol) { termination_tol_ = tol; };
-  void set_use_kkt_criteria(bool inBool) { use_kkt_criteria_ = inBool; };
 
-  double get_termination_tolerance() const { return termination_tol_; };
-  bool get_use_kkt_criteria() const { return use_kkt_criteria_; }
+  const std::vector<Eigen::VectorXd>& get_xs_try() const { return xs_try_; };
+  const std::vector<Eigen::VectorXd>& get_us_try() const { return us_try_; };
 
+  double get_KKT() const { return KKT_; };
+  double get_gap_norm() const { return gap_norm_; };
+  double get_xgrad_norm() const { return x_grad_norm_; };
+  double get_ugrad_norm() const { return u_grad_norm_; };
+  double get_merit() const { return merit_; };
+  bool get_extra_iteration_for_last_kkt() const { return extra_iteration_for_last_kkt_; };
   bool get_use_filter_line_search() const { return use_filter_line_search_; };
+  double get_mu() const { return mu_; };
+  double get_termination_tolerance() const { return termination_tol_; };
   std::size_t get_filter_size() const { return filter_size_; };
+
+  void printCallbacks();
+  void setCallbacks(bool inCallbacks);
+  bool getCallbacks();
+
+
+  void set_mu(double mu) { mu_ = mu; };
+  void set_termination_tolerance(double tol) { termination_tol_ = tol; };
+  void set_extra_iteration_for_last_kkt(bool inBool) { extra_iteration_for_last_kkt_ = inBool; };
   void set_use_filter_line_search(bool inBool) { use_filter_line_search_ = inBool; };
   void set_filter_size(const std::size_t inFilterSize) { filter_size_ = inFilterSize; 
                                                          gap_list_.resize(filter_size_); 
                                                          cost_list_.resize(filter_size_); };
-  double get_gap_norm() const { return gap_norm_; };
-  double get_KKT() const { return KKT_; };
-
-  boost::circular_buffer<double> gap_list_;                //!< memory buffer of gap norms (used in filter line-search)
-  boost::circular_buffer<double> cost_list_;               //!< memory buffer of gap norms (used in filter line-search)
-  bool use_filter_line_search_ = true;                    //!< Use filter line search
-  std::size_t filter_size_ = 1;                            //!< Filter size for line-search (do not change the default value !)
-  bool is_worse_than_memory_ = false;                      //!< Boolean for filter line-search criteria 
-                         
-  std::vector<Eigen::VectorXd> lag_mul_;                   //!< the Lagrange multiplier of the dynamics constraint
-  bool use_kkt_criteria_ = true;                           //!< Use KKT conditions as termination criteria 
-  Eigen::VectorXd fs_flat_;                                //!< Gaps/defects between shooting nodes (1D array)
-  double termination_tol_ = 1e-6;                          //!< Termination tolerance
-
-  std::vector<Eigen::VectorXd> fs_try_;                    //!< Gaps/defects between shooting nodes
-
-  double gap_norm_ = 0;                                    //!< 1 norm of the gaps
-  double gap_norm_try_ = 0;                                //!< 1 norm of the gaps
-
+  
+ public:
+  using SolverDDP::xs_try_;
+  using SolverDDP::us_try_;
+  using SolverDDP::cost_try_;
+  std::vector<Eigen::VectorXd> fs_try_;                        //!< Gaps/defects between shooting nodes
+  std::vector<Eigen::VectorXd> dx_;                            //!< the descent direction for x
+  std::vector<Eigen::VectorXd> du_;                            //!< the descent direction for u
+  std::vector<Eigen::VectorXd> lag_mul_;                       //!< the Lagrange multiplier of the dynamics constraint
+  boost::circular_buffer<double> gap_list_;                    //!< memory buffer of gap norms (used in filter line-search)
+  boost::circular_buffer<double> cost_list_;                   //!< memory buffer of gap norms (used in filter line-search)
+  Eigen::VectorXd fs_flat_;                                    //!< Gaps/defects between shooting nodes (1D array)
+  bool use_filter_line_search_ = true;                         //!< Use filter line search
+  
  protected:
-  double dg_;                                              //!< Internal data for computing the expected improvement
-  double dq_;                                              //!< Internal data for computing the expected improvement
-  double dv_;                                              //!< Internal data for computing the expected improvement
-  double KKT_ = std::numeric_limits<double>::infinity();   //!< KKT conditions residual
+  double merit_ = 0;                                           //!< merit function at nominal traj
+  double merit_try_ = 0;                                       //!< merit function for the step length tried
+  double x_grad_norm_ = 0;                                     //!< 1 norm of the delta x
+  double u_grad_norm_ = 0;                                     //!< 1 norm of the delta u
+  double gap_norm_ = 0;                                        //!< 1 norm of the gaps
+  double gap_norm_try_ = 0;                                    //!< 1 norm of the gaps
+  double mu_ = 1e0;                                            //!< penalty no constraint violation
+  double termination_tol_ = 1e-6;                              //!< Termination tolerance
+  bool with_callbacks_ = false;                                //!< With callbacks
+  bool extra_iteration_for_last_kkt_ = false;                  //!< Additional iteration if SQP max. iter reached
+  std::size_t filter_size_ = 1;                                //!< Filter size for line-search (do not change the default value !)
+  double KKT_ = std::numeric_limits<double>::infinity();       //!< KKT conditions residual
 
  private:
-  double th_acceptnegstep_;  //!< Threshold used for accepting step along ascent direction
+  double th_acceptnegstep_;                                    //!< Threshold used for accepting step along ascent direction
+  bool is_worse_than_memory_ = false;                          //!< Boolean for filter line-search criteria 
+  Eigen::VectorXd tmp_vec_x_;                                  //!< Temporary variable
+  std::vector<Eigen::VectorXd> tmp_vec_u_;                     //!< Temporary variable
 };
 
 }  // namespace mim_solvers
 
-#endif  // MIM_SOLVERSS_FDDP_HPP_
+#endif  // MIM_SOLVERS_SQP_HPP_
```

### Comparing `cmeel_mim_solvers-0.0.2/include/mim_solvers/kkt.hpp` & `cmeel_mim_solvers-0.0.4/include/mim_solvers/kkt.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   explicit SolverKKT(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
   virtual ~SolverKKT();
 
   virtual bool solve(
       const std::vector<Eigen::VectorXd>& init_xs = crocoddyl::DEFAULT_VECTOR,
       const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR,
       const std::size_t maxiter = 100, const bool is_feasible = false,
-      const double regInit = 1e-9);
+      const double regInit = NAN);
   virtual void computeDirection(const bool recalc = true);
   virtual double tryStep(const double steplength = 1);
   virtual double stoppingCriteria();
   virtual const Eigen::Vector2d& expectedImprovement();
 
   const Eigen::MatrixXd& get_kkt() const;
   const Eigen::VectorXd& get_kktref() const;
@@ -50,17 +50,15 @@
   std::size_t get_nu() const;
 
   /**
    * @brief Compute the KKT conditions residual
    */
   virtual void checkKKTConditions();
   void set_termination_tolerance(double tol) { termination_tol_ = tol; };
-  void set_use_kkt_criteria(bool inBool) { use_kkt_criteria_ = inBool; };
   double get_termination_tolerance() const { return termination_tol_; };
-  bool get_use_kkt_criteria() const { return use_kkt_criteria_; }
   double get_KKT() const { return KKT_; };
 
  protected:
   double reg_incfactor_;
   double reg_decfactor_;
   double reg_min_;
   double reg_max_;
@@ -90,15 +88,14 @@
   Eigen::VectorXd dual_;
   std::vector<double> alphas_;
   double th_grad_;
   bool was_feasible_;
   Eigen::VectorXd kkt_primal_;
   Eigen::VectorXd dF;
   double KKT_ = std::numeric_limits<double>::infinity();   //!< KKT conditions residual
-  bool use_kkt_criteria_ = true;                           //!< Use KKT conditions as termination criteria 
   Eigen::VectorXd fs_flat_;                                //!< Gaps/defects between shooting nodes (1D array)
   double termination_tol_ = 1e-6;                          //!< Termination tolerance
 
 };
 
 }  // namespace mim_solvers
```

### Comparing `cmeel_mim_solvers-0.0.2/include/mim_solvers/python.hpp` & `cmeel_mim_solvers-0.0.4/include/mim_solvers/python.hpp`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/include/mim_solvers/sqp.hpp` & `cmeel_mim_solvers-0.0.4/include/mim_solvers/fddp.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 ///////////////////////////////////////////////////////////////////////////////
+// 
+// This file is a modified version of SolverDDP from the Crocoddyl library
+// This modified version is used for benchmarking purposes only
+// Original file : https://github.com/loco-3d/crocoddyl/blob/devel/include/crocoddyl/core/solvers/fddp.hpp
+// 
 // BSD 3-Clause License
 // Copyright (C) 2023, New York University
 //
 // Copyright note valid unless otherwise stated in individual files.
 // All rights reserved.
 ///////////////////////////////////////////////////////////////////////////////
 
-#ifndef MIM_SOLVERS_SQP_HPP_
-#define MIM_SOLVERS_SQP_HPP_
+#ifndef MIM_SOLVERS_FDDP_HPP_
+#define MIM_SOLVERS_FDDP_HPP_
 
 #include <Eigen/Cholesky>
 #include <vector>
 #include <boost/circular_buffer.hpp>
 
 #include "mim_solvers/ddp.hpp"
 
 namespace mim_solvers {
 
 /**
- * @brief SQP solver
+ * @brief Feasibility-driven Differential Dynamic Programming (FDDP) solver
  *
- * The SQP solver computes an optimal trajectory and control commands by iterates running `backwardPass()` and
- * `forwardPass()`. The backward pass accepts infeasible guess as described in the `crocoddyl::SolverDDP::backwardPass()`.
+ * The FDDP solver computes an optimal trajectory and control commands by iterates running `backwardPass()` and
+ * `forwardPass()`. The backward pass accepts infeasible guess as described in the `SolverDDP::backwardPass()`.
  * Additionally, the forward pass handles infeasibility simulations that resembles the numerical behaviour of
  * a multiple-shooting formulation, i.e.:
  * \f{eqnarray}
  *   \mathbf{\hat{x}}_0 &=& \mathbf{\tilde{x}}_0 - (1 - \alpha)\mathbf{\bar{f}}_0,\\
  *   \mathbf{\hat{u}}_k &=& \mathbf{u}_k + \alpha\mathbf{k}_k + \mathbf{K}_k(\mathbf{\hat{x}}_k-\mathbf{x}_k),\\
  *   \mathbf{\hat{x}}_{k+1} &=& \mathbf{f}_k(\mathbf{\hat{x}}_k,\mathbf{\hat{u}}_k) - (1 -
  * \alpha)\mathbf{\bar{f}}_{k+1}.
@@ -42,122 +47,106 @@
  *   V_{\mathbf{xx}_k}\mathbf{x}_k),\nonumber\\ \Delta_2 = \sum_{k=0}^{N-1}
  *   \mathbf{k}_k^\top\mathbf{Q}_{\mathbf{uu}_k}\mathbf{k}_k + \mathbf{\bar{f}}_k^\top(2 V_{\mathbf{xx}_k}\mathbf{x}_k
  * - V_{\mathbf{xx}_k}\mathbf{\bar{f}}_k). \f}
  *
  * For more details about the feasibility-driven differential dynamic programming algorithm see:
  * \include mastalli-icra20.bib
  *
- * \sa `crocoddyl::SolverDDP()`, `backwardPass()`, `forwardPass()`, `expectedImprovement()` and `updateExpectedImprovement()`
+ * \sa `SolverDDP()`, `backwardPass()`, `forwardPass()`, `expectedImprovement()` and `updateExpectedImprovement()`
  */
-class SolverSQP : public SolverDDP {
+class SolverFDDP : public SolverDDP {
  public:
   EIGEN_MAKE_ALIGNED_OPERATOR_NEW
 
   /**
-   * @brief Initialize the SQP solver
+   * @brief Initialize the FDDP solver
    *
    * @param[in] problem  shooting problem
    */
-  explicit SolverSQP(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
-  virtual ~SolverSQP();
+  explicit SolverFDDP(boost::shared_ptr<crocoddyl::ShootingProblem> problem);
+  virtual ~SolverFDDP();
 
   virtual bool solve(const std::vector<Eigen::VectorXd>& init_xs = crocoddyl::DEFAULT_VECTOR,
-                     const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR, 
-                     const std::size_t maxiter = 100,
-                     const bool is_feasible = false, 
-                     const double regInit = 1e-9);
+                     const std::vector<Eigen::VectorXd>& init_us = crocoddyl::DEFAULT_VECTOR, const std::size_t maxiter = 100,
+                     const bool is_feasible = false, const double regInit = NAN);
 
   /**
    * @copybrief SolverAbstract::expectedImprovement
    *
    * This function requires to first run `updateExpectedImprovement()`. The expected improvement computation considers
    * the gaps in the dynamics: \f{equation} \Delta J(\alpha) = \Delta_1\alpha + \frac{1}{2}\Delta_2\alpha^2, \f} with
    * \f{eqnarray}
    *   \Delta_1 = \sum_{k=0}^{N-1} \mathbf{k}_k^\top\mathbf{Q}_{\mathbf{u}_k} +\mathbf{\bar{f}}_k^\top(V_{\mathbf{x}_k}
    * - V_{\mathbf{xx}_k}\mathbf{x}_k),\nonumber\\ \Delta_2 = \sum_{k=0}^{N-1}
    *   \mathbf{k}_k^\top\mathbf{Q}_{\mathbf{uu}_k}\mathbf{k}_k + \mathbf{\bar{f}}_k^\top(2
    * V_{\mathbf{xx}_k}\mathbf{x}_k
    * - V_{\mathbf{xx}_k}\mathbf{\bar{f}}_k). \f}
    */
-  // virtual const Eigen::Vector2d& expectedImprovement();
+  virtual const Eigen::Vector2d& expectedImprovement();
 
   /**
    * @brief Update internal values for computing the expected improvement
    */
   void updateExpectedImprovement();
+  virtual void forwardPass(const double stepLength);
 
-  virtual void forwardPass();
   /**
    * @brief Computes the merit function, gaps at the given xs, us along with delta x and delta u
    */
   virtual void computeDirection(const bool recalcDiff);
+  
+  /**
+   * @brief Return the threshold used for accepting step along ascent direction
+   */
+  double get_th_acceptnegstep() const;
 
-  virtual double tryStep(const double stepLength);
+  /**
+   * @brief Modify the threshold used for accepting step along ascent direction
+   */
+  void set_th_acceptnegstep(const double th_acceptnegstep);
 
   /**
    * @brief Compute the KKT conditions residual
    */
   virtual void checkKKTConditions();
+    
+  void set_termination_tolerance(double tol) { termination_tol_ = tol; };
 
-  const std::vector<Eigen::VectorXd>& get_xs_try() const { return xs_try_; };
-  const std::vector<Eigen::VectorXd>& get_us_try() const { return us_try_; };
+  double get_termination_tolerance() const { return termination_tol_; };
 
-  double get_KKT() const { return KKT_; };
-  double get_gap_norm() const { return gap_norm_; };
-  double get_xgrad_norm() const { return x_grad_norm_; };
-  double get_ugrad_norm() const { return u_grad_norm_; };
-  double get_merit() const { return merit_; };
-  bool get_use_kkt_criteria() const { return use_kkt_criteria_; };
   bool get_use_filter_line_search() const { return use_filter_line_search_; };
-  double get_mu() const { return mu_; };
-  double get_termination_tolerance() const { return termination_tol_; };
   std::size_t get_filter_size() const { return filter_size_; };
-
-  void printCallbacks();
-  void setCallbacks(bool inCallbacks);
-  bool getCallbacks();
-
-
-  void set_mu(double mu) { mu_ = mu; };
-  void set_termination_tolerance(double tol) { termination_tol_ = tol; };
-  void set_use_kkt_criteria(bool inBool) { use_kkt_criteria_ = inBool; };
   void set_use_filter_line_search(bool inBool) { use_filter_line_search_ = inBool; };
   void set_filter_size(const std::size_t inFilterSize) { filter_size_ = inFilterSize; 
                                                          gap_list_.resize(filter_size_); 
                                                          cost_list_.resize(filter_size_); };
-  
- public:
-  using SolverDDP::xs_try_;
-  using SolverDDP::us_try_;
-  using SolverDDP::cost_try_;
-  std::vector<Eigen::VectorXd> fs_try_;                                //!< Gaps/defects between shooting nodes
-  std::vector<Eigen::VectorXd> dx_;                                    //!< the descent direction for x
-  std::vector<Eigen::VectorXd> du_;                                    //!< the descent direction for u
-  std::vector<Eigen::VectorXd> lag_mul_;                               //!< the Lagrange multiplier of the dynamics constraint
-  boost::circular_buffer<double> gap_list_;                            //!< memory buffer of gap norms (used in filter line-search)
-  boost::circular_buffer<double> cost_list_;                           //!< memory buffer of gap norms (used in filter line-search)
-  Eigen::VectorXd fs_flat_;                                            //!< Gaps/defects between shooting nodes (1D array)
-  bool use_filter_line_search_ = true;                                 //!< Use filter line search
-  
+  double get_gap_norm() const { return gap_norm_; };
+  double get_KKT() const { return KKT_; };
+
+  boost::circular_buffer<double> gap_list_;                //!< memory buffer of gap norms (used in filter line-search)
+  boost::circular_buffer<double> cost_list_;               //!< memory buffer of gap norms (used in filter line-search)
+  bool use_filter_line_search_ = true;                    //!< Use filter line search
+  std::size_t filter_size_ = 1;                            //!< Filter size for line-search (do not change the default value !)
+  bool is_worse_than_memory_ = false;                      //!< Boolean for filter line-search criteria 
+                         
+  std::vector<Eigen::VectorXd> lag_mul_;                   //!< the Lagrange multiplier of the dynamics constraint
+  Eigen::VectorXd fs_flat_;                                //!< Gaps/defects between shooting nodes (1D array)
+  double termination_tol_ = 1e-6;                          //!< Termination tolerance
+
+  std::vector<Eigen::VectorXd> fs_try_;                    //!< Gaps/defects between shooting nodes
+
+  double gap_norm_ = 0;                                    //!< 1 norm of the gaps
+  double gap_norm_try_ = 0;                                //!< 1 norm of the gaps
+
  protected:
-  double merit_ = 0;                                           //!< merit function at nominal traj
-  double merit_try_ = 0;                                       //!< merit function for the step length tried
-  double x_grad_norm_ = 0;                                     //!< 1 norm of the delta x
-  double u_grad_norm_ = 0;                                     //!< 1 norm of the delta u
-  double gap_norm_ = 0;                                        //!< 1 norm of the gaps
-  double gap_norm_try_ = 0;                                    //!< 1 norm of the gaps
-  double cost_ = 0;                                            //!< cost function
-  double mu_ = 1e0;                                            //!< penalty no constraint violation
-  double termination_tol_ = 1e-6;                              //!< Termination tolerance
-  bool with_callbacks_ = false;                                //!< With callbacks
-  bool use_kkt_criteria_ = true;                               //!< Use KKT conditions as termination criteria 
-  std::size_t filter_size_ = 1;                                //!< Filter size for line-search (do not change the default value !)
-  double KKT_ = std::numeric_limits<double>::infinity();       //!< KKT conditions residual
+  double dg_;                                              //!< Internal data for computing the expected improvement
+  double dq_;                                              //!< Internal data for computing the expected improvement
+  double dv_;                                              //!< Internal data for computing the expected improvement
+  double KKT_ = std::numeric_limits<double>::infinity();   //!< KKT conditions residual
 
  private:
-  double th_acceptnegstep_;           //!< Threshold used for accepting step along ascent direction
-  bool is_worse_than_memory_ = false; //!< Boolean for filter line-search criteria 
+  double th_acceptnegstep_;  //!< Threshold used for accepting step along ascent direction
 };
 
 }  // namespace mim_solvers
 
-#endif  // MIM_SOLVERS_SQP_HPP_
+#endif  // MIM_SOLVERSS_FDDP_HPP_
```

### Comparing `cmeel_mim_solvers-0.0.2/package.xml` & `cmeel_mim_solvers-0.0.4/package.xml`

 * *Files 1% similar despite different names*

#### Comparing `cmeel_mim_solvers-0.0.2/package.xml` & `cmeel_mim_solvers-0.0.4/package.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <package format="3">
   <name>mim_solvers</name>
-  <version>0.0.2</version>
+  <version>0.0.4</version>
   <description>Numerical solvers of the Machines in Motion Laboratory.</description>
   <maintainer email="sk8001@nyu.edu">Sébastien Kleff</maintainer>
   <author email="sk8001@nyu.edu">Sébastien Kleff</author>
   <license>BSD</license>
   <url type="website">https://github.com/machines-in-motion/mim_solvers</url>
   <build_depend>git</build_depend>
   <build_depend>doxygen</build_depend>
```

### Comparing `cmeel_mim_solvers-0.0.2/pyproject.toml` & `cmeel_mim_solvers-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 requires = ["cmeel[build]", "crocoddyl[build]", "proxsuite[build]", "cmeel-boost ~= 1.83.0"]
 
 [project]
 dependencies = ["crocoddyl", "proxsuite", "cmeel-boost ~= 1.83.0"]
 description = "A fast and flexible implementation of Rigid Body Dynamics algorithms and their analytical derivatives"
 license = "BSD-3-Clause"
 name = "cmeel-mim-solvers"
-version = "0.0.2"
+version = "0.0.4"
 
 [project.urls]
 homepage = "https://github.com/cmake-wheel/mim_solvers"
 upstream = "https://github.com/machines-in-motion/mim_solvers"
```

### Comparing `cmeel_mim_solvers-0.0.2/python/csqp.cpp` & `cmeel_mim_solvers-0.0.4/bindings/csqp.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
            "")
       .def("backwardPass", &SolverCSQP::backwardPass, bp::args("self"),
            "")
       .def("backwardPass_without_constraints", &SolverCSQP::backwardPass_without_constraints, bp::args("self"),
            "")
       .def("backwardPass_without_rho_update", &SolverCSQP::backwardPass_without_rho_update, bp::args("self"),
            "")
-      .def("update_rho_sparse", &SolverCSQP::update_rho_sparse, bp::args("self", "iter"),
+      .def("update_rho_vec", &SolverCSQP::update_rho_vec, bp::args("self", "iter"),
            "")
       .def("computeDirection", &SolverCSQP::computeDirection, bp::args("self", "recalcDiff"),
            "")
       .def("checkKKTConditions", &SolverCSQP::checkKKTConditions, bp::args("self"),
            "")
       .def_readwrite("xs_try", &SolverCSQP::xs_try_, "xs try")
       .def_readwrite("us_try", &SolverCSQP::us_try_, "us try")  
@@ -74,22 +74,26 @@
       .def_readwrite("norm_primal", &SolverCSQP::norm_primal_, "norm_primal")
       .def_readwrite("norm_dual", &SolverCSQP::norm_dual_, "norm_dual ")
       .def_readwrite("norm_dual_rel", &SolverCSQP::norm_dual_rel_, "norm_dual_rel")
       .def_readwrite("norm_primal_rel", &SolverCSQP::norm_primal_rel_, "norm_primal_rel")
       .def_readwrite("rho_vec", &SolverCSQP::rho_vec_, "rho vector")
       .def_readwrite("y", &SolverCSQP::y_, "y")
       .def_readwrite("z", &SolverCSQP::z_, "z")
-      .def_readwrite("warm_start_y", &SolverCSQP::warm_start_y_, "Warm-start ADMM Lagrange multipliers with previous solution (default: False, i.e. reset to 0)")
-      .def_readwrite("reset_rho", &SolverCSQP::reset_rho_, "Reset the rho parameter (default: False, i.e. not reset to base values)")
+      .def_readwrite("reset_y", &SolverCSQP::reset_y_, "Reset ADMM Lagrange multipliers to zero (default: False, i.e. reset to previous)")
+      .def_readwrite("reset_rho", &SolverCSQP::reset_rho_, "Reset the rho parameter (default: False, i.e. reset to previous)")
+      .def_readwrite("update_rho_with_heuristic", &SolverCSQP::update_rho_with_heuristic_, "Update the heuristic for the rho update (default: False)")
+      .def_readwrite("remove_reg", &SolverCSQP::remove_reg_, "Removes Crocoddyl's regularization by setting (preg,dreg)=0 when True (default: False)")
 
 
       .add_property("with_callbacks", bp::make_function(&SolverCSQP::getCallbacks), bp::make_function(&SolverCSQP::setCallbacks),
                     "Activates the callbacks when true (default: False)")
-      .add_property("use_kkt_criteria", bp::make_function(&SolverCSQP::get_use_kkt_criteria), bp::make_function(&SolverCSQP::set_use_kkt_criteria),
-                    "Use the KKT residual condition as a termination criteria (default: True)")
+      .add_property("with_qp_callbacks", bp::make_function(&SolverCSQP::getQPCallbacks), bp::make_function(&SolverCSQP::setQPCallbacks),
+                    "Activates the QP callbacks when true (default: False)")
+      .add_property("extra_iteration_for_last_kkt", bp::make_function(&SolverCSQP::get_extra_iteration_for_last_kkt), bp::make_function(&SolverCSQP::set_extra_iteration_for_last_kkt),
+                    "Additional iteration if SQP max. iter reached (default: False)")
       .add_property("mu", bp::make_function(&SolverCSQP::get_mu), bp::make_function(&SolverCSQP::set_mu),
                     "Penalty term for dynamic violation in the merit function (default: 1.)")
       .add_property("xs", make_function(&SolverCSQP::get_xs, bp::return_value_policy<bp::copy_const_reference>()), bp::make_function(&SolverCSQP::set_xs), "xs")
       .add_property("us", make_function(&SolverCSQP::get_us, bp::return_value_policy<bp::copy_const_reference>()), bp::make_function(&SolverCSQP::set_us), "us")
       .add_property("dx_tilde", make_function(&SolverCSQP::get_xs_tilde, bp::return_value_policy<bp::copy_const_reference>()), "dx_tilde")
       .add_property("du_tilde", make_function(&SolverCSQP::get_us_tilde, bp::return_value_policy<bp::copy_const_reference>()), "du_tilde")
       
@@ -101,23 +105,23 @@
                     "Gap norm")
       .add_property("qp_iters", bp::make_function(&SolverCSQP::get_qp_iters),
                     "Number of QP iterations")
       .add_property("KKT", bp::make_function(&SolverCSQP::get_KKT),
                     "KKT residual norm")
                     
       .add_property("mu", bp::make_function(&SolverCSQP::get_mu), bp::make_function(&SolverCSQP::set_mu),
-                    "Penalty term for dynamic violation in the merit function (default: 1.)")
+                    "Penalty term for dynamic violation in the merit function (default: 10.)")
       .add_property("eps_abs", bp::make_function(&SolverCSQP::get_eps_abs), bp::make_function(&SolverCSQP::set_eps_abs),
                     "sets epsillon absolute termination criteria for qp solver")
       .add_property("eps_rel", bp::make_function(&SolverCSQP::get_eps_rel), bp::make_function(&SolverCSQP::set_eps_rel),
                     "sets epsillon relative termination criteria for qp solver")
       .add_property("rho_sparse", bp::make_function(&SolverCSQP::get_rho_sparse), bp::make_function(&SolverCSQP::set_rho_sparse),
                     "Penalty term for dynamic violation in the merit function (default: 1.)")
-      .add_property("warm_start", bp::make_function(&SolverCSQP::get_warm_start), bp::make_function(&SolverCSQP::set_warm_start),
-                    "Penalty term for dynamic violation in the merit function (default: 1.)")
+      .add_property("equality_qp_initial_guess", bp::make_function(&SolverCSQP::get_equality_qp_initial_guess), bp::make_function(&SolverCSQP::set_equality_qp_initial_guess),
+                    "initialize each qp with the solution of the equality qp. (default: True)")
       .add_property("sigma", bp::make_function(&SolverCSQP::get_sigma), bp::make_function(&SolverCSQP::set_sigma),
                     "get and set sigma")
       .add_property("alpha", bp::make_function(&SolverCSQP::get_alpha), bp::make_function(&SolverCSQP::set_alpha),
                     "get and set alpha (relaxed update)")
 
       .add_property("use_filter_line_search", bp::make_function(&SolverCSQP::get_use_filter_line_search), bp::make_function(&SolverCSQP::set_use_filter_line_search),
                     "Use the filter line search criteria (default: True)")
```

### Comparing `cmeel_mim_solvers-0.0.2/python/csqp_proxqp.cpp` & `cmeel_mim_solvers-0.0.4/bindings/csqp_proxqp.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -55,29 +55,26 @@
            "")
 
       .def_readwrite("xs_try", &SolverPROXQP::xs_try_, "xs try")
       .def_readwrite("us_try", &SolverPROXQP::us_try_, "us try")  
       .def_readwrite("cost_try", &SolverPROXQP::cost_try_, "cost try")
       .def_readwrite("fs_try", &SolverPROXQP::fs_try_, "fs_try")
       .def_readwrite("lag_mul", &SolverPROXQP::lag_mul_, "lagrange multipliers")
-      .def_readwrite("KKT", &SolverPROXQP::KKT_, "KKT residual")
 
       .add_property("constraint_norm", bp::make_function(&SolverPROXQP::get_constraint_norm),
                     "Constraint norm")
       .add_property("gap_norm", bp::make_function(&SolverPROXQP::get_gap_norm), 
                     "Gap norm")
       .add_property("qp_iters", bp::make_function(&SolverPROXQP::get_qp_iters),
                     "Number of QP iterations")
-      .add_property("KKT_norm", bp::make_function(&SolverPROXQP::get_KKT_norm),
+      .add_property("KKT_norm", bp::make_function(&SolverPROXQP::get_KKT),
                     "KKT norm")
 
       .add_property("with_callbacks", bp::make_function(&SolverPROXQP::getCallbacks), bp::make_function(&SolverPROXQP::setCallbacks),
                     "Activates the callbacks when true (default: False)")
-      .add_property("use_kkt_criteria", bp::make_function(&SolverPROXQP::get_use_kkt_criteria), bp::make_function(&SolverPROXQP::set_use_kkt_criteria),
-                    "Use the KKT residual condition as a termination criteria (default: True)")
       .add_property("xs", make_function(&SolverPROXQP::get_xs, bp::return_value_policy<bp::copy_const_reference>()), bp::make_function(&SolverPROXQP::set_xs), "xs")
       .add_property("us", make_function(&SolverPROXQP::get_us, bp::return_value_policy<bp::copy_const_reference>()), bp::make_function(&SolverPROXQP::set_us), "us")
       .add_property("P", make_function(&SolverPROXQP::get_P, bp::return_value_policy<bp::copy_const_reference>()), "P")
       .add_property("A", make_function(&SolverPROXQP::get_A, bp::return_value_policy<bp::copy_const_reference>()), "A")
       .add_property("C", make_function(&SolverPROXQP::get_C, bp::return_value_policy<bp::copy_const_reference>()), "C")
       .add_property("q", make_function(&SolverPROXQP::get_q, bp::return_value_policy<bp::copy_const_reference>()), "q")
       .add_property("b", make_function(&SolverPROXQP::get_b, bp::return_value_policy<bp::copy_const_reference>()), "b")
```

### Comparing `cmeel_mim_solvers-0.0.2/python/ddp.cpp` & `cmeel_mim_solvers-0.0.4/bindings/ddp.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 
 namespace bp = boost::python;
 
 BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(SolverDDP_solves, SolverDDP::solve, 0, 5)
 BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(SolverDDP_computeDirections, SolverDDP::computeDirection, 0, 1)
 BOOST_PYTHON_MEMBER_FUNCTION_OVERLOADS(SolverDDP_trySteps, SolverDDP::tryStep, 0, 1)
 
+// Wrapper function to handle deprecation warning upon instantiation
+boost::shared_ptr<SolverDDP> createSolverDDP(boost::shared_ptr<crocoddyl::ShootingProblem> problem) {
+      std::cerr << "Warning: Do not use mim_solvers.SolverDDP !!! " << std::endl;
+      std::cerr << "It may differ significantly from its Crocoddyl counterpart. " << std::endl;
+      std::cerr << "This class served only as a development tool and will be REMOVED in future releases." << std::endl;
+     return boost::make_shared<SolverDDP>(problem);
+}
+
 void exposeSolverDDP() {
   bp::register_ptr_to_python<boost::shared_ptr<SolverDDP> >();
 
   bp::class_<SolverDDP, bp::bases<crocoddyl::SolverAbstract> >(
       "SolverDDP",
       "DDP solver.\n\n"
       "The DDP solver computes an optimal trajectory and control commands by iterates\n"
@@ -33,14 +41,15 @@
       "quadratic approximation of the problem and computes descent direction,\n"
       "and the forward-pass rollouts this new policy by integrating the system dynamics\n"
       "along a tuple of optimized control commands U*.\n"
       ":param shootingProblem: shooting problem (list of action models along trajectory.)",
       bp::init<boost::shared_ptr<crocoddyl::ShootingProblem> >(bp::args("self", "problem"),
                                                     "Initialize the vector dimension.\n\n"
                                                     ":param problem: shooting problem."))
+      .def("__init__", bp::make_constructor(&createSolverDDP))  // Custom constructor
       .def("solve", &SolverDDP::solve,
            SolverDDP_solves(
                bp::args("self", "init_xs", "init_us", "maxiter", "isFeasible", "regInit"),
                "Compute the optimal trajectory xopt, uopt as lists of T+1 and T terms.\n\n"
                "From an initial guess init_xs,init_us (feasible or not), iterate\n"
                "over computeDirection and tryStep until stoppingCriteria is below\n"
                "threshold. It also describes the globalization strategy used\n"
@@ -126,14 +135,12 @@
                     bp::make_function(&SolverDDP::get_alphas, bp::return_value_policy<bp::copy_const_reference>()),
                     bp::make_function(&SolverDDP::set_alphas), "list of step length (alpha) values")
       .def_readwrite("lag_mul", &SolverDDP::lag_mul_, "lagrange multipliers")
       
       .add_property("KKT", bp::make_function(&SolverDDP::get_KKT),
                     "KKT residual norm")
 
-      .add_property("use_kkt_criteria", bp::make_function(&SolverDDP::get_use_kkt_criteria), bp::make_function(&SolverDDP::set_use_kkt_criteria),
-                    "Use the KKT residual condition as a termination criteria (default: True)")
       .add_property("termination_tolerance", bp::make_function(&SolverDDP::get_termination_tolerance), bp::make_function(&SolverDDP::set_termination_tolerance),
                     "Termination criteria to exit the iteration (default: 1e-8)");
 }
 
 }  // namespace mim_solvers
```

### Comparing `cmeel_mim_solvers-0.0.2/python/fddp.cpp` & `cmeel_mim_solvers-0.0.4/bindings/fddp.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -57,16 +57,14 @@
            "Update the expected improvement model\n\n")
       
       .def_readwrite("lag_mul", &SolverFDDP::lag_mul_, "lagrange multipliers")
       
       .add_property("KKT", bp::make_function(&SolverFDDP::get_KKT),
                     "KKT residual norm")
 
-      .add_property("use_kkt_criteria", bp::make_function(&SolverFDDP::get_use_kkt_criteria), bp::make_function(&SolverFDDP::set_use_kkt_criteria),
-                    "Use the KKT residual condition as a termination criteria (default: True)")
       .add_property("termination_tolerance", bp::make_function(&SolverFDDP::get_termination_tolerance), bp::make_function(&SolverFDDP::set_termination_tolerance),
                     "Termination criteria to exit the iteration (default: 1e-6)")
       .add_property("th_acceptNegStep", bp::make_function(&SolverFDDP::get_th_acceptnegstep),
                     bp::make_function(&SolverFDDP::set_th_acceptnegstep),
                     "threshold for step acceptance in ascent direction")
       .add_property("use_filter_line_search", bp::make_function(&SolverFDDP::get_use_filter_line_search), bp::make_function(&SolverFDDP::set_use_filter_line_search),
                     "Use the filter line search criteria (default: False)")
```

### Comparing `cmeel_mim_solvers-0.0.2/python/main.cpp` & `cmeel_mim_solvers-0.0.4/bindings/main.cpp`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/python/py_mim_solvers/sqp.py` & `cmeel_mim_solvers-0.0.4/python/sqp.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,45 +11,42 @@
 
 import crocoddyl
 from crocoddyl import SolverAbstract
 import scipy.linalg as scl
 import collections
 LINE_WIDTH = 100 
 
-VERBOSE = False    
 
 def rev_enumerate(l):
     return reversed(list(enumerate(l)))
 
 
 def raiseIfNan(A, error=None):
     if error is None:
         error = scl.LinAlgError("NaN in array")
     if np.any(np.isnan(A)) or np.any(np.isinf(A)) or np.any(abs(np.asarray(A)) > 1e30):
         raise error
 
 class SQP(SolverAbstract):
-    def __init__(self, shootingProblem, use_filter_ls=True, VERBOSE=False):
+    def __init__(self, shootingProblem, use_filter_line_search=True, with_callbacks=False):
         SolverAbstract.__init__(self, shootingProblem)
-        self.x_reg = 0
-        self.u_reg = 0
-        self.regFactor = 10
-        self.regMax = 1e9
-        self.regMin = 1e-9
-        self.mu = 1e0
-        self.termination_tolerance = 1e-8
+        # self.x_reg = 0
+        # self.u_reg = 0
+        # self.regFactor = 10
+        # self.regMax = 1e9
+        # self.regMin = 1e-9
+        self.mu = 1.
+        self.termination_tolerance = 1e-6
 
 
-        self.use_filter_ls = use_filter_ls
-        self.filter_size = 10
-        self.gap_list = collections.deque(self.filter_size * [np.inf], maxlen=self.filter_size)
-        self.cost_list = collections.deque(self.filter_size * [np.inf], maxlen=self.filter_size)
-
-        self.VERBOSE = VERBOSE
+        self.use_filter_line_search = use_filter_line_search
+        self.filter_size = 1
+        self.with_callbacks = with_callbacks
         
+        self.extra_iteration_for_last_kkt = False
         self.allocateData()
 
     def models(self):
         mod = [m for m in self.problem.runningModels]
         mod += [self.problem.terminalModel]
         return mod  
         
@@ -68,15 +65,14 @@
         self.gap_norm = sum(np.linalg.norm(self.gap.copy(), 1, axis = 1))
 
         self.cost += self.problem.terminalData.cost 
         self.merit =  self.cost + self.mu*self.gap_norm
 
     def computeDirection(self, recalc=True):
         self.calc()
-        self.KKT_check()
         self.backwardPass()  
         self.computeUpdates()
 
         # self.compute_expected_decrease()
 
     def LQ_problem_KKT_check(self):
         KKT = 0
@@ -179,15 +175,15 @@
             Q = data.Lxx
             P = data.Lxu.T
             A = data.Fx
             B = data.Fu 
 
             h = r + B.T@(self.s[t+1] + self.S[t+1]@self.gap[t])
             G = P + B.T@self.S[t+1]@A
-            self.H = R + B.T@self.S[t+1]@B 
+            self.H = R + B.T@self.S[t+1]@B #+ 1e-9 * np.eye(model.nu)
 
             if len(G.shape) == 1:
                 G = np.resize(G,(1,G.shape[0]))
             ## Making sure H is PD
             Lb_uu = scl.cho_factor(self.H, lower=True)
             # while True:
             #     try:
@@ -208,32 +204,45 @@
     def solve(self, init_xs=None, init_us=None, maxiter=100, isFeasible=False, regInit=None):
         #___________________ Initialize ___________________#
         if init_xs is None or len(init_xs) < 1:
             init_xs = [self.problem.x0.copy() for m in self.models()] 
         if init_us is None or len(init_us) < 1:
             init_us = [np.zeros(m.nu) for m in self.problem.runningModels] 
 
-        init_xs[0][:] = self.problem.x0.copy() # Initial condition guess must be x0
+        init_xs[0] = self.problem.x0.copy() # Initial condition guess must be x0
         
-        # self.setCandidate(init_xs, init_us, False)
+        self.gap_list = collections.deque(self.filter_size * [np.inf], maxlen=self.filter_size)
+        self.cost_list = collections.deque(self.filter_size * [np.inf], maxlen=self.filter_size)
+
+        self.setCandidate(init_xs, init_us, False)
+
         alpha = None
-        if (self.VERBOSE):
+        if (self.with_callbacks):
             headings = ["iter", "merit", "cost", "grad", "step", "||gaps||", "KKT"]
             
             print("{:>3} {:>9} {:>10} {:>11} {:>8} {:>11} {:>8}".format(*headings))
         for iter in range(maxiter):
             recalc = True   # this will recalculated derivatives in Compute Direction 
             self.computeDirection(recalc=recalc)
+
+            # self.check_optimality()
+
+            self.KKT_check()
+            if self.KKT < self.termination_tolerance:            
+                if(self.with_callbacks):
+                    print("{:>4} {:.5e} {:.5e} {:.5e} {:.4f} {:.5e} {:.5e}".format(iter, float(self.merit), self.cost, self.x_grad_norm + self.u_grad_norm, alpha, self.gap_norm, self.KKT))
+                return True
+
             self.gap_list.append(self.gap_norm)
             self.cost_list.append(self.cost)
             alpha = 1.
-            max_search = 20
+            max_search = 10
             for k in range(max_search):
                 self.tryStep(alpha)
-                if self.use_filter_ls:
+                if self.use_filter_line_search:
                     is_worse_than_memory = False
                     count = 0
                     while count < self.filter_size and not is_worse_than_memory and count <= iter:
                         is_worse_than_memory = self.cost_list[self.filter_size - 1 - count] < self.cost_try and \
                             self.gap_list[self.filter_size - 1 - count] < self.gap_norm_try
                         count += 1
                         
@@ -246,21 +255,29 @@
                         return False
                     if self.merit > self.merit_try:
                         self.acceptStep()
                         break
 
                 alpha *= 0.5
 
-            # self.check_optimality()
-            if self.KKT < self.termination_tolerance:
-                return True
             
-            if(self.VERBOSE):
+            if(self.with_callbacks):
                 print("{:>4} {:.5e} {:.5e} {:.5e} {:.4f} {:.5e} {:.5e}".format(iter, float(self.merit), self.cost, self.x_grad_norm + self.u_grad_norm, alpha, self.gap_norm, self.KKT))
 
+        if self.extra_iteration_for_last_kkt:
+            recalc = True   # this will recalculated derivatives in Compute Direction 
+            self.computeDirection(recalc=recalc)
+
+            # self.check_optimality()
+
+            self.KKT_check()
+            if self.KKT < self.termination_tolerance:            
+                if(self.with_callbacks):
+                    print("{:>4} {:.5e} {:.5e} {:.5e} {:.4f} {:.5e} {:.5e}".format(iter, float(self.merit), self.cost, self.x_grad_norm + self.u_grad_norm, alpha, self.gap_norm, self.KKT))
+                return True
         return False 
 
     def allocateData(self):
         self.xs_try = [np.zeros(m.state.nx) for m in self.models()] 
         self.xs_try[0][:] = self.problem.x0.copy()
         self.us_try = [np.zeros(m.nu) for m in self.problem.runningModels] 
         #
```

### Comparing `cmeel_mim_solvers-0.0.2/python/sqp.cpp` & `cmeel_mim_solvers-0.0.4/bindings/sqp.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -54,20 +54,20 @@
       .def_readwrite("lag_mul", &SolverSQP::lag_mul_, "lagrange multipliers")
 
       .add_property("KKT", bp::make_function(&SolverSQP::get_KKT),
                     "KKT residual norm")
 
       .add_property("with_callbacks", bp::make_function(&SolverSQP::getCallbacks), bp::make_function(&SolverSQP::setCallbacks),
                     "Activates the callbacks when true (default: False)")
-      .add_property("use_kkt_criteria", bp::make_function(&SolverSQP::get_use_kkt_criteria), bp::make_function(&SolverSQP::set_use_kkt_criteria),
-                    "Use the KKT residual condition as a termination criteria (default: True)")
+      .add_property("extra_iteration_for_last_kkt", bp::make_function(&SolverSQP::get_extra_iteration_for_last_kkt), bp::make_function(&SolverSQP::set_extra_iteration_for_last_kkt),
+                    "Additional iteration if SQP max. iter reached (default: False)")
       .add_property("mu", bp::make_function(&SolverSQP::get_mu), bp::make_function(&SolverSQP::set_mu),
                     "Penalty term for dynamic violation in the merit function (default: 1.)")
       .add_property("use_filter_line_search", bp::make_function(&SolverSQP::get_use_filter_line_search), bp::make_function(&SolverSQP::set_use_filter_line_search),
-                    "Use the filter line search criteria (default: False)")
+                    "Use the filter line search criteria (default: True)")
       .add_property("termination_tolerance", bp::make_function(&SolverSQP::get_termination_tolerance), bp::make_function(&SolverSQP::set_termination_tolerance),
                     "Termination criteria to exit the iteration (default: 1e-6)")
       .add_property("filter_size", bp::make_function(&SolverSQP::get_filter_size), bp::make_function(&SolverSQP::set_filter_size),
                     "filter size for the line-search (default: 1)");
      
 }
```

### Comparing `cmeel_mim_solvers-0.0.2/src/csqp.cpp` & `cmeel_mim_solvers-0.0.4/src/csqp.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -22,121 +22,140 @@
 
 
 SolverCSQP::SolverCSQP(boost::shared_ptr<crocoddyl::ShootingProblem> problem)
     : SolverDDP(problem){
       
       const std::size_t T = this->problem_->get_T();
       const std::size_t ndx = problem_->get_ndx();
-      sigma_diag_x = sigma_* Eigen::MatrixXd::Identity(ndx, ndx);
-      sigma_diag_u.resize(T);
-      Cdx_Cdu.resize(T+1);
       constraint_list_.resize(filter_size_);
       gap_list_.resize(filter_size_);
       cost_list_.resize(filter_size_);
-      fs_try_.resize(T + 1);
+
       fs_flat_.resize(ndx*(T + 1));
       fs_flat_.setZero();
-      lag_mul_.resize(T+1);
+      
+      xs_try_.resize(T+1); 
+      us_try_.resize(T);
+      dx_.resize(T+1); 
       du_.resize(T);
+      dxtilde_.resize(T+1);
+      dutilde_.resize(T);
+      lag_mul_.resize(T+1);
+      fs_try_.resize(T + 1);
       
-      dx_.resize(T+1); dxtilde_.resize(T+1);
-      du_.resize(T); dutilde_.resize(T);
-      z_.resize(T+1); z_relaxed_.resize(T+1); y_.resize(T+1); rho_vec_.resize(T+1); inv_rho_vec_.resize(T+1);
+      z_.resize(T+1); 
+      z_relaxed_.resize(T+1); 
       z_prev_.resize(T+1);
-      xs_try_.resize(T+1); us_try_.resize(T);
-
-      rho_sparse_base_ = rho_sparse_;
+      y_.resize(T+1); 
+      rho_vec_.resize(T+1); 
+      inv_rho_vec_.resize(T+1);
+      rho_sparse_ = rho_sparse_base_;
+      std::size_t n_eq_crocoddyl = 0;
+      
+      tmp_Vx_.resize(ndx); 
+      tmp_Vx_.setZero();
+      tmp_vec_x_.resize(ndx);
+      tmp_vec_x_.setZero();
+
+      tmp_Cdx_Cdu_.resize(T+1);
+      tmp_dual_cwise_.resize(T+1);
+      tmp_rhoGx_mat_.resize(T+1);
+      tmp_rhoGu_mat_.resize(T);
+      tmp_vec_u_.resize(T);
+      Vxx_fs_.resize(T);
 
       const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
       for (std::size_t t = 0; t < T; ++t) {
         const boost::shared_ptr<crocoddyl::ActionModelAbstract>& model = models[t];
         const std::size_t nu = model->get_nu();
-        sigma_diag_u[t] = sigma_ * Eigen::MatrixXd::Identity(nu, nu);
+        std::size_t nc = model->get_ng(); 
+        n_eq_crocoddyl += model->get_nh();
+
         xs_try_[t] = model->get_state()->zero();
         us_try_[t] = Eigen::VectorXd::Zero(nu);
-
-        dx_[t].resize(ndx); du_[t].resize(nu);
-        dxtilde_[t].resize(ndx); dutilde_[t].resize(nu);
-        fs_try_[t].resize(ndx);
-        lag_mul_[t].resize(ndx); 
-        lag_mul_[t].setZero();
-        dx_[t].setZero(); dxtilde_[t].setZero();
+        dx_[t].resize(ndx); 
+        dx_[t].setZero(); 
+        du_[t].resize(nu);
         du_[t] = Eigen::VectorXd::Zero(nu);
+        dxtilde_[t].resize(ndx); 
+        dxtilde_[t].setZero();
+        dutilde_[t].resize(nu);
         dutilde_[t] = Eigen::VectorXd::Zero(nu);
+        lag_mul_[t].resize(ndx); 
+        lag_mul_[t].setZero();
+        fs_try_[t].resize(ndx);
+        fs_try_[t] = Eigen::VectorXd::Zero(ndx);     
 
-        fs_try_[t] = Eigen::VectorXd::Zero(ndx);
-
-        std::size_t nc = model->get_ng(); 
-        Cdx_Cdu[t].resize(nc); Cdx_Cdu[t].setZero();
+        z_[t].resize(nc); 
+        z_[t].setZero();
+        z_relaxed_[t].resize(nc); 
+        z_relaxed_[t].setZero();
+        z_prev_[t].resize(nc); 
+        z_prev_[t].setZero();
+        y_[t].resize(nc); 
+        y_[t].setZero();
 
+        tmp_Cdx_Cdu_[t].resize(nc); 
+        tmp_Cdx_Cdu_[t].setZero();
+        tmp_dual_cwise_[t].resize(nc); 
+        tmp_dual_cwise_[t].setZero();
+        tmp_rhoGx_mat_[t].resize(nc, ndx);  
+        tmp_rhoGx_mat_[t].setZero();
+        tmp_rhoGu_mat_[t].resize(nc, nu);   
+        tmp_rhoGu_mat_[t].setZero();
+        tmp_vec_u_[t].resize(nu); 
+        tmp_vec_u_[t].setZero();
+        Vxx_fs_[t].resize(ndx);
+        Vxx_fs_[t].setZero();
 
-        z_[t].resize(nc); z_[t].setZero();
-        z_prev_[t].resize(nc); z_prev_[t].setZero();
-        z_relaxed_[t].resize(nc); z_relaxed_[t].setZero();
-        y_[t].resize(nc); y_[t].setZero();
         rho_vec_[t].resize(nc); 
         inv_rho_vec_[t].resize(nc); 
-
-        auto lb = model->get_g_lb(); 
-        auto ub = model->get_g_ub();
-        double infty = std::numeric_limits<double>::infinity();
-
-        for (std::size_t k = 0; k < nc; ++k){
-          if (lb[k] == -infty && ub[k] == infty){
-              rho_vec_[t][k] = rho_min_;
-              inv_rho_vec_[t][k] = 1.0/rho_min_;
-          }
-          else if (abs(lb[k] - ub[k]) <= 1e-6){
-              rho_vec_[t][k] = 1e3 * rho_sparse_;
-              inv_rho_vec_[t][k] = 1/(1e3 * rho_sparse_);
-
-          }
-          else if (lb[k] < ub[k]){
-              rho_vec_[t][k] = rho_sparse_;
-              inv_rho_vec_[t][k] = rho_sparse_;
-
-          }
-        }
       }
 
       xs_try_.back() = problem_->get_terminalModel()->get_state()->zero();
-
+      dx_.back().resize(ndx); 
+      dx_.back().setZero(); 
+      dxtilde_.back().resize(ndx);
+      dxtilde_.back().setZero();
       lag_mul_.back().resize(ndx);
       lag_mul_.back().setZero();
-      dx_.back().resize(ndx); dxtilde_.back().resize(ndx);
-      dx_.back().setZero(); dxtilde_.back().setZero();
       fs_try_.back().resize(ndx);
       fs_try_.back() = Eigen::VectorXd::Zero(ndx);
 
-      // Constraint Models
       std::size_t nc = problem_->get_terminalModel()->get_ng(); 
-      z_.back().resize(nc); z_.back().setZero();
-      z_prev_.back().resize(nc); z_prev_.back().setZero();
-      z_relaxed_.back().resize(nc); z_relaxed_.back().setZero();
-      y_.back().resize(nc); y_.back().setZero();
+
+      z_.back().resize(nc); 
+      z_.back().setZero();
+      z_relaxed_.back().resize(nc); 
+      z_relaxed_.back().setZero();
+      z_prev_.back().resize(nc); 
+      z_prev_.back().setZero();
+      y_.back().resize(nc); 
+      y_.back().setZero();
+
+      tmp_Cdx_Cdu_.back().resize(nc); 
+      tmp_Cdx_Cdu_.back().setZero();
+      tmp_dual_cwise_.back().resize(nc);
+      tmp_dual_cwise_.back().setZero();
+      tmp_rhoGx_mat_.back().resize(nc, ndx);
+      tmp_rhoGx_mat_.back().setZero();
+
+      
       rho_vec_.back().resize(nc);
       inv_rho_vec_.back().resize(nc);
 
-      for (std::size_t k = 0; k < nc; ++k){
-        auto lb = problem_->get_terminalModel()->get_g_lb(); 
-        auto ub = problem_->get_terminalModel()->get_g_ub();
-        double infty = std::numeric_limits<double>::infinity();
-        if (lb[k] == -infty && ub[k] == infty){
-            rho_vec_.back()[k] = rho_min_;
-            inv_rho_vec_.back()[k] = 1/rho_min_;
-        }
-        else if (abs(lb[k] - ub[k]) <= 1e-6){
-            rho_vec_.back()[k] = 1e3 * rho_sparse_;
-            inv_rho_vec_.back()[k] = 1/(1e3 * rho_sparse_);
-        }
-        else if (lb[k] < ub[k]){
-            rho_vec_.back()[k] = rho_sparse_;
-            inv_rho_vec_.back()[k] = 1/rho_sparse_;
-        }
-      }
+
+      // Check that no equality constraint was specified through Crocoddyl's API
+      n_eq_crocoddyl += problem_->get_terminalModel()->get_nh(); 
+      if(n_eq_crocoddyl != 0){
+        throw_pretty("Error: nh must be zero !!! Crocoddyl's equality constraints API is not supported by mim_solvers.\n"
+                     "  >> Equality constraints of the form H(x,u) = h must be implemented as g <= G(x,u) <= g by specifying \n"
+                     "     lower and upper bounds in the constructor of the constraint model residual or by setting g_ub and g_lb.")
+      } 
+
 
       const std::size_t n_alphas = 10;
       alphas_.resize(n_alphas);
       for (std::size_t n = 0; n < n_alphas; ++n) {
         alphas_[n] = 1. / pow(2., static_cast<double>(n));
       }
       if (th_stepinc_ < alphas_[n_alphas - 1]) {
@@ -144,197 +163,210 @@
         std::cerr << "Warning: th_stepinc has higher value than lowest alpha value, set to "
                   << std::to_string(alphas_[n_alphas - 1]) << std::endl;
       }
     }
 
 
 
+
+
+
 void SolverCSQP::reset_params(){
 
-  rho_sparse_ = rho_sparse_base_;
+  if (reset_rho_){
+    reset_rho_vec();
+  }
   
   const std::size_t T = this->problem_->get_T();
-  const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
-    for (std::size_t t = 0; t < T; ++t) {
-      const boost::shared_ptr<crocoddyl::ActionModelAbstract>& model = models[t];
-      std::size_t nc = model->get_ng();
-      z_[t].setZero();
-      z_prev_[t].setZero();
-      z_relaxed_[t].setZero();
-      
-      // Warm start y
-      if(!warm_start_y_){
-        y_[t].setZero();
-      } 
-        
-      auto lb = model->get_g_lb(); 
-      auto ub = model->get_g_ub();
-      double infty = std::numeric_limits<double>::infinity();
-
-      // Reset rho
-      if(reset_rho_){
-        for (std::size_t k = 0; k < nc; ++k){
-          if (lb[k] == -infty && ub[k] == infty){
-              rho_vec_[t][k] = rho_min_;
-              inv_rho_vec_[t][k] = 1/rho_min_;
 
-          }
-          else if (abs(lb[k] - ub[k]) <= 1e-6){
-              rho_vec_[t][k] = 1e3 * rho_sparse_;
-              inv_rho_vec_[t][k] = 1.0/(1e3 * rho_sparse_);
-          }
-          else if (lb[k] < ub[k]){
-              rho_vec_[t][k] = rho_sparse_;
-              inv_rho_vec_[t][k] = 1/rho_sparse_;
+  for (std::size_t t = 0; t < T; ++t) {
 
-          }
-        }
-      }
+    z_[t].setZero();
+    z_prev_[t].setZero();
+    z_relaxed_[t].setZero();
+
+    if(reset_y_){
+      y_[t].setZero();
+    } 
+  }
+  z_.back().setZero();
+  z_prev_.back().setZero();
+  z_relaxed_.back().setZero();
 
-    }
-    const boost::shared_ptr<crocoddyl::ActionModelAbstract>& model = problem_->get_terminalModel();
-    lag_mul_.back().setZero();
-    std::size_t nc = model->get_ng();
-    z_.back().setZero();
-    z_prev_.back().setZero();
-    z_relaxed_.back().setZero();
-    // Warm-start y
-    if(!warm_start_y_){
-      y_.back().setZero();
-    }
-    // Reset rho
-    if(reset_rho_){
-      for (std::size_t k = 0; k < nc; ++k){
-        auto lb = problem_->get_terminalModel()->get_g_lb(); 
-        auto ub = problem_->get_terminalModel()->get_g_ub();
-        double infty = std::numeric_limits<double>::infinity();
-        if (lb[k] == -infty && ub[k] == infty){
-            rho_vec_.back()[k] = rho_min_;
-            inv_rho_vec_.back()[k] = 1/rho_min_;
-        }
-        else if (abs(lb[k] - ub[k]) <= 1e-6){
-            rho_vec_.back()[k] = 1e3 * rho_sparse_;
-            inv_rho_vec_.back()[k] = 1/(1e3 * rho_sparse_);
-        }
-        else if (lb[k] < ub[k]){
-            rho_vec_.back()[k] = rho_sparse_;
-            inv_rho_vec_.back()[k] = 1/rho_sparse_;
-        }
-      }
-    }
+  if(reset_y_){
+    y_.back().setZero();
+  }
 }
 
+
 SolverCSQP::~SolverCSQP() {}
 
 bool SolverCSQP::solve(const std::vector<Eigen::VectorXd>& init_xs, const std::vector<Eigen::VectorXd>& init_us,
                        const std::size_t maxiter, const bool is_feasible, const double reginit) {
   
   (void)is_feasible;
-  (void)reginit;
 
   START_PROFILER("SolverCSQP::solve");
   if (problem_->is_updated()) {
     resizeData();
   }
   setCandidate(init_xs, init_us, false);
   xs_[0] = problem_->get_x0();      // Otherwise xs[0] is overwritten by init_xs inside setCandidate()
   xs_try_[0] = problem_->get_x0();  // it is needed in case that init_xs[0] is infeasible
 
-  // REMOVED REGULARIZATION : 
-  // if (std::isnan(reginit)) {
-  //   xreg_ = reg_min_;
-  //   ureg_ = reg_min_;
-  // } else {
-  //   xreg_ = reginit;
-  //   ureg_ = reginit;
-  // }
+  // Optionally remove Crocoddyl's regularization
+  if(remove_reg_){
+    preg_ = 0.;
+    dreg_ = 0;
+  } 
+  else {
+    if (std::isnan(reginit)) {
+      preg_ = reg_min_;
+      dreg_ = reg_min_;
+    } else {
+      preg_ = reginit;
+      dreg_ = reginit;
+    }
+  }
 
+  // Main SQP loop
   for (iter_ = 0; iter_ < maxiter; ++iter_) {
 
+    // Compute gradients
+    calc(true);
 
-    was_feasible_ = false;
-    bool recalcDiff = true;
-    // computeDirection(recalcDiff);
-
-    while (true) {
-      try {
-        computeDirection(recalcDiff);
-      } 
-      catch (std::exception& e) {
-        recalcDiff = false;
-        increaseRegularization();
-        if (xreg_ == reg_max_) {
-          return false;
-        } else {
-          continue;
+    // reset rho only at the beginning of each solve if reset_rho_ is false 
+    // (after calc to get correct lb and ub)
+    if (iter_ == 0 && !reset_rho_){
+      reset_rho_vec();
+    }
+
+    // Solve QP
+    if(remove_reg_){
+      computeDirection(true);
+    } else {
+      while (true) {
+        try {
+          computeDirection(true);
+        } 
+        catch (std::exception& e) {
+          increaseRegularization();
+          if (preg_ == reg_max_) {
+            return false;
+          } else {
+            continue;
+          }
         }
+        break;
       }
-      break;
     }
 
-    // KKT termination criteria
-    if(use_kkt_criteria_){
-      if (KKT_  <= termination_tol_) {
-        STOP_PROFILER("SolverCSQP::solve");
-        return true;
+    // Check KKT criteria
+    checkKKTConditions();
+    if (KKT_  <= termination_tol_) {
+      if(with_callbacks_){
+        printCallbacks();
       }
-    }  
+      STOP_PROFILER("SolverCSQP::solve");
+      return true;
+    }
+  
 
+    // Line search
     constraint_list_.push_back(constraint_norm_);
     gap_list_.push_back(gap_norm_);
     cost_list_.push_back(cost_);
-
     // We need to recalculate the derivatives when the step length passes
     for (std::vector<double>::const_iterator it = alphas_.begin(); it != alphas_.end(); ++it) {
       steplength_ = *it;
       try {
         merit_try_ = tryStep(steplength_);
       } catch (std::exception& e) {
         continue;
       }
       // Filter line search criteria 
-      // Equivalent to heuristic cost_ > cost_try_ || gap_norm_ > gap_norm_try_ when filter_size=1
       if(use_filter_line_search_){
         is_worse_than_memory_ = false;
         std::size_t count = 0.; 
         while( count < filter_size_ && is_worse_than_memory_ == false and count <= iter_){
           is_worse_than_memory_ = cost_list_[filter_size_-1-count] <= cost_try_ && gap_list_[filter_size_-1-count] <= gap_norm_try_ && constraint_list_[filter_size_-1-count] <= constraint_norm_try_;
           count++;
         }
         if( is_worse_than_memory_ == false ) {
           setCandidate(xs_try_, us_try_, false);
-          recalcDiff = true;
           break;
         } 
       }
       // Line-search criteria using merit function
       else{
         if (merit_ > merit_try_) {
           setCandidate(xs_try_, us_try_, false);
-          recalcDiff = true;
           break;
         }
       }
     }
 
-    if (steplength_ > th_stepdec_) {
-      decreaseRegularization();
-    }
-    if (steplength_ <= th_stepinc_) {
-      increaseRegularization();
-      if (xreg_ == reg_max_) {
-        STOP_PROFILER("SolverCSQP::solve");
-        return false;
+    // Regularization logic
+    if(remove_reg_ == false){
+      if (steplength_ > th_stepdec_) {
+        decreaseRegularization();
+      }
+      if (steplength_ <= th_stepinc_) {
+        increaseRegularization();
+        if (preg_ == reg_max_) {
+          STOP_PROFILER("SolverCSQP::solve");
+          return false;
+        }
       }
     }
 
+    // Print
     if(with_callbacks_){
       printCallbacks();
     }
   }
+
+  // If reached max iter, still compute KKT residual
+  if (extra_iteration_for_last_kkt_){
+    // Compute gradients
+    calc(true);
+
+    // Solve QP
+    if(remove_reg_){
+      computeDirection(true);
+    } else {
+      while (true) {
+        try {
+          computeDirection(true);
+        } 
+        catch (std::exception& e) {
+          increaseRegularization();
+          if (preg_ == reg_max_) {
+            return false;
+          } else {
+            continue;
+          }
+        }
+        break;
+      }
+    }    
+
+    // Check KKT criteria
+    checkKKTConditions();
+    if(with_callbacks_){
+      printCallbacks(true);
+    }
+
+    if (KKT_  <= termination_tol_) {
+      STOP_PROFILER("SolverCSQP::solve");
+      return true;
+    }
+  
+  }
+
   STOP_PROFILER("SolverCSQP::solve");
   return false;
 }
 
 
 void SolverCSQP::calc(const bool recalc){
   if (recalc){
@@ -377,269 +409,331 @@
 
   merit_ = cost_ + mu_*gap_norm_ + mu2_*constraint_norm_;
 
 }
 
 
 void SolverCSQP::computeDirection(const bool recalcDiff){
+
   START_PROFILER("SolverCSQP::computeDirection");
-  if (recalcDiff) {
-    calc(recalcDiff);
-  }
-  if(use_kkt_criteria_){
-    checkKKTConditions();
-  }
 
-  if (warm_start_){
-    reset_params();
+  (void)recalcDiff;
+
+  reset_params();
+
+  if (equality_qp_initial_guess_){
     backwardPass_without_constraints();
-    forwardPass();
-    update_lagrangian_parameters(false);
+    forwardPass_without_constraints();
+  }
+
+  if(with_qp_callbacks_){
+    printQPCallbacks(0);
   }
   bool converged_ = false;
   for (std::size_t iter = 1; iter < max_qp_iters_+1; ++iter){
     if (iter % rho_update_interval_ == 1 || iter == 1){
       backwardPass();
     }
     else{
       backwardPass_without_rho_update();
     }
     forwardPass();
-    update_lagrangian_parameters(true);
-    update_rho_sparse(iter);
-    if(norm_primal_ <= eps_abs_ + eps_rel_ * norm_primal_rel_ && norm_dual_ <= eps_abs_ + eps_rel_ * norm_dual_rel_){
+    update_lagrangian_parameters();
+    update_rho_vec(iter);
+    // Because (eps_rel=0) x inf = NaN
+    if(eps_rel_ == 0){
+      norm_primal_tolerance_ = eps_abs_;
+      norm_dual_tolerance_   = eps_abs_;
+    } 
+    else{
+      norm_primal_tolerance_ = eps_abs_ + eps_rel_ * norm_primal_rel_;
+      norm_dual_tolerance_   = eps_abs_ + eps_rel_ * norm_dual_rel_;
+    }
+    if(norm_primal_ <= norm_primal_tolerance_ && norm_dual_ <= norm_dual_tolerance_){
         qp_iters_ = iter;
         converged_ = true;
         break;
     }
-
-    // std::cout << "Iters " << iter << " res-primal " << norm_primal_ << " res-dual " << norm_dual_ << " optimal rho estimate " << rho_estimate_sparse_
-    //         << " rho " << rho_sparse_ << std::endl;
+    if(with_qp_callbacks_){
+      printQPCallbacks(iter);
+    }
   }
 
   if (!converged_){
     qp_iters_ = max_qp_iters_;
   }
 
   STOP_PROFILER("SolverCSQP::computeDirection");
 
 }
 
-
-void SolverCSQP::update_rho_sparse(int iter){
+void SolverCSQP::update_rho_vec(int iter){
   double scale = (norm_primal_ * norm_dual_rel_)/ (norm_dual_ * norm_primal_rel_);
   scale = std::sqrt(scale);
   rho_estimate_sparse_ = scale * rho_sparse_;
   rho_estimate_sparse_ = std::min(std::max(rho_estimate_sparse_, rho_min_), rho_max_);
 
+
   if (iter % rho_update_interval_ == 0 && iter > 1){
     if(rho_estimate_sparse_ > rho_sparse_ * adaptive_rho_tolerance_ || 
             rho_estimate_sparse_ < rho_sparse_ / adaptive_rho_tolerance_){
       rho_sparse_ = rho_estimate_sparse_;
-      const std::size_t T = problem_->get_T();
-      // Running models
-      for (std::size_t t = 0; t < T; ++t){
-        const boost::shared_ptr<crocoddyl::ActionModelAbstract>& model = problem_->get_runningModels()[t];
-        std::size_t nc = model->get_ng();
-        auto lb = model->get_g_lb(); 
-        auto ub = model->get_g_ub();
-        double infty = std::numeric_limits<double>::infinity();
-
-        for (std::size_t k = 0; k < nc; ++k){
-          if (lb[k] == -infty && ub[k] == infty){
-              rho_vec_[t][k] = rho_min_;
-              inv_rho_vec_[t][k] = 1/rho_min_;
-          }
-          else if (abs(lb[k] - ub[k]) < 1e-6) {
-              rho_vec_[t][k] = 1e3 * rho_sparse_;
-              inv_rho_vec_[t][k] = 1/(1e3 * rho_sparse_);
-          }
-          else if (lb[k] < ub[k]){
-              rho_vec_[t][k] = rho_sparse_;
-              inv_rho_vec_[t][k] = 1/rho_sparse_;
-          }
-        }  
+      apply_rho_update(rho_sparse_);
+    }  
+  }
+}
+
+
+void SolverCSQP::reset_rho_vec(){
+  rho_sparse_ = rho_sparse_base_;
+  apply_rho_update(rho_sparse_);
+}
+
+
+void SolverCSQP::apply_rho_update(double rho_sparse_){
+  const std::size_t T = this->problem_->get_T();
+  const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
+  double infty = std::numeric_limits<double>::infinity();
+
+  for (std::size_t t = 0; t < T; ++t) {
+
+    const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m = models[t];
+    std::size_t nc = m->get_ng();
+    const auto ub = m->get_g_ub(); 
+    const auto lb = m->get_g_lb();
+
+    for (std::size_t k = 0; k < nc; ++k){
+      if (lb[k] == -infty && ub[k] == infty){
+          rho_vec_[t][k] = rho_min_;
+          inv_rho_vec_[t][k] = 1/rho_min_;
+      }
+      else if (abs(lb[k] - ub[k]) <= 1e-6){
+          rho_vec_[t][k] = 1e3 * rho_sparse_;
+          inv_rho_vec_[t][k] = 1.0/(1e3 * rho_sparse_);
+      }
+      else if (lb[k] < ub[k]){
+          rho_vec_[t][k] = rho_sparse_;
+          inv_rho_vec_[t][k] = 1/rho_sparse_;
       }
+    }
+  }
 
-      // Terminal model
-      const boost::shared_ptr<crocoddyl::ActionModelAbstract>& model = problem_->get_terminalModel();
-      std::size_t nc = model->get_ng();
-      auto lb = model->get_g_lb(); 
-      auto ub = model->get_g_ub();
-      double infty = std::numeric_limits<double>::infinity();
-      for (std::size_t k = 0; k < nc; ++k){
-        if (lb[k] == -infty && ub[k] == infty){
-            rho_vec_.back()[k] = rho_min_;
-            inv_rho_vec_.back()[k] = 1/rho_min_;
-        }
-        else if (abs(lb[k] - ub[k]) < 1e-6) {
-            rho_vec_.back()[k] = 1e3 * rho_sparse_;
-            inv_rho_vec_.back()[k] = 1/(1e3 * rho_sparse_);
-        }
-        else if (lb[k] < ub[k]){
-            rho_vec_.back()[k] = rho_sparse_;
-            inv_rho_vec_.back()[k] = 1/rho_sparse_;
-        }
-      }  
+  std::size_t nc = problem_->get_terminalModel()->get_ng();
+  auto lb = problem_->get_terminalModel()->get_g_lb(); 
+  auto ub = problem_->get_terminalModel()->get_g_ub();
+  
+  for (std::size_t k = 0; k < nc; ++k){
+    if (lb[k] == -infty && ub[k] == infty){
+        rho_vec_.back()[k] = rho_min_;
+        inv_rho_vec_.back()[k] = 1/rho_min_;
+    }
+    else if (abs(lb[k] - ub[k]) <= 1e-6){
+        rho_vec_.back()[k] = 1e3 * rho_sparse_;
+        inv_rho_vec_.back()[k] = 1/(1e3 * rho_sparse_);
+    }
+    else if (lb[k] < ub[k]){
+        rho_vec_.back()[k] = rho_sparse_;
+        inv_rho_vec_.back()[k] = 1/rho_sparse_;
     }
   }
 }
 
 void SolverCSQP::checkKKTConditions(){
   KKT_ = 0.;
   const std::size_t T = problem_->get_T();
+
+  for (std::size_t t = 0; t < T; ++t) {
+    lag_mul_[t].noalias() = Vx_[t];
+    lag_mul_[t].noalias() += Vxx_[t] * dxtilde_[t];
+  }
+  lag_mul_.back().noalias() = Vx_.back();
+  lag_mul_.back().noalias() += Vxx_.back() * dxtilde_.back() ;
   const std::size_t ndx = problem_->get_ndx();
-  const std::vector<boost::shared_ptr<crocoddyl::ActionDataAbstract> >& datas = problem_->get_runningDatas();
+  const std::vector<boost::shared_ptr<ActionDataAbstract> >& datas = problem_->get_runningDatas();
   for (std::size_t t = 0; t < T; ++t) {
-    const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d = datas[t];
+    const boost::shared_ptr<ActionDataAbstract>& d = datas[t];
+    tmp_vec_x_ = d->Lx;
+    tmp_vec_x_.noalias() += d->Fx.transpose() * lag_mul_[t+1];
+    tmp_vec_x_ -= lag_mul_[t];
     if (t > 0){
-      KKT_ = std::max(KKT_, (d->Lu + d->Fu.transpose() * lag_mul_[t+1] + d->Gu.transpose() * y_[t]).lpNorm<Eigen::Infinity>());
+      tmp_vec_x_.noalias() += d->Gx.transpose() * y_[t];
     }
-    KKT_ = std::max(KKT_, (d->Lx + d->Fx.transpose() * lag_mul_[t+1] - lag_mul_[t] + d->Gx.transpose() * y_[t]).lpNorm<Eigen::Infinity>());
+    KKT_ = std::max(KKT_, tmp_vec_x_.lpNorm<Eigen::Infinity>());
+    tmp_vec_u_[t] = d->Lu;
+    tmp_vec_u_[t].noalias() += d->Fu.transpose() * lag_mul_[t+1];
+    tmp_vec_u_[t].noalias() += d->Gu.transpose() * y_[t];
+    KKT_ = std::max(KKT_, tmp_vec_u_[t].lpNorm<Eigen::Infinity>());
     fs_flat_.segment(t*ndx, ndx) = fs_[t];
   }
   fs_flat_.tail(ndx) = fs_.back();
-  const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d_ter = problem_->get_terminalData();
-  KKT_ = std::max(KKT_, (d_ter->Lx - lag_mul_.back() + d_ter->Gx.transpose() * y_.back()).lpNorm<Eigen::Infinity>());
+  const boost::shared_ptr<ActionDataAbstract>& d_ter = problem_->get_terminalData();
+  tmp_vec_x_ = d_ter->Lx;
+  tmp_vec_x_ -= lag_mul_.back();
+  tmp_vec_x_ += d_ter->Gx.transpose() * y_.back();
+  KKT_ = std::max(KKT_, tmp_vec_x_.lpNorm<Eigen::Infinity>());
   KKT_ = std::max(KKT_, fs_flat_.lpNorm<Eigen::Infinity>());
   KKT_ = std::max(KKT_, constraint_norm_);
 }
 
 
-void SolverCSQP::forwardPass(){
+void SolverCSQP::forwardPass(const double stepLength){
+
+    (void)stepLength;
+
     START_PROFILER("SolverCSQP::forwardPass");
-    x_grad_norm_ = 0; u_grad_norm_ = 0;
+    x_grad_norm_ = 0; 
+    u_grad_norm_ = 0;
 
     const std::size_t T = problem_->get_T();
     const std::vector<boost::shared_ptr<crocoddyl::ActionDataAbstract> >& datas = problem_->get_runningDatas();
     for (std::size_t t = 0; t < T; ++t) {
       const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d = datas[t];
-      lag_mul_[t] = Vxx_[t] * dxtilde_[t] + Vx_[t];
-      dutilde_[t].noalias() = -K_[t]*(dxtilde_[t]) - k_[t];
-      dxtilde_[t+1].noalias() = (d->Fx - (d->Fu * K_[t]))*(dxtilde_[t]) - (d->Fu * (k_[t])) + fs_[t+1];
-      
-      x_grad_norm_ += dxtilde_[t].lpNorm<1>(); // assuming that there is no gap in the initial state
+
+      dutilde_[t].noalias() = -K_[t] * dxtilde_[t];
+      dutilde_[t].noalias() -= k_[t];
+      dxtilde_[t+1].noalias() = d->Fx * dxtilde_[t];
+      dxtilde_[t+1].noalias() += d->Fu * dutilde_[t];
+      dxtilde_[t+1].noalias() += fs_[t+1];
+
+      x_grad_norm_ += dxtilde_[t].lpNorm<1>(); 
       u_grad_norm_ += dutilde_[t].lpNorm<1>();
     }
-    
-    lag_mul_.back() = Vxx_.back() * dxtilde_.back() + Vx_.back();
 
-    x_grad_norm_ += dxtilde_.back().lpNorm<1>(); // assuming that there is no gap in the initial state
+    x_grad_norm_ += dxtilde_.back().lpNorm<1>(); 
     x_grad_norm_ = x_grad_norm_/(T+1);
     u_grad_norm_ = u_grad_norm_/T; 
     STOP_PROFILER("SolverCSQP::forwardPass");
 
 }
 
+
+void SolverCSQP::forwardPass_without_constraints(){
+    START_PROFILER("SolverCSQP::forwardPass_without_constraints");
+
+    const std::size_t T = problem_->get_T();
+    const std::vector<boost::shared_ptr<crocoddyl::ActionDataAbstract> >& datas = problem_->get_runningDatas();
+    for (std::size_t t = 0; t < T; ++t) {
+      const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d = datas[t];
+
+      du_[t].noalias() = -K_[t] * dx_[t];
+      du_[t].noalias() -= k_[t];
+      dx_[t+1].noalias() = d->Fx * dx_[t];
+      dx_[t+1].noalias() += d->Fu * du_[t];
+      dx_[t+1].noalias() += fs_[t+1];
+    }
+
+    STOP_PROFILER("SolverCSQP::forwardPass_without_constraints");
+
+}
+
+
+
 void SolverCSQP::backwardPass() {
   START_PROFILER("SolverCSQP::backwardPass");
 
   const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d_T = problem_->get_terminalData();
 
-  Vxx_.back() = d_T->Lxx + sigma_diag_x;
-  Vx_.back() = d_T->Lx - sigma_ * dx_.back();
-
-  if (problem_->get_terminalModel()->get_ng()){ // constraint model
-    // TODO : make sure this is not used later
-    Vxx_.back().noalias() += d_T->Gx.transpose() * rho_vec_.back().asDiagonal() * d_T->Gx;
-    Vx_.back() += d_T->Gx.transpose() * (y_.back() - rho_vec_.back().cwiseProduct(z_.back()));
+  Vxx_.back() = d_T->Lxx; 
+  Vxx_.back().diagonal().array() += sigma_;
+  Vx_.back() = d_T->Lx;
+  Vx_.back().noalias() -= sigma_ * dx_.back();
+
+  if (problem_->get_terminalModel()->get_ng()){ 
+    tmp_rhoGx_mat_.back().noalias() = rho_vec_.back().asDiagonal() * d_T->Gx;
+    Vxx_.back().noalias() += d_T->Gx.transpose() * tmp_rhoGx_mat_.back();
+    tmp_dual_cwise_.back() = y_.back() - rho_vec_.back().cwiseProduct(z_.back());
+    Vx_.back() += d_T->Gx.transpose() * tmp_dual_cwise_.back();
   }
-  if (!std::isnan(xreg_)) {
-    Vxx_.back().diagonal().array() += xreg_;
+  if (!std::isnan(preg_)) {
+    Vxx_.back().diagonal().array() += preg_;
   }
 
-  // if (!is_feasible_) {
-  //   Vx_.back().noalias() += Vxx_.back() * fs_.back();
-  // }
-
-
 
   const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
   const std::vector<boost::shared_ptr<crocoddyl::ActionDataAbstract> >& datas = problem_->get_runningDatas();
   for (int t = static_cast<int>(problem_->get_T()) - 1; t >= 0; --t) {
     const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m = models[t];
     const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d = datas[t];
     const Eigen::MatrixXd& Vxx_p = Vxx_[t + 1];
-    const Eigen::VectorXd& Vx_p = Vx_[t + 1] + Vxx_[t+1] * fs_[t+1];
+
+    Vxx_fs_[t].noalias() = Vxx_[t+1] * fs_[t+1];
+    tmp_Vx_ = Vxx_fs_[t] + Vx_[t + 1];
+
     const std::size_t nu = m->get_nu();
     std::size_t nc = m->get_ng();
     FxTVxx_p_.noalias() = d->Fx.transpose() * Vxx_p;
     START_PROFILER("SolverCSQP::Qx");
-    Qx_[t] = d->Lx - sigma_ * dx_[t];
-
-    if (t > 0 && nc != 0){ //constraint model
-      Qx_[t] += d->Gx.transpose() * (y_[t] -  rho_vec_[t].cwiseProduct(z_[t]));
+    Qx_[t] = d->Lx;
+    Qx_[t].noalias() -= sigma_ * dx_[t];
+    if (t > 0 && nc != 0){ 
+      tmp_dual_cwise_[t] = y_[t] - rho_vec_[t].cwiseProduct(z_[t]);
+      Qx_[t] += d->Gx.transpose() * tmp_dual_cwise_[t];
     }
-    
-    Qx_[t].noalias() += d->Fx.transpose() * Vx_p;
+    Qx_[t].noalias() += d->Fx.transpose() * tmp_Vx_;
     STOP_PROFILER("SolverCSQP::Qx");
-    START_PROFILER("SolverCSQP::Qxx");
-    Qxx_[t] = d->Lxx + sigma_diag_x;
-    if (t > 0 && nc != 0){ //constraint model
-      Qxx_[t].noalias() += d->Gx.transpose() * rho_vec_[t].asDiagonal() * d->Gx;
 
+    START_PROFILER("SolverCSQP::Qxx");
+    Qxx_[t] = d->Lxx; 
+    Qxx_[t].diagonal().array() += sigma_;
+    if (t > 0 && nc != 0){ 
+      tmp_rhoGx_mat_[t].noalias() = rho_vec_[t].asDiagonal() * d->Gx;
+      Qxx_[t].noalias() += d->Gx.transpose() * tmp_rhoGx_mat_[t];
     }
-
     Qxx_[t].noalias() += FxTVxx_p_ * d->Fx;
     STOP_PROFILER("SolverCSQP::Qxx");
+
     if (nu != 0) {
-      FuTVxx_p_[t].noalias() = d->Fu.transpose() * Vxx_p;
       START_PROFILER("SolverCSQP::Qu");
+      FuTVxx_p_[t].noalias() = d->Fu.transpose() * Vxx_p;
       Qu_[t] = d->Lu - sigma_ * du_[t];
-      if (nc != 0){ //constraint model
-        Qu_[t] += d->Gu.transpose() * (y_[t] - rho_vec_[t].cwiseProduct(z_[t]));
+      if (nc != 0){ 
+        tmp_dual_cwise_[t] = y_[t] - rho_vec_[t].cwiseProduct(z_[t]);
+        Qu_[t] += d->Gu.transpose() * tmp_dual_cwise_[t];
       }
-      
-
-      Qu_[t].noalias() += d->Fu.transpose() * Vx_p;
-
+      Qu_[t].noalias() += d->Fu.transpose() * tmp_Vx_;
       STOP_PROFILER("SolverCSQP::Qu");
-      START_PROFILER("SolverCSQP::Quu");
-      Quu_[t] = d->Luu + sigma_diag_u[t];
-      if (nc != 0){ //constraint model
-        Quu_[t].noalias() += d->Gu.transpose() * rho_vec_[t].asDiagonal() * d->Gu;
-      }
 
+      START_PROFILER("SolverCSQP::Quu");
+      Quu_[t] = d->Luu; 
+      Quu_[t].diagonal().array() += sigma_;
       Quu_[t].noalias() += FuTVxx_p_[t] * d->Fu;
+      if (nc != 0){ 
+        tmp_rhoGu_mat_[t].noalias() = rho_vec_[t].asDiagonal() * d->Gu;
+        Quu_[t].noalias() += d->Gu.transpose() * tmp_rhoGu_mat_[t];
+      }
       STOP_PROFILER("SolverCSQP::Quu");
+
       START_PROFILER("SolverCSQP::Qxu");
-      Qxu_[t] = d->Lxu; // TODO : check if this should also have added terms
-      if (nc != 0){ //constraint model
-        Qxu_[t].noalias() += d->Gx.transpose() * rho_vec_[t].asDiagonal() * d->Gu;
+      Qxu_[t] = d->Lxu;
+      if (t > 0 && nc != 0){ 
+        Qxu_[t].noalias() += d->Gx.transpose() * tmp_rhoGu_mat_[t];
       }
-
-
       Qxu_[t].noalias() += FxTVxx_p_ * d->Fu;
       STOP_PROFILER("SolverCSQP::Qxu");
 
-      if (!std::isnan(ureg_)) {
-        Quu_[t].diagonal().array() += ureg_;
+      if (!std::isnan(dreg_)) {
+        Quu_[t].diagonal().array() += dreg_;
       }
     }
     computeGains(t);
     Vx_[t] = Qx_[t];
     Vxx_[t] = Qxx_[t];
     if (nu != 0) {
       Quuk_[t].noalias() = Quu_[t] * k_[t];
       Vx_[t].noalias() -= K_[t].transpose() * Qu_[t];
       START_PROFILER("SolverCSQP::Vxx");
       Vxx_[t].noalias() -= Qxu_[t] * K_[t];
       STOP_PROFILER("SolverCSQP::Vxx");
     }
     Vxx_tmp_ = 0.5 * (Vxx_[t] + Vxx_[t].transpose());
     Vxx_[t] = Vxx_tmp_;
-    if (!std::isnan(xreg_)) {
-      Vxx_[t].diagonal().array() += xreg_;
+    if (!std::isnan(preg_)) {
+      Vxx_[t].diagonal().array() += preg_;
     }
 
-    // Compute and store the Vx gradient at end of the interval (rollout state)
-    // if (!is_feasible_) {
-    //   Vx_[t].noalias() += Vxx_[t] * fs_[t];
-    // }
-
     if (raiseIfNaN(Vx_[t].lpNorm<Eigen::Infinity>())) {
       throw_pretty("backward_error");
     }
     if (raiseIfNaN(Vxx_[t].lpNorm<Eigen::Infinity>())) {
       throw_pretty("backward_error");
     }
   }
@@ -650,59 +744,56 @@
   START_PROFILER("SolverCSQP::backwardPass_without_constraints");
 
   const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d_T = problem_->get_terminalData();
 
   Vxx_.back() = d_T->Lxx;
   Vx_.back() = d_T->Lx ;
 
-  if (!std::isnan(xreg_)) {
-    Vxx_.back().diagonal().array() += xreg_;
+  if (!std::isnan(preg_)) {
+    Vxx_.back().diagonal().array() += preg_;
   }
 
-  // if (!is_feasible_) {
-  //   Vx_.back().noalias() += Vxx_.back() * fs_.back();
-  // }
-
   const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
   const std::vector<boost::shared_ptr<crocoddyl::ActionDataAbstract> >& datas = problem_->get_runningDatas();
   for (int t = static_cast<int>(problem_->get_T()) - 1; t >= 0; --t) {
     const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m = models[t];
     const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d = datas[t];
     const Eigen::MatrixXd& Vxx_p = Vxx_[t + 1];
-    const Eigen::VectorXd& Vx_p = Vx_[t + 1] + Vxx_[t+1] * fs_[t+1];;
+    tmp_Vx_.noalias() = Vxx_[t+1] * fs_[t+1];
+    tmp_Vx_.noalias() += Vx_[t + 1];
     const std::size_t nu = m->get_nu();
     FxTVxx_p_.noalias() = d->Fx.transpose() * Vxx_p;
     START_PROFILER("SolverCSQP::Qx");
     Qx_[t] = d->Lx;
 
-    Qx_[t].noalias() += d->Fx.transpose() * Vx_p;
+    Qx_[t].noalias() += d->Fx.transpose() * tmp_Vx_;
     STOP_PROFILER("SolverCSQP::Qx");
     START_PROFILER("SolverCSQP::Qxx");
     Qxx_[t] = d->Lxx;
     
     Qxx_[t].noalias() += FxTVxx_p_ * d->Fx;
     STOP_PROFILER("SolverCSQP::Qxx");
     if (nu != 0) {
       FuTVxx_p_[t].noalias() = d->Fu.transpose() * Vxx_p;
       START_PROFILER("SolverCSQP::Qu");
       Qu_[t] = d->Lu;
-      Qu_[t].noalias() += d->Fu.transpose() * Vx_p;
+      Qu_[t].noalias() += d->Fu.transpose() * tmp_Vx_;
 
       STOP_PROFILER("SolverCSQP::Qu");
       START_PROFILER("SolverCSQP::Quu");
       Quu_[t] = d->Luu;
       Quu_[t].noalias() += FuTVxx_p_[t] * d->Fu;
       STOP_PROFILER("SolverCSQP::Quu");
       START_PROFILER("SolverCSQP::Qxu");
-      Qxu_[t] = d->Lxu; // TODO : check if this should also have added terms
+      Qxu_[t] = d->Lxu; 
       Qxu_[t].noalias() += FxTVxx_p_ * d->Fu;
       STOP_PROFILER("SolverCSQP::Qxu");
 
-      if (!std::isnan(ureg_)) {
-        Quu_[t].diagonal().array() += ureg_;
+      if (!std::isnan(dreg_)) {
+        Quu_[t].diagonal().array() += dreg_;
       }
     }
 
     computeGains(t);
 
     Vx_[t] = Qx_[t];
     Vxx_[t] = Qxx_[t];
@@ -712,23 +803,18 @@
       START_PROFILER("SolverCSQP::Vxx");
       Vxx_[t].noalias() -= Qxu_[t] * K_[t];
       STOP_PROFILER("SolverCSQP::Vxx");
     }
     Vxx_tmp_ = 0.5 * (Vxx_[t] + Vxx_[t].transpose());
     Vxx_[t] = Vxx_tmp_;
 
-    if (!std::isnan(xreg_)) {
-      Vxx_[t].diagonal().array() += xreg_;
+    if (!std::isnan(preg_)) {
+      Vxx_[t].diagonal().array() += preg_;
     }
 
-    // Compute and store the Vx gradient at end of the interval (rollout state)
-    // if (!is_feasible_) {
-    //   Vx_[t].noalias() += Vxx_[t] * fs_[t];
-    // }
-
     if (raiseIfNaN(Vx_[t].lpNorm<Eigen::Infinity>())) {
       throw_pretty("backward_error");
     }
     if (raiseIfNaN(Vxx_[t].lpNorm<Eigen::Infinity>())) {
       throw_pretty("backward_error");
     }
   }
@@ -738,154 +824,189 @@
 
 void SolverCSQP::backwardPass_without_rho_update() {
   START_PROFILER("SolverCSQP::backwardPass_without_rho_update");
 
   const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m_T = problem_->get_terminalModel();
   const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d_T = problem_->get_terminalData();
 
-  Vx_.back() = d_T->Lx - sigma_ * dx_.back();
+  Vx_.back() = d_T->Lx;
+  Vx_.back().noalias() -= sigma_ * dx_.back();
 
   if (m_T->get_ng()){ // constraint model
-    Vx_.back() += d_T->Gx.transpose() * (y_.back() - rho_vec_.back().cwiseProduct(z_.back()));
+    tmp_dual_cwise_.back() = y_.back();
+    tmp_dual_cwise_.back().noalias() -= rho_vec_.back().cwiseProduct(z_.back());
+    Vx_.back().noalias() += d_T->Gx.transpose() * tmp_dual_cwise_.back();
   }
 
-  // if (!is_feasible_) {
-  //   Vx_.back().noalias() += Vxx_.back() * fs_.back();
-  // }
-
   const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
   const std::vector<boost::shared_ptr<crocoddyl::ActionDataAbstract> >& datas = problem_->get_runningDatas();
   for (int t = static_cast<int>(problem_->get_T()) - 1; t >= 0; --t) {
     const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m = models[t];
     const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d = datas[t];
-    const Eigen::VectorXd& Vx_p = Vx_[t + 1] + Vxx_[t+1] * fs_[t+1];;
+
+    tmp_Vx_ = Vxx_fs_[t] + Vx_[t + 1];
     const std::size_t nu = m->get_nu();
     std::size_t nc = m->get_ng();
     START_PROFILER("SolverCSQP::Qx");
-    Qx_[t] = d->Lx - sigma_ * dx_[t];
+    Qx_[t] = d->Lx;
+    Qx_[t].noalias() -= sigma_ * dx_[t];
 
-    if (t > 0 && nc != 0){ //constraint model
-      Qx_[t] += d->Gx.transpose() * (y_[t] - rho_vec_[t].cwiseProduct(z_[t]));
+    if (t > 0 && nc != 0){ 
+      tmp_dual_cwise_[t] = y_[t]; 
+      tmp_dual_cwise_[t].noalias() -= rho_vec_[t].cwiseProduct(z_[t]);
+      Qx_[t].noalias() += d->Gx.transpose() * tmp_dual_cwise_[t];
     }
 
-    Qx_[t].noalias() += d->Fx.transpose() * Vx_p;
+    Qx_[t].noalias() += d->Fx.transpose() * tmp_Vx_;
 
     STOP_PROFILER("SolverCSQP::Qxx");
     if (nu != 0) {
       START_PROFILER("SolverCSQP::Qu");
-      Qu_[t] = d->Lu - sigma_ * du_[t];
-      if (nc != 0){ //constraint model
-        Qu_[t] += d->Gu.transpose() * (y_[t] - rho_vec_[t].cwiseProduct(z_[t]));
+      Qu_[t] = d->Lu;
+      Qu_[t].noalias() -= sigma_ * du_[t];
+      if (nc != 0){ 
+        tmp_dual_cwise_[t] = y_[t]; 
+        tmp_dual_cwise_[t].noalias() -= rho_vec_[t].cwiseProduct(z_[t]);
+        Qu_[t].noalias() += d->Gu.transpose() * tmp_dual_cwise_[t];
       }
 
-      Qu_[t].noalias() += d->Fu.transpose() * Vx_p;
+      Qu_[t].noalias() += d->Fu.transpose() * tmp_Vx_;
 
     }
 
-    // computing gains efficiently
     k_[t] = Qu_[t];
     Quu_llt_[t].solveInPlace(k_[t]);
 
     Vx_[t] = Qx_[t];
     if (nu != 0) {
       Vx_[t].noalias() -= K_[t].transpose() * Qu_[t];
     }
 
-    // Compute and store the Vx gradient at end of the interval (rollout state)
-    // if (!is_feasible_) {
-    //   Vx_[t].noalias() += Vxx_[t] * fs_[t];
-    // }
-
     if (raiseIfNaN(Vx_[t].lpNorm<Eigen::Infinity>())) {
       throw_pretty("backward_error");
     }
     if (raiseIfNaN(Vxx_[t].lpNorm<Eigen::Infinity>())) {
       throw_pretty("backward_error");
     }
   }
   STOP_PROFILER("SolverCSQP::backwardPass_without_rho_update");
 }
 
 
-void SolverCSQP::update_lagrangian_parameters(bool update_y){
+void SolverCSQP::update_lagrangian_parameters(){
     norm_primal_ = -1* std::numeric_limits<double>::infinity();
     norm_dual_ = -1* std::numeric_limits<double>::infinity();
     norm_primal_rel_ = -1* std::numeric_limits<double>::infinity();
     norm_dual_rel_ = -1* std::numeric_limits<double>::infinity();
 
     const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
     const std::vector<boost::shared_ptr<crocoddyl::ActionDataAbstract> >& datas = problem_->get_runningDatas();
 
     const std::size_t T = problem_->get_T();
+
     for (std::size_t t = 0; t < T; ++t) {    
 
       const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m = models[t];
       const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d = datas[t];
 
       std::size_t nc = m->get_ng();
 
       if (nc == 0){
         dx_[t] = dxtilde_[t];
         du_[t] = dutilde_[t];
         continue;
       }
 
       z_prev_[t] = z_[t];
-      Cdx_Cdu[t] = d->Gx * dxtilde_[t] + d->Gu * dutilde_[t];
-      z_relaxed_[t] = alpha_ * Cdx_Cdu[t] + (1 - alpha_) * z_[t];
+      tmp_Cdx_Cdu_[t].noalias() = d->Gx * dxtilde_[t];
+      tmp_Cdx_Cdu_[t].noalias() += d->Gu * dutilde_[t];
+      z_relaxed_[t].noalias() = alpha_ * tmp_Cdx_Cdu_[t];
+      z_relaxed_[t].noalias() += (1 - alpha_) * z_[t];
+
 
       const auto ub = m->get_g_ub(); 
       const auto lb = m->get_g_lb();
-      z_[t] = (z_relaxed_[t] + (y_[t].cwiseProduct(inv_rho_vec_[t])));
+
+
+      tmp_dual_cwise_[t] = y_[t].cwiseProduct(inv_rho_vec_[t]);
+
+      z_[t] = (z_relaxed_[t] + tmp_dual_cwise_[t]);
       z_[t] = z_[t].cwiseMax(lb - d->g).cwiseMin(ub - d->g);
      
-      if (update_y){
-        y_[t] = y_[t] + rho_vec_[t].cwiseProduct(z_relaxed_[t] - z_[t]);
-      }
-      dx_[t] = dxtilde_[t]; du_[t] = dutilde_[t];
+      
+      y_[t] += rho_vec_[t].cwiseProduct(z_relaxed_[t] - z_[t]);
+      
+      dx_[t] = dxtilde_[t];
+      du_[t] = dutilde_[t];
 
-      // operation repeated
-      dual_vecx = d->Gx.transpose() * (rho_vec_[t].cwiseProduct(z_[t] - z_prev_[t]));
-      dual_vecu = d->Gu.transpose() * (rho_vec_[t].cwiseProduct(z_[t] - z_prev_[t]));
-
-      norm_dual_ = std::max(norm_dual_, std::max(dual_vecx.lpNorm<Eigen::Infinity>(), dual_vecu.lpNorm<Eigen::Infinity>()));
-      norm_primal_ = std::max(norm_primal_, (Cdx_Cdu[t] - z_[t]).lpNorm<Eigen::Infinity>());
-      norm_primal_rel_= std::max(norm_primal_rel_, Cdx_Cdu[t].lpNorm<Eigen::Infinity>());
-      norm_primal_rel_= std::max(norm_primal_rel_, z_[t].lpNorm<Eigen::Infinity>());
-      norm_dual_rel_ = std::max(norm_dual_rel_, (d->Gx.transpose() * y_[t]).lpNorm<Eigen::Infinity>());
-      norm_dual_rel_ = std::max(norm_dual_rel_, (d->Gu.transpose() * y_[t]).lpNorm<Eigen::Infinity>());
+      if (update_rho_with_heuristic_){
+        tmp_dual_cwise_[t] = rho_vec_[t].cwiseProduct(z_[t] - z_prev_[t]);
+        norm_dual_ = std::max(norm_dual_, tmp_dual_cwise_[t].lpNorm<Eigen::Infinity>());
+        norm_primal_ = std::max(norm_primal_, (tmp_Cdx_Cdu_[t] - z_[t]).lpNorm<Eigen::Infinity>());
+
+        norm_primal_rel_= std::max(norm_primal_rel_, tmp_Cdx_Cdu_[t].lpNorm<Eigen::Infinity>());
+        norm_primal_rel_= std::max(norm_primal_rel_, z_[t].lpNorm<Eigen::Infinity>());
+        norm_dual_rel_ = std::max(norm_dual_rel_, y_[t].lpNorm<Eigen::Infinity>());
+      } 
+      else {
+        tmp_dual_cwise_[t] = rho_vec_[t].cwiseProduct(z_[t] - z_prev_[t]);
+        tmp_vec_x_.noalias() = d->Gx.transpose() * tmp_dual_cwise_[t];
+        tmp_vec_u_[t].noalias() = d->Gu.transpose() * tmp_dual_cwise_[t];
+        norm_dual_ = std::max(norm_dual_, std::max(tmp_vec_x_.lpNorm<Eigen::Infinity>(), tmp_vec_u_[t].lpNorm<Eigen::Infinity>()));
+        norm_primal_ = std::max(norm_primal_, (tmp_Cdx_Cdu_[t] - z_[t]).lpNorm<Eigen::Infinity>());
+        
+        norm_primal_rel_= std::max(norm_primal_rel_, tmp_Cdx_Cdu_[t].lpNorm<Eigen::Infinity>());
+        norm_primal_rel_= std::max(norm_primal_rel_, z_[t].lpNorm<Eigen::Infinity>());
+        tmp_vec_x_.noalias() = d->Gx.transpose() * y_[t];
+        tmp_vec_u_[t].noalias() = d->Gu.transpose() * y_[t];
+        norm_dual_rel_ = std::max(norm_dual_rel_, tmp_vec_x_.lpNorm<Eigen::Infinity>());
+        norm_dual_rel_ = std::max(norm_dual_rel_, tmp_vec_u_[t].lpNorm<Eigen::Infinity>());
+      }
     }
 
   dx_.back() = dxtilde_.back();
   const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m_T = problem_->get_terminalModel();
   const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d_T = problem_->get_terminalData();
   std::size_t nc = m_T->get_ng();
 
   if (nc != 0){
     z_prev_.back() = z_.back();
-    Cdx_Cdu.back() = d_T->Gx * dxtilde_.back() ;
+    tmp_Cdx_Cdu_.back().noalias() = d_T->Gx * dxtilde_.back() ;
+    z_relaxed_.back().noalias() = alpha_ * tmp_Cdx_Cdu_.back();
+    z_relaxed_.back().noalias() += (1 - alpha_) * z_.back();
 
-    z_relaxed_.back() = alpha_ * Cdx_Cdu.back() + (1 - alpha_) * z_.back();
     auto ub = m_T->get_g_ub(); 
     auto lb = m_T->get_g_lb(); 
-    z_.back() = (z_relaxed_.back() + (y_.back().cwiseProduct(inv_rho_vec_.back())));
+
+    tmp_dual_cwise_.back() = y_.back().cwiseProduct(inv_rho_vec_.back());
+    z_.back() = (z_relaxed_.back() + tmp_dual_cwise_.back());
     z_.back() = z_.back().cwiseMax(lb - d_T->g).cwiseMin(ub - d_T->g);
+    y_.back() += rho_vec_.back().cwiseProduct(z_relaxed_.back() - z_.back());
+    
 
-    if (update_y){
-      y_.back() = y_.back() + rho_vec_.back().cwiseProduct(z_relaxed_.back() - z_.back());
+    if (update_rho_with_heuristic_){
+      tmp_dual_cwise_.back() = rho_vec_.back().cwiseProduct(z_.back() - z_prev_.back());
+      norm_dual_ = std::max(norm_dual_, tmp_dual_cwise_.back().lpNorm<Eigen::Infinity>());
+      norm_primal_ = std::max(norm_primal_, (tmp_Cdx_Cdu_.back() - z_.back()).lpNorm<Eigen::Infinity>());
+
+      norm_primal_rel_= std::max(norm_primal_rel_, tmp_Cdx_Cdu_.back().lpNorm<Eigen::Infinity>());
+      norm_primal_rel_= std::max(norm_primal_rel_, z_.back().lpNorm<Eigen::Infinity>());
+      norm_dual_rel_ = std::max(norm_dual_rel_, y_.back().lpNorm<Eigen::Infinity>());
+    }
+    else {
+      tmp_dual_cwise_.back() = rho_vec_.back().cwiseProduct(z_.back() - z_prev_.back());
+      tmp_vec_x_.noalias() = d_T->Gx.transpose() * tmp_dual_cwise_.back();
+      norm_dual_ = std::max(norm_dual_, tmp_vec_x_.lpNorm<Eigen::Infinity>());
+      norm_primal_ = std::max(norm_primal_, (tmp_Cdx_Cdu_.back() - z_.back()).lpNorm<Eigen::Infinity>());
+
+      norm_primal_rel_= std::max(norm_primal_rel_, tmp_Cdx_Cdu_.back().lpNorm<Eigen::Infinity>());
+      norm_primal_rel_= std::max(norm_primal_rel_, z_.back().lpNorm<Eigen::Infinity>());
+      tmp_vec_x_.noalias() = d_T->Gx.transpose() * y_.back();
+      norm_dual_rel_ = std::max(norm_dual_rel_, tmp_vec_x_.lpNorm<Eigen::Infinity>());
     }
-    dx_.back() = dxtilde_.back();
-
-    dual_vecx = d_T->Gx.transpose() * rho_vec_.back().cwiseProduct(z_.back() - z_prev_.back());
-
-    norm_dual_ = std::max(norm_dual_, dual_vecx.lpNorm<Eigen::Infinity>());
-    norm_primal_ = std::max(norm_primal_, (Cdx_Cdu.back() - z_.back()).lpNorm<Eigen::Infinity>());
-    norm_primal_rel_= std::max(norm_primal_rel_, Cdx_Cdu.back().lpNorm<Eigen::Infinity>());
-    norm_primal_rel_= std::max(norm_primal_rel_, z_.back().lpNorm<Eigen::Infinity>());
-    norm_dual_rel_ = std::max(norm_dual_rel_, (d_T->Gx.transpose() * y_.back()).lpNorm<Eigen::Infinity>());
   }
 
 }
 
 double SolverCSQP::tryStep(const double steplength) {
     if (steplength > 1. || steplength < 0.) {
         throw_pretty("Invalid argument: "
@@ -904,15 +1025,16 @@
 
     for (std::size_t t = 0; t < T; ++t) {
       const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m = models[t];
       m->get_state()->integrate(xs_[t], steplength * dx_[t], xs_try_[t]); 
       const std::size_t nu = m->get_nu();
 
       if (nu != 0) {
-        us_try_[t].noalias() = us_[t] + steplength * du_[t];
+        us_try_[t] = us_[t];
+        us_try_[t].noalias() += steplength * du_[t];
         }        
       } 
 
     const boost::shared_ptr<crocoddyl::ActionModelAbstract>& m_ter = problem_->get_terminalModel();
     const boost::shared_ptr<crocoddyl::ActionDataAbstract>& d_ter = problem_->get_terminalData();
 
     m_ter->get_state()->integrate(xs_.back(), steplength * dx_.back(), xs_try_.back()); 
@@ -957,44 +1079,77 @@
     }
 
     STOP_PROFILER("SolverCSQP::tryStep");
 
     return merit_try_;
 }
 
-void SolverCSQP::printCallbacks(){
+void SolverCSQP::printCallbacks(bool isLastIteration){
   if (this->get_iter() % 10 == 0) {
-    std::cout << "iter     merit        cost         grad       step     ||gaps||       KKT       Constraint Norms    QP Iters";
+    std::cout << std::scientific << std::setprecision(4) <<  "iter"               << "  "; // Iteration number
+    std::cout << std::scientific << std::setprecision(4) <<  "   merit"           << "  "; // Merit function value
+    std::cout << std::scientific << std::setprecision(4) <<  "      cost"         << "  "; // Cost function value
+    std::cout << std::scientific << std::setprecision(4) <<  "     ||gaps||"      << "  "; // Gaps norm 
+    std::cout << std::scientific << std::setprecision(4) <<  " ||Constraint||"    << "";   // Constraint norm 
+    std::cout << std::scientific << std::setprecision(4) <<  "  ||(dx,du)||"      << " ";  // Step norm
+    std::cout << std::fixed      << std::setprecision(4) <<  "    step"           << "  "; // Step size
+    std::cout << std::scientific << std::setprecision(4) <<  " KKT criteria"      << "  "; // KKT residual norm
+    std::cout << std::fixed      << std::setprecision(4) <<  "QP iters"           << " ";  // Number of QP iterations
     std::cout << std::endl;
   }
-  std::cout << std::setw(4) << this->get_iter() << "  ";
-  std::cout << std::scientific << std::setprecision(5) << this->get_merit() << "  ";
-  std::cout << std::scientific << std::setprecision(5) << this->get_cost() << "  ";
-  std::cout << this->get_xgrad_norm() + this->get_ugrad_norm() << "  ";
-  std::cout << std::fixed << std::setprecision(4) << this->get_steplength() << "  ";
-  std::cout << std::scientific << std::setprecision(5) << this->get_gap_norm() << "  ";
-  std::cout << std::scientific << std::setprecision(5) << KKT_ << "    ";
-  std::cout << std::scientific << std::setprecision(5) << constraint_norm_ << "         ";
-  std::cout << std::scientific << std::setprecision(5) << qp_iters_;
+  if(KKT_ < termination_tol_ || isLastIteration){
+    std::cout << std::setw(4) << "END" << "  ";
+    std::cout << std::scientific << std::setprecision(4) << this->get_merit()     << "   ";    
+    std::cout << std::scientific << std::setprecision(4) << this->get_cost()      << "   ";
+    std::cout << std::scientific << std::setprecision(4) << this->get_gap_norm()  << "    ";
+    std::cout << std::scientific << std::setprecision(4) << constraint_norm_      << "    ";
+    std::cout << std::fixed <<      std::setprecision(5) << "   ---- "            << "    ";
+    std::cout << std::scientific << std::setprecision(4) << "    ---- "           << "   ";
+    std::cout << std::scientific << std::setprecision(4) << KKT_                  << "    ";
+    std::cout << std::fixed <<      std::setprecision(4) << "-----";
+  } else {
+    std::cout << std::setw(4) << this->get_iter()+1 << "  ";
+    std::cout << std::scientific << std::setprecision(4) << this->get_merit()                                     << "   ";
+    std::cout << std::scientific << std::setprecision(4) << this->get_cost()                                      << "   ";
+    std::cout << std::scientific << std::setprecision(4) << this->get_gap_norm()                                  << "    ";
+    std::cout << std::scientific << std::setprecision(4) << constraint_norm_                                      << "    ";
+    std::cout << std::scientific << std::setprecision(5) << (this->get_xgrad_norm() + this->get_ugrad_norm()) / 2 << "    ";
+    std::cout << std::fixed      << std::setprecision(4) << this->get_steplength()                                << "   ";
+    if(iter_ == 0){
+      std::cout << std::scientific << std::setprecision(4) << "   ----   "                                        << "     ";
+    } else {
+      std::cout << std::scientific << std::setprecision(4) << KKT_                                                << "     ";
+    }
+    std::cout << std::fixed      << std::setprecision(4) << qp_iters_;
+  }
+  std::cout << std::endl;
+  std::cout << std::flush;
+}
 
+void SolverCSQP::printQPCallbacks(int iter){
+  std::cout << "Iters " << iter;
+  std::cout << " norm_primal = "     << std::scientific << std::setprecision(4) << norm_primal_;
+  std::cout << " norm_primal_tol = " << std::scientific << std::setprecision(4) << norm_primal_tolerance_;
+  std::cout << " norm_dual =  "      << std::scientific << std::setprecision(4) << norm_dual_;
+  std::cout << " norm_dual_tol = "   << std::scientific << std::setprecision(4) << norm_dual_tolerance_;
   std::cout << std::endl;
   std::cout << std::flush;
 }
 
 void SolverCSQP::setCallbacks(bool inCallbacks){
   with_callbacks_ = inCallbacks;
 }
 
 bool SolverCSQP::getCallbacks(){
   return with_callbacks_;
 }
-// double SolverCSQP::get_th_acceptnegstep() const { return th_acceptnegstep_; }
 
-// void SolverCSQP::set_th_acceptnegstep(const double th_acceptnegstep) {
-//   if (0. > th_acceptnegstep) {
-//     throw_pretty("Invalid argument: "
-//                  << "th_acceptnegstep value has to be positive.");
-//   }
-//   th_acceptnegstep_ = th_acceptnegstep;
-// }
+void SolverCSQP::setQPCallbacks(bool inQPCallbacks){
+  with_qp_callbacks_ = inQPCallbacks;
+}
+
+bool SolverCSQP::getQPCallbacks(){
+  return with_qp_callbacks_;
+}
+
 
 }  // namespace mim_solvers
```

### Comparing `cmeel_mim_solvers-0.0.2/src/csqp_proxqp.cpp` & `cmeel_mim_solvers-0.0.4/src/csqp_proxqp.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,21 @@
       cost_list_.resize(filter_size_);
       fs_try_.resize(T + 1);
       fs_flat_.resize(ndx*(T + 1));
       fs_flat_.setZero();
       lag_mul_.resize(T+1);
       y_.resize(T+1);
       du_.resize(T);
-      KKT_ = 0.;
-
       dx_.resize(T+1); 
       du_.resize(T);
 
       xs_try_.resize(T+1); us_try_.resize(T);
 
+      std::size_t n_eq_crocoddyl = 0;
+
       const std::vector<boost::shared_ptr<ActionModelAbstract> >& models = problem_->get_runningModels();
       // We allow nx and nu to change with time
       n_vars = 0;
       n_eq = 0;
       for (std::size_t t = 0; t < T; ++t){
         if(t < T-1){
           n_vars += models[t+1]->get_state()->get_nx();
@@ -71,14 +71,15 @@
         fs_try_[t].resize(ndx); fs_try_[t] = Eigen::VectorXd::Zero(ndx);
         lag_mul_[t].resize(ndx); lag_mul_[t].setZero();
         dx_[t].resize(ndx); du_[t].resize(nu);
         dx_[t].setZero();du_[t] = Eigen::VectorXd::Zero(nu);
         
         // Constraint Models
         int nc = model->get_ng();
+        n_eq_crocoddyl += model->get_nh();
         y_[t].resize(nc); y_[t].setZero();
         n_in += nc;
 
       }
 
       xs_try_.back() = problem_->get_terminalModel()->get_state()->zero();
 
@@ -87,14 +88,23 @@
       dx_.back().resize(ndx); 
       dx_.back().setZero();
       fs_try_.back().resize(ndx);
       fs_try_.back() = Eigen::VectorXd::Zero(ndx);
 
       // Constraint Models
       int nc = problem_->get_terminalModel()->get_ng();
+
+      // Check that no equality constraint was specified through Crocoddyl's API
+      n_eq_crocoddyl += problem_->get_terminalModel()->get_nh(); 
+      if(n_eq_crocoddyl != 0){
+        throw_pretty("Error: nh must be zero !!! Crocoddyl's equality constraints API is not supported by mim_solvers.\n"
+                     "  >> Equality constraints of the form H(x,u) = h must be implemented as g <= G(x,u) <= g by specifying \n"
+                     "     lower and upper bounds in the constructor of the constraint model residual or by setting g_ub and g_lb.")
+      } 
+
       y_.back().resize(nc); y_.back().setZero();
       n_in += nc;
       // n_eq = T* nx;
 
       C_.resize(n_in, n_vars); C_.setZero();
       l_.resize(n_in); l_.setZero();
       u_.resize(n_in); u_.setZero();
@@ -127,19 +137,19 @@
   }
   setCandidate(init_xs, init_us, false);
   xs_[0] = problem_->get_x0();      // Otherwise xs[0] is overwritten by init_xs inside setCandidate()
   xs_try_[0] = problem_->get_x0();  // it is needed in case that init_xs[0] is infeasible
 
 
   if (std::isnan(reginit)) {
-    xreg_ = reg_min_;
-    ureg_ = reg_min_;
+    preg_ = reg_min_;
+    dreg_ = reg_min_;
   } else {
-    xreg_ = reginit;
-    ureg_ = reginit;
+    preg_ = reginit;
+    dreg_ = reginit;
   }
 
   for (iter_ = 0; iter_ < maxiter; ++iter_) {
 
 
     was_feasible_ = false;
     bool recalcDiff = true;
@@ -147,29 +157,30 @@
     while (true) {
       try {
         computeDirection(recalcDiff);
       } 
       catch (std::exception& e) {
         recalcDiff = false;
         increaseRegularization();
-        if (xreg_ == reg_max_) {
+        if (preg_ == reg_max_) {
           return false;
         } else {
           continue;
         }
       }
       break;
     }
 
     // KKT termination criteria
-    if(use_kkt_criteria_){
-      if (KKT_  <= termination_tol_) {
-        STOP_PROFILER("SolverPROXQP::solve");
-        return true;
+    if (KKT_  <= termination_tol_) {
+      if(with_callbacks_){
+        printCallbacks();
       }
+      STOP_PROFILER("SolverPROXQP::solve");
+      return true;
     }
 
     constraint_list_.push_back(constraint_norm_);
     gap_list_.push_back(gap_norm_);
     cost_list_.push_back(cost_);
 
     // We need to recalculate the derivatives when the step length passes
@@ -206,15 +217,15 @@
     }
 
     if (steplength_ > th_stepdec_) {
       decreaseRegularization();
     }
     if (steplength_ <= th_stepinc_) {
       increaseRegularization();
-      if (xreg_ == reg_max_) {
+      if (preg_ == reg_max_) {
         STOP_PROFILER("SolverPROXQP::solve");
         return false;
       }
     }
     if(with_callbacks_){
       printCallbacks();
     }
@@ -323,62 +334,60 @@
 
 void SolverPROXQP::computeDirection(const bool recalcDiff){
   START_PROFILER("SolverPROXQP::computeDirection");
   const std::size_t T = problem_->get_T();
   if (recalcDiff) {
     calc(recalcDiff);
   }
-  if(use_kkt_criteria_){
-    checkKKTConditions();
-  }
+  checkKKTConditions();
+
+  // proxsuite::proxqp::dense::QP<double> qp_(n_vars, n_eq, n_in);
+  // qp_.init(P_, q_, A_, b_, C_, l_, u_);
 
-  // proxsuite::proxqp::dense::QP<double> qp(n_vars, n_eq, n_in);
-  // qp.init(P_, q_, A_, b_, C_, l_, u_);
+  proxsuite::proxqp::sparse::QP<double, long long> qp_(n_vars, n_eq, n_in);
+  qp_.init(Psp_, q_, Asp_, b_, Csp_, l_, u_);
 
-  proxsuite::proxqp::sparse::QP<double, long long> qp(n_vars, n_eq, n_in);
-  qp.init(Psp_, q_, Asp_, b_, Csp_, l_, u_);
-
-  // std::cout << "max qp iter = " << eps_abs_ << std::endl;
-  // std::cout << "was set from = " << qp.settings.eps_abs << std::endl;
-  qp.settings.eps_abs = eps_abs_;
-  // std::cout << "was set in to = " << qp.settings.eps_abs << std::endl;
-  qp.settings.max_iter = max_qp_iters_;
-  qp.settings.max_iter_in = max_qp_iters_;
-  qp.solve(); 
-  auto res = qp.results.x;
-  qp_iters_ = qp.results.info.iter;
+  qp_.settings.eps_abs = eps_abs_;
+  qp_.settings.eps_rel = eps_rel_;
+  qp_.settings.max_iter = max_qp_iters_;
+  qp_.settings.max_iter_in = max_qp_iters_;
+  qp_.solve(); 
+  qp_iters_ = qp_.results.info.iter;
+  norm_primal_ = qp_.results.info.pri_res;
+  norm_dual_ = qp_.results.info.dua_res;
 
+  // std::cout << "ProxQP iters " << qp_iters_ << " norm_primal=" << norm_primal_ << " norm_dual= " << norm_dual_ << std::endl;
   const std::vector<boost::shared_ptr<ActionModelAbstract> >& models = problem_->get_runningModels();
   x_grad_norm_ = 0; u_grad_norm_ = 0;
   double nin_count = 0;
   double index_u = n_eq;
   for (std::size_t t = 0; t < T; ++t){
     const boost::shared_ptr<ActionModelAbstract>& m = models[t];
     const int nx = m->get_state()->get_nx();
     const int nu = m->get_nu();
     int nc = m->get_ng();
 
-    dx_[t+1] = res.segment(t * nx, nx);
+    dx_[t+1] = qp_.results.x.segment(t * nx, nx);
     // double index_u = T *nx + t * nu;
-    du_[t] = res.segment(index_u, nu);
+    du_[t] = qp_.results.x.segment(index_u, nu);
     x_grad_norm_ += dx_[t+1].lpNorm<1>(); // assuming that there is no gap in the initial state
     u_grad_norm_ += du_[t].lpNorm<1>(); // assuming that there is no gap in the initial state
 
 
-    lag_mul_[t+1] = -qp.results.y.segment(t* nx, nx);
-    lag_mul_[t+1] = -qp.results.y.segment(t* nx, nx);
-    y_[t] = qp.results.z.segment(nin_count, nc);
+    lag_mul_[t+1] = -qp_.results.y.segment(t* nx, nx);
+    lag_mul_[t+1] = -qp_.results.y.segment(t* nx, nx);
+    y_[t] = qp_.results.z.segment(nin_count, nc);
     nin_count += nc;
     index_u += nu;
   }
   x_grad_norm_ = x_grad_norm_/(T+1);
   u_grad_norm_ = u_grad_norm_/T; 
 
   int nc = problem_->get_terminalModel()->get_ng();
-  y_.back() = qp.results.z.segment(nin_count, nc);
+  y_.back() = qp_.results.z.segment(nin_count, nc);
 
   STOP_PROFILER("SolverPROXQP::computeDirection");
 }
 
 void SolverPROXQP::checkKKTConditions(){
   const std::size_t T = problem_->get_T();
   const std::size_t ndx = problem_->get_ndx();
@@ -484,19 +493,27 @@
 
 
 void SolverPROXQP::printCallbacks(){
   if (this->get_iter() % 10 == 0) {
     std::cout << "iter     merit        cost         grad       step     ||gaps||       KKT       Constraint Norms    QP Iters";
     std::cout << std::endl;
   }
-  std::cout << std::setw(4) << this->get_iter() << "  ";
+  if(KKT_ < termination_tol_){
+    std::cout << std::setw(4) << "END" << "  ";
+  } else {
+    std::cout << std::setw(4) << this->get_iter()+1 << "  ";
+  }
   std::cout << std::scientific << std::setprecision(5) << this->get_merit() << "  ";
   std::cout << std::scientific << std::setprecision(5) << this->get_cost() << "  ";
   std::cout << this->get_xgrad_norm() + this->get_ugrad_norm() << "  ";
-  std::cout << std::fixed << std::setprecision(4) << this->get_steplength() << "  ";
+  if(KKT_ < termination_tol_){
+    std::cout << std::fixed << std::setprecision(4) << " ---- " << "  ";
+  } else {
+    std::cout << std::fixed << std::setprecision(4) << this->get_steplength() << "  ";
+  }
   std::cout << std::scientific << std::setprecision(5) << this->get_gap_norm() << "  ";
   std::cout << std::scientific << std::setprecision(5) << KKT_ << "    ";
   std::cout << std::scientific << std::setprecision(5) << constraint_norm_ << "         ";
   std::cout << std::scientific << std::setprecision(5) << qp_iters_;
 
   std::cout << std::endl;
   std::cout << std::flush;
```

### Comparing `cmeel_mim_solvers-0.0.2/src/ddp.cpp` & `cmeel_mim_solvers-0.0.4/src/ddp.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -63,47 +63,46 @@
   if (problem_->is_updated()) {
     resizeData();
   }
   xs_try_[0] = problem_->get_x0();  // it is needed in case that init_xs[0] is infeasible
   setCandidate(init_xs, init_us, is_feasible);
 
   if (std::isnan(reginit)) {
-    xreg_ = reg_min_;
-    ureg_ = reg_min_;
+    preg_ = reg_min_;
+    dreg_ = reg_min_;
   } else {
-    xreg_ = reginit;
-    ureg_ = reginit;
+    preg_ = reginit;
+    dreg_ = reginit;
   }
   was_feasible_ = false;
 
   bool recalcDiff = true;
   for (iter_ = 0; iter_ < maxiter; ++iter_) {
     while (true) {
       try {
         computeDirection(recalcDiff);
       } catch (std::exception& e) {
         recalcDiff = false;
         increaseRegularization();
-        if (xreg_ == reg_max_) {
+        if (preg_ == reg_max_) {
           return false;
         } else {
           continue;
         }
       }
       break;
     }
     expectedImprovement();
 
     // KKT termination criteria
-    if(use_kkt_criteria_){
-      if (KKT_  <= termination_tol_) {
-        STOP_PROFILER("SolverDDP::solve");
-        return true;
-      }
-    } 
+    checkKKTConditions();
+    if (KKT_  <= termination_tol_) {
+      STOP_PROFILER("SolverDDP::solve");
+      return true;
+    }
 
     // We need to recalculate the derivatives when the step length passes
     recalcDiff = false;
     for (std::vector<double>::const_iterator it = alphas_.begin(); it != alphas_.end(); ++it) {
       steplength_ = *it;
 
       try {
@@ -125,15 +124,15 @@
     }
 
     if (steplength_ > th_stepdec_) {
       decreaseRegularization();
     }
     if (steplength_ <= th_stepinc_) {
       increaseRegularization();
-      if (xreg_ == reg_max_) {
+      if (preg_ == reg_max_) {
         STOP_PROFILER("SolverDDP::solve");
         return false;
       }
     }
     stoppingCriteria();
 
     const std::size_t n_callbacks = callbacks_.size();
@@ -152,18 +151,14 @@
 }
 
 void SolverDDP::computeDirection(const bool recalcDiff) {
   START_PROFILER("SolverDDP::computeDirection");
   if (recalcDiff) {
     calcDiff();
   }
-  // KKT termination criteria
-  if(use_kkt_criteria_){
-    checkKKTConditions();
-  }  
   backwardPass();
   STOP_PROFILER("SolverDDP::computeDirection");
 }
 
 double SolverDDP::tryStep(const double steplength) {
   START_PROFILER("SolverDDP::tryStep");
   forwardPass(steplength);
@@ -252,16 +247,16 @@
 
 void SolverDDP::backwardPass() {
   START_PROFILER("SolverDDP::backwardPass");
   const boost::shared_ptr<ActionDataAbstract>& d_T = problem_->get_terminalData();
   Vxx_.back() = d_T->Lxx;
   Vx_.back() = d_T->Lx;
 
-  if (!std::isnan(xreg_)) {
-    Vxx_.back().diagonal().array() += xreg_;
+  if (!std::isnan(preg_)) {
+    Vxx_.back().diagonal().array() += preg_;
   }
 
   if (!is_feasible_) {
     Vx_.back().noalias() += Vxx_.back() * fs_.back();
   }
   const std::vector<boost::shared_ptr<ActionModelAbstract> >& models = problem_->get_runningModels();
   const std::vector<boost::shared_ptr<ActionDataAbstract> >& datas = problem_->get_runningDatas();
@@ -291,16 +286,16 @@
       Quu_[t] = d->Luu;
       Quu_[t].noalias() += FuTVxx_p_[t] * d->Fu;
       STOP_PROFILER("SolverDDP::Quu");
       START_PROFILER("SolverDDP::Qxu");
       Qxu_[t] = d->Lxu;
       Qxu_[t].noalias() += FxTVxx_p_ * d->Fu;
       STOP_PROFILER("SolverDDP::Qxu");
-      if (!std::isnan(ureg_)) {
-        Quu_[t].diagonal().array() += ureg_;
+      if (!std::isnan(dreg_)) {
+        Quu_[t].diagonal().array() += dreg_;
       }
     }
 
     computeGains(t);
 
     Vx_[t] = Qx_[t];
     Vxx_[t] = Qxx_[t];
@@ -310,16 +305,16 @@
       START_PROFILER("SolverDDP::Vxx");
       Vxx_[t].noalias() -= Qxu_[t] * K_[t];
       STOP_PROFILER("SolverDDP::Vxx");
     }
     Vxx_tmp_ = 0.5 * (Vxx_[t] + Vxx_[t].transpose());
     Vxx_[t] = Vxx_tmp_;
 
-    if (!std::isnan(xreg_)) {
-      Vxx_[t].diagonal().array() += xreg_;
+    if (!std::isnan(preg_)) {
+      Vxx_[t].diagonal().array() += preg_;
     }
 
     // Compute and store the Vx gradient at end of the interval (rollout state)
     if (!is_feasible_) {
       Vx_[t].noalias() += Vxx_[t] * fs_[t];
     }
 
@@ -402,27 +397,27 @@
     k_[t] = Qu_[t];
     Quu_llt_[t].solveInPlace(k_[t]);
   }
   STOP_PROFILER("SolverDDP::computeGains");
 }
 
 void SolverDDP::increaseRegularization() {
-  xreg_ *= reg_incfactor_;
-  if (xreg_ > reg_max_) {
-    xreg_ = reg_max_;
+  preg_ *= reg_incfactor_;
+  if (preg_ > reg_max_) {
+    preg_ = reg_max_;
   }
-  ureg_ = xreg_;
+  dreg_ = preg_;
 }
 
 void SolverDDP::decreaseRegularization() {
-  xreg_ /= reg_decfactor_;
-  if (xreg_ < reg_min_) {
-    xreg_ = reg_min_;
+  preg_ /= reg_decfactor_;
+  if (preg_ < reg_min_) {
+    preg_ = reg_min_;
   }
-  ureg_ = xreg_;
+  dreg_ = preg_;
 }
 
 void SolverDDP::allocateData() {
   const std::size_t T = problem_->get_T();
   Vxx_.resize(T + 1);
   Vx_.resize(T + 1);
   Qxx_.resize(T);
```

### Comparing `cmeel_mim_solvers-0.0.2/src/fddp.cpp` & `cmeel_mim_solvers-0.0.4/src/fddp.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 using namespace crocoddyl;
 
 namespace mim_solvers {
 
 SolverFDDP::SolverFDDP(boost::shared_ptr<crocoddyl::ShootingProblem> problem)
     : SolverDDP(problem), dg_(0), dq_(0), dv_(0), th_acceptnegstep_(2) {
+      std::cerr << "Warning: Do not use mim_solvers.SolverFDDP !!! " << std::endl;
+      std::cerr << "It may differ significantly from its Crocoddyl counterpart. " << std::endl;
+      std::cerr << "This class served only as a development tool and will be REMOVED in future releases." << std::endl;
       const std::size_t T = this->problem_->get_T();
       const std::size_t ndx = problem_->get_ndx();
       fs_try_.resize(T + 1);
       lag_mul_.resize(T+1);
       fs_flat_.resize(ndx*(T + 1));
       fs_flat_.setZero();
       gap_list_.resize(filter_size_);
@@ -52,46 +55,45 @@
   if (problem_->is_updated()) {
     resizeData();
   }
   xs_try_[0] = problem_->get_x0();  // it is needed in case that init_xs[0] is infeasible
   setCandidate(init_xs, init_us, is_feasible);
 
   if (std::isnan(reginit)) {
-    xreg_ = reg_min_;
-    ureg_ = reg_min_;
+    preg_ = reg_min_;
+    dreg_ = reg_min_;
   } else {
-    xreg_ = reginit;
-    ureg_ = reginit;
+    preg_ = reginit;
+    dreg_ = reginit;
   }
   was_feasible_ = false;
   bool recalcDiff = true;
   for (iter_ = 0; iter_ < maxiter; ++iter_) {
     while (true) {
       try {
         computeDirection(recalcDiff);
       } catch (std::exception& e) {
         recalcDiff = false;
         increaseRegularization();
-        if (xreg_ == reg_max_) {
+        if (preg_ == reg_max_) {
           return false;
         } else {
           continue;
         }
       }
       break;
     }
     updateExpectedImprovement();
 
     // KKT termination criteria
-    if(use_kkt_criteria_){
-      if (KKT_  <= termination_tol_) {
-        STOP_PROFILER("SolverFDDP::solve");
-        return true;
-      }
-    } 
+    checkKKTConditions();
+    if (KKT_  <= termination_tol_) {
+      STOP_PROFILER("SolverFDDP::solve");
+      return true;
+    }
 
     gap_list_.push_back(gap_norm_);
     cost_list_.push_back(cost_);
 
     // We need to recalculate the derivatives when the step length passes
     recalcDiff = false;
     for (std::vector<double>::const_iterator it = alphas_.begin(); it != alphas_.end(); ++it) {
@@ -144,15 +146,15 @@
     }
 
     if (steplength_ > th_stepdec_) {
       decreaseRegularization();
     }
     if (steplength_ <= th_stepinc_) {
       increaseRegularization();
-      if (xreg_ == reg_max_) {
+      if (preg_ == reg_max_) {
         STOP_PROFILER("SolverFDDP::solve");
         return false;
       }
     }
     stoppingCriteria();
 
     const std::size_t n_callbacks = callbacks_.size();
@@ -175,18 +177,14 @@
   gap_norm_ = 0;
   const std::size_t T = problem_->get_T();
   for (std::size_t t = 0; t < T; ++t) {
     gap_norm_ += fs_[t].lpNorm<1>();   
   }
   gap_norm_ += fs_.back().lpNorm<1>();
 
-  // KKT termination criteria
-  if(use_kkt_criteria_){
-    checkKKTConditions();
-  }  
   backwardPass();
   STOP_PROFILER("SolverFDDP::computeDirection");
 }
 
 void SolverFDDP::checkKKTConditions(){
   KKT_ = 0.;
   const std::size_t T = problem_->get_T();
```

### Comparing `cmeel_mim_solvers-0.0.2/src/kkt.cpp` & `cmeel_mim_solvers-0.0.4/src/kkt.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -60,19 +60,17 @@
       }
       break;
     }
 
     expectedImprovement();
 
     // KKT termination criteria
-    if(use_kkt_criteria_){
-      if (KKT_  <= termination_tol_) {
-        return true;
-      }
-    } 
+    if (KKT_  <= termination_tol_) {
+      return true;
+    }
 
     for (std::vector<double>::const_iterator it = alphas_.begin();
          it != alphas_.end(); ++it) {
       steplength_ = *it;
       try {
         dV_ = tryStep(steplength_);
       } catch (std::exception& e) {
@@ -126,17 +124,15 @@
     iu += nui;
   }
   const std::size_t ndxi =
       problem_->get_terminalModel()->get_state()->get_ndx();
   dxs_.back() = p_x.segment(ix, ndxi);
   lambdas_.back() = dual_.segment(ix, ndxi);
   // KKT termination criteria
-  if(use_kkt_criteria_){
-    checkKKTConditions();
-  }  
+  checkKKTConditions();
 }
 
 double SolverKKT::tryStep(const double steplength) {
   const std::size_t T = problem_->get_T();
   const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models =
       problem_->get_runningModels();
   for (std::size_t t = 0; t < T; ++t) {
```

### Comparing `cmeel_mim_solvers-0.0.2/src/sqp.cpp` & `cmeel_mim_solvers-0.0.4/src/sqp.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -30,33 +30,35 @@
       fs_flat_.resize(ndx*(T + 1));
       fs_flat_.setZero();
       dx_.resize(T+1);
       lag_mul_.resize(T+1);
       du_.resize(T);
       gap_list_.resize(filter_size_);
       cost_list_.resize(filter_size_);
+      tmp_vec_x_.resize(ndx);
+      tmp_vec_u_.resize(T);
       const std::vector<boost::shared_ptr<crocoddyl::ActionModelAbstract> >& models = problem_->get_runningModels();
       for (std::size_t t = 0; t < T; ++t) {
         const boost::shared_ptr<crocoddyl::ActionModelAbstract>& model = models[t];
         const std::size_t nu = model->get_nu();
         dx_[t].resize(ndx); du_[t].resize(nu);
         fs_try_[t].resize(ndx);
         lag_mul_[t].resize(ndx); 
         lag_mul_[t].setZero();
         dx_[t].setZero();
         du_[t] = Eigen::VectorXd::Zero(nu);
         fs_try_[t] = Eigen::VectorXd::Zero(ndx);
+        tmp_vec_u_[t].resize(nu);
       }
       lag_mul_.back().resize(ndx);
       lag_mul_.back().setZero();
       dx_.back().resize(ndx);
       dx_.back().setZero();
       fs_try_.back().resize(ndx);
       fs_try_.back() = Eigen::VectorXd::Zero(ndx);
-      
 
       const std::size_t n_alphas = 10;
       alphas_.resize(n_alphas);
       for (std::size_t n = 0; n < n_alphas; ++n) {
         alphas_[n] = 1. / pow(2., static_cast<double>(n));
       }
       if (th_stepinc_ < alphas_[n_alphas - 1]) {
@@ -78,50 +80,52 @@
     resizeData();
   }
   setCandidate(init_xs, init_us, false);
   xs_[0] = problem_->get_x0();      // Otherwise xs[0] is overwritten by init_xs inside setCandidate()
   xs_try_[0] = problem_->get_x0();  // it is needed in case that init_xs[0] is infeasible
 
   if (std::isnan(reginit)) {
-    xreg_ = reg_min_;
-    ureg_ = reg_min_;
+    preg_ = reg_min_;
+    dreg_ = reg_min_;
   } else {
-    xreg_ = reginit;
-    ureg_ = reginit;
+    preg_ = reginit;
+    dreg_ = reginit;
   }
   
+  bool recalcDiff = true;
   for (iter_ = 0; iter_ < maxiter; ++iter_) {
 
-
-    was_feasible_ = false;
-    bool recalcDiff = true;
+    recalcDiff = true;
 
     while (true) {
       try {
         computeDirection(recalcDiff);
       } 
       catch (std::exception& e) {
         recalcDiff = false;
         increaseRegularization();
-        if (xreg_ == reg_max_) {
+        if (preg_ == reg_max_) {
           return false;
         } else {
           continue;
         }
       }
       break;
     }
 
     // KKT termination criteria
-    if(use_kkt_criteria_){
-      if (KKT_  <= termination_tol_) {
-        STOP_PROFILER("SolverSQP::solve");
-        return true;
+    checkKKTConditions();
+    if (KKT_  <= termination_tol_) {
+      if(with_callbacks_){
+        printCallbacks();
       }
-    }  
+      STOP_PROFILER("SolverSQP::solve");
+      return true;
+    }
+      
 
     gap_list_.push_back(gap_norm_);
     cost_list_.push_back(cost_);
 
     // We need to recalculate the derivatives when the step length passes
     for (std::vector<double>::const_iterator it = alphas_.begin(); it != alphas_.end(); ++it) {
       steplength_ = *it;
@@ -156,24 +160,57 @@
     }
 
     if (steplength_ > th_stepdec_) {
       decreaseRegularization();
     }
     if (steplength_ <= th_stepinc_) {
       increaseRegularization();
-      if (xreg_ == reg_max_) {
+      if (preg_ == reg_max_) {
         STOP_PROFILER("SolverSQP::solve");
         return false;
       }
     }
 
     if(with_callbacks_){
       printCallbacks();
     }
   }
+
+
+  if (extra_iteration_for_last_kkt_){
+    recalcDiff = true;
+
+    while (true) {
+      try {
+        computeDirection(recalcDiff);
+      } 
+      catch (std::exception& e) {
+        recalcDiff = false;
+        increaseRegularization();
+        if (preg_ == reg_max_) {
+          return false;
+        } else {
+          continue;
+        }
+      }
+      break;
+    }
+
+    // KKT termination criteria
+    checkKKTConditions();
+    if (KKT_  <= termination_tol_) {
+      if(with_callbacks_){
+        printCallbacks();
+      }
+      STOP_PROFILER("SolverSQP::solve");
+      return true;
+    }
+  }
+
+
   STOP_PROFILER("SolverSQP::solve");
   return false;
 }
 
 
 void SolverSQP::computeDirection(const bool recalcDiff){
   START_PROFILER("SolverSQP::computeDirection");
@@ -185,59 +222,72 @@
   for (std::size_t t = 0; t < T; ++t) {
     gap_norm_ += fs_[t].lpNorm<1>();   
   }
   gap_norm_ += fs_.back().lpNorm<1>();   
 
   merit_ = cost_ + mu_*gap_norm_;
 
-  // KKT termination criteria
-  if(use_kkt_criteria_){
-    checkKKTConditions();
-  }  
-
   backwardPass();
   forwardPass();
 
   STOP_PROFILER("SolverSQP::computeDirection");
 
 }
 
 void SolverSQP::checkKKTConditions(){
   KKT_ = 0.;
   const std::size_t T = problem_->get_T();
   const std::size_t ndx = problem_->get_ndx();
   const std::vector<boost::shared_ptr<ActionDataAbstract> >& datas = problem_->get_runningDatas();
   for (std::size_t t = 0; t < T; ++t) {
     const boost::shared_ptr<ActionDataAbstract>& d = datas[t];
-    KKT_ = std::max(KKT_, (d->Lx + d->Fx.transpose() * lag_mul_[t+1] - lag_mul_[t]).lpNorm<Eigen::Infinity>());
-    KKT_ = std::max(KKT_, (d->Lu + d->Fu.transpose() * lag_mul_[t+1]).lpNorm<Eigen::Infinity>());
+    tmp_vec_x_ = d->Lx;
+    tmp_vec_x_.noalias() += d->Fx.transpose() * lag_mul_[t+1];
+    tmp_vec_x_ -= lag_mul_[t];
+    tmp_vec_u_[t] = d->Lu;
+    tmp_vec_u_[t].noalias() += d->Fu.transpose() * lag_mul_[t+1];
+    KKT_ = std::max(KKT_, tmp_vec_x_.lpNorm<Eigen::Infinity>());
+    KKT_ = std::max(KKT_, tmp_vec_u_[t].lpNorm<Eigen::Infinity>());
     fs_flat_.segment(t*ndx, ndx) = fs_[t];
   }
   fs_flat_.tail(ndx) = fs_.back();
   const boost::shared_ptr<ActionDataAbstract>& d_ter = problem_->get_terminalData();
-  KKT_ = std::max(KKT_, (d_ter->Lx - lag_mul_.back()).lpNorm<Eigen::Infinity>());
+  tmp_vec_x_ = d_ter->Lx;
+  tmp_vec_x_ -= lag_mul_.back();
+  KKT_ = std::max(KKT_, tmp_vec_x_.lpNorm<Eigen::Infinity>());
   KKT_ = std::max(KKT_, fs_flat_.lpNorm<Eigen::Infinity>());
 }
 
 
-void SolverSQP::forwardPass(){
+void SolverSQP::forwardPass(const double stepLength){
+    (void)stepLength;
+
     START_PROFILER("SolverSQP::forwardPass");
-    x_grad_norm_ = 0; u_grad_norm_ = 0;
+    x_grad_norm_ = 0; 
+    u_grad_norm_ = 0;
 
     const std::size_t T = problem_->get_T();
     const std::vector<boost::shared_ptr<ActionDataAbstract> >& datas = problem_->get_runningDatas();
     for (std::size_t t = 0; t < T; ++t) {
       const boost::shared_ptr<ActionDataAbstract>& d = datas[t];
-      lag_mul_[t].noalias() = Vxx_[t] * (dx_[t] - fs_[t]) + Vx_[t];
-      du_[t].noalias() = -K_[t]*(dx_[t]) - k_[t];
-      dx_[t+1].noalias() = (d->Fx - (d->Fu * K_[t]))*(dx_[t]) - (d->Fu * (k_[t])) + fs_[t+1];
+      tmp_vec_x_ = dx_[t] - fs_[t];
+      lag_mul_[t].noalias() = Vxx_[t] * tmp_vec_x_;
+      lag_mul_[t].noalias() += Vx_[t];
+      du_[t].noalias() = - K_[t] * dx_[t];
+      du_[t].noalias() -= k_[t];
+      dx_[t+1].noalias() = fs_[t+1];
+      dx_[t+1].noalias() += d->Fu * du_[t];
+      dx_[t+1].noalias() += d->Fx * dx_[t];
       x_grad_norm_ += dx_[t].lpNorm<1>(); // assuming that there is no gap in the initial state
       u_grad_norm_ += du_[t].lpNorm<1>();
     }
-    lag_mul_.back() = Vxx_.back() * (dx_.back() - fs_.back()) + Vx_.back();
+
+    lag_mul_.back() = Vx_.back();
+    tmp_vec_x_ = dx_.back() - fs_.back();
+    lag_mul_.back().noalias() += Vxx_.back() * tmp_vec_x_;
     x_grad_norm_ += dx_.back().lpNorm<1>(); // assuming that there is no gap in the initial state
     x_grad_norm_ = x_grad_norm_/(double)(T+1);
     u_grad_norm_ = u_grad_norm_/(double)T; 
     STOP_PROFILER("SolverSQP::forwardPass");
 
 }
 
@@ -257,19 +307,18 @@
     const std::vector<boost::shared_ptr<ActionDataAbstract> >& datas = problem_->get_runningDatas();
 
     for (std::size_t t = 0; t < T; ++t) {
         const boost::shared_ptr<ActionModelAbstract>& m = models[t];
         const boost::shared_ptr<ActionDataAbstract>& d = datas[t];
         const std::size_t nu = m->get_nu();
 
-        // error = x + dx - f(x + dx, u + du)
-        // std::cout << dx_.size() << std::endl;
         m->get_state()->integrate(xs_[t], steplength * dx_[t], xs_try_[t]); 
         if (nu != 0) {
-            us_try_[t].noalias() = us_[t] + steplength * du_[t];
+            us_try_[t].noalias() = us_[t];
+            us_try_[t].noalias() += steplength * du_[t];
         }        
         m->calc(d, xs_try_[t], us_try_[t]);        
         cost_try_ += d->cost;
 
         if (t > 0){
           const boost::shared_ptr<ActionDataAbstract>& d_prev = datas[t-1];
           m->get_state()->diff(xs_try_[t], d_prev->xnext, fs_try_[t-1]);
@@ -308,19 +357,27 @@
 }
 
 void SolverSQP::printCallbacks(){
   if (this->get_iter() % 10 == 0) {
     std::cout << "iter     merit         cost         grad      step    ||gaps||        KKT";
     std::cout << std::endl;
   }
-  std::cout << std::setw(4) << this->get_iter() << "  ";
+  if(KKT_ < termination_tol_){
+    std::cout << std::setw(4) << "END" << "  ";
+  } else {
+    std::cout << std::setw(4) << this->get_iter()+1 << "  ";
+  }
   std::cout << std::scientific << std::setprecision(5) << this->get_merit() << "  ";
   std::cout << std::scientific << std::setprecision(5) << this->get_cost() << "  ";
   std::cout << this->get_xgrad_norm() + this->get_ugrad_norm() << "  ";
-  std::cout << std::fixed << std::setprecision(4) << this->get_steplength() << "  ";
+  if(KKT_ < termination_tol_){
+    std::cout << std::fixed << std::setprecision(4) << " ---- " << "  ";
+  } else {
+    std::cout << std::fixed << std::setprecision(4) << this->get_steplength() << "  ";
+  }
   std::cout << std::scientific << std::setprecision(5) << this->get_gap_norm() << "  ";
   std::cout << std::scientific << std::setprecision(5) << KKT_;
   std::cout << std::endl;
   std::cout << std::flush;
 }
 
 void SolverSQP::setCallbacks(bool inCallbacks){
```

### Comparing `cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/activation.cpp` & `cmeel_mim_solvers-0.0.4/tests/factory/model.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,66 @@
 ///////////////////////////////////////////////////////////////////////////////
 // 
-// This file is a modified version of the activation model unittests factory from the Crocoddyl library
+// This file is a modified version of the cost model unittests factory from the Crocoddyl library
 // This modified version is used for testing purposes only
-// Original file : https://github.com/loco-3d/crocoddyl/blob/devel/unittest/factory/activation.cpp
+// Original file : https://github.com/loco-3d/crocoddyl/blob/devel/unittest/factory/cost.hpp
 // 
 // BSD 3-Clause License
 // Copyright (C) 2023, New York University
 //
 // Copyright note valid unless otherwise stated in individual files.
 // All rights reserved.
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "activation.hpp"
+#ifndef MIM_SOLVERS_MODEL_FACTORY_HPP_
+#define MIM_SOLVERS_MODEL_FACTORY_HPP_
 
-#include "../../random_generator.hpp"
-#include <crocoddyl/core/activations/quadratic-barrier.hpp>
-#include <crocoddyl/core/activations/quadratic.hpp>
-#include <crocoddyl/core/utils/exception.hpp>
+#include "constraints.hpp"
+#include "point-mass.hpp"
 
 namespace mim_solvers {
 namespace unittest {
 
-const std::vector<ActivationModelTypes::Type> ActivationModelTypes::all(
-    ActivationModelTypes::init_all());
-
-std::ostream& operator<<(std::ostream& os, ActivationModelTypes::Type type) {
-  switch (type) {
-    case ActivationModelTypes::ActivationModelQuad:
-      os << "ActivationModelQuad";
-      break;
-    case ActivationModelTypes::ActivationModelQuadraticBarrier:
-      os << "ActivationModelQuadraticBarrier";
-      break;
-    case ActivationModelTypes::NbActivationModelTypes:
-      os << "NbActivationModelTypes";
-      break;
-    default:
-      break;
+struct ModelTypes {
+  enum Type {
+    PointMass1D,
+    PointMass2D,
+    NbModelTypes
+  };
+  static std::vector<Type> init_all() {
+    std::vector<Type> v;
+    v.reserve(NbModelTypes);
+    for (int i = 0; i < NbModelTypes; ++i) {
+      v.push_back((Type)i);
+    }
+    return v;
   }
-  return os;
-}
-
-ActivationModelFactory::ActivationModelFactory() {}
-ActivationModelFactory::~ActivationModelFactory() {}
+  static const std::vector<Type> all;
+};
 
-boost::shared_ptr<crocoddyl::ActivationModelAbstract>
-ActivationModelFactory::create(ActivationModelTypes::Type activation_type,
-                               std::size_t nr) const {
-  boost::shared_ptr<crocoddyl::ActivationModelAbstract> activation;
-  Eigen::VectorXd lb = Eigen::VectorXd::Random(nr);
-  Eigen::VectorXd ub =
-      lb + Eigen::VectorXd::Ones(nr) + Eigen::VectorXd::Random(nr);
-
-  switch (activation_type) {
-    case ActivationModelTypes::ActivationModelQuad:
-      activation = boost::make_shared<crocoddyl::ActivationModelQuad>(nr);
-      break;
-    case ActivationModelTypes::ActivationModelQuadraticBarrier:
-      activation =
-          boost::make_shared<crocoddyl::ActivationModelQuadraticBarrier>(
-              crocoddyl::ActivationBounds(lb, ub));
-      break;
-    default:
-      throw_pretty(__FILE__ ":\n Construct wrong ActivationModelTypes::Type");
-      break;
-  }
-  return activation;
-}
+std::ostream& operator<<(std::ostream& os, ModelTypes::Type type);
 
+class ModelFactory {
+ public:
+  EIGEN_MAKE_ALIGNED_OPERATOR_NEW
+
+  // typedef crocoddyl::MathBaseTpl<double> MathBase;
+  // typedef typename MathBase::Vector6s Vector6d;
+
+  explicit ModelFactory();
+  ~ModelFactory();
+
+  boost::shared_ptr<crocoddyl::DifferentialActionModelAbstract> create(
+      ModelTypes::Type model_type, 
+      XConstraintType::Type x_cstr_type,
+      UConstraintType::Type u_cstr_type,
+      bool isInitial,
+      bool isTerminal) const;
+};
+
+// boost::shared_ptr<crocoddyl::CostModelAbstract> create_random_cost(
+//     StateModelTypes::Type state_type,
+//     std::size_t nu = std::numeric_limits<std::size_t>::max());
 }  // namespace unittest
 }  // namespace mim_solvers
+
+#endif  // MIM_SOLVERS_COST_FACTORY_HPP_
```

### Comparing `cmeel_mim_solvers-0.0.2/tests/factory/crocoddyl/state.hpp` & `cmeel_mim_solvers-0.0.4/tests/factory/solver.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 ///////////////////////////////////////////////////////////////////////////////
 // 
-// This file is a modified version of the state model unittests factory from the Crocoddyl library
-// This modified version is used for testing purposes only
-// Original file : https://github.com/loco-3d/crocoddyl/blob/devel/unittest/factory/state.hpp
+// This file is a modified version of the solvers unittests from the Crocoddyl library
+// This modified version is used to test our solvers (mim_solvers repository)
+// Original file : https://github.com/loco-3d/crocoddyl/blob/devel/unittest/factory/solver.hpp
 // 
 // BSD 3-Clause License
 // Copyright (C) 2023, New York University
 //
 // Copyright note valid unless otherwise stated in individual files.
 // All rights reserved.
 ///////////////////////////////////////////////////////////////////////////////
 
-#ifndef MIM_SOLVERS_STATE_FACTORY_HPP_
-#define MIM_SOLVERS_STATE_FACTORY_HPP_
+#ifndef MIM_SOLVERS_SOLVER_FACTORY_HPP_
+#define MIM_SOLVERS_SOLVER_FACTORY_HPP_
 
-#include <crocoddyl/core/numdiff/state.hpp>
-#include <crocoddyl/core/state-base.hpp>
-#include <crocoddyl/core/utils/exception.hpp>
+#include <crocoddyl/core/solver-base.hpp>
 
-#include "pinocchio_model.hpp"
+#include "mim_solvers/sqp.hpp"
+#include "mim_solvers/csqp.hpp"
+#ifdef MIM_SOLVERS_WITH_PROXQP
+  #include "mim_solvers/csqp_proxqp.hpp"
+#endif
+#include "problem.hpp"
 
 namespace mim_solvers {
 namespace unittest {
 
-struct StateModelTypes {
+struct SolverTypes {
   enum Type {
-    StateVector,
-    StateMultibody_Hector,
-    StateMultibody_TalosArm,
-    StateMultibody_HyQ,
-    StateMultibody_Talos,
-    StateMultibody_RandomHumanoid,
-    NbStateModelTypes
+    SolverSQP,
+    SolverCSQP,
+    SolverPROXQP,
+    NbSolverTypes
   };
   static std::vector<Type> init_all() {
     std::vector<Type> v;
-    v.clear();
-    for (int i = 0; i < NbStateModelTypes; ++i) {
+    v.reserve(NbSolverTypes);
+    for (int i = 0; i < NbSolverTypes; ++i) {
+#ifndef MIM_SOLVERS_WITH_PROXQP
+      if ((Type)i == SolverPROXQP) {
+        continue;
+      }
+#endif
       v.push_back((Type)i);
     }
     return v;
   }
   static const std::vector<Type> all;
 };
 
-std::ostream& operator<<(std::ostream& os, StateModelTypes::Type type);
+std::ostream& operator<<(std::ostream& os, SolverTypes::Type type);
 
-class StateModelFactory {
+class SolverFactory {
  public:
   EIGEN_MAKE_ALIGNED_OPERATOR_NEW
 
-  explicit StateModelFactory();
-  ~StateModelFactory();
+  explicit SolverFactory();
+  ~SolverFactory();
 
-  boost::shared_ptr<crocoddyl::StateAbstract> create(
-      StateModelTypes::Type state_type) const;
+  boost::shared_ptr<crocoddyl::SolverAbstract> create(
+      SolverTypes::Type solver_type, 
+      ProblemTypes::Type problem_type,
+      ModelTypes::Type model_type,
+      XConstraintType::Type x_cstr_type,
+      UConstraintType::Type u_cstr_type) const;
 };
 
 }  // namespace unittest
 }  // namespace mim_solvers
 
-#endif  // MIM_SOLVERS_STATE_FACTORY_HPP_
+#endif  // MIM_SOLVERS_SOLVER_FACTORY_HPP_
```

### Comparing `cmeel_mim_solvers-0.0.2/tests/random_generator.hpp` & `cmeel_mim_solvers-0.0.4/tests/random_generator.hpp`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/tests/unittest_common.hpp` & `cmeel_mim_solvers-0.0.4/tests/unittest_common.hpp`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.cmake-format.py` & `cmeel_mim_solvers-0.0.4/cmake/.cmake-format.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/Makefile` & `cmeel_mim_solvers-0.0.4/cmake/.docs/Makefile`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/cmake.py` & `cmeel_mim_solvers-0.0.4/cmake/.docs/cmake.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/conf.py` & `cmeel_mim_solvers-0.0.4/cmake/.docs/conf.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/examples/minimal-with-packages.cmake` & `cmeel_mim_solvers-0.0.4/cmake/.docs/examples/minimal-with-packages.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/index.rst` & `cmeel_mim_solvers-0.0.4/cmake/.docs/index.rst`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/pages/base.rst` & `cmeel_mim_solvers-0.0.4/cmake/.docs/pages/base.rst`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/pages/cmake-packages.rst` & `cmeel_mim_solvers-0.0.4/cmake/.docs/pages/cmake-packages.rst`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/pages/dependencies.rst` & `cmeel_mim_solvers-0.0.4/cmake/.docs/pages/dependencies.rst`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/pages/developers.rst` & `cmeel_mim_solvers-0.0.4/cmake/.docs/pages/developers.rst`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.docs/pages/other.rst` & `cmeel_mim_solvers-0.0.4/cmake/.docs/pages/other.rst`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.github/workflows/cmake.yml` & `cmeel_mim_solvers-0.0.4/cmake/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/.pre-commit-config.yaml` & `cmeel_mim_solvers-0.0.4/cmake/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/Config.cmake.in` & `cmeel_mim_solvers-0.0.4/cmake/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/GNUInstallDirs.cmake` & `cmeel_mim_solvers-0.0.4/cmake/GNUInstallDirs.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/README.md` & `cmeel_mim_solvers-0.0.4/cmake/README.md`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/_unittests/catkin/CMakeLists.txt` & `cmeel_mim_solvers-0.0.4/cmake/_unittests/catkin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/_unittests/cpp/CMakeLists.txt` & `cmeel_mim_solvers-0.0.4/cmake/_unittests/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/_unittests/dependency/CMakeLists.txt` & `cmeel_mim_solvers-0.0.4/cmake/_unittests/dependency/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/_unittests/python/CMakeLists.txt` & `cmeel_mim_solvers-0.0.4/cmake/_unittests/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/_unittests/run_unit_tests.sh` & `cmeel_mim_solvers-0.0.4/cmake/_unittests/run_unit_tests.sh`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/_unittests/test_pkg-config.cmake` & `cmeel_mim_solvers-0.0.4/cmake/_unittests/test_pkg-config.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/announce-gen` & `cmeel_mim_solvers-0.0.4/cmake/announce-gen`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/apple.cmake` & `cmeel_mim_solvers-0.0.4/cmake/apple.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/base.cmake` & `cmeel_mim_solvers-0.0.4/cmake/base.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/boost.cmake` & `cmeel_mim_solvers-0.0.4/cmake/boost.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/boost/FindBoost.cmake` & `cmeel_mim_solvers-0.0.4/cmake/boost/FindBoost.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/catkin.cmake` & `cmeel_mim_solvers-0.0.4/cmake/catkin.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cmake_reinstall.cmake.in` & `cmeel_mim_solvers-0.0.4/cmake/cmake_reinstall.cmake.in`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cmake_uninstall.cmake.in` & `cmeel_mim_solvers-0.0.4/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/compiler.cmake` & `cmeel_mim_solvers-0.0.4/cmake/compiler.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/componentConfig.cmake.in` & `cmeel_mim_solvers-0.0.4/cmake/componentConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/config.h.cmake` & `cmeel_mim_solvers-0.0.4/cmake/config.h.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/config.hh.cmake` & `cmeel_mim_solvers-0.0.4/cmake/config.hh.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/coverage.cmake` & `cmeel_mim_solvers-0.0.4/cmake/coverage.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cpack.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cpack.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/createshexe.cmake` & `cmeel_mim_solvers-0.0.4/cmake/createshexe.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cxx-standard.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cxx-standard.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cxx11.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cxx11.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cython/cython.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cython/cython.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython/Support.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython2.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython2.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cython/python/FindPython3.cmake` & `cmeel_mim_solvers-0.0.4/cmake/cython/python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/cython/setup.in.py` & `cmeel_mim_solvers-0.0.4/cmake/cython/setup.in.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/debian.cmake` & `cmeel_mim_solvers-0.0.4/cmake/debian.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/deprecated.hh.cmake` & `cmeel_mim_solvers-0.0.4/cmake/deprecated.hh.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/dist.cmake` & `cmeel_mim_solvers-0.0.4/cmake/dist.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/distcheck.cmake` & `cmeel_mim_solvers-0.0.4/cmake/distcheck.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen.cmake` & `cmeel_mim_solvers-0.0.4/cmake/doxygen.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/LICENSE` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/LICENSE`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/MathJax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/MathJax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/CHTML-preview.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/CHTML-preview.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/FontWarnings.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/FontWarnings.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/HelpDialog.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/HelpDialog.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MatchWebFonts.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MatchWebFonts.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MathEvents.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MathEvents.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MathMenu.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MathMenu.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/MathZoom.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/MathZoom.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/Safe.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/Safe.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/AMScd.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/AMScd.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/AMSmath.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/AMSmath.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/AMSsymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/AMSsymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/HTML.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/HTML.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/action.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/action.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/autobold.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/autobold.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/autoload-all.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/autoload-all.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/bbox.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/bbox.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/begingroup.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/begingroup.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/boldsymbol.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/boldsymbol.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/cancel.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/cancel.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/color.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/color.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/enclose.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/enclose.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/extpfeil.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/extpfeil.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/mathchoice.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/mathchoice.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/mediawiki-texvc.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/mediawiki-texvc.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/mhchem.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/mhchem.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/newcommand.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/newcommand.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/noErrors.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/noErrors.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/noUndefined.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/noUndefined.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/unicode.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/unicode.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/TeX/verb.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/TeX/verb.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/jsMath2jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/jsMath2jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/tex2jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/tex2jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/extensions/toMathML.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/extensions/toMathML.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/Arrows.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/Arrows.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiactForSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/CombDiactForSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/Dingbats.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/Dingbats.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/GeneralPunctuation.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/GeneralPunctuation.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/GeometricShapes.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/GeometricShapes.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/GreekAndCoptic.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/GreekAndCoptic.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/Latin1Supplement.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/Latin1Supplement.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/LetterlikeSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/LetterlikeSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsB.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscMathSymbolsB.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscSymbolsAndArrows.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscSymbolsAndArrows.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/MiscTechnical.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/MiscTechnical.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SpacingModLetters.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SpacingModLetters.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SuppMathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SuppMathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsB.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/element/mml/optable/SupplementalArrowsB.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/AsciiMath/config.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/AsciiMath/config.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/AsciiMath/jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/AsciiMath/jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/config.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/config.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/a.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/a.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/b.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/b.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/c.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/c.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/d.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/d.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/e.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/e.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/f.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/f.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/fr.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/fr.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/g.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/g.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/h.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/h.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/i.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/i.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/j.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/j.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/k.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/k.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/l.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/l.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/m.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/m.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/n.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/n.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/o.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/o.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/opf.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/opf.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/p.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/p.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/q.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/q.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/r.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/r.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/s.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/s.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/scr.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/scr.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/t.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/t.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/u.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/u.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/v.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/v.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/w.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/w.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/x.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/x.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/y.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/y.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/entities/z.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/entities/z.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/MathML/jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/MathML/jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/TeX/config.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/TeX/config.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/input/TeX/jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/input/TeX/jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/CommonHTML/config.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/CommonHTML/config.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/CommonHTML/jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/CommonHTML/jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/annotation-xml.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/annotation-xml.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/maction.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/maction.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/menclose.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/menclose.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/mglyph.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/mglyph.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/mmultiscripts.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/mmultiscripts.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/ms.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/ms.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/mtable.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/mtable.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/autoload/multiline.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/autoload/multiline.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/config.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/config.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Arrows.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Arrows.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/BoxDrawing.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/BoxDrawing.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Dingbats.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Dingbats.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/EnclosedAlphanum.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/EnclosedAlphanum.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeneralPunctuation.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeneralPunctuation.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeometricShapes.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GeometricShapes.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GreekAndCoptic.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/GreekAndCoptic.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Latin1Supplement.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Latin1Supplement.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LatinExtendedA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LatinExtendedA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LetterlikeSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/LetterlikeSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscMathSymbolsB.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscMathSymbolsB.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscTechnical.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/MiscTechnical.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/PUA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/PUA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SpacingModLetters.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SpacingModLetters.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SuppMathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/AMS/Regular/SuppMathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Bold/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Bold/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Caligraphic/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Other.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/Other.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/PUA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Bold/PUA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Other.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/Other.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/PUA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Fraktur/Regular/PUA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Arrows.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Arrows.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiactForSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/CombDiactForSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeneralPunctuation.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeneralPunctuation.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeometricShapes.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GeometricShapes.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GreekAndCoptic.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/GreekAndCoptic.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Latin1Supplement.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Latin1Supplement.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedB.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LatinExtendedB.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LetterlikeSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/LetterlikeSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscMathSymbolsA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscMathSymbolsA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscTechnical.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/MiscTechnical.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SpacingModLetters.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SpacingModLetters.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SuppMathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SuppMathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SupplementalArrowsA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Bold/SupplementalArrowsA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GeneralPunctuation.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GeneralPunctuation.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GreekAndCoptic.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/GreekAndCoptic.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedB.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LatinExtendedB.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LetterlikeSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/LetterlikeSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/MathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Italic/MathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GeometricShapes.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GeometricShapes.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GreekAndCoptic.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/GreekAndCoptic.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedA.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedA.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedB.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LatinExtendedB.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LetterlikeSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/LetterlikeSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MiscSymbols.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/MiscSymbols.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SpacingModLetters.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SpacingModLetters.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SuppMathOperators.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Main/Regular/SuppMathOperators.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/BoldItalic/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/BoldItalic/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/Italic/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Math/Italic/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Other.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Bold/Other.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Other.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Italic/Other.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Other.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/SansSerif/Regular/Other.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Script/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size1/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size1/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size2/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size2/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size3/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size3/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size4/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Size4/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/BasicLatin.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/BasicLatin.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/CombDiacritMarks.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/CombDiacritMarks.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Main.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Main.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Other.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/Typewriter/Regular/Other.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata-extra.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata-extra.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/fonts/TeX/fontdata.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/MathJax/jax/output/SVG/jax.js` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/MathJax/jax/output/SVG/jax.js`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/doxygen.css` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/doxygen.css`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/footer.html` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/footer.html`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/header-mathjax.html` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/header-mathjax.html`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/header.html` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/header.html`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/header.tex` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/header.tex`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/style.rtf` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/style.rtf`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/style.tex` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/style.tex`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/doxygen/tabs.css` & `cmeel_mim_solvers-0.0.4/cmake/doxygen/tabs.css`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/dynamic_graph/python-module-py.cc.in` & `cmeel_mim_solvers-0.0.4/cmake/dynamic_graph/python-module-py.cc.in`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/dynamic_graph/submodule/__init__.py.cmake` & `cmeel_mim_solvers-0.0.4/cmake/dynamic_graph/submodule/__init__.py.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/eigen.cmake` & `cmeel_mim_solvers-0.0.4/cmake/eigen.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/filefilter.txt` & `cmeel_mim_solvers-0.0.4/cmake/filefilter.txt`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/CDD/FindCDD.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/CDD/FindCDD.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/CLP/FindCLP.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/CLP/FindCLP.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/CoinUtils/FindCoinUtils.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/CoinUtils/FindCoinUtils.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/CppAD/Findcppad.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/CppAD/Findcppad.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/CppAD/Findcppadcg.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/CppAD/Findcppadcg.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/GMP/FindGMP.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/GMP/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/Julia/FindJulia.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/Julia/FindJulia.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/MPFR/FindMPFR.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/MPFR/FindMPFR.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/OpenMP/FindOpenMP.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/OpenMP/FindOpenMP.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/OpenRTM/FindOpenRTM.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/OpenRTM/FindOpenRTM.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/Qhull/FindQhull.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/Qhull/FindQhull.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/Simde/FindSimde.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/Simde/FindSimde.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/TinyXML/FindTinyXML.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/TinyXML/FindTinyXML.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/assimp/Findassimp.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/assimp/Findassimp.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/glpk/Findglpk.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/glpk/Findglpk.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/find-external/qpOASES/FindqpOASES.cmake` & `cmeel_mim_solvers-0.0.4/cmake/find-external/qpOASES/FindqpOASES.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/fix-license.sh` & `cmeel_mim_solvers-0.0.4/cmake/fix-license.sh`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/geometric-tools.cmake` & `cmeel_mim_solvers-0.0.4/cmake/geometric-tools.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/git-archive-all.py` & `cmeel_mim_solvers-0.0.4/cmake/git-archive-all.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/git-archive-all.sh` & `cmeel_mim_solvers-0.0.4/cmake/git-archive-all.sh`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/github/update-doxygen-doc.sh` & `cmeel_mim_solvers-0.0.4/cmake/github/update-doxygen-doc.sh`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/gitlog-to-changelog` & `cmeel_mim_solvers-0.0.4/cmake/gitlog-to-changelog`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/gtest.cmake` & `cmeel_mim_solvers-0.0.4/cmake/gtest.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/header.cmake` & `cmeel_mim_solvers-0.0.4/cmake/header.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/hpp.cmake` & `cmeel_mim_solvers-0.0.4/cmake/hpp.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/hpp/doc.cmake` & `cmeel_mim_solvers-0.0.4/cmake/hpp/doc.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/hpp/doc/layout.xml` & `cmeel_mim_solvers-0.0.4/cmake/hpp/doc/layout.xml`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/hpp/idl/omniidl_be_python_with_docstring.py` & `cmeel_mim_solvers-0.0.4/cmake/hpp/idl/omniidl_be_python_with_docstring.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/ide.cmake` & `cmeel_mim_solvers-0.0.4/cmake/ide.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/idl.cmake` & `cmeel_mim_solvers-0.0.4/cmake/idl.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/idlrtc.cmake` & `cmeel_mim_solvers-0.0.4/cmake/idlrtc.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/image/visp.cmake` & `cmeel_mim_solvers-0.0.4/cmake/image/visp.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/install-data.cmake` & `cmeel_mim_solvers-0.0.4/cmake/install-data.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/julia.cmake` & `cmeel_mim_solvers-0.0.4/cmake/julia.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/kineo.cmake` & `cmeel_mim_solvers-0.0.4/cmake/kineo.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/lapack.cmake` & `cmeel_mim_solvers-0.0.4/cmake/lapack.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/logging.cmake` & `cmeel_mim_solvers-0.0.4/cmake/logging.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/man.cmake` & `cmeel_mim_solvers-0.0.4/cmake/man.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/memorycheck_unit_test.cmake.in` & `cmeel_mim_solvers-0.0.4/cmake/memorycheck_unit_test.cmake.in`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/metapodfromurdf.cmake` & `cmeel_mim_solvers-0.0.4/cmake/metapodfromurdf.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/modernize-links.cmake` & `cmeel_mim_solvers-0.0.4/cmake/modernize-links.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/msvc-specific.cmake` & `cmeel_mim_solvers-0.0.4/cmake/msvc-specific.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/msvc.vcxproj.user.in` & `cmeel_mim_solvers-0.0.4/cmake/msvc.vcxproj.user.in`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/openhrp.cmake` & `cmeel_mim_solvers-0.0.4/cmake/openhrp.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/openhrpcontroller.cmake` & `cmeel_mim_solvers-0.0.4/cmake/openhrpcontroller.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/openrtm.cmake` & `cmeel_mim_solvers-0.0.4/cmake/openrtm.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/oscheck.cmake` & `cmeel_mim_solvers-0.0.4/cmake/oscheck.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/package-config.cmake` & `cmeel_mim_solvers-0.0.4/cmake/package-config.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/pkg-config.cmake` & `cmeel_mim_solvers-0.0.4/cmake/pkg-config.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/pkg-config.pc.cmake` & `cmeel_mim_solvers-0.0.4/cmake/pkg-config.pc.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/portability.cmake` & `cmeel_mim_solvers-0.0.4/cmake/portability.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/post-project.cmake` & `cmeel_mim_solvers-0.0.4/cmake/post-project.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/pthread.cmake` & `cmeel_mim_solvers-0.0.4/cmake/pthread.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/pyproject.py` & `cmeel_mim_solvers-0.0.4/cmake/pyproject.py`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/python-helpers.cmake` & `cmeel_mim_solvers-0.0.4/cmake/python-helpers.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/python.cmake` & `cmeel_mim_solvers-0.0.4/cmake/python.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/qhull.cmake` & `cmeel_mim_solvers-0.0.4/cmake/qhull.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/release.cmake` & `cmeel_mim_solvers-0.0.4/cmake/release.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/relpath.cmake` & `cmeel_mim_solvers-0.0.4/cmake/relpath.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/ros.cmake` & `cmeel_mim_solvers-0.0.4/cmake/ros.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/sdformat.cmake` & `cmeel_mim_solvers-0.0.4/cmake/sdformat.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/shared-library.cmake` & `cmeel_mim_solvers-0.0.4/cmake/shared-library.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/sphinx.cmake` & `cmeel_mim_solvers-0.0.4/cmake/sphinx.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/stubs.cmake` & `cmeel_mim_solvers-0.0.4/cmake/stubs.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/swig.cmake` & `cmeel_mim_solvers-0.0.4/cmake/swig.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/test.cmake` & `cmeel_mim_solvers-0.0.4/cmake/test.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/uninstall.cmake` & `cmeel_mim_solvers-0.0.4/cmake/uninstall.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/version-script.cmake` & `cmeel_mim_solvers-0.0.4/cmake/version-script.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/version.cmake` & `cmeel_mim_solvers-0.0.4/cmake/version.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/warning.hh.cmake` & `cmeel_mim_solvers-0.0.4/cmake/warning.hh.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/cmake/xacro.cmake` & `cmeel_mim_solvers-0.0.4/cmake/xacro.cmake`

 * *Files identical despite different names*

### Comparing `cmeel_mim_solvers-0.0.2/PKG-INFO` & `cmeel_mim_solvers-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmeel-mim-solvers
-Version: 0.0.2
+Version: 0.0.4
 Summary: A fast and flexible implementation of Rigid Body Dynamics algorithms and their analytical derivatives
 Requires-Python: >=3.8
 License-Expression: BSD-3-Clause
 Home-page: https://github.com/cmake-wheel/mim_solvers
 Project-URL: Upstream, https://github.com/machines-in-motion/mim_solvers
 Requires-Dist: cmeel
 Requires-Dist: crocoddyl
@@ -12,27 +12,26 @@
 Requires-Dist: cmeel-boost ~= 1.83.0
 Provides-Extra: build
 Requires-Dist: crocoddyl[build] ; extra == "build"
 Requires-Dist: proxsuite[build] ; extra == "build"
 Description-Content-Type: text/markdown
 
 # mim_solvers
-Implementation of numerical solvers used in the Machines in Motion Laboratory. 
-In particular, the Sequential Quadratic Programming (SQP) solver described in [this paper](https://laas.hal.science/hal-04330251) solves nonlinear constrained OCPs efficiently.
+Implementation of efficient numerical optimal control solvers. 
+In particular, the Sequential Quadratic Programming (SQP) solver described in [this paper](https://laas.hal.science/hal-04330251) solves nonlinear constrained OCPs efficiently by leveraging sparsity.
 
-All solvers are implemented by using [Crocoddyl](https://github.com/loco-3d/crocoddyl/tree/devel) (v2.0) as the base software. 
-Consequently, Crocoddyl users can use our efficient solvers while constructing their OCPs using the same API they are used to. 
-The default solvers of Crocoddyl are also re-implemented for benchmarking purposes (namely DDP and FDDP) but with modified termination criteria and line-search.
+All the solvers are implemented based on the API of [Crocoddyl](https://github.com/loco-3d/crocoddyl/tree/devel) (v2). 
+In other words, our solvers take as input a `crocoddyl.ShootingProblem`.
 
 Examples on how to use the solvers can be found in the `examples` directory.
 
 # Dependencies
 - [Pinocchio](https://github.com/stack-of-tasks/pinocchio) (rigid-body dynamics computations)
 - [Crocoddyl](https://github.com/loco-3d/crocoddyl) (optimal control library)
-- [ProxSuite](https://github.com/Simple-Robotics/proxsuite) (quadratic programming) [OPTIONAL]
+- [ProxSuite](https://github.com/Simple-Robotics/proxsuite) (quadratic programming) (optional)
 
 # Installation
 
   ## Using conda
 
 `conda install mim-solvers --channel conda-forge`
 
@@ -42,18 +41,21 @@
 
 `cd mim_solvers && mkdir build && cd build`
 
 `cmake .. [-DCMAKE_BUILD_TYPE=Release] [-DCMAKE_INSTALL_PREFIX=...]`
 
 `make [-j6] && make install`
 
+You can also run unittests using `ctest -v` and benchmarks using `./benchmarks/ur5` or `./benchmarks/solo12` from the build directory.
+
 
 # Contributors
 
 -   [Armand Jordana](https://github.com/ajordana) (NYU): main developer and manager of the project
 -   [Sébastien Kleff](https://github.com/skleff1994) (NYU): main developer and manager of the project
 -   [Avadesh Meduri](https://github.com/avadesh02) (NYU): main developer and manager of the project
 -   [Ludovic Righetti](https://engineering.nyu.edu/faculty/ludovic-righetti) (NYU): project instructor
 -   [Justin Carpentier](https://jcarpent.github.io) (INRIA): project instructor
 -   [Nicolas Mansard](http://projects.laas.fr/gepetto/index.php/Members/NicolasMansard) (LAAS-CNRS): project instructor
 -   [Yann de Mont-Marin](https://github.com/ymontmarin) (INRIA): Conda integration and support
-
+-   [Louis Montaut](https://github.com/lmontaut) (INRIA): CMake support
+-   [Guilhem Saurel](https://github.com/nim65s) (LAAS-CNRS): CMake & pip packaging support
```

