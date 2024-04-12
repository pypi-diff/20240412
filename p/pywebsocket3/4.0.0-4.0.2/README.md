# Comparing `tmp/pywebsocket3-4.0.0.tar.gz` & `tmp/pywebsocket3-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebsocket3-4.0.0.tar", last modified: Fri Apr 12 12:21:34 2024, max compression
+gzip compressed data, was "pywebsocket3-4.0.2.tar", last modified: Fri Apr 12 12:43:06 2024, max compression
```

## Comparing `pywebsocket3-4.0.0.tar` & `pywebsocket3-4.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.192013 pywebsocket3-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 12:21:34.192013 pywebsocket3-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.184013 pywebsocket3-4.0.0/example/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/abort_handshake_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/abort_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/bench_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/benchmark_helper_wsh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.184013 pywebsocket3-4.0.0/example/cgi-bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/cgi-bin/hi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/close_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/cookie_wsh.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25791 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/echo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/echo_noext_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/echo_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/hsts_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/internal_error_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/example/origin_check_wsh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.188013 pywebsocket3-4.0.0/pywebsocket3/
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/_stream_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15001 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.188013 pywebsocket3-4.0.0/pywebsocket3/handshake/
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/handshake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/handshake/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/handshake/hybi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/http_header_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/memorizingfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/msgutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/server_util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18790 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)    34985 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/pywebsocket3/websocket_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.192013 pywebsocket3-4.0.0/pywebsocket3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 12:21:34.000000 pywebsocket3-4.0.0/pywebsocket3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-12 12:21:34.000000 pywebsocket3-4.0.0/pywebsocket3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:21:34.000000 pywebsocket3-4.0.0/pywebsocket3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 12:21:34.000000 pywebsocket3-4.0.0/pywebsocket3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 12:21:34.000000 pywebsocket3-4.0.0/pywebsocket3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 12:21:34.192013 pywebsocket3-4.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2881 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.192013 pywebsocket3-4.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25389 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/client_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/mock.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3289 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/run_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/set_sys_path.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13266 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_dispatch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27161 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_endtoend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8670 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_extensions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6933 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_handshake.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17448 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_handshake_hybi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3634 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_http_header_util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4232 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_memorizingfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5236 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_mock.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37829 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_msgutil.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2822 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7290 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.184013 pywebsocket3-4.0.0/test/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.192013 pywebsocket3-4.0.0/test/testdata/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/abort_by_user_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/blank_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/origin_check_wsh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:21:34.192013 pywebsocket3-4.0.0/test/testdata/handlers/sub/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/sub/exception_in_transfer_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/sub/no_wsh_at_the_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/sub/non_callable_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/sub/plain_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/sub/wrong_handshake_sig_wsh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 12:21:28.000000 pywebsocket3-4.0.0/test/testdata/handlers/sub/wrong_transfer_sig_wsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.540227 pywebsocket3-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 12:43:06.540227 pywebsocket3-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.528227 pywebsocket3-4.0.2/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/abort_handshake_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/abort_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/bench_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/benchmark_helper_wsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.528227 pywebsocket3-4.0.2/example/cgi-bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/cgi-bin/hi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/close_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/cookie_wsh.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25791 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/echo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/echo_noext_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/echo_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/hsts_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/internal_error_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/example/origin_check_wsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.532227 pywebsocket3-4.0.2/pywebsocket3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/_stream_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15001 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18077 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.532227 pywebsocket3-4.0.2/pywebsocket3/handshake/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/handshake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14404 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/handshake/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/handshake/hybi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/http_header_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/memorizingfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/msgutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/server_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18790 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34985 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/pywebsocket3/websocket_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.540227 pywebsocket3-4.0.2/pywebsocket3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 12:43:06.000000 pywebsocket3-4.0.2/pywebsocket3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-12 12:43:06.000000 pywebsocket3-4.0.2/pywebsocket3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:43:06.000000 pywebsocket3-4.0.2/pywebsocket3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 12:43:06.000000 pywebsocket3-4.0.2/pywebsocket3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 12:43:06.000000 pywebsocket3-4.0.2/pywebsocket3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 12:43:06.540227 pywebsocket3-4.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2881 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.536227 pywebsocket3-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25389 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/client_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/mock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3289 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/set_sys_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13266 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_dispatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27161 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_endtoend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8670 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_extensions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6933 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_handshake.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17448 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_handshake_hybi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3634 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_http_header_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4232 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_memorizingfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5236 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_mock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37829 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_msgutil.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2822 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7290 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.528227 pywebsocket3-4.0.2/test/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.536227 pywebsocket3-4.0.2/test/testdata/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/abort_by_user_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/blank_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/origin_check_wsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:43:06.536227 pywebsocket3-4.0.2/test/testdata/handlers/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/sub/exception_in_transfer_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/sub/no_wsh_at_the_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/sub/non_callable_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/sub/plain_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/sub/wrong_handshake_sig_wsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 12:43:00.000000 pywebsocket3-4.0.2/test/testdata/handlers/sub/wrong_transfer_sig_wsh.py
```

### Comparing `pywebsocket3-4.0.0/LICENSE` & `pywebsocket3-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/README.md` & `pywebsocket3-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/abort_handshake_wsh.py` & `pywebsocket3-4.0.2/example/abort_handshake_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/abort_wsh.py` & `pywebsocket3-4.0.2/example/abort_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/bench_wsh.py` & `pywebsocket3-4.0.2/example/bench_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/benchmark_helper_wsh.py` & `pywebsocket3-4.0.2/example/benchmark_helper_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/close_wsh.py` & `pywebsocket3-4.0.2/example/close_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/cookie_wsh.py` & `pywebsocket3-4.0.2/example/cookie_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/echo_client.py` & `pywebsocket3-4.0.2/example/echo_client.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/echo_noext_wsh.py` & `pywebsocket3-4.0.2/example/echo_noext_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/echo_wsh.py` & `pywebsocket3-4.0.2/example/echo_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/hsts_wsh.py` & `pywebsocket3-4.0.2/example/hsts_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/internal_error_wsh.py` & `pywebsocket3-4.0.2/example/internal_error_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/example/origin_check_wsh.py` & `pywebsocket3-4.0.2/example/origin_check_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/__init__.py` & `pywebsocket3-4.0.2/pywebsocket3/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/_stream_exceptions.py` & `pywebsocket3-4.0.2/pywebsocket3/_stream_exceptions.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/common.py` & `pywebsocket3-4.0.2/pywebsocket3/common.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/dispatch.py` & `pywebsocket3-4.0.2/pywebsocket3/dispatch.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/extensions.py` & `pywebsocket3-4.0.2/pywebsocket3/extensions.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/handshake/__init__.py` & `pywebsocket3-4.0.2/pywebsocket3/handshake/__init__.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/handshake/base.py` & `pywebsocket3-4.0.2/pywebsocket3/handshake/base.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/handshake/hybi.py` & `pywebsocket3-4.0.2/pywebsocket3/handshake/hybi.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/http_header_util.py` & `pywebsocket3-4.0.2/pywebsocket3/http_header_util.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/memorizingfile.py` & `pywebsocket3-4.0.2/pywebsocket3/memorizingfile.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/msgutil.py` & `pywebsocket3-4.0.2/pywebsocket3/msgutil.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/request_handler.py` & `pywebsocket3-4.0.2/pywebsocket3/request_handler.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/server_util.py` & `pywebsocket3-4.0.2/pywebsocket3/server_util.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/standalone.py` & `pywebsocket3-4.0.2/pywebsocket3/standalone.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/stream.py` & `pywebsocket3-4.0.2/pywebsocket3/stream.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/util.py` & `pywebsocket3-4.0.2/pywebsocket3/util.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3/websocket_server.py` & `pywebsocket3-4.0.2/pywebsocket3/websocket_server.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/pywebsocket3.egg-info/SOURCES.txt` & `pywebsocket3-4.0.2/pywebsocket3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/setup.py` & `pywebsocket3-4.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,11 +64,11 @@
                       'See pywebsocket3/__init__.py for more detail.'),
     license='See LICENSE',
     name=_PACKAGE_NAME,
     packages=[_PACKAGE_NAME, _PACKAGE_NAME + '.handshake'],
     python_requires='>=2.7',
     install_requires=['six'],
     url='https://github.com/GoogleChromeLabs/pywebsocket3',
-    version='4.0.0',
+    version='4.0.2',
 )
 
 # vi:sts=4 sw=4 et
```

### Comparing `pywebsocket3-4.0.0/test/client_for_testing.py` & `pywebsocket3-4.0.2/test/client_for_testing.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/mock.py` & `pywebsocket3-4.0.2/test/mock.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/run_all.py` & `pywebsocket3-4.0.2/test/run_all.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/set_sys_path.py` & `pywebsocket3-4.0.2/test/set_sys_path.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_dispatch.py` & `pywebsocket3-4.0.2/test/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_endtoend.py` & `pywebsocket3-4.0.2/test/test_endtoend.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_extensions.py` & `pywebsocket3-4.0.2/test/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_handshake.py` & `pywebsocket3-4.0.2/test/test_handshake.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_handshake_hybi.py` & `pywebsocket3-4.0.2/test/test_handshake_hybi.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_http_header_util.py` & `pywebsocket3-4.0.2/test/test_http_header_util.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_memorizingfile.py` & `pywebsocket3-4.0.2/test/test_memorizingfile.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_mock.py` & `pywebsocket3-4.0.2/test/test_mock.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_msgutil.py` & `pywebsocket3-4.0.2/test/test_msgutil.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_stream.py` & `pywebsocket3-4.0.2/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/test_util.py` & `pywebsocket3-4.0.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/abort_by_user_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/abort_by_user_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/blank_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/blank_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/origin_check_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/origin_check_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/sub/exception_in_transfer_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/sub/exception_in_transfer_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/sub/no_wsh_at_the_end.py` & `pywebsocket3-4.0.2/test/testdata/handlers/sub/no_wsh_at_the_end.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/sub/non_callable_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/sub/non_callable_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/sub/plain_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/sub/plain_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/sub/wrong_handshake_sig_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/sub/wrong_handshake_sig_wsh.py`

 * *Files identical despite different names*

### Comparing `pywebsocket3-4.0.0/test/testdata/handlers/sub/wrong_transfer_sig_wsh.py` & `pywebsocket3-4.0.2/test/testdata/handlers/sub/wrong_transfer_sig_wsh.py`

 * *Files identical despite different names*

