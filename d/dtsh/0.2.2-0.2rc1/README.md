# Comparing `tmp/dtsh-0.2.2.tar.gz` & `tmp/dtsh-0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtsh-0.2.2.tar", last modified: Fri Apr 12 17:55:16 2024, max compression
+gzip compressed data, was "dtsh-0.2rc1.tar", last modified: Fri Feb  9 04:38:51 2024, max compression
```

## Comparing `dtsh-0.2.2.tar` & `dtsh-0.2rc1.tar`

### file list

```diff
@@ -1,81 +1,78 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.246240 dtsh-0.2.2/
--rw-r--r--   0 chris     (1000) chris     (1000)    11357 2024-04-02 13:40:11.000000 dtsh-0.2.2/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     3803 2024-04-12 17:55:16.246240 dtsh-0.2.2/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     2278 2024-04-12 17:11:58.000000 dtsh-0.2.2/README.rst
--rw-r--r--   0 chris     (1000) chris     (1000)      601 2024-04-02 13:40:11.000000 dtsh-0.2.2/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)     1882 2024-04-12 17:55:16.247240 dtsh-0.2.2/setup.cfg
--rw-r--r--   0 chris     (1000) chris     (1000)      246 2024-04-03 10:33:46.000000 dtsh-0.2.2/setup.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.238240 dtsh-0.2.2/src/
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.240240 dtsh-0.2.2/src/devicetree/
--rw-r--r--   0 chris     (1000) chris     (1000)      115 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/devicetree/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1227 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/devicetree/_private.py
--rw-r--r--   0 chris     (1000) chris     (1000)    75929 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/devicetree/dtlib.py
--rw-r--r--   0 chris     (1000) chris     (1000)   123133 2024-04-12 17:11:47.000000 dtsh-0.2.2/src/devicetree/edtlib.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5953 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/devicetree/grutils.py
--rw-r--r--   0 chris     (1000) chris     (1000)      128 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/devicetree/typed.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.241240 dtsh-0.2.2/src/dtsh/
--rw-r--r--   0 chris     (1000) chris     (1000)      134 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)    26579 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/autocomp.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.242240 dtsh-0.2.2/src/dtsh/builtins/
--rw-r--r--   0 chris     (1000) chris     (1000)      143 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2247 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/alias.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3170 2024-04-12 16:57:50.000000 dtsh-0.2.2/src/dtsh/builtins/board.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13264 2024-04-12 13:21:54.000000 dtsh-0.2.2/src/dtsh/builtins/cat.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1044 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/cd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2265 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/chosen.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9426 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/find.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6907 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/ls.py
--rw-r--r--   0 chris     (1000) chris     (1000)      775 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/pwd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3606 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/builtins/tree.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5751 2024-04-08 11:28:26.000000 dtsh-0.2.2/src/dtsh/cli.py
--rw-r--r--   0 chris     (1000) chris     (1000)    20889 2024-04-12 16:57:33.000000 dtsh-0.2.2/src/dtsh/config.py
--rw-r--r--   0 chris     (1000) chris     (1000)    29676 2024-04-08 12:25:16.000000 dtsh-0.2.2/src/dtsh/dts.py
--rw-r--r--   0 chris     (1000) chris     (1000)    11257 2024-04-12 16:57:33.000000 dtsh-0.2.2/src/dtsh/dtsh.ini
--rw-r--r--   0 chris     (1000) chris     (1000)     9930 2024-04-12 16:57:41.000000 dtsh-0.2.2/src/dtsh/io.py
--rw-r--r--   0 chris     (1000) chris     (1000)    68494 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/model.py
--rw-r--r--   0 chris     (1000) chris     (1000)    29526 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/modelutils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.243240 dtsh-0.2.2/src/dtsh/rich/
--rw-r--r--   0 chris     (1000) chris     (1000)      133 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/rich/__init__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7989 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/rich/autocomp.py
--rw-r--r--   0 chris     (1000) chris     (1000)    16602 2024-04-12 16:57:44.000000 dtsh-0.2.2/src/dtsh/rich/io.py
--rw-r--r--   0 chris     (1000) chris     (1000)    77083 2024-04-12 16:57:37.000000 dtsh-0.2.2/src/dtsh/rich/modelview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6386 2024-04-08 08:51:42.000000 dtsh-0.2.2/src/dtsh/rich/session.py
--rw-r--r--   0 chris     (1000) chris     (1000)    13244 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/rich/shellutils.py
--rw-r--r--   0 chris     (1000) chris     (1000)    23074 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/rich/svg.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6946 2024-04-08 12:25:16.000000 dtsh-0.2.2/src/dtsh/rich/text.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4726 2024-04-08 12:25:16.000000 dtsh-0.2.2/src/dtsh/rich/theme.ini
--rw-r--r--   0 chris     (1000) chris     (1000)     6073 2024-04-08 12:25:16.000000 dtsh-0.2.2/src/dtsh/rich/theme.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6057 2024-04-08 15:08:02.000000 dtsh-0.2.2/src/dtsh/rich/tui.py
--rw-r--r--   0 chris     (1000) chris     (1000)     9263 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/rl.py
--rw-r--r--   0 chris     (1000) chris     (1000)    11110 2024-04-12 16:57:53.000000 dtsh-0.2.2/src/dtsh/session.py
--rw-r--r--   0 chris     (1000) chris     (1000)    37259 2024-04-12 17:11:58.000000 dtsh-0.2.2/src/dtsh/shell.py
--rw-r--r--   0 chris     (1000) chris     (1000)    29756 2024-04-08 12:25:16.000000 dtsh-0.2.2/src/dtsh/shellutils.py
--rw-r--r--   0 chris     (1000) chris     (1000)      128 2024-04-02 13:40:11.000000 dtsh-0.2.2/src/dtsh/typed.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.245240 dtsh-0.2.2/src/dtsh.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     3803 2024-04-12 17:55:16.000000 dtsh-0.2.2/src/dtsh.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     1764 2024-04-12 17:55:16.000000 dtsh-0.2.2/src/dtsh.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-12 17:55:16.000000 dtsh-0.2.2/src/dtsh.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-12 17:55:16.000000 dtsh-0.2.2/src/dtsh.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      194 2024-04-12 17:55:16.000000 dtsh-0.2.2/src/dtsh.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       16 2024-04-12 17:55:16.000000 dtsh-0.2.2/src/dtsh.egg-info/top_level.txt
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-12 17:55:16.245240 dtsh-0.2.2/tests/
--rw-r--r--   0 chris     (1000) chris     (1000)    14196 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_autocomp.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1276 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_alias.py
--rw-r--r--   0 chris     (1000) chris     (1000)      881 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_cat.py
--rw-r--r--   0 chris     (1000) chris     (1000)      859 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_cd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1291 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_chosen.py
--rw-r--r--   0 chris     (1000) chris     (1000)     2309 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_find.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1608 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_ls.py
--rw-r--r--   0 chris     (1000) chris     (1000)      684 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_pwd.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1646 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_builtin_tree.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5225 2024-04-08 12:25:16.000000 dtsh-0.2.2/tests/test_dtsh_config.py
--rw-r--r--   0 chris     (1000) chris     (1000)    11282 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_dts.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1186 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_io.py
--rw-r--r--   0 chris     (1000) chris     (1000)    34753 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_model.py
--rw-r--r--   0 chris     (1000) chris     (1000)    41755 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_modelutils.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5000 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_rich_shellutils.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6746 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_rich_svg.py
--rw-r--r--   0 chris     (1000) chris     (1000)    19896 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_shell.py
--rw-r--r--   0 chris     (1000) chris     (1000)    46842 2024-04-08 12:25:16.000000 dtsh-0.2.2/tests/test_dtsh_shellutils.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4691 2024-04-08 12:25:16.000000 dtsh-0.2.2/tests/test_dtsh_theme.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1665 2024-04-02 13:40:11.000000 dtsh-0.2.2/tests/test_dtsh_uthelpers.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.539608 dtsh-0.2rc1/
+-rw-r--r--   0 chris     (1000) chris     (1000)    11357 2024-02-08 19:45:41.000000 dtsh-0.2rc1/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     3129 2024-02-09 04:38:51.539608 dtsh-0.2rc1/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1621 2024-02-09 03:56:32.000000 dtsh-0.2rc1/README.rst
+-rw-r--r--   0 chris     (1000) chris     (1000)      601 2024-02-09 03:56:32.000000 dtsh-0.2rc1/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)     1851 2024-02-09 04:38:51.539608 dtsh-0.2rc1/setup.cfg
+-rw-r--r--   0 chris     (1000) chris     (1000)      246 2024-02-09 03:56:32.000000 dtsh-0.2rc1/setup.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.531608 dtsh-0.2rc1/src/
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.533608 dtsh-0.2rc1/src/devicetree/
+-rw-r--r--   0 chris     (1000) chris     (1000)      115 2024-02-08 19:45:41.000000 dtsh-0.2rc1/src/devicetree/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1227 2024-02-08 19:45:41.000000 dtsh-0.2rc1/src/devicetree/_private.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    75929 2024-02-08 19:45:41.000000 dtsh-0.2rc1/src/devicetree/dtlib.py
+-rw-r--r--   0 chris     (1000) chris     (1000)   118783 2024-02-08 19:45:41.000000 dtsh-0.2rc1/src/devicetree/edtlib.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5953 2024-02-08 19:45:41.000000 dtsh-0.2rc1/src/devicetree/grutils.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      128 2024-02-08 19:45:41.000000 dtsh-0.2rc1/src/devicetree/typed.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.534608 dtsh-0.2rc1/src/dtsh/
+-rw-r--r--   0 chris     (1000) chris     (1000)      134 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    24542 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/autocomp.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.535608 dtsh-0.2rc1/src/dtsh/builtins/
+-rw-r--r--   0 chris     (1000) chris     (1000)      143 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2247 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/alias.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1044 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/cd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2265 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/chosen.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9426 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/find.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6907 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/ls.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      775 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/pwd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3606 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/builtins/tree.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4218 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/cli.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    18648 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/config.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    25945 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/dts.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9511 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/dtsh.ini
+-rw-r--r--   0 chris     (1000) chris     (1000)     6999 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/io.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    58292 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/model.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    21224 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/modelutils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.536608 dtsh-0.2rc1/src/dtsh/rich/
+-rw-r--r--   0 chris     (1000) chris     (1000)      133 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/__init__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7373 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/autocomp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    15143 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/io.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    43371 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/modelview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4450 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/session.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    13244 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/shellutils.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    23074 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/svg.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6159 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/text.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3613 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/theme.ini
+-rw-r--r--   0 chris     (1000) chris     (1000)     4539 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/theme.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6057 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rich/tui.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     9263 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/rl.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    10434 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/session.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    37260 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/shell.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    25924 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/shellutils.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      128 2024-02-09 03:56:32.000000 dtsh-0.2rc1/src/dtsh/typed.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.538608 dtsh-0.2rc1/src/dtsh.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     3129 2024-02-09 04:38:51.000000 dtsh-0.2rc1/src/dtsh.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     1681 2024-02-09 04:38:51.000000 dtsh-0.2rc1/src/dtsh.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-02-09 04:38:51.000000 dtsh-0.2rc1/src/dtsh.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-02-09 04:38:51.000000 dtsh-0.2rc1/src/dtsh.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      189 2024-02-09 04:38:51.000000 dtsh-0.2rc1/src/dtsh.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       16 2024-02-09 04:38:51.000000 dtsh-0.2rc1/src/dtsh.egg-info/top_level.txt
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-02-09 04:38:51.538608 dtsh-0.2rc1/tests/
+-rw-r--r--   0 chris     (1000) chris     (1000)    13375 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_autocomp.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1276 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_builtin_alias.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      859 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_builtin_cd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1291 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_builtin_chosen.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2309 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_builtin_find.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1608 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_builtin_ls.py
+-rw-r--r--   0 chris     (1000) chris     (1000)      684 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_builtin_pwd.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1646 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_builtin_tree.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4635 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_config.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    11006 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_dts.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1186 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_io.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    32761 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_model.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    37647 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_modelutils.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5000 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_rich_shellutils.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6746 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_rich_svg.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    19896 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_shell.py
+-rw-r--r--   0 chris     (1000) chris     (1000)    43384 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_shellutils.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3693 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_theme.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1665 2024-02-09 03:56:32.000000 dtsh-0.2rc1/tests/test_dtsh_uthelpers.py
```

### Comparing `dtsh-0.2.2/LICENSE` & `dtsh-0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/pyproject.toml` & `dtsh-0.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/setup.cfg` & `dtsh-0.2rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [metadata]
 name = dtsh
-version = 0.2.2
+version = 0.2rc1
 author = Christophe Dufaza
 author_email = chris@openmarl.org
 description = Shell-like interface with Zephyr Devicetree
 long_description = file: README.rst
 license = Apache License version 2.0
 url = https://github.com/dottspina/dtsh
 keywords = devicetree, zephyr, dts, embedded
 classifiers = 
-	Development Status :: 5 - Production/Stable
+	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
 	Intended Audience :: Developers
 	Topic :: Software Development :: Embedded Systems
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 python_requires = >=3.8
 install_requires = 
-	PyYAML>=6.0
+	PyYAML
 	rich
 	gnureadline ; sys_platform == 'darwin'
 packages = 
 	dtsh
 	dtsh.builtins
 	dtsh.rich
 	devicetree
@@ -95,15 +95,14 @@
 	E203
 
 [mypy]
 mypy_path = src:tests
 exclude = tests/res
 python_version = 3.8
 packages = dtsh
-strict = true
 
 [pylsp-mypy]
 enabled = true
 dmypy = false
 live_mode = true
 strict = true
```

### Comparing `dtsh-0.2.2/src/devicetree/_private.py` & `dtsh-0.2rc1/src/devicetree/_private.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/devicetree/dtlib.py` & `dtsh-0.2rc1/src/devicetree/dtlib.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/devicetree/edtlib.py` & `dtsh-0.2rc1/src/devicetree/edtlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,15 @@
       this is a Binding object for those children; it is None otherwise.
       A Binding object's 'child_binding.child_binding' is not None if there
       are multiple levels of 'child-binding' descriptions in the binding.
     """
 
     def __init__(self, path: Optional[str], fname2path: Dict[str, str],
                  raw: Any = None, require_compatible: bool = True,
-                 require_description: bool = True,
-                 inc_allowlist: Optional[List[str]] = None,
-                 inc_blocklist: Optional[List[str]] = None):
+                 require_description: bool = True):
         """
         Binding constructor.
 
         path:
           Path to binding YAML file. May be None.
 
         fname2path:
@@ -189,44 +187,24 @@
           if it is present in the binding.
 
         require_description:
           If True, it is an error if the binding does not contain a
           "description:" line. If False, a missing "description:" is
           not an error. Either way, "description:" must be a string
           if it is present in the binding.
-
-        inc_allowlist:
-          The property-allowlist filter set by including bindings.
-
-        inc_blocklist:
-          The property-blocklist filter set by including bindings.
         """
         self.path: Optional[str] = path
         self._fname2path: Dict[str, str] = fname2path
 
-        self._inc_allowlist: Optional[List[str]] = inc_allowlist
-        self._inc_blocklist: Optional[List[str]] = inc_blocklist
-
         if raw is None:
             if path is None:
                 _err("you must provide either a 'path' or a 'raw' argument")
             with open(path, encoding="utf-8") as f:
                 raw = yaml.load(f, Loader=_BindingLoader)
 
-        # Get the properties this binding modifies
-        # before we merge the included ones.
-        last_modified_props = list(raw.get("properties", {}).keys())
-
-        # Map property names to their specifications:
-        # - first, _merge_includes() will recursively populate prop2specs with
-        #   the properties specified by the included bindings
-        # - eventually, we'll update prop2specs with the properties
-        #   this binding itself defines or modifies
-        self.prop2specs: Dict[str, 'PropertySpec'] = {}
-
         # Merge any included files into self.raw. This also pulls in
         # inherited child binding definitions, so it has to be done
         # before initializing those.
         self.raw: dict = self._merge_includes(raw, self.path)
 
         # Recursively initialize any child bindings. These don't
         # require a 'compatible' or 'description' to be well defined,
@@ -242,19 +220,18 @@
                 require_description=False)
         else:
             self.child_binding = None
 
         # Make sure this is a well defined object.
         self._check(require_compatible, require_description)
 
-        # Update specs with the properties this binding defines or modifies.
-        for prop_name in last_modified_props:
-            self.prop2specs[prop_name] = PropertySpec(prop_name, self)
-
         # Initialize look up tables.
+        self.prop2specs: Dict[str, 'PropertySpec'] = {}
+        for prop_name in self.raw.get("properties", {}).keys():
+            self.prop2specs[prop_name] = PropertySpec(prop_name, self)
         self.specifier2cells: Dict[str, List[str]] = {}
         for key, val in self.raw.items():
             if key.endswith("-cells"):
                 self.specifier2cells[key[:-len("-cells")]] = val
 
     def __repr__(self) -> str:
         if self.compatible:
@@ -310,65 +287,40 @@
         # file has a 'required:' for a particular property, OR the values
         # together, so that 'required: true' wins.
 
         merged: Dict[str, Any] = {}
 
         if isinstance(include, str):
             # Simple scalar string case
-            # Load YAML file and register property specs into prop2specs.
-            inc_raw = self._load_raw(include, self._inc_allowlist,
-                                     self._inc_blocklist)
-
-            _merge_props(merged, inc_raw, None, binding_path,  False)
+            _merge_props(merged, self._load_raw(include), None, binding_path,
+                         False)
         elif isinstance(include, list):
             # List of strings and maps. These types may be intermixed.
             for elem in include:
                 if isinstance(elem, str):
-                    # Load YAML file and register property specs into prop2specs.
-                    inc_raw = self._load_raw(elem, self._inc_allowlist,
-                                             self._inc_blocklist)
-
-                    _merge_props(merged, inc_raw, None, binding_path, False)
+                    _merge_props(merged, self._load_raw(elem), None,
+                                 binding_path, False)
                 elif isinstance(elem, dict):
                     name = elem.pop('name', None)
-
-                    # Merge this include property-allowlist filter
-                    # with filters from including bindings.
                     allowlist = elem.pop('property-allowlist', None)
-                    if allowlist is not None:
-                        if self._inc_allowlist:
-                            allowlist.extend(self._inc_allowlist)
-                    else:
-                        allowlist = self._inc_allowlist
-
-                    # Merge this include property-blocklist filter
-                    # with filters from including bindings.
                     blocklist = elem.pop('property-blocklist', None)
-                    if blocklist is not None:
-                        if self._inc_blocklist:
-                            blocklist.extend(self._inc_blocklist)
-                    else:
-                        blocklist = self._inc_blocklist
-
                     child_filter = elem.pop('child-binding', None)
 
                     if elem:
                         # We've popped out all the valid keys.
                         _err(f"'include:' in {binding_path} should not have "
                              f"these unexpected contents: {elem}")
 
                     _check_include_dict(name, allowlist, blocklist,
                                         child_filter, binding_path)
 
-                    # Load YAML file, and register (filtered) property specs
-                    # into prop2specs.
-                    contents = self._load_raw(name,
-                                              allowlist, blocklist,
-                                              child_filter)
+                    contents = self._load_raw(name)
 
+                    _filter_properties(contents, allowlist, blocklist,
+                                       child_filter, binding_path)
                     _merge_props(merged, contents, None, binding_path, False)
                 else:
                     _err(f"all elements in 'include:' in {binding_path} "
                          "should be either strings or maps with a 'name' key "
                          "and optional 'property-allowlist' or "
                          f"'property-blocklist' keys, but got: {elem}")
         else:
@@ -380,85 +332,32 @@
         # 'raw' has 'required: false' while the merged included files have
         # 'required: true'.
 
         _merge_props(raw, merged, None, binding_path, check_required=True)
 
         return raw
 
-
-    def _load_raw(self, fname: str,
-                  allowlist: Optional[List[str]] = None,
-                  blocklist: Optional[List[str]] = None,
-                  child_filter: Optional[dict] = None) -> dict:
+    def _load_raw(self, fname: str) -> dict:
         # Returns the contents of the binding given by 'fname' after merging
-        # any bindings it lists in 'include:' into it, according to the given
-        # property filters.
-        #
-        # Will also register the (filtered) included property specs
-        # into prop2specs.
+        # any bindings it lists in 'include:' into it. 'fname' is just the
+        # basename of the file, so we check that there aren't multiple
+        # candidates.
 
         path = self._fname2path.get(fname)
 
         if not path:
             _err(f"'{fname}' not found")
 
         with open(path, encoding="utf-8") as f:
             contents = yaml.load(f, Loader=_BindingLoader)
             if not isinstance(contents, dict):
                 _err(f'{path}: invalid contents, expected a mapping')
 
-        # Apply constraints to included YAML contents.
-        _filter_properties(contents,
-                           allowlist, blocklist,
-                           child_filter, self.path)
-
-        # Register included property specs.
-        self._add_included_prop2specs(fname, contents, allowlist, blocklist)
-
         return self._merge_includes(contents, path)
 
-    def _add_included_prop2specs(self, fname: str, contents: dict,
-                                 allowlist: Optional[List[str]] = None,
-                                 blocklist: Optional[List[str]] = None) -> None:
-        # Registers the properties specified by an included binding file
-        # into the properties this binding supports/requires (aka prop2specs).
-        #
-        # Consider "this" binding B includes I1 which itself includes I2.
-        #
-        # We assume to be called in that order:
-        # 1) _add_included_prop2spec(B, I1)
-        # 2) _add_included_prop2spec(B, I2)
-        #
-        # Where we don't want I2 "taking ownership" for properties
-        # modified by I1.
-        #
-        # So we:
-        # - first create a binding that represents the included file
-        # - then add the property specs defined by this binding to prop2specs,
-        #   without overriding the specs modified by an including binding
-        #
-        # Note: Unfortunately, we can't cache these base bindings,
-        # as a same YAML file may be included with different filters
-        # (property-allowlist and such), leading to different contents.
-
-        inc_binding = Binding(
-            self._fname2path[fname],
-            self._fname2path,
-            contents,
-            require_compatible=False,
-            require_description=False,
-            # Recursively pass filters to included bindings.
-            inc_allowlist=allowlist,
-            inc_blocklist=blocklist,
-        )
-
-        for prop, spec in inc_binding.prop2specs.items():
-            if prop not in self.prop2specs:
-                self.prop2specs[prop] = spec
-
     def _check(self, require_compatible: bool, require_description: bool):
         # Does sanity checking on the binding.
 
         raw = self.raw
 
         if "compatible" in raw:
             compatible = raw["compatible"]
```

### Comparing `dtsh-0.2.2/src/devicetree/grutils.py` & `dtsh-0.2rc1/src/devicetree/grutils.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/autocomp.py` & `dtsh-0.2rc1/src/dtsh/autocomp.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 from typing import cast, List, Set
 
 import os
 
-from dtsh.model import DTPath, DTNode, DTBinding, DTNodeProperty
+from dtsh.model import DTPath, DTNode, DTBinding
 from dtsh.rl import DTShReadline
 from dtsh.io import DTShOutput
 from dtsh.config import DTShConfig
 from dtsh.shell import (
     DTSh,
     DTShCommand,
     DTShOption,
@@ -80,38 +80,14 @@
 
     @property
     def node(self) -> DTNode:
         """The corresponding Devicetree node."""
         return cast(DTNode, self._item)
 
 
-class RlStateDTProperty(DTShReadline.CompleterState):
-    """RL completer state for DT properties.
-
-    Produced for completion scopes like: "<path>$<property-name>", where:
-    - <path> is the DTSh path (absolute, relative, with DT labels) to a node
-    - <property-name> is the node's property name
-    """
-
-    def __init__(self, rlstr: str, prop: DTNodeProperty) -> None:
-        """Initialize completer state.
-
-        Args:
-          rlstr: The DT path expression to substitute
-            the RL completion scope with.
-          prop: The corresponding DT property.
-        """
-        super().__init__(rlstr, prop)
-
-    @property
-    def dtproperty(self) -> DTNodeProperty:
-        """The corresponding DT property."""
-        return cast(DTNodeProperty, self._item)
-
-
 class RlStateCompatStr(DTShReadline.CompleterState):
     """RL completer state for compatible strings."""
 
     _bindings: Set[DTBinding]
 
     def __init__(self, rlstr: str, bindings: Set[DTBinding]) -> None:
         """Initialize completer state.
@@ -417,52 +393,14 @@
                 for child in dirnode.children
                 if child.name.startswith(prefix)
             )
 
         return sorted(states)
 
     @staticmethod
-    def complete_dtpathx(
-        cs_txt: str, sh: DTSh
-    ) -> List[DTShReadline.CompleterState]:
-        """Complete devicetree path with support for properties.
-
-        These paths have the form "<path>[$<property-name>]",
-        see also RlStateDTProperty.
-
-        Behaves like complete_dtpath() if the extended path does not
-        contain a "$" separator.
-
-        Args:
-            cs_txt: The devicetree path to complete.
-            sh: The context shell.
-
-        Returns:
-            Sorted completion states for matched nodes or properties.
-        """
-        i_prop = cs_txt.rfind("$")
-        if i_prop == -1:
-            return DTShAutocomp.complete_dtpath(cs_txt, sh)
-
-        dtpath = cs_txt[:i_prop]
-        try:
-            node = sh.node_at(dtpath)
-        except DTPathNotFoundError:
-            return []
-
-        prefix = cs_txt[i_prop + 1 :]
-        states: List[DTShReadline.CompleterState] = [
-            RlStateDTProperty(f"{dtpath}${prop.name}", prop)
-            for prop in node.all_dtproperties()
-            if prop.name.startswith(prefix)
-        ]
-
-        return sorted(states)
-
-    @staticmethod
     def complete_dtcompat(
         cs_txt: str, sh: DTSh
     ) -> List[DTShReadline.CompleterState]:
         """Complete compatible string.
 
         Args:
             cs_txt: The compatible string to complete.
@@ -810,17 +748,14 @@
 
             elif isinstance(state, RlStateDTAlias):
                 out.write(state.alias)
 
             elif isinstance(state, RlStateDTChosen):
                 out.write(state.chosen)
 
-            elif isinstance(state, RlStateDTProperty):
-                out.write(state.dtproperty.name)
-
             elif isinstance(state, RlStateFsEntry):
                 dirent = state.dirent
                 if dirent.is_dir():
                     out.write(f"{dirent.name}{os.path.sep}")
                 else:
                     out.write(dirent.name)
```

### Comparing `dtsh-0.2.2/src/dtsh/builtins/alias.py` & `dtsh-0.2rc1/src/dtsh/builtins/alias.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/builtins/cat.py` & `dtsh-0.2rc1/src/dtsh/rich/shellutils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,389 +1,440 @@
-# Copyright (c) 2024 Christophe Dufaza <chris@openmarl.org>
+# Copyright (c) 2023 Christophe Dufaza <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-"""Devicetree shell built-in "cat".
+"""Helpers for formatted command output.
 
-Print node content.
+Command options to configure formatted outputs.
 
-Unit tests and examples: tests/test_dtsh_builtin_cat.py
+Base command with boilerplate code to support formatted outputs.
+
+Unit tests and examples: tests/test_dtsh_rich_shellutils.py
 """
 
-from typing import Sequence, List, Optional
 
+from typing import Optional, Sequence, List, Mapping
+
+import sys
 
-from dtsh.dts import YAMLFile
-from dtsh.model import DTNode, DTNodeProperty
-from dtsh.modelutils import DTSUtil
-from dtsh.io import DTShOutput
-from dtsh.shell import DTSh, DTShCommand, DTShFlag, DTShCommandError
-
-from dtsh.shellutils import (
-    DTShFlagPager,
-    DTShParamDTPathX,
-)
 from dtsh.config import DTShConfig
+from dtsh.model import DTNode, DTNodeSorter
+from dtsh.rl import DTShReadline
+from dtsh.shell import (
+    DTSh,
+    DTShOption,
+    DTShParameter,
+    DTShFlag,
+    DTShArg,
+    DTShError,
+    DTShCommand,
+)
+from dtsh.shellutils import DTShFlagReverse, DTShFlagEnabledOnly, DTShArgOrderBy
+from dtsh.autocomp import RlStateEnum
 
-from dtsh.rich.shellutils import DTShFlagLongList
-from dtsh.rich.text import TextUtil
 from dtsh.rich.modelview import (
-    ViewPropertyValueTable,
-    FormPropertySpec,
-    ViewNodeBinding,
-    ViewDescription,
-    ViewYAMLFile,
-    HeadingsContentWriter,
+    SketchMV,
+    NodeColumnMV,
+    PathNameNodeMV,
+    NodeNameNodeMV,
+    UnitNameNodeMV,
+    UnitAddrNodeMV,
+    DepOrdinalNodeMV,
+    DeviceLabelNodeMV,
+    NodeLabelsNodeMV,
+    CompatibleNodeMV,
+    BindingNodeMV,
+    BindingDepthNodeMV,
+    DescriptionNodeMV,
+    VendorNodeMV,
+    StatusNodeMV,
+    AliasesNodeMV,
+    AlsoKnownAsNodeMV,
+    OnBusNodeMV,
+    BusesNodeMV,
+    BusNodeMV,
+    InterruptsNodeMV,
+    RegistersNodeMV,
+    RegisterRangesNodeMV,
+    DepOnNodeMV,
+    ReqByNodeMV,
 )
 
 
 _dtshconf: DTShConfig = DTShConfig.getinstance()
 
 
-class DTShFlagAll(DTShFlag):
-    """Concatenate and output all available information about a node a property.
+class DTShFlagLongList(DTShFlag):
+    """Whether to use a long listing format."""
 
-    Ignored:
-    - in POSIX-like output mode ("-l" is not set)
-    - when "cat" operates on multiple properties
-    """
-
-    BRIEF = "show all info about node or property"
-    SHORTNAME = "A"
+    BRIEF = "use a long listing format"
+    SHORTNAME = "l"
 
 
-class DTShFlagDescription(DTShFlag):
-    """Output node or property full description from binding."""
+class DTShNodeFmt:
+    """Node output format.
 
-    BRIEF = "description from bindings"
-    SHORTNAME = "D"
+    An output format is a list of columns specified by a format string,
+    e.g. "pd" is a format string where specifiers "p" and "d" represent
+    the "Path" and "Description" columns.
+    """
 
+    T = Sequence[NodeColumnMV]
+    """A node output format is actually a list of columns (view factories)."""
 
-class DTShFlagBindings(DTShFlag):
-    """Output bindings of a node or property."""
+    class Spec:
+        """Output format specifier.
 
-    BRIEF = "bindings or property specification"
-    SHORTNAME = "B"
+        Associate meta-data to view factories (columns).
+        """
 
+        _key: str
+        _brief: str
+        _col: NodeColumnMV
+
+        def __init__(self, spec: str, brief: str, col: NodeColumnMV) -> None:
+            """Define output format specifier.
+
+            Args:
+                spec: Format specifier (single character).
+                header: Human readable name for the field.
+                brief: Brief description.
+                factory: Formatted view factory.
+            """
+            self._key = spec
+            self._brief = brief
+            self._col = col
+
+        @property
+        def key(self) -> str:
+            """Format specifier key (single character)."""
+            return self._key
+
+        @property
+        def brief(self) -> str:
+            """Brief description."""
+            return self._brief
+
+        @property
+        def col(self) -> NodeColumnMV:
+            """View factory associated to this specifier."""
+            return self._col
+
+        def __eq__(self, other: object) -> bool:
+            if isinstance(other, DTShNodeFmt.Spec):
+                return self._key == other._key
+            return False
+
+        def __lt__(self, other: object) -> bool:
+            if isinstance(other, DTShNodeFmt.Spec):
+                return self._key < other._key
+            raise TypeError(other)
+
+        def __hash__(self) -> int:
+            return hash(self._key)
+
+    @staticmethod
+    def parse(fmt: str) -> "DTShNodeFmt.T":
+        """Parse format string into node output format.
 
-class DTShFlagYamlFile(DTShFlag):
-    """Output the YAML view of bindings (with extended includes)."""
+        Args:
+            fmt: A format string.
 
-    BRIEF = "YAML view of bindings"
-    SHORTNAME = "Y"
+        Returns:
+            The format columns (view factories).
+        """
+        try:
+            return [DTSH_NODE_FMT_SPEC[spec].col for spec in fmt]
+        except KeyError as e:
+            raise DTShError(f"invalid format specifier: '{e}'") from e
+
+    @staticmethod
+    def is_valid(fmt: str) -> bool:
+        """Validate format string.
 
+        Args:
+            fmt: A format string.
 
-class DTShBuiltinCat(DTShCommand):
-    """Devicetree shell built-in "cat".
+        Returns:
+            False if the format string is invalid.
+        """
+        return all(spec in DTSH_NODE_FMT_SPEC for spec in fmt)
 
-    Concatenate and output info about a node and its properties.
 
-    If the user does not explicitly select what to cat
-    with command flags, will output all node property values.
+class DTShArgLongFmt(DTShArg):
+    """Argument to set the output format."""
 
-    Otherwise:
-    - POSIX-like output: '-A' is ignored, will output one of '-D', '-B', or '-Y'
-    - rich output: will output options among '-DBY', or all if '-A'
+    BRIEF = "node output format"
+    LONGNAME = "format"
 
-    """
+    _fmt: Optional[DTShNodeFmt.T]
 
     def __init__(self) -> None:
-        super().__init__(
-            "cat",
-            "concat and output info about a node and its properties",
+        super().__init__(argname="fmt")
+
+    @property
+    def fmt(self) -> Optional[DTShNodeFmt.T]:
+        """The parsed node output format."""
+        return self._fmt
+
+    def reset(self) -> None:
+        """Overrides DTShOption.reset()."""
+        super().reset()
+        self._fmt = None
+
+    def parsed(self, value: Optional[str] = None) -> None:
+        """Overrides DTShArg.parsed()."""
+        super().parsed(value)
+        if self._raw:
+            self._fmt = DTShNodeFmt.parse(self._raw)
+
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Overrides DTShArg.autocomp().
+
+        Auto-complete argument with format specifiers.
+        """
+        if not DTShNodeFmt.is_valid(txt):
+            # Don't complete when current format string is invalid.
+            return []
+        # Answer all available cells but those already set.
+        return sorted(
             [
-                DTShFlagDescription(),
-                DTShFlagYamlFile(),
-                DTShFlagBindings(),
-                DTShFlagAll(),
-                DTShFlagLongList(),
-                DTShFlagPager(),
+                RlStateEnum(key, spec.brief)
+                for key, spec in DTSH_NODE_FMT_SPEC.items()
+                if key not in txt
             ],
-            DTShParamDTPathX(),
+            key=lambda x: x.rlstr.lower(),
         )
 
-    def execute(self, argv: Sequence[str], sh: DTSh, out: DTShOutput) -> None:
-        """Overrides DTShCommand.execute()."""
-        super().execute(argv, sh, out)
-
-        parm_xpath = self.with_param(DTShParamDTPathX)
-        parm_dtnode: DTNode
-        parm_dtprops: Optional[List[DTNodeProperty]]
-        # Command will fail here if the xpath parameter is invalid
-        # (node or property not found).
-        parm_dtnode, parm_dtprops = parm_xpath.xsplit(self, sh)
-
-        # Setup pager after we could fail.
-        if self.with_flag(DTShFlagPager):
-            out.pager_enter()
-
-        if parm_dtprops is not None:
-            # The command is invoked with either:
-            # - PROP resolved to a single property name
-            # - PROP globbing expression matching zero,
-            #   one or more properties
-
-            if parm_xpath.is_globexpr():
-                # Globbing: we may have zero, one or more matching properties.
-                # Concatenate and output property values.
-                self.cat_dtproperties(parm_dtprops, out)
-            else:
-                # If not globbing, we have exactly one property name.
-                # Concatenate and output info about this property.
-                self.cat_dtproperty(parm_dtprops[0], out)
-
-        else:
-            # The command is invoked for node at PATH.
-            # Concatenate and output info about node.
-            self.cat_dtnode(parm_dtnode, out)
 
-        if self.with_flag(DTShFlagPager):
-            out.pager_exit()
+class DTShCommandLongFmt(DTShCommand):
+    """Base for commands that enumerate nodes with formatted output support.
+
+    Provide options and boilerplate code for:
+    - formatted output: the options DTShFlagLongList and DTShArgLongFmt
+      are appended to command specific options, get_sketch() and get_longfmt()
+      will help getting the appropriate formatted columns
+    - sorting nodes: if the options DTShFlagReverse and DTShArgOrderBy
+      are supported, they can be accessed as properties flag_reverse()
+      and arg_sorter(), and sort() will sort nodes according to
+      the command's supported options
+    - filtering disabled nodes if DTShFlagEnabledOnly is supported
+    """
 
-    def cat_dtnode(self, dtnode: DTNode, out: DTShOutput) -> None:
-        """The command is invoked with a DT node as parameter.
+    def __init__(
+        self,
+        name: str,
+        brief: str,
+        options: Optional[Sequence[DTShOption]],
+        parameter: Optional[DTShParameter],
+    ) -> None:
+        """Initialize command.
 
         Args:
-            dtnode: The node to cat information about.
-            out: Where to cat.
+            name: The command's name.
+            brief: Brief command description.
+            options: The options supported by this command.
+              Options DTShFlagLongList and DTShArgLongFmt are appended
+              to the command specific options.
+            parameter: The parameter expected by this command, if any.
         """
-        if self._with_longfmt():
-            self._out_dtnode_rich(dtnode, out)
-        else:
-            self._out_dtnode_raw(dtnode, out)
+        super().__init__(name, brief, options, parameter)
+        # Append flag and parameters related to long listing formats.
+        self._options.append(DTShFlagLongList())
+        self._options.append(DTShArgLongFmt())
+
+    @property
+    def has_longfmt(self) -> bool:
+        """Whether formatted output is disabled by an option or preference."""
+        return (
+            _dtshconf.pref_always_longfmt
+            or self.with_flag(DTShFlagLongList)
+            or self.with_arg(DTShArgLongFmt).isset
+        )
 
-    def cat_dtproperty(self, dtprop: DTNodeProperty, out: DTShOutput) -> None:
-        """The command is invoked with a single DT property as parameter.
+    @property
+    def flag_reverse(self) -> bool:
+        """Shortcut to the "reverse output" flag if supported."""
+        try:
+            return self.with_flag(DTShFlagReverse)
+        except KeyError:
+            # Option not supported.
+            pass
+        return False
+
+    @property
+    def arg_sorter(self) -> Optional[DTNodeSorter]:
+        """Shortcut to the "order-by" argument's value if supported."""
+        try:
+            return self.with_arg(DTShArgOrderBy).sorter
+        except KeyError:
+            # Option not supported.
+            pass
+        return None
+
+    @property
+    def flag_enabled_only(self) -> bool:
+        """Shortcut to the "ennabled only" flag if supported."""
+        try:
+            return self.with_flag(DTShFlagEnabledOnly)
+        except KeyError:
+            # Option not supported.
+            pass
+        return False
+
+    def sort(self, nodes: Sequence[DTNode]) -> Sequence[DTNode]:
+        """Sort nodes if the "order-by" argument is set
+        and/or the "reverse output" flag if set.
 
         Args:
-            dtprop: The property parameter.
-            out: Where to cat.
-        """
-        if self._with_longfmt():
-            self._out_dtproperty_rich(dtprop, out)
-        else:
-            self._out_dtproperty_raw(dtprop, out)
+            nodes: The nodes to sort.
 
-    def cat_dtproperties(
-        self, dtprops: List[DTNodeProperty], out: DTShOutput
-    ) -> None:
-        """The command is invoked with a PROP globbing expression.
+        Returns:
+            The sorted nodes.
+        """
+        if self.arg_sorter:
+            return self.arg_sorter.sort(nodes, reverse=self.flag_reverse)
+        if self.flag_reverse:
+            return list(reversed(nodes))
+        return nodes
 
-        It will output property values.
+    def prune(self, nodes: Sequence[DTNode]) -> Sequence[DTNode]:
+        """Filter out disabled nodes if the "ennabled only" flag is set.
 
         Args:
-            dtprops: The possibly empty list of properties
-              matching the PROP globbing expression.
-            out: Where to cat.
+            nodes: The nodes to filter.
+
+        Returns:
+            The filtered nodes.
         """
-        # Precondition for both POSIX-like and rich outputs.
-        if self.with_flag(DTShFlagAll) or self._nfmtspecs():
-            raise DTShCommandError(
-                self,
-                "globbing properties, options '-DBYA' not allowed",
-            )
-
-        # Ignore no match.
-        if dtprops:
-            if self._with_longfmt():
-                self._out_dtproperties_rich(dtprops, out)
-            else:
-                self._out_dtproperties_raw(dtprops, out)
-
-    def _out_dtnode_rich(self, dtnode: DTNode, out: DTShOutput) -> None:
-        show_all = self.with_flag(DTShFlagAll)
-        if not (show_all or self._nfmtspecs()):
-            # If the user hasn't explicitly selected what to cat,
-            # just dump all node property values, if any.
-            dtprops = dtnode.all_dtproperties()
-            if dtprops:
-                self._out_dtproperties_rich(dtprops, out)
-            return
-
-        # Otherwise, concatenate and output selected sections.
-        sections: List[HeadingsContentWriter.Section] = []
-        if show_all or self.with_flag(DTShFlagDescription):
-            sections.append(
-                HeadingsContentWriter.Section(
-                    "description", 1, ViewDescription(dtnode.description)
-                )
-            )
-        if show_all:
-            # Show property values only when '-A' is set.
-            dtprops = dtnode.all_dtproperties()
-            sections.append(
-                HeadingsContentWriter.Section(
-                    "Properties",
-                    1,
-                    ViewPropertyValueTable(dtprops)
-                    if dtprops
-                    else TextUtil.mk_apologies(
-                        "This node does not set any property."
-                    ),
-                )
-            )
-        if show_all or self.with_flag(DTShFlagBindings):
-            sections.append(
-                HeadingsContentWriter.Section(
-                    "Binding",
-                    1,
-                    ViewNodeBinding(dtnode)
-                    if dtnode.binding
-                    else TextUtil.mk_apologies("This node has no binding."),
-                )
-            )
-        if show_all or self.with_flag(DTShFlagYamlFile):
-            sections.append(
-                HeadingsContentWriter.Section(
-                    "YAML",
-                    1,
-                    ViewYAMLFile.create(
-                        dtnode.binding_path,
-                        dtnode.dt.dts.yamlfs,
-                        is_binding=True,
-                        expand_includes=_dtshconf.pref_yaml_expand,
-                    )
-                    if dtnode.binding_path
-                    else TextUtil.mk_apologies("YAML binding unavailable."),
-                )
-            )
-        self._out_rich_sections(sections, out)
+        enabled_only = self.flag_enabled_only
+        return [node for node in nodes if node.enabled or not enabled_only]
 
-    def _out_dtnode_raw(self, node: DTNode, out: DTShOutput) -> None:
-        # Precondition for POSIX-like output only.
-        if self._nfmtspecs() > 1:
-            raise DTShCommandError(
-                self, "more than one option among '-DBY' requires '-l'"
-            )
-
-        if self.with_flag(DTShFlagDescription):
-            if node.description:
-                out.write(node.description)
-        elif self.with_flag(DTShFlagYamlFile):
-            if node.binding_path:
-                yaml = YAMLFile(node.binding_path)
-                out.write(yaml.content)
-        elif self.with_flag(DTShFlagBindings):
-            if node.binding_path:
-                out.write(node.binding_path)
-        else:
-            # By default, dump property values.
-            self._out_dtproperties_raw(node.all_dtproperties(), out)
+    def get_sketch(self, layout: "SketchMV.Layout") -> SketchMV:
+        """Initialize a rendering context for formatted output.
 
-    def _out_dtproperties_rich(
-        self, dtprops: List[DTNodeProperty], out: DTShOutput
-    ) -> None:
-        # Multiple properties: dump values in table view.
-        view = ViewPropertyValueTable(dtprops)
-        view.left_indent(1)
-        out.write(view)
+        Args:
+            layout: The rendering layout to configure.
+              LIST_VIEW is promoted to LIST_MULTI if "pref_list_multi" is set.
 
-    def _out_dtproperty_rich(
-        self, dtprop: DTNodeProperty, out: DTShOutput
-    ) -> None:
-        show_all = self.with_flag(DTShFlagAll)
-        if not (show_all or self._nfmtspecs()):
-            # If the user hasn't explicitly selected what to cat,
-            # just dump property value.
-            out.write(ViewPropertyValueTable([dtprop]))
-            return
-
-        # Otherwise, concatenate and output selected sections.
-        sections: List[HeadingsContentWriter.Section] = []
-        if show_all or self.with_flag(DTShFlagDescription):
-            sections.append(
-                HeadingsContentWriter.Section(
-                    "description", 1, ViewDescription(dtprop.description)
-                )
-            )
-        if show_all or self.with_flag(DTShFlagBindings):
-            sections.append(
-                HeadingsContentWriter.Section(
-                    "specification",
-                    1,
-                    FormPropertySpec(dtprop.dtspec),
-                )
-            )
-        if show_all or self.with_flag(DTShFlagYamlFile):
-            sections.append(
-                HeadingsContentWriter.Section(
-                    "YAML",
-                    1,
-                    ViewYAMLFile.create(
-                        dtprop.path,
-                        dtprop.node.dt.dts.yamlfs,
-                        is_binding=(dtprop.path == dtprop.node.binding_path),
-                        expand_includes=_dtshconf.pref_yaml_expand,
-                    )
-                    if dtprop.path
-                    else TextUtil.mk_apologies(
-                        "YAML specification unavailable."
-                    ),
-                )
-            )
-        self._out_rich_sections(sections, out)
+        Returns:
+            A rendering context.
+        """
+        if (layout == SketchMV.Layout.LIST_VIEW) and _dtshconf.pref_list_multi:
+            # Allow multiple-line cells.
+            layout = SketchMV.Layout.LIST_MULTI
 
-    def _out_dtproperties_raw(
-        self, dtprops: List[DTNodeProperty], out: DTShOutput
-    ) -> None:
-        for dtprop in dtprops:
-            strval = DTSUtil.mk_property_value(dtprop)
-            out.write(f"{dtprop.name}: {strval}")
+        return SketchMV(layout, self.arg_sorter, self.flag_reverse)
 
-    def _out_dtproperty_raw(
-        self, dtprop: DTNodeProperty, out: DTShOutput
-    ) -> None:
-        # Precondition for POSIX-like output only.
-        if self._nfmtspecs() > 1:
-            raise DTShCommandError(
-                self, "more than one option among '-DBY' requires '-l'"
-            )
-
-        if self.with_flag(DTShFlagDescription):
-            if dtprop.description:
-                out.write(dtprop.description)
-        elif self.with_flag(DTShFlagYamlFile):
-            if dtprop.path:
-                yaml = YAMLFile(dtprop.path)
-                out.write(yaml.content)
-        elif self.with_flag(DTShFlagBindings):
-            if dtprop.path:
-                out.write(dtprop.path)
-        else:
-            # Default to property value.
-            out.write(DTSUtil.mk_property_value(dtprop))
+    def get_longfmt(self, default_fmt: Optional[str] = None) -> DTShNodeFmt.T:
+        """Get the node output format to use.
 
-    def _with_longfmt(self) -> bool:
-        # Should we use formatted output ?
-        return (
-            # "-l"
-            self.with_flag(DTShFlagLongList)
-            # "-A" implies "-l"
-            or self.with_flag(DTShFlagAll)
-            # Enforced by preferences.
-            or _dtshconf.pref_always_longfmt
-        )
+        Args:
+            default_fmt: A default format string to use when none
+              was parsed from the command line.
+              Typically set by the rendering context.
 
-    def _nfmtspecs(self) -> int:
-        # Number of output format specifier flags, among DTShFlagDescription,
-        # DTShFlagYamlFile and DTShFlagBindings, set on the command line.
-        # Each flag represents a headings in a rich output.
-        # With POSIX-like output, only one is allowed.
-        return sum(
-            [
-                self.with_flag(DTShFlagDescription),
-                self.with_flag(DTShFlagBindings),
-                self.with_flag(DTShFlagYamlFile),
-            ]
-        )
+        Returns:
+            The formatted columns as a list of view factories.
+        """
+        cols = self.with_arg(DTShArgLongFmt).fmt
+        if (not cols) and default_fmt:
+            try:
+                cols = DTShNodeFmt.parse(default_fmt)
+            except DTShError as e:
+                print(
+                    f"Invalid preferred format: '{default_fmt}' ('{e}')",
+                    file=sys.stderr,
+                )
 
-    def _out_rich_sections(
-        self, sections: List[HeadingsContentWriter.Section], out: DTShOutput
-    ) -> None:
-        if len(sections) == 1:
-            # If only on section, just write its content.
-            out.write(sections[0].content)
-        else:
-            # Otherwise, use headings writer.
-            hds_writer = HeadingsContentWriter()
-            for section in sections:
-                hds_writer.write_section(section, out)
+        return cols or [DTShNodeFmt.parse("p")[0]]
+
+
+DTSH_NODE_FMT_SPEC: Mapping[str, DTShNodeFmt.Spec] = {
+    spec.key: spec
+    for spec in [
+        DTShNodeFmt.Spec(
+            "p", "path name", NodeColumnMV("Path", PathNameNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "N", "node name", NodeColumnMV("Name", NodeNameNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "n", "unit name", NodeColumnMV("Name", UnitNameNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "a", "unit address", NodeColumnMV("Address", UnitAddrNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "o", "dependency ordinal", NodeColumnMV("Ordinal", DepOrdinalNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "l", "device label", NodeColumnMV("Label", DeviceLabelNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "L", "DTS labels", NodeColumnMV("Labels", NodeLabelsNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "c",
+            "compatible strings",
+            NodeColumnMV("Compatible", CompatibleNodeMV),
+        ),
+        DTShNodeFmt.Spec(
+            "C",
+            "binding's compatible or headline",
+            NodeColumnMV("Binding", BindingNodeMV),
+        ),
+        DTShNodeFmt.Spec(
+            "X",
+            "child-binding depth",
+            NodeColumnMV("Binding Depth", BindingDepthNodeMV),
+        ),
+        DTShNodeFmt.Spec(
+            "d", "description", NodeColumnMV("Description", DescriptionNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "v", "vendor name", NodeColumnMV("Vendor", VendorNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "s", "status string", NodeColumnMV("Status", StatusNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "A", "node aliases", NodeColumnMV("Aliases", AliasesNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "K",
+            "all labels and aliases",
+            NodeColumnMV("Also Known As", AlsoKnownAsNodeMV),
+        ),
+        DTShNodeFmt.Spec(
+            "b", "bus of appearance", NodeColumnMV("On Bus", OnBusNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "B", "supported bus protocols", NodeColumnMV("Buses", BusesNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "Y", "bus information", NodeColumnMV("Bus", BusNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "i",
+            "generated interrupts",
+            NodeColumnMV("IRQs", InterruptsNodeMV),
+        ),
+        DTShNodeFmt.Spec(
+            "r",
+            "registers (base address and size)",
+            NodeColumnMV("Registers", RegistersNodeMV),
+        ),
+        DTShNodeFmt.Spec(
+            "R",
+            "registers (address range)",
+            NodeColumnMV("Registers", RegisterRangesNodeMV),
+        ),
+        DTShNodeFmt.Spec(
+            "D", "node dependencies", NodeColumnMV("Depends-on", DepOnNodeMV)
+        ),
+        DTShNodeFmt.Spec(
+            "T", "dependent nodes", NodeColumnMV("Required-by", ReqByNodeMV)
+        ),
+    ]
+}
+"""Map meta-data to node format specifiers and view factories."""
```

### Comparing `dtsh-0.2.2/src/dtsh/builtins/cd.py` & `dtsh-0.2rc1/src/dtsh/builtins/cd.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/builtins/chosen.py` & `dtsh-0.2rc1/src/dtsh/builtins/chosen.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/builtins/find.py` & `dtsh-0.2rc1/src/dtsh/builtins/find.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/builtins/ls.py` & `dtsh-0.2rc1/src/dtsh/builtins/ls.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/builtins/pwd.py` & `dtsh-0.2rc1/src/dtsh/builtins/pwd.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/builtins/tree.py` & `dtsh-0.2rc1/src/dtsh/builtins/tree.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/config.py` & `dtsh-0.2rc1/src/dtsh/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,41 +102,34 @@
 
         - 1st, load bundled default configuration file
         - then, load user's configuration file to customize defaults
 
         Args:
             path: Path to configuration file,
               or None for default configuration initialization.
-
-        Raises:
-            DTShConfig.Error: Failed to read or parse the unique
-              preferences file. Unlikely to happen with typical API usage.
-
         """
         self._init_app_dir()
 
         self._cfg = configparser.ConfigParser(
             # Despite its name, extended interpolation seems more intuitive
             # to us than basic interpolation.
             interpolation=configparser.ExtendedInterpolation()
         )
 
         if path:
-            # If explicitly specified, load only this one: fault if invalid.
-            self.load_ini_file(path, fail_early=True)
+            # If explicitly specified, load only this one.
+            self.load_ini_file(path)
         else:
-            # Load defaults from bundled configuration file
-            # (fault if invalid, should not happen).
+            # Load defaults from bundled configuration file.
             path = os.path.join(os.path.dirname(__file__), "dtsh.ini")
-            self.load_ini_file(path, fail_early=True)
-
-            # Load user's configuration file if any: don't fault.
+            self.load_ini_file(path)
+            # Load user's configuration file if any.
             path = self.get_user_file("dtsh.ini")
             if os.path.isfile(path):
-                self.load_ini_file(path, fail_early=False)
+                self.load_ini_file(path)
 
     @property
     def app_dir(self) -> str:
         r"""Path to the per-user DTSh configuration and data directory.
 
         Location is platform-dependent:
 
@@ -224,20 +217,14 @@
 
     @property
     def pref_fs_no_overwrite(self) -> bool:
         """Whether to forbid redirection to overwrite existing files."""
         return self.getbool("pref.fs.no_overwrite")
 
     @property
-    def pref_fs_no_overwrite_strict(self) -> bool:
-        """Whether to forbid redirection to overwrite existing files,
-        even when appending."""
-        return self.getbool("pref.fs.no_overwrite_strict")
-
-    @property
     def pref_sizes_si(self) -> bool:
         """Whether to print sizes with SI units (bytes, kB, MB)."""
         return self.getbool("pref.sizes_si")
 
     @property
     def pref_hex_upper(self) -> bool:
         """Whether to print hexadicimal digits upper case."""
@@ -245,19 +232,14 @@
 
     @property
     def pref_list_headers(self) -> bool:
         """Whether to show the headers in list views."""
         return self.getbool("pref.list.headers")
 
     @property
-    def pref_list_no_wrap(self) -> bool:
-        """Whether to prevent from cells wrapping in list views."""
-        return self.getbool("pref.list.no_wrap")
-
-    @property
     def pref_list_placeholder(self) -> str:
         """Placeholder for missing values in list views."""
         return self.getstr("pref.list.place_holder")
 
     @property
     def pref_list_fmt(self) -> str:
         """Default format string for node fields in list views."""
@@ -341,49 +323,14 @@
         return self.getstr("pref.html.theme")
 
     @property
     def pref_html_font_family(self) -> str:
         """Font family for command output redirection to HTML."""
         return self.getstr("pref.html.font_family")
 
-    @property
-    def pref_yaml_theme(self) -> str:
-        """Theme for YAML syntax highlighting."""
-        return self.getstr("pref.yaml.theme")
-
-    @property
-    def pref_yaml_expand(self) -> bool:
-        """whether to expand included files in YAML views."""
-        return self.getbool("pref.yaml.expand")
-
-    @property
-    def pref_yaml_actionable_type(self) -> ActionableType:
-        """Actionable type for YAML views."""
-        return self.get_actionable_type("pref.yaml.actionable_type")
-
-    @property
-    def pref_dts_theme(self) -> str:
-        """Theme for DTS syntax highlighting."""
-        return self.getstr("pref.dts.theme")
-
-    @property
-    def pref_dts_actionable_type(self) -> ActionableType:
-        """Actionable type for DTS views."""
-        return self.get_actionable_type("pref.dts.actionable_type")
-
-    @property
-    def pref_form_show_all(self) -> bool:
-        """Whether to show missing fields in form views."""
-        return self.getbool("pref.form.show_all")
-
-    @property
-    def pref_form_actionable_type(self) -> ActionableType:
-        """Actionable type for forms."""
-        return self.get_actionable_type("pref.form.actionable_type")
-
     def init_user_files(self) -> int:
         """Initialize per-user configuration files."""
         if os.path.isdir(self._app_dir):
             src_dir = os.path.dirname(os.path.abspath(__file__))
 
             try:
                 dst = self.get_user_file("dtsh.ini")
@@ -400,20 +347,20 @@
                     shutil.copyfile(
                         os.path.join(src_dir, "rich", "theme.ini"), dst
                     )
                     print(f"User theme: {dst}")
 
                 return 0
 
-            except OSError as e:
+            except (OSError, OSError) as e:
                 print(f"Failed to create file: {dst}", file=sys.stderr)
-                print(f"Cause: {e.strerror}", file=sys.stderr)
-                return -e.errno
+                print(f"Cause: {e}", file=sys.stderr)
 
-        return 0
+        # Per-user configuration files don't exist (-ENOENT).
+        return -2
 
     def get_user_file(self, *paths: str) -> str:
         """Get path to a use file within the DTSh application directory.
 
         Args:
             paths: Relative path to the resource.
         """
@@ -548,41 +495,33 @@
             print(
                 f"{pref}: invalid actionable type '{actionable_type}'",
                 file=sys.stderr,
             )
         # Fall-back, we don't want to fault.
         return ActionableType.LINK
 
-    def load_ini_file(self, path: str, fail_early: bool = True) -> None:
+    def load_ini_file(self, path: str) -> None:
         """Load options from configuration file (INI format).
 
         Overrides already loaded values with the same keys.
 
         Args:
             path: Path to a configuration file.
-            fail_early: If set, fault when we can't open the file for reading,
-              or its content is invalid. This is the default.
 
         Raises:
             DTShConfig.Error: Failed to load configuration file.
         """
         try:
             f = open(  # pylint: disable=consider-using-with
                 path, "r", encoding="utf-8"
             )
             self._cfg.read_file(f)
 
         except (OSError, configparser.Error) as e:
-            if isinstance(e, OSError):
-                msg = e.strerror
-            else:
-                msg = e.message
-            if fail_early:
-                raise DTShConfig.Error(msg) from e
-            print(f"Failed to load preferences file: {msg}", file=sys.stderr)
+            raise DTShConfig.Error(str(e)) from e
 
     def _init_app_dir(self) -> None:
         if sys.platform == "darwin":
             self._app_dir = self._init_app_dir_darwin()
         elif os.name == "nt":
             self._app_dir = self._init_app_dir_nt()
         else:
```

### Comparing `dtsh-0.2.2/src/dtsh/dts.py` & `dtsh-0.2rc1/src/dtsh/dts.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,16 +110,16 @@
               YAML binding files the DTS depends on.
               If not set, the default bindings search path is assumed.
             vendors_file: Path to a file in vendor-prefixes.txt format.
         """
         self._dts_path = os.path.abspath(dts_path)
         self._cmake = self._init_cmake_cache()
         self._zephyr_base = self._init_zephyr_base()
-        self._binding_dirs = self._init_binding_dirs(binding_dirs)
         self._vendors_file = self._init_vendors_file(vendors_file)
+        self._binding_dirs = self._init_binding_dirs(binding_dirs)
         self._yamlfs = YAMLFilesystem(self._binding_dirs)
 
     @property
     def path(self) -> str:
         """Path to the DTS file."""
         return self._dts_path
 
@@ -228,24 +228,14 @@
         Shortcut to "${BOARD_DIR}/${BOARD}.dts".
         """
         if self.board_dir and self.board:
             return os.path.join(self.board_dir, f"{self.board}.dts")
         return None
 
     @property
-    def board_yaml(self) -> Optional[str]:
-        """Board YAML file with metadata.
-
-        Shortcut to "${BOARD_DIR}/${BOARD}.yaml".
-        """
-        if self.board_dir and self.board:
-            return os.path.join(self.board_dir, f"{self.board}.yaml")
-        return None
-
-    @property
     def shield_dirs(self) -> Sequence[str]:
         """Shield directories.
 
         Retrieved from the CMake cache (SHIELD_DIRS, CACHED_SHIELD_DIRS).
         """
         shield_dirs = []
         if self._cmake:
@@ -346,43 +336,29 @@
 
     def _init_zephyr_base(self) -> Optional[str]:
         if self._cmake:
             zephyr_base = self._cmake.getstr("ZEPHYR_BASE")
         else:
             zephyr_base = os.environ.get("ZEPHYR_BASE")
         if not zephyr_base:
-            # DTSh may be distributed with the Zephyr project:
-            # test ZEPHYR_BASE/scripts/dts/dtsh/src/dtsh/__file__
-            dtshdir = os.path.dirname(
+            # dtsh/src/dtsh/__file__
+            dtsh_base = os.path.dirname(
                 os.path.dirname(os.path.dirname(__file__))
             )
-            testdir = os.path.dirname(os.path.dirname(os.path.dirname(dtshdir)))
-            # ZEPHYR_BASE/Kconfig.zephyr should then exist.
-            if os.path.isfile(os.path.join(testdir, "Kconfig.zephyr")):
-                zephyr_base = testdir
-
+            # ZEPHYR_BASE/scripts/dts/dtsh
+            zephyr_base = os.path.dirname(
+                os.path.dirname(os.path.dirname(dtsh_base))
+            )
         return zephyr_base
 
     def _init_vendors_file(self, vendors_file: Optional[str]) -> Optional[str]:
-        if not vendors_file:
-            if self._zephyr_base:
-                # If we have a valid ZEPHYR_BASE, we assume the expected vendors
-                # are those defined by Zephyr.
-                vendors_file = os.path.join(
-                    self._zephyr_base, "dts", "bindings", "vendor-prefixes.txt"
-                )
-            else:
-                # Otherwise, it's very likely the user has explicitly set
-                # some binding directories, search them for a vendors file.
-                # NOTE: Linux uses a vendor-prefixes.yaml file, we should be
-                # able to also load that (requires changes in edtlib.EDT).
-                for binding_dir in self._binding_dirs:
-                    vndpath = os.path.join(binding_dir, "vendor-prefixes.txt")
-                    if os.path.isfile(vndpath):
-                        vendors_file = vndpath
+        if (not vendors_file) and self._zephyr_base:
+            vendors_file = os.path.join(
+                self._zephyr_base, "dts", "bindings", "vendor-prefixes.txt"
+            )
         return vendors_file
 
     def _init_binding_dirs(
         self, binding_dirs: Optional[Sequence[str]]
     ) -> List[str]:
         if binding_dirs:
             binding_dirs = [os.path.abspath(path) for path in binding_dirs]
@@ -728,142 +704,106 @@
     def __repr__(self) -> str:
         return f"{self._name}: {self._value}"
 
 
 class YAMLFile:
     """Cheap wrapper around a YAML file.
 
-    Rationale: simple API to access a YAML file's text content
-    and its "include: " element, if any.
-
-    We'll use this API for known valid binding files.
-    At this point, the DT model initialization has already red all involved
-    YAML bindings, ant it's very unlikely that reading or parsing the file
-    again will fail:
-
-    - this API won't fault: if an I/O or YAML error occurs, the content()
-      and raw() properties will just answer empty values
-    - the lasterr() property represents the last error, if any
-
-    This API is lazy-initialized:
-
-    - the file is opened and red when content() is first accessed
-    - the file is parsed into YAML when raw() or includes() is first accessed
+    This API is:
 
+    - lazy-initialized: properties are initialized when accessed
+    - fail-safe: errors are logged once to stderr, and empty values are returned
     """
 
     # Absolute file path.
     _path: str
 
     # Lazy-initialized file content.
     _content: Optional[str]
 
     # Lazy-initialized YAML model.
     _raw: Optional[Dict[str, object]]
 
     # Lazy-initialized YAML "include: ".
     _includes: Optional[List[str]]
 
-    # If set, we've failed to load the YAML file at some point:
-    # - OSError: all kinds of file system errors
-    # - YAMLError: invalid YAML content
-    _lasterr: Optional[Union[OSError, yaml.YAMLError]]
-
     def __init__(self, path: str) -> None:
         """Lazy-initialize wrapper.
 
+        Only the YAML file path is set upon initialization.
+
+        Then accessing:
+
+        - the *includes* will require initializing the YAML model
+        - the YAML model will require loading the YAML file content
+
         Args:
-            path: Absolute path to the YAML file.
-              Invalid path or file will produce an empty content.
+            path: Absolute path to a YAML file.
         """
         self._path = path
-        self._lasterr = None
         # Lazy-initialized.
         self._content = None
         self._raw = None
         self._includes = None
 
     @property
     def path(self) -> str:
         """Absolute file path."""
         return self._path
 
     @property
     def content(self) -> str:
-        """Text content."""
-        # Will Initialize an empty content if we can't read the YAML file.
+        """YAML file content."""
+        # Will Initialize an empty content if fails to load the YAML file.
         self._init_content()
         return self._content  # type: ignore
 
     @property
     def raw(self) -> Dict[str, object]:
-        """YAML model.
-
-        If empty, see lasterr().
-        """
-        # Will Initialize an empty model if the YAML file's content
-        # is unavailable or invalid.
+        """YAML model."""
+        # Will Initialize an empty model if the YAML file content unavailable.
         self._init_model()
         return self._raw  # type: ignore
 
     @property
     def includes(self) -> Sequence[str]:
         """Names of included YAML files."""
+        # Will Initialize an empty list if the YAML model is unavailable.
         self._init_includes()
         return self._includes  # type: ignore
 
-    @property
-    def lasterr(self) -> Optional[Union[OSError, yaml.YAMLError]]:
-        """Last error that happened while loading this YAML file.
-
-        Possible values:
-
-        - None: no error
-        - OSError: IO errors
-        - YAMLError: invalid YAML content
-        """
-        return self._lasterr
-
     def _init_content(self) -> None:
-        # Actually try top open the YAML file and read its content.
-        # Set lasterr accordingly.
-
         if self._content is not None:
             return
         # Only one attempt to initialize content.
         self._content = ""
 
         try:
             with open(self._path, mode="r", encoding="utf-8") as f:
                 self._content = f.read().strip()
         except OSError as e:
-            self._lasterr = e
+            print(f"YAML: {e}", file=sys.stderr)
 
     def _init_model(self) -> None:
-        # Actually try to parse the file's content into YAML.
-        # Set lasterr accordingly.
-
         if self._raw is not None:
             return
-        # Only one attempt to initialize YAML model.
+        # Only one attempt to initialize model.
         self._raw = {}
 
-        # Depends on file's content.
+        # Depends on YAML content.
         self._init_content()
         if not self._content:
             return
 
         try:
             self._raw = yaml.load(self._content, Loader=YAMLBindingLoader)
         except yaml.YAMLError as e:
-            self._lasterr = e
+            print(f"YAML: {self._path}: {e}", file=sys.stderr)
 
     def _init_includes(self) -> None:
-        # Search YAML model for include directives.
-
         if self._includes is not None:
             return
         # Only one attempt to initialize includes.
         self._includes = []
 
         # Depends on YAML model.
         self._init_model()
@@ -878,63 +818,7 @@
             for inc in yaml_inc:
                 if isinstance(inc, str):
                     self._includes.append(inc)
                 elif isinstance(inc, dict):
                     basename = inc.get("name")
                     if basename:
                         self._includes.append(basename)
-
-
-class DTSFile:
-    """Simple fail-safe wrapper around a DTS file."""
-
-    # Absolute file path.
-    _path: str
-
-    # DTS.
-    _content: Optional[str]
-
-    # If set, we've failed to load the DTS file (IO error).
-    _lasterr: Optional[OSError]
-
-    def __init__(self, path: str) -> None:
-        """Initialize wrapper.
-
-        Open DTS file and read content, no lazy-initialization.
-
-        Args:
-            path: Absolute path to the DTS file.
-              Invalid path or file will produce an empty content.
-        """
-        self._path = path
-        self._lasterr = None
-        self._content = self._init_content()
-
-    @property
-    def path(self) -> str:
-        """Absolute file path."""
-        return self._path
-
-    @property
-    def content(self) -> str:
-        """Text content, or None if we failed to read the DTS file."""
-        return self._content  # type: ignore
-
-    @property
-    def lasterr(self) -> Optional[OSError]:
-        """Last error that happened while loading this DTS file.
-
-        Possible values:
-
-        - None: no error
-        - OSError: IO error
-        """
-        return self._lasterr
-
-    def _init_content(self) -> Optional[str]:
-        try:
-            with open(self._path, mode="r", encoding="utf-8") as f:
-                return f.read().strip()
-        except OSError as e:
-            self._lasterr = e
-        # Empty content on error.
-        return ""
```

### Comparing `dtsh-0.2.2/src/dtsh/dtsh.ini` & `dtsh-0.2rc1/src/dtsh/dtsh.ini`

 * *Files 14% similar despite different names*

```diff
@@ -191,35 +191,21 @@
 # Whether to forbid command output redirection
 # to overwrite existing files.
 #
 # Type: Bool
 # Default: True
 pref.fs.no_overwrite = yes
 
-# Whether to forbid command output redirection
-# to overwrite existing files,
-# even when appending.
-#
-# Type: Bool
-# Default: False
-pref.fs.no_overwrite_strict = no
-
 
 # List views: whether to show the headers.
 #
 # Type: Bool
 # Default: True
 pref.list.headers = yes
 
-# List views: whether to prevent from wrapping cell contents.
-#
-# Type: Bool
-# Default: True
-pref.list.no_wrap = yes
-
 # List views: placeholder for missing values.
 #
 # Type: String
 # Default: Unset (no place holder)
 pref.list.place_holder =
 
 # List views: default format string for node fields.
@@ -375,73 +361,7 @@
 
 # Command output redirection to SVG: font aspect ratio.
 # This is the width to height ratio, typically 3:5.
 #
 # Type: Float
 # Default: 0.6
 pref.svg.font_ratio = 0.6
-
-
-# Pygments theme for YAML syntax highlighting.
-#
-# E.g.:
-#
-# - dark: "monokai", "dracula", "material"
-# - light: "bw", "sas", "arduino"
-#
-# See also:
-# - https://pygments.org/styles/
-# - https://rich.readthedocs.io/en/latest/syntax.html
-#
-# Type: String
-# Default: monokai
-pref.yaml.theme = monokai
-
-# Whether to expand included files
-# in YAML views.
-pref.yaml.expand = yes
-
-# YAML views: rendering for actionable texts (aka links).
-#
-# Type: String
-#   - "none": do not create hyperlinks
-#   - "link" (default): link text like browsers do
-#   - "alt": append alternative actionable view
-pref.yaml.actionable_type = alt
-
-
-# Pygments theme for DTS syntax highlighting.
-#
-# E.g.:
-#
-# - dark: "monokai", "dracula", "material"
-# - light: "bw", "sas", "arduino"
-#
-# See also:
-# - https://pygments.org/styles/
-#
-# Type: String
-# Default: monokai
-pref.dts.theme = monokai
-
-# DTS views: rendering for actionable texts (aka links).
-#
-# Type: String
-#   - "none": do not create hyperlinks
-#   - "link" (default): link text like browsers do
-#   - "alt": append alternative actionable view
-pref.dts.actionable_type = alt
-
-
-# Whether to show missing fields in form views.
-#
-# Type: bool
-# Default: yes
-pref.form.show_all = yes
-
-# Rendering for actionable texts (aka links) in forms.
-#
-# Type: String
-#   - "none": do not create hyperlinks
-#   - "link" (default): link text like browsers do
-#   - "alt": append alternative actionable view
-pref.form.actionable_type = link
```

### Comparing `dtsh-0.2.2/src/dtsh/model.py` & `dtsh-0.2rc1/src/dtsh/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,25 +25,23 @@
   such as preferring oranges
 
 Unit tests and examples: tests/test_dtsh_model.py
 """
 
 
 from typing import (
-    cast,
     Any,
     Optional,
     Iterator,
     List,
     Set,
     Mapping,
     Dict,
     Tuple,
     Sequence,
-    Union,
 )
 
 import os
 import posixpath
 import sys
 
 from devicetree import edtlib
@@ -489,25 +487,14 @@
         return self._cb_depth
 
     @property
     def child_binding(self) -> Optional["DTBinding"]:
         """The nested child-binding this binding defines, if any."""
         return self._child_binding
 
-    def all_dtproperties(self) -> List["DTPropertySpec"]:
-        """Enumerate specifications for all properties defined by this binding.
-
-        Returns:
-            A list client code can sort, filter, etc.
-        """
-        return [
-            DTPropertySpec(edtspec)
-            for edtspec in self._edtbinding.prop2specs.values()
-        ]
-
     def get_headline(self) -> Optional[str]:
         """The headline of this binding description, if any."""
         desc = self._edtbinding.description
         if desc:
             return desc.lstrip().split("\n", 1)[0]
         return None
 
@@ -580,17 +567,15 @@
         """
         self._edtirq = edtirq
         self._node = node
 
     @property
     def number(self) -> int:
         """The IRQ number."""
-        if "irq" in self._edtirq.data:
-            return cast(int, self._edtirq.data["irq"])
-        return sys.maxsize
+        return self._edtirq.data.get("irq", sys.maxsize)
 
     @property
     def priority(self) -> Optional[int]:
         """The IRQ priority.
 
         Although interrupts have a priority on most platforms,
         it's not actually true for all boards, e.g. the EPS32 SoC.
@@ -723,292 +708,14 @@
             return self.address < other.address
         raise TypeError(other)
 
     def __repr__(self) -> str:
         return f"addr:{hex(self.address)}, size:{hex(self.size)}"
 
 
-class DTNodePHandleData:
-    """An entry in a property value of type "phandle-array".
-
-    phandle-array properties:
-    These properties are commonly used to specify a resource that is owned
-    by another node along with additional metadata about the resource.
-
-    E.g. < &ctrl-1 0x10 0x1 > in:
-
-        cs-gpios = < &ctrl-1 0x10 0x1 &ctrl-1 0x11 0x0 >;
-
-    Where:
-    - &ctrl-1 is a phandle DTS-generated by referencing a label
-    - < 0x10 0x1 > is the associated data, e.g. PIN=0x10 and flags=0x1
-
-    The phandle itself points to the controller node.
-
-    Note: although relying on the same edtlib.ControllerAndData peer model type,
-    we treat interrupts differently (see DTNodeInterrupt).
-    """
-
-    _node: "DTNode"
-    _edthandle: edtlib.ControllerAndData
-
-    def __init__(
-        self, edtcad: edtlib.ControllerAndData, node: "DTNode"
-    ) -> None:
-        """Initialize phandle and data.
-
-        Args:
-            edtcad: Peer edtlib object.
-            node: The node this is a property value of.
-        """
-        self._edtcad = edtcad
-        self._node = node
-
-    @property
-    def name(self) -> Optional[str]:
-        """The phandle name.
-
-        Args:
-            name: The name of the entry as given in "gpio-names" or "pwm-names",
-              or None if there is no "*-names" property.
-        """
-        return self._edtcad.name
-
-    @property
-    def phandle(self) -> "DTNode":
-        """The controller node for the phandle."""
-        return self._node.dt[self._edtcad.controller.path]
-
-    @property
-    def data(self) -> Mapping[str, Any]:
-        """Raw representation of associated data.
-
-        Expected keys and values interpretation depend on
-        the actual controller kind (e.g. GPIO or PWM).
-        """
-        return self._edtcad.data
-
-    def __repr__(self) -> str:
-        return f"{self.phandle}: {self._edtcad.data}"
-
-
-class DTPropertySpec:
-    """DT property specification."""
-
-    _edtspec: edtlib.PropertySpec
-
-    def __init__(self, edtspec: edtlib.PropertySpec) -> None:
-        """Initialize specification.
-
-        Args:
-            edtcad: Peer edtlib object.
-        """
-        self._edtspec = edtspec
-
-    @property
-    def name(self) -> str:
-        """See edtlib.PropertySpec.name"""
-        return self._edtspec.name
-
-    @property
-    def path(self) -> Optional[str]:
-        """See edtlib.PropertySpec.path"""
-        return self._edtspec.path
-
-    @property
-    def dttype(self) -> str:
-        """See edtlib.PropertySpec.path"""
-        return self._edtspec.type
-
-    @property
-    def description(self) -> Optional[str]:
-        """See edtlib.PropertySpec.description"""
-        return self._edtspec.description
-
-    @property
-    def enum(self) -> Optional[List[Any]]:
-        """See edtlib.PropertySpec.enum"""
-        return self._edtspec.enum
-
-    @property
-    def const(self) -> Union[None, int, List[int], str, List[str]]:
-        """See edtlib.PropertySpec.const"""
-        return self._edtspec.const
-
-    @property
-    def default(self) -> Union[None, int, List[int], str, List[str]]:
-        """See edtlib.PropertySpec.default"""
-        return self._edtspec.default
-
-    @property
-    def required(self) -> bool:
-        """See edtlib.PropertySpec.required"""
-        return self._edtspec.required
-
-    @property
-    def deprecated(self) -> bool:
-        """See edtlib.PropertySpec.deprecated"""
-        return self._edtspec.deprecated
-
-    @property
-    def specifier_space(self) -> Optional[str]:
-        """See edtlib.PropertySpec.specifier_space"""
-        return self._edtspec.specifier_space
-
-
-class DTNodeProperty:
-    """Node property value and bindings."""
-
-    ValueType = Union[
-        bool,
-        int,
-        str,
-        bytes,
-        List[int],
-        List[str],
-        "DTNode",
-        List["DTNode"],
-        List[DTNodePHandleData],
-        None,
-    ]
-    """Property value types.
-
-    Peer of edtlib.PropertyValType, plus booleans (not list of).
-    """
-
-    _node: "DTNode"
-    _edtprop: edtlib.Property
-
-    def __init__(self, edtprop: edtlib.Property, node: "DTNode") -> None:
-        """Initialize node property.
-
-        Args:
-            node: The node this is a property of.
-            edtprop: The edtlib peer object.
-        """
-        self._node = node
-        self._edtprop = edtprop
-
-    @property
-    def node(self) -> "DTNode":
-        "The node this is a property of."
-        return self._node
-
-    @property
-    def name(self) -> str:
-        """Property name."""
-        return self._edtprop.name
-
-    @property
-    def description(self) -> Optional[str]:
-        """Property description from binding file, if any."""
-        return self._edtprop.description
-
-    @property
-    def path(self) -> Optional[str]:
-        """Path to the binding file that specifies this property, if any."""
-        return self._edtprop.spec.path
-
-    @property
-    def dttype(self) -> str:
-        """Property type from bindings.
-
-        Determines how the property value is serialized to DTS by Zephyr.
-
-        Known "type:" values:
-        - "boolean", "int", "array", "uint8-array", "string", "string-array"
-        - "phandle"," path"
-        - "phandles"
-        - "phandle-array"
-        """
-        return self._edtprop.type
-
-    @property
-    def dtspec(self) -> DTPropertySpec:
-        """Property specification."""
-        return DTPropertySpec(self._edtprop.spec)
-
-    @property
-    def value(self) -> "DTNodeProperty.ValueType":
-        """Property value, the type of which is determined by the bindings.
-
-        - For DT type "boolean": Python bool
-        - For DT type "int", "array", "string", and "string-array": Python int,
-          string, or a list of them
-        - For DT type "uint8-array": Python bytes
-        - For DT types "phandle": the pointed-to DTNode instance
-        - For DT type "phandles": a list of the pointed-to DTNode instances
-        - For DT type "phandle-array": a list of DTNodePHandleData
-        """
-        if self._edtprop.val is None:
-            return None
-
-        if isinstance(self._edtprop.val, list):
-            # Non empty list of int, string, Node, or ControllerAndData
-            if self._edtprop.val:
-                val0: Union[
-                    int, str, edtlib.Node, edtlib.ControllerAndData, None
-                ] = self._edtprop.val[0]
-
-                # List[int]
-                if isinstance(val0, int):
-                    return [cast(int, i) for i in self._edtprop.val]
-                # List[str]
-                if isinstance(val0, str):
-                    return [cast(str, s) for s in self._edtprop.val]
-                # List[DTNode]
-                if isinstance(val0, edtlib.Node):
-                    edtnodes = (cast(edtlib.Node, n) for n in self._edtprop.val)
-                    return [self._node.dt[edtnode.path] for edtnode in edtnodes]
-                # List[DTNodePHandleData]
-                if isinstance(val0, edtlib.ControllerAndData):
-                    edtcads = (
-                        cast(edtlib.ControllerAndData, edtcad)
-                        for edtcad in self._edtprop.val
-                    )
-                    return [
-                        DTNodePHandleData(edtcad, self._node)
-                        for edtcad in edtcads
-                    ]
-            else:
-                # Empty list of "something".
-                return []
-
-        # One bool, int, string, bytes, or DTNode
-        if isinstance(self._edtprop.val, bool):
-            return self._edtprop.val
-        if isinstance(self._edtprop.val, int):
-            return self._edtprop.val
-        if isinstance(self._edtprop.val, str):
-            return self._edtprop.val
-        if isinstance(self._edtprop.val, bytes):
-            return self._edtprop.val
-        if isinstance(self._edtprop.val, edtlib.Node):
-            return self._node.dt[self._edtprop.val.path]
-
-        # Unsupported property type.
-        raise ValueError(self._edtprop.val)
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, DTNodeProperty):
-            return (self._node == other._node) and (self.name == other.name)
-        return False
-
-    def __repr__(self) -> str:
-        vlist: List[Any]
-        if isinstance(self.value, list):
-            vlist = self.value
-        else:
-            vlist = [self.value]
-        vstr = " ".join(
-            [hex(val) if isinstance(val, int) else str(val) for val in vlist]
-        )
-        return f"{self.name}: {vstr}"
-
-
 class DTWalkable:
     """Virtual devicetree we can walk through.
 
     The simplest walk-able is a Devicetree branch,
     implemented by DTNode objects.
 
     DTWalkableComb permits to define a virtual devicetree as a root node
@@ -1065,17 +772,14 @@
 
     # Child nodes (DTS-order).
     _children: List["DTNode"]
 
     # The binding that specifies the node content, if any.
     _binding: Optional[DTBinding]
 
-    # (All) properties, lazy initialized.
-    _props: Dict[str, DTNodeProperty]
-
     def __init__(
         self,
         edtnode: edtlib.Node,
         model: "DTModel",
         parent: Optional["DTNode"],
     ) -> None:
         """Insert a node in a devicetree model.
@@ -1094,16 +798,14 @@
         self._dt = model
         # The devicetree root is its own parent.
         self._parent = parent or self
         # Nodes are first inserted childless.
         self._children = []
         # Device bindings are initialized on start-up.
         self._binding = self._dt.get_device_binding(self)
-        # Initialized on first access.
-        self._props = {}
 
     @property
     def dt(self) -> "DTModel":
         """The devicetree model this node belongs to."""
         return self._dt
 
     @property
@@ -1305,49 +1007,14 @@
     @property
     def depends_on(self) -> List["DTNode"]:
         """The nodes this device directly depends on."""
         return [
             self._dt[edt_node.path] for edt_node in self._edtnode.depends_on
         ]
 
-    def has_dtproperty(self, name: str) -> bool:
-        """Whether a DT property is defined.
-
-        Args:
-            name: The property name to look for.
-
-        Returns:
-            True if this node has a property with the requested name.
-        """
-        self._init_props()
-        return name in self._props
-
-    def dtproperty(self, name: str) -> DTNodeProperty:
-        """Access node properties by name.
-
-        The property MUST exist.
-
-        Args:
-            name: A property name.
-
-        Returns:
-            True if this node has a property with the requested name.
-        """
-        self._init_props()
-        return self._props[name]
-
-    def all_dtproperties(self) -> List[DTNodeProperty]:
-        """Enumerate all node properties.
-
-        Returns:
-            A list client code can sort, filter, etc.
-        """
-        self._init_props()
-        return list(self._props.values())
-
     def get_child(self, name: str) -> "DTNode":
         """Retrieve a child node by name.
 
         The requested child MUST exist.
 
         Args:
             name: The child node name to search for.
@@ -1481,21 +1148,14 @@
     def _rwalk(self, node: "DTNode") -> Iterator["DTNode"]:
         # Walk the subtree backward to the root node,
         # which is by convention its own parent.
         yield node
         if node.parent != node:
             yield from self._rwalk(node.parent)
 
-    def _init_props(self) -> None:
-        if not self._props:
-            self._props = {
-                edtprop.name: DTNodeProperty(edtprop, self)
-                for edtprop in self._edtnode.props.values()
-            }
-
     def __eq__(self, other: object) -> bool:
         if isinstance(other, DTNode):
             return other.path == self.path
         return False
 
     def __lt__(self, other: object) -> bool:
         if isinstance(other, DTNode):
```

### Comparing `dtsh-0.2.2/src/dtsh/modelutils.py` & `dtsh-0.2rc1/src/dtsh/shellutils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,995 +1,924 @@
 # Copyright (c) 2023 Christophe Dufaza <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-"""Devicetree model helpers.
+"""Devicetree shell helpers.
 
-- Match node with text based criteria (implement DTNodeTextCriterion)
-- Match node with integer based criteria (implement DTNodeIntCriterion)
-- Sort nodes (implement DTNodeSorter)
-- Arbitrary virtual devicetree (DTWalkableComb)
+Flags, arguments and parameters for DTSh commands.
 
-Unit tests and examples: tests/test_dtsh_modelutils.py
+Unit tests and examples: tests/test_dtsh_shellutils.py
 """
 
 
-from typing import (
-    cast,
-    Any,
-    Union,
-    Callable,
-    Tuple,
-    Set,
-    List,
-    Optional,
-    Sequence,
-    Iterator,
-    Mapping,
-)
+from typing import Any, Type, Optional, Sequence, Mapping, List
 
-import operator
 import re
-import sys
 
-from dtsh.model import (
-    DTWalkable,
-    DTNode,
-    DTNodeProperty,
-    DTNodePHandleData,
-    DTNodeSorter,
-    DTNodeCriterion,
+from dtsh.model import DTNodeSorter, DTNodeCriterion
+from dtsh.modelutils import (
+    DTNodeSortByPathName,
+    DTNodeSortByNodeName,
+    DTNodeSortByUnitName,
+    DTNodeSortByUnitAddr,
+    DTNodeSortByDeviceLabel,
+    DTNodeSortByNodeLabel,
+    DTNodeSortByAlias,
+    DTNodeSortByCompatible,
+    DTNodeSortByBinding,
+    DTNodeSortByVendor,
+    DTNodeSortByBus,
+    DTNodeSortByOnBus,
+    DTNodeSortByDepOrdinal,
+    DTNodeSortByIrqNumber,
+    DTNodeSortByIrqPriority,
+    DTNodeSortByRegSize,
+    DTNodeSortByRegAddr,
+    DTNodeSortByBindingDepth,
+    # Text-based criteria.
+    DTNodeTextCriterion,
+    DTNodeWithPath,
+    DTNodeWithStatus,
+    DTNodeWithName,
+    DTNodeWithUnitName,
+    DTNodeWithCompatible,
+    DTNodeWithBinding,
+    DTNodeWithVendor,
+    DTNodeWithDeviceLabel,
+    DTNodeWithNodeLabel,
+    DTNodeWithAlias,
+    DTNodeWithChosen,
+    DTNodeAlsoKnownAs,
+    DTNodeWithBus,
+    DTNodeWithOnBus,
+    DTNodeWithDescription,
+    # Integer-based criteria.
+    DTNodeIntCriterion,
+    DTNodeWithUnitAddr,
+    DTNodeWithIrqPriority,
+    DTNodeWithIrqNumber,
+    DTNodeWithRegAddr,
+    DTNodeWithRegSize,
+    DTNodeWithBindingDepth,
+)
+from dtsh.rl import DTShReadline
+from dtsh.autocomp import DTShAutocomp, RlStateEnum
+from dtsh.shell import (
+    DTSh,
+    DTShCommand,
+    DTShFlag,
+    DTShArg,
+    DTShParameter,
+    DTShError,
+    DTPathNotFoundError,
+    DTShCommandError,
 )
 
 
-class DTNodeSortByAttr(DTNodeSorter):
-    """Base for sorters that weight node attributes."""
+class DTShFlagReverse(DTShFlag):
+    """Flag to reverse command output.
 
-    # The name of the dtsh.model.Node attribute this sorter is based on.
-    _attname: str
+    If the command outputs a tree, reverse the children order when walking.
+    If the command outputs a list, reverse this list.
+    """
 
-    # Whether we should compare minimums or maximums when the attribute
-    # value is a list.
-    _reverse: bool = False
+    BRIEF = "reverse command output"
+    SHORTNAME = "r"
 
-    def __init__(self, attname: str) -> None:
-        """Initialize sorter.
 
-        Args:
-            attname: The Python attribute name.
-        """
-        self._attname = attname
+class DTShFlagEnabledOnly(DTShFlag):
+    """Flag to filter out disabled nodes or stop at disabled branches."""
 
-    def split_sortable_unsortable(
-        self, nodes: Sequence[DTNode]
-    ) -> Tuple[List[DTNode], List[DTNode]]:
-        """Overrides DTNodeSorter.split_sortable_unsortable().
+    BRIEF = "filter out disabled nodes or branches"
+    LONGNAME = "enabled-only"
 
-        Returns:
-            The tuple of (sortable, unsortable) where unsortable include
-            nodes for which :
-            - the attribute has no value
-            - the attribute value is an empty lists: [] is less than
-              any non empty list, which would not match
-              the expected semantic (empty lists would appear first)
-        """
-        sortable = []
-        unsortable = []
-        for node in nodes:
-            attr = getattr(node, self._attname)
-            if (attr is not None) and (attr != []):
-                sortable.append(node)
-            else:
-                unsortable.append(node)
-        return (sortable, unsortable)
 
-    def gravity(self, node: DTNode) -> Any:
-        """Input of the weight function.
+class DTShFlagPager(DTShFlag):
+    """Flag to page command output."""
 
-        This is typically the value of the attribute this sorter is based on,
-        but subclasses may override this method to provide a more precise
-        semantic: e.g. a sorter based on the node registers may either
-        weight the register addresses or the register sizes.
+    BRIEF = "page command output"
+    LONGNAME = "pager"
 
-        Args:
-            node: The node to weight.
 
-        Returns:
-            The input for the weight function.
-        """
-        return getattr(node, self._attname)
+class DTShFlagRegex(DTShFlag):
+    """Flag to enforce patterns are interpreted as Regular Expressions.
+
+    If unset, a text search (with wild-card substitution) is assumed.
+    """
 
-    def weight(self, node: DTNode) -> Any:
-        """Overrides DTNodeSorter.weight().
+    BRIEF = "patterns are regular expressions"
+    SHORTNAME = "E"
 
-        The node weight is based on its gravity.
 
-        If the gravity value is a list:
+class DTShFlagIgnoreCase(DTShFlag):
+    """Flag to ignore case in patterns.
 
-        - in ascending order: we expect to compare minimum,
-          so the weight is min(gravity)
-        - in descending order: we expect to compare maximum,
-          so the weight is max(gravity)
+    If unset, case-insensitive patterns are assumed.
+    """
 
-        Returns:
-            The node weight.
-        """
-        w = self.gravity(node)
-        if isinstance(w, list):
-            w = max(w) if self._reverse else min(w)
-        return w
+    BRIEF = "ignore case"
+    SHORTNAME = "i"
 
-    def sort(
-        self, nodes: Sequence[DTNode], reverse: bool = False
-    ) -> List[DTNode]:
-        """Overrides DTNodeSorter.sort()."""
-        # Set the reverse flag that the weight function will rely on.
-        self._reverse = reverse
-        # Then sort nodes with the base DTNodeSorter implementation.
-        return super().sort(nodes, reverse)
 
+class DTShFlagCount(DTShFlag):
+    """Print matches count."""
 
-class DTNodeSortByPathName(DTNodeSortByAttr):
-    """Sort nodes by path name."""
+    BRIEF = "print matches count"
+    LONGNAME = "count"
 
-    def __init__(self) -> None:
-        super().__init__("path")
 
+class DTShFlagTreeLike(DTShFlag):
+    """Whether to list results in tree-like format."""
 
-class DTNodeSortByNodeName(DTNodeSortByAttr):
-    """Sort nodes by node name."""
+    BRIEF = "list results in tree-like format"
+    SHORTNAME = "T"
 
-    def __init__(self) -> None:
-        super().__init__("name")
 
+class DTShFlagNoChildren(DTShFlag):
+    """Whether to list branches themselves, not their contents."""
 
-class DTNodeSortByUnitName(DTNodeSortByAttr):
-    """Sort nodes by unit-name."""
+    BRIEF = "list nodes, not branch contents"
+    SHORTNAME = "d"
 
-    def __init__(self) -> None:
-        super().__init__("unit_name")
 
+class DTShFlagRecursive(DTShFlag):
+    """Whether to list branches rescursively."""
 
-class DTNodeSortByUnitAddr(DTNodeSortByAttr):
-    """Sort nodes by unit-address."""
+    BRIEF = "list recursively"
+    SHORTNAME = "R"
 
-    def __init__(self) -> None:
-        super().__init__("unit_addr")
 
+class DTShFlagLogicalOr(DTShFlag):
+    """Whether to match any criterion instead of all."""
 
-class DTNodeSortByCompatible(DTNodeSortByAttr):
-    """Sort nodes by compatible strings."""
+    BRIEF = "match any criterion instead of all"
+    LONGNAME = "OR"
 
-    def __init__(self) -> None:
-        super().__init__("compatibles")
 
+class DTShFlagLogicalNot(DTShFlag):
+    """Whether to negate the criterion chain."""
 
-class DTNodeSortByBinding(DTNodeSortByAttr):
-    """Sort nodes by binding (compatible value)."""
+    BRIEF = "negate the criterion chain"
+    LONGNAME = "NOT"
 
-    def __init__(self) -> None:
-        super().__init__("compatible")
 
+class DTShArgFixedDepth(DTShArg):
+    """Argument that limits the depth when walking the devicetree.
+
+    The default value is 0, which means unlimited depth.
+    """
+
+    BRIEF = "limit devicetree depth"
+    LONGNAME = "fixed-depth"
 
-class DTNodeSortByVendor(DTNodeSortByAttr):
-    """Sort nodes by vendor name."""
+    # Argument state: depth parsed on the command line.
+    _depth: Optional[int]
 
     def __init__(self) -> None:
-        super().__init__("vendor")
+        super().__init__(argname="depth")
 
-    def gravity(self, node: DTNode) -> Any:
-        """Overrides DTNodeSortByAttrValue.weight().
+    @property
+    def depth(self) -> int:
+        """The fixed depth value.
 
-        Returns:
-            The vendor name.
+        Defaults to zero if unset.
         """
-        # At this point, we know the device has a vendor.
-        return [node.vendor.name]  # type: ignore
+        if self._depth is not None:
+            return self._depth
+        return 0
 
+    def reset(self) -> None:
+        """Reset this argument to its default value (zero).
 
-class DTNodeSortByDeviceLabel(DTNodeSortByAttr):
-    """Sort nodes by device label."""
+        Overrides DTShOption.reset().
+        """
+        super().reset()
+        self._depth = None
 
-    def __init__(self) -> None:
-        super().__init__("label")
+    def parsed(self, value: Optional[str] = None) -> None:
+        """Overrides DTShOption.parsed()."""
+        super().parsed(value)
+        if self._raw:
+            try:
+                depth = int(self._raw or "0")
+            except ValueError as e:
+                raise DTShError(
+                    f"expects an integer value (got '{self._raw}')"
+                ) from e
 
+            if depth < 0:
+                raise DTShError(f"expects a non negative value (got {depth})")
 
-class DTNodeSortByNodeLabel(DTNodeSortByAttr):
-    """Sort nodes by DTS label."""
+            self._depth = depth
 
-    def __init__(self) -> None:
-        super().__init__("labels")
 
+class DTShArgCriterion(DTShArg):
+    """Base for arguments that append a criterion to the chain."""
 
-class DTNodeSortByAlias(DTNodeSortByAttr):
-    """Sort nodes by alias."""
+    def get_criterion(  # pylint: disable=useless-return
+        self, **kwargs: Any
+    ) -> Optional[DTNodeCriterion]:
+        """Get the criterion set by this argument.
 
-    def __init__(self) -> None:
-        super().__init__("aliases")
+        Args:
+            kwargs: Criterion-specific parameters as keyword arguments.
 
+        Returns:
+            The criterion set by the command line, if any.
 
-class DTNodeSortByBus(DTNodeSortByAttr):
-    """Sort nodes by supported bus protocols."""
+        Raises:
+            DTShError: Failed to initialize criterion, should eventually
+              come up as a command usage error.
+        """
+        del kwargs
+        return None
 
-    def __init__(self) -> None:
-        super().__init__("buses")
 
+class DTShArgIntCriterion(DTShArgCriterion):
+    """Base for arguments that append an integer-based (expression) criterion.
 
-class DTNodeSortByOnBus(DTNodeSortByAttr):
-    """Sort nodes by bus of appearance."""
+    Argument format: [OPERATOR] N [UNIT]
 
-    def __init__(self) -> None:
-        super().__init__("on_bus")
+    OPERATOR: "<" | ">" | "<=" | ">=" | "=" | "!="
+    N: the integer to compare with
+    UNIT (case-insensitive):  "k" | "kb" | "m" | "mb"
+    """
 
+    # Match argument with <operator><integer><unit>.
+    _re: re.Pattern[str] = re.compile(
+        r"^(?P<operator>[<>=!]+)?[\s]*(?P<integer>[\da-fA-FxX]+)[\s]*(?P<unit>[kKbBmM]+)?$"
+    )
 
-class DTNodeSortByDepOrdinal(DTNodeSortByAttr):
-    """Sort nodes by dependency ordinal."""
+    # Concrete criterion class.
+    _criter_cls: Type[DTNodeIntCriterion]
 
-    def __init__(self) -> None:
-        super().__init__("dep_ordinal")
+    # Parsed criterion instance.
+    _criterion: Optional[DTNodeIntCriterion]
 
+    def __init__(self, criter_cls: Type[DTNodeIntCriterion]) -> None:
+        """Initialize criterion.
 
-class DTNodeSortByIrqNumber(DTNodeSortByAttr):
-    """Sort nodes by interrupt number."""
+        Args:
+            criter_cls: The concrete type for this criterion.
+        """
+        super().__init__(argname="expr")
+        self._criter_cls = criter_cls
 
-    def __init__(self) -> None:
-        super().__init__("interrupts")
+    def parsed(self, value: Optional[str] = None) -> None:
+        """Overrides DTShArg.parsed()."""
+        super().parsed(value)
+        if not self._raw:
+            return
+
+        if self._raw == "*":
+            # Match any integer value.
+            self._criterion = self._criter_cls(None, None)
+        else:
+            match = DTShArgIntCriterion._re.match(self._raw)
+            if match:
+                op_str = match.group("operator")
+                if op_str:
+                    # Optional spaces after operator.
+                    op_str = op_str.rstrip()
+                    try:
+                        criter_op = DTNodeIntCriterion.OPERATORS[op_str]
+                    except KeyError as e:
+                        raise DTShError(f"invalid operator: '{op_str}'") from e
+                else:
+                    criter_op = None
+
+                int_str = match.group("integer")
+                try:
+                    criter_int = int(int_str, base=0)
+                except ValueError as e:
+                    raise DTShError(f"not a number: '{int_str}'") from e
+
+                unit_str = match.group("unit")
+                if unit_str:
+                    unit_str = unit_str.lower()
+                    if unit_str in ("k", "kb"):
+                        criter_int *= 1024
+                    elif unit_str in ("m", "mb"):
+                        criter_int *= 1024**2
+                    else:
+                        raise DTShError(f"not an SI unit: '{unit_str}'")
 
-    def gravity(self, node: DTNode) -> Any:
-        """Overrides DTNodeSortByAttrValue.weight().
+                self._criterion = self._criter_cls(criter_op, criter_int)
+            else:
+                raise DTShError(f"invalid integer expression: '{self._raw}'")
 
-        Returns:
-            The interrupt numbers.
+    def reset(self) -> None:
+        """Reset this argument.
+
+        Overrides DTShOption.reset().
         """
-        return [irq.number for irq in node.interrupts]
+        super().reset()
+        self._criterion = None
 
+    def get_criterion(self, **kwargs: Any) -> Optional[DTNodeCriterion]:
+        """Overrides DTShArgCriterion.get_criterion()."""
+        return self._criterion
 
-class DTNodeSortByIrqPriority(DTNodeSortByAttr):
-    """Sort nodes by interrupt priority."""
 
-    def __init__(self) -> None:
-        super().__init__("interrupts")
+class DTShArgNodeWithUnitAddr(DTShArgIntCriterion):
+    """Match unit address."""
 
-    def gravity(self, node: DTNode) -> Any:
-        """Overrides DTNodeSortByAttrValue.weight().
+    BRIEF = "match unit addresse"
+    LONGNAME = "with-unit-addr"
 
-        Returns:
-            The interrupt priorities.
-        """
-        return [
-            irq.priority if irq.priority is not None else sys.maxsize
-            for irq in node.interrupts
-        ]
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithUnitAddr)
 
 
-class DTNodeSortByRegAddr(DTNodeSortByAttr):
-    """Sort nodes by register address."""
+class DTShArgNodeWithIrqNumber(DTShArgIntCriterion):
+    """Match IRQ number."""
 
-    def __init__(self) -> None:
-        super().__init__("registers")
+    BRIEF = "match IRQ numbers"
+    LONGNAME = "with-irq-number"
 
-    def gravity(self, node: DTNode) -> Any:
-        """Overrides DTNodeSortByAttrValue.weight().
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithIrqNumber)
 
-        Returns:
-            The register addresses.
-        """
-        return [reg.address for reg in node.registers]
 
+class DTShArgNodeWithIrqPriority(DTShArgIntCriterion):
+    """Match IRQ priority."""
 
-class DTNodeSortByRegSize(DTNodeSortByAttr):
-    """Sort nodes by register size."""
+    BRIEF = "match IRQ priorities"
+    LONGNAME = "with-irq-priority"
 
     def __init__(self) -> None:
-        super().__init__("registers")
-
-    def gravity(self, node: DTNode) -> Any:
-        """Overrides DTNodeSortByAttrValue.weight().
+        super().__init__(DTNodeWithIrqPriority)
 
-        Returns:
-            The register addresses.
-        """
-        return [reg.size for reg in node.registers]
 
+class DTShArgNodeWithRegAddr(DTShArgIntCriterion):
+    """Match  register address."""
 
-class DTNodeSortByBindingDepth(DTNodeSortByAttr):
-    """Sort nodes by child-binding depth."""
+    BRIEF = "match register addresses"
+    LONGNAME = "with-reg-addr"
 
     def __init__(self) -> None:
-        super().__init__("binding")
+        super().__init__(DTNodeWithRegAddr)
 
-    def gravity(self, node: DTNode) -> Any:
-        """Overrides DTNodeSortByAttrValue.weight().
 
-        Returns:
-            The interrupt priorities.
-        """
-        return node.binding.cb_depth if node.binding else None
+class DTShArgNodeWithRegSize(DTShArgIntCriterion):
+    """Match  register address."""
 
+    BRIEF = "match register sizes"
+    LONGNAME = "with-reg-size"
 
-class DTNodeTextCriterion(DTNodeCriterion):
-    """Basis for text-based (pattern) criteria.
-
-    A search pattern is matched to a node aspect that has
-    a textual representation.
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithRegSize)
 
-    This criterion may either match a Regular Expression
-    or search for plain text.
 
-    When the pattern is a strict RE, the criterion behaves as a RE-match,
-    and any character in the pattern may be interpreted as special character:
+class DTShArgNodeWithBindingDepth(DTShArgIntCriterion):
+    """Match  child-binding depth."""
 
-    - in particular, "*" will represent a repetition qualifier,
-      not a wild-card for any character: e.g. a pattern starting with "*"
-      would be an invalid RE because there's nothing to repeat
-    - parenthesis will group sub-expressions, as in "(image|storage).*"
-    - brackets will mark the beginning ("[") and end ("]") of a character set
+    BRIEF = "match child-binding depth"
+    LONGNAME = "with-binding-depth"
 
-    When the pattern is not a strict RE, but contains at least one "*":
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithBindingDepth)
 
-    - "*" is actually interpreted as a wild-card and not a repetition qualifier:
-      here "*" is a valid expression that actually means "anything"
-    - the criterion behaves as a RE-match: "*pattern" means ends with "pattern",
-      "pattern*" starts with "pattern", and "*pattern*" contains "pattern"
 
-    If the pattern is not  a strict RE, and does not contain any "*":
+class DTShArgTextCriterion(DTShArgCriterion):
+    """Base for arguments that append a text-based (pattern) criterion.
 
-    - specials characters won't be interpreted (plain text search)
-    - the criterion will behave as a RE-search
+    See DTNodeTextCriterion.
     """
 
-    # The PATTERN argument from the command line.
-    _pattern: str
+    # Concrete criterion class.
+    _criter_cls: Type[DTNodeTextCriterion]
 
-    # The RE that implements this criterion.
-    _re: re.Pattern[str]
-
-    def __init__(
-        self, pattern: str, re_strict: bool = False, ignore_case: bool = False
-    ) -> None:
+    def __init__(self, criter_cls: Type[DTNodeTextCriterion]) -> None:
         """Initialize criterion.
 
         Args:
-            pattern: The string pattern.
-            re_strict: Whether to assume the pattern us a Regular Expression.
-              Default is plain text search with wild-card substitution.
-            ignore_case: Whether to ignore case.
-              Default is case sensitive search.
-
-        Raises:
-            re.error: Malformed regular expression.
+            criter_cls: The concrete type for this criterion.
         """
-        self._pattern = pattern
-        if re_strict:
-            self._re = self._init_strict_re(pattern, ignore_case)
-        else:
-            self._re = self._init_plain_text(pattern, ignore_case)
+        super().__init__(argname="pattern")
+        self._criter_cls = criter_cls
 
-    @property
-    def pattern(self) -> str:
-        """The pattern string this criterion is built on."""
-        return self._pattern
-
-    def match(self, node: DTNode) -> bool:
-        """Overrides DTNodeCriterion.match()."""
-        return any(
-            self._re.match(txt) is not None for txt in self.get_haystack(node)
-        )
+    def get_criterion(self, **kwargs: Any) -> Optional[DTNodeCriterion]:
+        """Overrides DTShArgCriterion.get_criterion()."""
+        if self._raw:
+            try:
+                return self._criter_cls(
+                    self._raw,
+                    re_strict=kwargs.get("re_strict", False),
+                    ignore_case=kwargs.get("ignore_case", False),
+                )
+            except re.error as e:
+                raise DTShError(f"invalid RE '{self._raw}': {e.msg}") from e
+        return None
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Get the textual representation of the haystack to search.
 
-        The criterion is always False when the haystack is empty.
+class DTShArgNodeWithPath(DTShArgTextCriterion):
+    """Match path name."""
 
-        Returns:
-            The strings that this pattern may match.
-        """
-        del node
-        return []
+    BRIEF = "match path name"
+    LONGNAME = "with-path"
 
-    def _init_strict_re(
-        self, pattern: str, ignore_case: bool
-    ) -> re.Pattern[str]:
-        # RE strict mode, use pattern (e.g. from command string) as-is.
-        return re.compile(pattern, flags=re.IGNORECASE if ignore_case else 0)
-
-    def _init_plain_text(
-        self, pattern: str, ignore_case: bool
-    ) -> re.Pattern[str]:
-        # Plain text search, escape all.
-        pattern = re.escape(pattern)
-        if r"\*" in pattern:
-            # Convert wild-card to repeated printable.
-            pattern = pattern.replace(r"\*", ".*")
-            # Ensure starts/ends with semantic.
-            pattern = f"^{pattern}$"
-        else:
-            # Convert RE-match to RE-search.
-            pattern = f".*{pattern}.*"
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithPath)
 
-        return re.compile(pattern, flags=re.IGNORECASE if ignore_case else 0)
 
-    def __repr__(self) -> str:
-        return self._re.pattern
+class DTShArgNodeWithStatus(DTShArgTextCriterion):
+    """Match status string."""
 
+    BRIEF = "match status string"
+    LONGNAME = "with-status"
 
-class DTNodeWithPath(DTNodeTextCriterion):
-    """Match path."""
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithStatus)
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return [node.path]
 
+class DTShArgNodeWithName(DTShArgTextCriterion):
+    """Match  unit name."""
 
-class DTNodeWithStatus(DTNodeTextCriterion):
-    """Match status string."""
+    BRIEF = "match node name"
+    LONGNAME = "with-name"
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return [node.status]
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithName)
 
 
-class DTNodeWithName(DTNodeTextCriterion):
-    """Match node name."""
+class DTShArgNodeWithUnitName(DTShArgTextCriterion):
+    """Match  unit name."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return [node.name]
+    BRIEF = "match unit name"
+    LONGNAME = "with-unit-name"
 
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithUnitName)
 
-class DTNodeWithUnitName(DTNodeTextCriterion):
-    """Match unit-name."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return [node.unit_name]
+class DTShArgNodeWithCompatible(DTShArgTextCriterion):
+    """Match compatible strings."""
 
+    BRIEF = "match compatible strings"
+    LONGNAME = "with-compatible"
 
-class DTNodeWithCompatible(DTNodeTextCriterion):
-    """Match compatible value."""
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithCompatible)
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return node.compatibles
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with compatible strings.
 
+        Overrides DTShArg.autocomp().
+        """
+        return DTShAutocomp.complete_dtcompat(txt, sh)
 
-class DTNodeWithBinding(DTNodeTextCriterion):
-    """Match binding compatible string.
 
-    If the pattern is "*", will match any node with a binding,
-    including bindings without compatible string.
-    """
+class DTShArgNodeWithBinding(DTShArgTextCriterion):
+    """Match binding compatible or description."""
 
-    def match(self, node: DTNode) -> bool:
-        """Overrides DTNodeCriterion.match()."""
-        if self.pattern == ".*":
-            return node.binding is not None
-        return super().match(node)
-
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        if not node.binding:
-            return []
+    BRIEF = "match binding's compatible or headline"
+    LONGNAME = "with-binding"
 
-        haystack = []
-        if node.binding.compatible:
-            haystack.append(node.binding.compatible)
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithBinding)
 
-        headline = node.binding.get_headline()
-        if headline:
-            haystack.append(headline)
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with compatible strings.
 
-        return haystack
+        Overrides DTShArg.autocomp().
+        """
+        return DTShAutocomp.complete_dtcompat(txt, sh)
 
 
-class DTNodeWithVendor(DTNodeTextCriterion):
+class DTShArgNodeWithVendor(DTShArgTextCriterion):
     """Match vendor prefix or name."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return [node.vendor.prefix, node.vendor.name] if node.vendor else []
+    BRIEF = "match vendor prefix or name"
+    LONGNAME = "with-vendor"
+
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithVendor)
 
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with vendor prefixes.
 
-class DTNodeWithDeviceLabel(DTNodeTextCriterion):
-    """Match device label."""
+        Overrides DTShArg.autocomp().
+        """
+        return DTShAutocomp.complete_dtvendor(txt, sh)
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return [node.label] if node.label else []
 
+class DTShArgNodeWithDescription(DTShArgTextCriterion):
+    """Match description."""
 
-class DTNodeWithNodeLabel(DTNodeTextCriterion):
-    """Match DTS labels."""
+    BRIEF = "grep binding's description"
+    LONGNAME = "with-description"
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return node.labels
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithDescription)
 
 
-class DTNodeWithAlias(DTNodeTextCriterion):
-    """Match aliases."""
+class DTShArgNodeWithBus(DTShArgTextCriterion):
+    """Match supported bus protocol."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return node.aliases
+    BRIEF = "match supported bus protocols"
+    LONGNAME = "with-bus"
 
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithBus)
 
-class DTNodeWithChosen(DTNodeTextCriterion):
-    """Match chosen."""
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with bus protocols.
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return node.chosen
+        Overrides DTShArg.autocomp().
+        """
+        return DTShAutocomp.complete_dtbus(txt, sh)
 
 
-class DTNodeWithBus(DTNodeTextCriterion):
-    """Match nodes with supported bus protocols."""
+class DTShArgNodeWithOnBus(DTShArgTextCriterion):
+    """Match bus of appearance."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return node.buses
+    BRIEF = "match bus of appearance"
+    LONGNAME = "on-bus"
 
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithOnBus)
 
-class DTNodeWithOnBus(DTNodeTextCriterion):
-    """Match nodes with bus of appearance."""
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with bus protocols.
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        return [node.on_bus] if node.on_bus else []
+        Overrides DTShArg.autocomp().
+        """
+        return DTShAutocomp.complete_dtbus(txt, sh)
 
 
-class DTNodeWithDescription(DTNodeTextCriterion):
-    """Match node with description line by line."""
+class DTShArgNodeWithDeviceLabel(DTShArgTextCriterion):
+    """Match device label."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        if not node.description:
-            return []
-        return node.description.splitlines()
+    BRIEF = "match device label"
+    LONGNAME = "with-device-label"
 
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithDeviceLabel)
 
-class DTNodeAlsoKnownAs(DTNodeTextCriterion):
-    """Match nodes with labels and aliases."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[str]:
-        """Overrides DTNodeTextCriterion.get_haystack()."""
-        aka = [
-            *node.aliases,
-            *node.labels,
-        ]
-        if node.label:
-            aka.append(node.label)
-        return aka
-
-
-class DTNodeIntCriterion(DTNodeCriterion):
-    """Basis for integer-based (expression) criteria."""
-
-    OPERATORS: Mapping[str, Callable[[int, int], bool]] = {
-        "<": operator.lt,
-        ">": operator.gt,
-        "=": operator.eq,
-        ">=": operator.ge,
-        "<=": operator.le,
-        "!=": operator.ne,
-    }
-
-    _operator: Callable[[int, int], bool]
-    _int: Optional[int]
-
-    def __init__(
-        self,
-        criter_op: Optional[Callable[[int, int], bool]],
-        criter_int: Optional[int],
-    ) -> None:
-        """Initialize criterion.
+class DTShArgNodeWithNodeLabel(DTShArgTextCriterion):
+    """Match node labels."""
 
-        Args:
-            criter_op: The expression operator,
-              one of DTNodeIntCriterion.OPERATORS.
-              Defaults to equality.
-            criter_int: The integer value the criterion expression should match.
-              None means any integer value will match.
-        """
-        self._operator = criter_op or operator.eq
-        self._int = criter_int
-
-    def match(self, node: DTNode) -> bool:
-        """Overrides DTNodeCriterion.match()."""
-        return any(
-            ((self._int is None) or self._operator(hay, self._int))
-            for hay in self.get_haystack(node)
-        )
+    BRIEF = "match node labels"
+    LONGNAME = "with-label"
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Get the integer representation of the haystack to search.
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithNodeLabel)
 
-        The criterion is always False when the haystack is empty.
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with node labels.
 
-        Returns:
-            The integers that this expression may match.
+        Overrides DTShArg.autocomp().
         """
-        del node
-        return []
+        if txt.startswith("&"):
+            # We're completing labels, and labels can't start with "&".
+            return []
+        return DTShAutocomp.complete_dtlabel(txt, sh)
 
 
-class DTNodeWithUnitAddr(DTNodeIntCriterion):
-    """Match unit-address."""
+class DTShArgNodeWithAlias(DTShArgTextCriterion):
+    """Match nodes with device label."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Overrides DTNodeIntCriterion.get_haystack()."""
-        return [node.unit_addr] if node.unit_addr is not None else []
+    BRIEF = "match aliases"
+    LONGNAME = "with-alias"
 
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithAlias)
 
-class DTNodeWithIrqNumber(DTNodeIntCriterion):
-    """Match IRQ number."""
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with alias names.
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Overrides DTNodeIntCriterion.get_haystack()."""
-        return [irq.number for irq in node.interrupts]
+        Overrides DTShArg.autocomp().
+        """
+        return DTShAutocomp.complete_dtalias(txt, sh)
 
 
-class DTNodeWithIrqPriority(DTNodeIntCriterion):
-    """Match IRQ priority."""
+class DTShArgNodeWithChosen(DTShArgTextCriterion):
+    """Match chosen nodes."""
+
+    BRIEF = "match chosen nodes"
+    LONGNAME = "chosen-for"
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Overrides DTNodeIntCriterion.get_haystack()."""
-        return [
-            irq.priority for irq in node.interrupts if irq.priority is not None
-        ]
+    def __init__(self) -> None:
+        super().__init__(DTNodeWithChosen)
+
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with parameter names.
+
+        Overrides DTShArg.autocomp().
+        """
+        return DTShAutocomp.complete_dtchosen(txt, sh)
 
 
-class DTNodeWithRegAddr(DTNodeIntCriterion):
-    """Match register address."""
+class DTShArgNodeAlsoKnownAs(DTShArgTextCriterion):
+    """Match labels and aliases."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Overrides DTNodeIntCriterion.get_haystack()."""
-        return [reg.address for reg in node.registers]
+    BRIEF = "match labels or aliases"
+    LONGNAME = "also-known-as"
 
+    def __init__(self) -> None:
+        super().__init__(DTNodeAlsoKnownAs)
 
-class DTNodeWithRegSize(DTNodeIntCriterion):
-    """Match register size."""
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Overrides DTNodeIntCriterion.get_haystack()."""
-        return [reg.size for reg in node.registers]
+DTSH_ARG_NODE_CRITERIA: Sequence[DTShArgCriterion] = [
+    # Text-based criteria.
+    DTShArgNodeWithPath(),
+    DTShArgNodeWithStatus(),
+    DTShArgNodeWithName(),
+    DTShArgNodeWithUnitName(),
+    DTShArgNodeWithCompatible(),
+    DTShArgNodeWithBinding(),
+    DTShArgNodeWithVendor(),
+    DTShArgNodeWithDescription(),
+    DTShArgNodeWithBus(),
+    DTShArgNodeWithOnBus(),
+    DTShArgNodeWithDeviceLabel(),
+    DTShArgNodeWithNodeLabel(),
+    DTShArgNodeWithAlias(),
+    DTShArgNodeWithChosen(),
+    DTShArgNodeAlsoKnownAs(),
+    # Integer-based criteria.
+    DTShArgNodeWithUnitAddr(),
+    DTShArgNodeWithIrqNumber(),
+    DTShArgNodeWithIrqPriority(),
+    DTShArgNodeWithRegAddr(),
+    DTShArgNodeWithRegSize(),
+    DTShArgNodeWithBindingDepth(),
+]
+"""Pre-defined criteria shell commands may use to match nodes."""
 
 
-class DTNodeWithBindingDepth(DTNodeIntCriterion):
-    """Match child-binding depth."""
+class DTShNodeOrderBy:
+    """Node sorter definition to be used by shell commands.
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Overrides DTNodeIntCriterion.get_haystack()."""
-        return [node.binding.cb_depth] if node.binding else []
+    Associate user friendly meta-data to sorter implementations.
+    """
 
+    _key: str
+    # Order by what (human readable form) ?
+    _what: str
+
+    # The sorter implementation.
+    _sorter: DTNodeSorter
+
+    def __init__(self, key: str, by_what: str, sorter: DTNodeSorter) -> None:
+        """Initialize sorted definition.
+
+        Args:
+            key: A single character key to reference the sorter with.
+            by_what: A human readable name for the node aspect this sorter
+              relies on.
+            sorter: The corresponding sorter implementation.
+        """
+        self._key = key
+        self._what = by_what
+        self._sorter = sorter
 
-class DTNodeWithDepOrd(DTNodeIntCriterion):
-    """Match dependency ordinal (aka DTS order)."""
+    @property
+    def key(self) -> str:
+        """A single character key to reference the sorter with."""
+        return self._key
 
-    def get_haystack(self, node: DTNode) -> Sequence[int]:
-        """Overrides DTNodeIntCriterion.get_haystack()."""
-        return [node.dep_ordinal]
+    @property
+    def brief(self) -> str:
+        """A brief description of the sorter."""
+        return f"sort by {self._what}"
 
+    @property
+    def sorter(self) -> DTNodeSorter:
+        """The sorter implementation."""
+        return self._sorter
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, DTShNodeOrderBy):
+            return self._key == other._key
+        return False
+
+    def __lt__(self, other: object) -> bool:
+        if isinstance(other, DTShNodeOrderBy):
+            return self._key < other._key
+        raise TypeError(other)
+
+    def __hash__(self) -> int:
+        return hash(self._key)
+
+
+DTSH_NODE_ORDER_BY: Mapping[str, DTShNodeOrderBy] = {
+    order_by.key: order_by
+    for order_by in [
+        DTShNodeOrderBy("p", "node path", DTNodeSortByPathName()),
+        DTShNodeOrderBy("N", "node name", DTNodeSortByNodeName()),
+        DTShNodeOrderBy("n", "unit name", DTNodeSortByUnitName()),
+        DTShNodeOrderBy("a", "unit address", DTNodeSortByUnitAddr()),
+        DTShNodeOrderBy("c", "compatible strings", DTNodeSortByCompatible()),
+        DTShNodeOrderBy("C", "binding", DTNodeSortByBinding()),
+        DTShNodeOrderBy("v", "vendor name", DTNodeSortByVendor()),
+        DTShNodeOrderBy("l", "device label", DTNodeSortByDeviceLabel()),
+        DTShNodeOrderBy("L", "node labels", DTNodeSortByNodeLabel()),
+        DTShNodeOrderBy("A", "aliases", DTNodeSortByAlias()),
+        DTShNodeOrderBy("B", "supported bus protocols", DTNodeSortByBus()),
+        DTShNodeOrderBy("b", "bus of appearance", DTNodeSortByOnBus()),
+        DTShNodeOrderBy("o", "dependency ordinal", DTNodeSortByDepOrdinal()),
+        DTShNodeOrderBy("i", "IRQ numbers", DTNodeSortByIrqNumber()),
+        DTShNodeOrderBy("I", "IRQ priorities", DTNodeSortByIrqPriority()),
+        DTShNodeOrderBy("r", "register addresses", DTNodeSortByRegAddr()),
+        DTShNodeOrderBy("s", "register sizes", DTNodeSortByRegSize()),
+        DTShNodeOrderBy("X", "child-binding depth", DTNodeSortByBindingDepth()),
+    ]
+}
+"""Pre-defined order relationships shell commands may use to sort nodes."""
 
-class DTWalkableComb(DTWalkable):
-    """Walk an arbitrary subset of a devicetree.
 
-    Permits to define a virtual devicetree as the minimal graph
-    that will contain the paths from a given root to a selected
-    set of leaves.
+class DTShArgOrderBy(DTShArg):
+    """Argument to set the nodes sorter.
 
-    The comb is the set of nodes this graph includes.
+    The relationship is selected with a key specifier.
     """
 
-    _root: DTNode
-    _comb: Set[DTNode]
+    BRIEF = "sort nodes or branches"
+    LONGNAME = "order-by"
 
-    def __init__(self, root: DTNode, leaves: Sequence[DTNode]) -> None:
-        """Initialize the virtual devicetree.
+    # Argument state: sorter implementation, no default value.
+    _sorter: Optional[DTNodeSorter]
 
-        Args:
-            root: Set the root node from where we'll later on
-              walk the virtual devicetree.
-            leaves: The leaf nodes of the virtual devicetree.
-        """
-        self._root = root
-        self._comb: Set[DTNode] = set()
-        for leaf in leaves:
-            self._comb.update(list(leaf.rwalk()))
+    def __init__(self) -> None:
+        super().__init__(argname="key")
+
+    def reset(self) -> None:
+        """Overrides DTShOption.reset()."""
+        super().reset()
+        self._sorter = None
+
+    def parsed(self, value: Optional[str] = None) -> None:
+        """Overrides DTShOption.parsed()."""
+        super().parsed(value)
+        if self._raw:
+            try:
+                self._sorter = DTSH_NODE_ORDER_BY[self._raw].sorter
+            except KeyError as e:
+                raise DTShError(f"invalid sort key: '{self._raw}'") from e
 
     @property
-    def comb(self) -> Set[DTNode]:
-        """All the nodes required to represent this virtual devicetree."""
-        return self._comb
-
-    def walk(
-        self,
-        /,
-        order_by: Optional[DTNodeSorter] = None,
-        reverse: bool = False,
-        enabled_only: bool = False,
-        fixed_depth: int = 0,
-    ) -> Iterator[DTNode]:
-        """Walk from the predefined root node through to all leaves.
+    def sorter(self) -> Optional[DTNodeSorter]:
+        """The sorter argument parsed on the command line."""
+        return self._sorter
+
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with the predefined sorter definitions.
+
+        Overrides DTShArg.autocomp().
+        """
+        return sorted(
+            [
+                RlStateEnum(key, order_by.brief)
+                for key, order_by in DTSH_NODE_ORDER_BY.items()
+                if key.startswith(txt)
+            ],
+            key=lambda x: x.rlstr.lower(),
+        )
 
-        Overrides DTWalkable.walk().
 
-        Args:
-            enabled_only: Ignored, will always walk through to its leaves.
-            fixed_depth: Ignored, will always walk through to its leaves.
-        """
-        return self._walk(self._root, order_by=order_by, reverse=reverse)
+class DTShParamDTPath(DTShParameter):
+    """Devicetree path parameter.
 
-    def _walk(
-        self,
-        branch: Optional[DTNode] = None,
-        /,
-        order_by: Optional[DTNodeSorter] = None,
-        reverse: bool = False,
-    ) -> Iterator[DTNode]:
-        if branch in self._comb:
-            yield branch
-            children = branch.children
-            if children:
-                if order_by:
-                    children = order_by.sort(children, reverse=reverse)
-                elif reverse:
-                    # Reverse DTS-order.
-                    children = list(reversed(children))
-                for child in children:
-                    yield from self._walk(
-                        child, order_by=order_by, reverse=reverse
-                    )
-
-
-class DTSUtil:
-    """Factory for string representations of DTS types."""
-
-    @classmethod
-    def mk_property_value(cls, prop: DTNodeProperty) -> str:
-        """Make a string representation of a property value that resembles
-        its DTS format.
+    This parameter accepts an optional single value,
+    and is not intended to support path expansion (globbing).
+    """
 
-        Args:
-            prop: The DT property.
+    def __init__(self) -> None:
+        super().__init__(
+            name="path",
+            multiplicity="?",
+            brief="devicetree path",
+        )
 
-        Returns:
-            The property value as it could appear in the DTS:
-            - DT type "bool": true or false
-            - DT type "int": e.g. < 0x01 >
-            - DT type "array": e.g. < 0x2f >, < 0x01 >
-            - DT type "string": e.g. "str"
-            - DT type "string-array": e.g. "str1", "str2"
-            - DT type "uint8-array": e.g. [ C2 28 17 ]
-            - DT type "phandle": e.g. < &spi3_sleep >
-            - DT type "phandles": e.g. < &spi3_sleep &spi3_default >
-            - DT type "phandle-array": e.g. < &ctrl-1 0x01 0x02 >, < &ctrl-2 0x01 0x02 >
-        """
-        value: DTNodeProperty.ValueType = prop.value
-
-        if isinstance(value, list):
-            val0: Union[int, str, DTNode, DTNodePHandleData, None] = value[0]
-
-            if isinstance(val0, int):
-                # DTS "type: array".
-                int_array: List[int] = cast(List[int], value)
-                return cls.mk_array(int_array)
-
-            if isinstance(val0, str):
-                # DTS "type: string-array".
-                str_array: List[str] = cast(List[str], value)
-                return cls.mk_string_array(str_array)
-
-            if isinstance(val0, DTNode):
-                # DTS "type: phandles".
-                phandles: List[DTNode] = cast(List[DTNode], value)
-                return cls.mk_phandles(phandles)
-
-            if isinstance(val0, DTNodePHandleData):
-                # DTS "type: phandle-array".
-                phandle_array: List[DTNodePHandleData] = cast(
-                    List[DTNodePHandleData], value
-                )
-                return cls.mk_phandle_array(phandle_array)
+    @property
+    def path(self) -> str:
+        """The path parameter value set by the command line.
 
-        if isinstance(value, bool):
-            # DTS "type: boolean".
-            return cls.mk_boolean(value)
-        if isinstance(value, int):
-            # DTS "type: int".
-            return cls.mk_int(value, as_cell=True)
-        if isinstance(value, str):
-            # DTS "type: string".
-            return cls.mk_string(value)
-        if isinstance(value, bytes):
-            # DTS "type: uint8-array".
-            return cls.mk_bytes(value)
-        if isinstance(value, DTNode):
-            # DTS "type: phandle".
-            return cls.mk_phandle(value)
-
-        # Answer empty string for properties with None value,
-        # e.g. the "ranges" property of the /soc node, of type "compound".
-        return ""
-
-    @classmethod
-    def mk_boolean(cls, value: bool) -> str:
-        """Make DTS-like output for values of type "boolean".
+        If unset, will answer an empty string,
+        the semantic of which will depend on the
+        supporting command.
+        """
+        return self._raw[0] if self._raw else ""
 
-        Args:
-            value: The DT value.
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with Devicetree paths.
 
-        Returns:
-            "true" or "false".
+        Overrides DTShParameter.autocomp().
         """
-        return str(value).lower()
+        return DTShAutocomp.complete_dtpath(txt, sh)
 
-    @classmethod
-    def mk_int(cls, value: int, as_cell: bool) -> str:
-        """Make DTS-like output for values of type "int".
 
-        Args:
-            value: The DT value.
-            as_cell: Whether to put the value in a "<>" cell.
+class DTShParamDTPaths(DTShParameter):
+    """Devicetree paths parameter.
 
-        Returns:
-            An integer cell, e.g. "< 0x01 >"
-        """
-        # We'll format hex according to the required number of bytes.
-        nbytes = 0
-        x = value
-        while x:
-            x >>= 8
-            nbytes += 1
-        nbytes = nbytes or 1
-
-        fmt = f"0x{{:0{2*nbytes}x}}"
-        strval = fmt.format(value)
-
-        if as_cell:
-            strval = cls._mk_cell(strval)
-        return strval
-
-    @classmethod
-    def mk_string(cls, value: str) -> str:
-        """Make DTS-like output for values of type "string".
+    This parameter accepts any number of values,
+    each representing a path expression that may expand (globbing)
+    to several Devicetree paths.
+    """
 
-        Args:
-            value: The DT value.
+    def __init__(self) -> None:
+        super().__init__(
+            name="path",
+            multiplicity="*",
+            brief="devicetree path",
+        )
 
-        Returns:
-            A quoted string.
+    @property
+    def paths(self) -> Sequence[str]:
+        """The path parameter values set by the command line.
+
+        If unset, will answer an single empty value,
+        representing the current working branch.
         """
-        return f'"{value}"'
+        return self._raw if self._raw else [""]
 
-    @classmethod
-    def mk_bytes(cls, value: bytes) -> str:
-        """Make DTS-like output for values of type "uint8-array".
+    def expand(self, cmd: DTShCommand, sh: DTSh) -> List[DTSh.PathExpansion]:
+        """Expand this parameter.
 
         Args:
-            value: The DT value.
+            cmd: The executing command.
+            sh: The context shell.
 
         Returns:
-            An array of un-prefixed uppercase bytes, e.g. "[ C2 28 17 ]".
+            A list containing one path expansion per parameter value.
+            For convenience, nodes are filtered if the command supports
+            the "enabled only" flag.
+
+        Raises:
+            DTShCommandError: Path expansion failed (node not found).
         """
-        strbytes = " ".join(f"{b:02X}" for b in value)
-        return f"[ {strbytes} ]"
+        enabled_only: bool = False
+        try:
+            enabled_only = cmd.with_flag(DTShFlagEnabledOnly)
+        except KeyError:
+            # Unsupported option, no filter.
+            enabled_only = False
 
-    @classmethod
-    def mk_phandle(cls, node: DTNode, as_cell: bool = True) -> str:
-        """Make DTS-like output for values of type "phandle".
+        try:
+            return [
+                sh.path_expansion(path, enabled_only)
+                for path in self._raw or [""]
+            ]
+        except DTPathNotFoundError as e:
+            raise DTShCommandError(cmd, e.msg) from e
 
-        Args:
-            node: The DT value.
-            as_cell: Whether to put the value in a "<>" cell.
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete with Devicetree paths.
 
-        Returns:
-            By default, a cell containing the handle, e.g. "< &spi3_sleep >".
+        Overrides DTShParameter.autocomp().
         """
-        # These usually have at least one DTS label.
-        if node.labels:
-            strhandle = f"&{node.labels[0]}"
-        else:
-            # Fallback to node's path.
-            strhandle = node.path
+        return DTShAutocomp.complete_dtpath(txt, sh)
 
-        if as_cell:
-            strhandle = cls._mk_cell(strhandle)
-        return strhandle
-
-    @classmethod
-    def mk_array(cls, int_arr: List[int], as_cell: bool = True) -> str:
-        """Make DTS-like output for values of type "array".
 
-        Args:
-            int_arr: The DT value.
-            as_cell: Whether to put the array in a single "<>" cell instead
-              of a comma separated list.
+class DTShParamAlias(DTShParameter):
+    """Alias name parameter."""
 
-        Returns:
-            A comma separated list of integer cells, e.g. "< 0x2f >, < 0x01 >"
-            or the array as a single cell e.g. "< 0x2f 0x01 >".
+    def __init__(self) -> None:
+        super().__init__(
+            name="name",
+            multiplicity="?",
+            brief="alias name",
+        )
+
+    @property
+    def alias(self) -> str:
+        """The parameter value set by the command line.
+
+        If unset, will answer an empty string means (any/all aliased nodes).
         """
-        if as_cell:
-            # Array as single cell.
-            strval = " ".join(cls.mk_int(val, as_cell=False) for val in int_arr)
-            return cls._mk_cell(strval)
-
-        # Comma separated list.
-        return ", ".join(cls.mk_int(val, as_cell=True) for val in int_arr)
-
-    @classmethod
-    def mk_string_array(cls, str_arr: List[str]) -> str:
-        """Make DTS-like output for values of type "string-array".
+        return self._raw[0] if self._raw else ""
 
-        Args:
-            str_arr: The DT value.
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete parameter with alias names.
 
-        Returns:
-            A comma separated list of quoted strings.
+        Overrides DTShParameter.autocomp().
         """
-        return ", ".join(cls.mk_string(val) for val in str_arr)
+        return DTShAutocomp.complete_dtalias(txt, sh)
 
-    @classmethod
-    def mk_phandles(cls, phandles: List[DTNode]) -> str:
-        """Make DTS-like output for values of type "phandles".
 
-        Args:
-            phandles: The DT value.
+class DTShParamChosen(DTShParameter):
+    """Chosen name parameter."""
 
-        Returns:
-            A cell containing one or more phandles, e.g. "< &ctrl-1 &ctrl-2 >".
-        """
-        strval = " ".join(
-            cls.mk_phandle(node, as_cell=False) for node in phandles
+    def __init__(self) -> None:
+        super().__init__(
+            name="name",
+            multiplicity="?",
+            brief="chosen name",
         )
-        return cls._mk_cell(strval)
 
-    @classmethod
-    def mk_phandle_array(cls, phandle_array: List[DTNodePHandleData]) -> str:
-        """Make DTS-like output for values of type "phandle-array".
-
-        Args:
-            phandle_array: The DT value.
+    @property
+    def chosen(self) -> str:
+        """The parameter value set by the command line.
 
-        Returns:
-            A comma separated list of phandle-array entries.
+        If unset, will answer an empty string means (any/all aliased nodes).
         """
-        phdata_entries = [
-            cls.mk_phandle_and_data(entry, as_cell=True)
-            for entry in phandle_array
-        ]
-        return ", ".join(phdata_entries)
-
-    @classmethod
-    def mk_phandle_and_data(
-        cls, phdata: DTNodePHandleData, as_cell: bool = True
-    ) -> str:
-        """Make DTS-like output for entries in a "phandle-array".
+        return self._raw[0] if self._raw else ""
 
-        Args:
-            phdata: The DT value.
+    def autocomp(self, txt: str, sh: DTSh) -> List[DTShReadline.CompleterState]:
+        """Auto-complete argument value with chosen names.
 
-        Returns:
-            By default, a cell containing the PHandle and its data,
-            e.g. < &ctrl-1 0x01 0x10 >.
-            Non-integer data values are converted to their default
-            string representation.
-        """
-        data_values: List[str] = [
-            cls.mk_int(data, as_cell=False)
-            if isinstance(data, int)
-            else str(data)
-            for data in phdata.data.values()
-        ]
-
-        str_data = " ".join(val for val in data_values)
-        str_phandle = cls.mk_phandle(phdata.phandle, as_cell=False)
-        strval = f"{str_phandle} {str_data}"
-
-        if as_cell:
-            strval = cls._mk_cell(strval)
-        return strval
-
-    @classmethod
-    def _mk_cell(cls, content: str) -> str:
-        return f"< {content} >"
+        Overrides DTShParameter.autocomp().
+        """
+        return DTShAutocomp.complete_dtchosen(txt, sh)
```

### Comparing `dtsh-0.2.2/src/dtsh/rich/autocomp.py` & `dtsh-0.2rc1/src/dtsh/rich/autocomp.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     RlStateDTPath,
     RlStateCompatStr,
     RlStateDTVendor,
     RlStateDTBus,
     RlStateDTAlias,
     RlStateDTChosen,
     RlStateDTLabel,
-    RlStateDTProperty,
     RlStateFsEntry,
     RlStateEnum,
 )
 
 from dtsh.rich.theme import DTShTheme
 from dtsh.rich.text import TextUtil
 from dtsh.rich.tui import GridLayout
@@ -79,17 +78,14 @@
 
             elif isinstance(state, RlStateDTChosen):
                 self._rlstates_view_add_chosen(grid, state)
 
             elif isinstance(state, RlStateDTLabel):
                 self._rlstates_view_add_label(grid, state)
 
-            elif isinstance(state, RlStateDTProperty):
-                self._rlstates_view_add_dtprop(grid, state)
-
             elif isinstance(state, RlStateFsEntry):
                 self._rlstates_view_add_fspath(grid, state)
 
             elif isinstance(state, RlStateEnum):
                 self._rlstates_view_add_enum(grid, state)
 
             else:
@@ -123,15 +119,15 @@
             # The compatible string associates bindings,
             # look for description.
             if len(state.bindings) == 1:
                 # Single binding, use its description if any.
                 binding = state.bindings.pop()
                 if binding.description:
                     txt_desc = TextUtil.mk_headline(
-                        binding.description, DTShTheme.STYLE_DT_DESCRIPTION
+                        binding.description, DTShTheme.STYLE_DT_BINDING_DESC
                     )
             else:
                 headlines: Set[str] = set()
                 buses: Set[str] = set()
 
                 for binding in state.bindings:
                     if binding.on_bus:
@@ -140,15 +136,15 @@
                     if headline:
                         headlines.add(headline)
 
                 if len(headlines) == 1:
                     # All associated bindings have the same description
                     # headline, use it.
                     txt_desc = TextUtil.mk_headline(
-                        headlines.pop(), DTShTheme.STYLE_DT_DESCRIPTION
+                        headlines.pop(), DTShTheme.STYLE_DT_BINDING_DESC
                     )
                 elif buses:
                     # Tell user about different buses of appearance.
                     txt_desc = TextUtil.assemble(
                         TextUtil.italic("Available for different buses: "),
                         TextUtil.mk_text(
                             ", ".join(buses), DTShTheme.STYLE_DT_BUS
@@ -197,15 +193,15 @@
         self, grid: GridLayout, state: RlStateDTLabel
     ) -> None:
         txt_label = TextUtil.mk_text(state.label, DTShTheme.STYLE_DT_NODE_LABEL)
         if not state.node.enabled:
             TextUtil.dim(txt_label)
         if state.node.description:
             txt_desc = TextUtil.mk_headline(
-                state.node.description, DTShTheme.STYLE_DT_DESCRIPTION
+                state.node.description, DTShTheme.STYLE_DT_BINDING_DESC
             )
             if not state.node.enabled:
                 TextUtil.dim(txt_desc)
         else:
             txt_desc = None
         grid.add_row(txt_label, txt_desc)
 
@@ -220,27 +216,11 @@
         else:
             txt = TextUtil.mk_text(
                 state.dirent.name,
                 style=DTShTheme.STYLE_FS_FILE,
             )
         layout.add_row(txt, None)
 
-    def _rlstates_view_add_dtprop(
-        self, grid: GridLayout, state: RlStateDTProperty
-    ) -> None:
-        txt_prop = TextUtil.mk_text(
-            state.dtproperty.name, DTShTheme.STYLE_DT_PROPERTY
-        )
-
-        if state.dtproperty.description:
-            txt_desc = TextUtil.mk_headline(
-                state.dtproperty.description, DTShTheme.STYLE_DT_DESCRIPTION
-            )
-        else:
-            txt_desc = None
-
-        grid.add_row(txt_prop, txt_desc)
-
     def _rlstates_view_add_enum(
         self, grid: GridLayout, state: RlStateEnum
     ) -> None:
         grid.add_row(TextUtil.bold(state.value), state.brief)
```

### Comparing `dtsh-0.2.2/src/dtsh/rich/io.py` & `dtsh-0.2rc1/src/dtsh/rich/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - rich VT
 - rich redirection streams for SVG and HTML
 
 Rich I/O streams implementations are based on the rich.console module.
 """
 
 
-from typing import Any, IO, List, Mapping, Optional, Sequence
+from typing import Any, IO, List, Mapping, Optional
 
 import os
 
 from rich.console import Console, PagerContext
 from rich.measure import Measurement
 from rich.theme import Theme
 from rich.terminal_theme import (
@@ -24,15 +24,15 @@
     MONOKAI,
     DIMMED_MONOKAI,
     NIGHT_OWLISH,
     TerminalTheme,
 )
 
 from dtsh.config import DTShConfig
-from dtsh.io import DTShVT, DTShInput, DTShOutput, DTShRedirect
+from dtsh.io import DTShVT, DTShOutput, DTShRedirect
 
 from dtsh.rich.theme import DTShTheme
 from dtsh.rich.svg import SVGContentsFmt, SVGContents
 
 _dtshconf: DTShConfig = DTShConfig.getinstance()
 _theme: DTShTheme = DTShTheme.getinstance()
 
@@ -84,59 +84,14 @@
     def pager_exit(self) -> None:
         """Overrides DTShOutput.pager_exit()."""
         if self._pager:
             self._pager.__exit__(None, None, None)
             self._pager = None
 
 
-class DTShBatchRichVT(DTShRichVT):
-    """Rich terminal for devicetree shells with batch mode support.
-
-    Batch mode support, will:
-    - first read command lines from the batch input stream until EOF
-    - then, if interactive, read command lines from VT input stream until EOF
-    """
-
-    # Batch input stream, reset to None on EOF.
-    _batch_is: Optional[DTShInput]
-
-    # Whether to read from VT after batch.
-    _interactive: bool
-
-    def __init__(self, batch_is: DTShInput, interactive: bool) -> None:
-        """Initialize VT.
-
-        Args:
-            batch: Batch input stream.
-            interactive: Whether to read from VT after batch
-              (interactive sessions).
-        """
-        super().__init__()
-        self._batch_is = batch_is
-        self._interactive = interactive
-
-    def is_tty(self) -> bool:
-        """Overrides DTShInput.is_tty()."""
-        return self._batch_is is None
-
-    def readline(self, multi_prompt: Optional[Sequence[Any]] = None) -> str:
-        """Overrides DTShVT.readline()."""
-        if self._batch_is:
-            try:
-                return self._batch_is.readline(multi_prompt)
-            except EOFError:
-                # Exhausted batch input stream.
-                self._batch_is = None
-
-        if not self._interactive:
-            # Signal EOF if we don't continue in interactive mode.
-            raise EOFError()
-        return super().readline(multi_prompt)
-
-
 class DTShOutputFileText(DTShOutput):
     """Text output file for commands output redirection."""
 
     _out: IO[str]
     _console: Console
 
     def __init__(self, path: str, append: bool) -> None:
```

### Comparing `dtsh-0.2.2/src/dtsh/rich/svg.py` & `dtsh-0.2rc1/src/dtsh/rich/svg.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/rich/text.py` & `dtsh-0.2rc1/src/dtsh/rich/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -207,50 +207,14 @@
                 # Remove trailing dot if ellipsis.
                 headline = headline[:-1]
             headline = f"{headline}{_dtshconf.wchar_ellipsis}"
 
         return cls.mk_text(headline, style)
 
     @classmethod
-    def mk_apologies(cls, msg: str) -> Text:
-        """Make a simple message styled for apologies.
-
-        Args:
-            msg: The message.
-
-        Returns:
-            A new text view.
-        """
-        return Text(msg, style=DTShTheme.STYLE_APOLOGIES)
-
-    @classmethod
-    def mk_error(cls, msg: str) -> Text:
-        """Make an error message.
-
-        Args:
-            msg: The message.
-
-        Returns:
-            A new text view.
-        """
-        return Text(msg, style=DTShTheme.STYLE_ERROR)
-
-    @classmethod
-    def mk_warning(cls, msg: str) -> Text:
-        """Make a warning message.
-
-        Args:
-            msg: The message.
-
-        Returns:
-            A new text view.
-        """
-        return Text(msg, style=DTShTheme.STYLE_WARNING)
-
-    @classmethod
     def join(cls, sep: Union[str, Text], parts: Iterable[Text]) -> Text:
         """Join rich text elements."""
         if isinstance(sep, str):
             sep = cls.mk_text(sep)
         return sep.join(parts)
 
     @classmethod
```

### Comparing `dtsh-0.2.2/src/dtsh/rich/theme.py` & `dtsh-0.2rc1/src/dtsh/rich/theme.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 
 Unit tests and examples: tests/test_dtsh_theme.py
 """
 
 
 from typing import Optional, Dict, Mapping
 
-import configparser
 import os
-import sys
+
 
 from rich.errors import StyleError, StyleSyntaxError
 from rich.style import Style
 from rich.theme import Theme
 
 from dtsh.config import DTShConfig
 
@@ -38,30 +37,27 @@
 class DTShTheme:
     """Rich styles."""
 
     STYLE_DEFAULT = "dtsh.default"
     STYLE_ERROR = "dtsh.error"
     STYLE_WARNING = "dtsh.warning"
     STYLE_DISABLED = "dtsh.disabled"
-    STYLE_APOLOGIES = "dtsh.apologies"
 
     STYLE_FS_FILE = "dtsh.fs.file"
     STYLE_FS_DIR = "dtsh.fs.dir"
 
     STYLE_LINK_LOCAL = "dtsh.link.local"
     STYLE_LINK_WWW = "dtsh.link.www"
 
     STYLE_LIST_HEADER = "dtsh.list.header"
     STYLE_TREE_HEADER = "dtsh.tree.header"
 
     STYLE_DT_PATH_BRANCH = "dtsh.dt.path_branch"
     STYLE_DT_PATH_NODE = "dtsh.dt.path_node"
 
-    STYLE_DT_DESCRIPTION = "dtsh.dt.description"
-
     STYLE_DT_NODE_NAME = "dtsh.dt.node_name"
     STYLE_DT_UNIT_NAME = "dtsh.dt.unit_name"
     STYLE_DT_UNIT_ADDR = "dtsh.dt.unit_addr"
     STYLE_DT_DEVICE_LABEL = "dtsh.dt.device_label"
     STYLE_DT_NODE_LABEL = "dtsh.dt.node_label"
     STYLE_DT_COMPAT_STR = "dtsh.dt.compat_str"
     STYLE_DT_BINDING_COMPAT = "dtsh.dt.binding_compat"
@@ -82,32 +78,14 @@
     STYLE_DT_ORDINAL = "dtsh.dt.dep_ordinal"
     STYLE_DT_DEP_ON = "dtsh.dt.depend_on"
     STYLE_DT_DEP_FAILED = "dtsh.dt.depend_failed"
     STYLE_DT_REQ_BY = "dtsh.dt.required_by"
     STYLE_DT_VENDOR_NAME = "dtsh.dt.vendor_name"
     STYLE_DT_VENDOR_PREFIX = "dtsh.dt.vendor_prefix"
 
-    STYLE_DT_PROPERTY = "dtsh.dt.property"
-    STYLE_DTVALUE_BOOL = "dtsh.dtvalue.bool"
-    STYLE_DTVALUE_TRUE = "dtsh.dtvalue.true"
-    STYLE_DTVALUE_FALSE = "dtsh.dtvalue.false"
-    STYLE_DTVALUE_INT = "dtsh.dtvalue.int"
-    STYLE_DTVALUE_INT_ARRAY = "dtsh.dtvalue.int_array"
-    STYLE_DTVALUE_STR = "dtsh.dtvalue.string"
-    STYLE_DTVALUE_UINT8 = "dtsh.dtvalue.uint8"
-    STYLE_DTVALUE_PHANDLE = "dtsh.dtvalue.phandle"
-    STYLE_DTVALUE_PHANDLE_DATA = "dtsh.dtvalue.phandle_data"
-
-    STYLE_YAML_BINDING = "dtsh.yaml.binding"
-    STYLE_YAML_INCLUDE = "dtsh.yaml.include"
-    STYLE_DTS_FILE = "dtsh.dts"
-
-    STYLE_FORM_LABEL = "dtsh.form.label"
-    STYLE_FORM_DEFAULT = "dtsh.form.default"
-
     class Error(BaseException):
         """Error loading styles file."""
 
     @classmethod
     def getinstance(cls) -> "DTShTheme":
         """Access the rich styles configuration instance."""
         return _dtshtheme
@@ -129,57 +107,39 @@
         Args:
             path: Path to theme file,
               or None for default theme initialization.
         """
         self._styles = {}
 
         if path:
-            # If explicitly specified, load only this one: fault if invalid.
-            self.load_theme_file(path, fail_early=True)
+            # If explicitly specified, load only this one.
+            self.load_theme_file(path)
         else:
-            # Load defaults from bundled styles file
-            # (fault if invalid, should not happen).
+            # Load defaults from bundled configuration file.
             path = os.path.join(os.path.dirname(__file__), "theme.ini")
-            self.load_theme_file(path, fail_early=True)
-
-            # Load user's theme file if any,
-            # don't fault if unreadable or invalid.
+            self.load_theme_file(path)
+            # Load user's theme file if any.
             path = _dtshconf.get_user_file("theme.ini")
             if path and os.path.isfile(path):
-                self.load_theme_file(path, fail_early=False)
+                self.load_theme_file(path)
 
     @property
     def styles(self) -> Mapping[str, Style]:
         """The theme's rich styles."""
         return self._styles
 
-    def load_theme_file(self, path: str, fail_early: bool = True) -> None:
+    def load_theme_file(self, path: str) -> None:
         """Load a rich styles file.
 
         Args:
             path: Path to a styles file.
-            fail_early: If set, fault when we can't open the file for reading,
-              or its content is invalid. This is the default.
 
         Raises:
-            DTShTheme.Error: Failed to load styles file.
+            DTShTheme.Error: Failed to styles file.
         """
         try:
             self._styles.update(Theme.read(path, encoding="utf-8").styles)
-        except (
-            OSError,
-            StyleError,
-            StyleSyntaxError,
-            configparser.Error,
-        ) as e:
-            if isinstance(e, OSError):
-                msg = e.strerror
-            elif isinstance(e, configparser.Error):
-                msg = e.message
-            else:
-                msg = str(e)
-            if fail_early:
-                raise DTShTheme.Error(msg) from e
-            print(f"Failed to load theme file: {msg}", file=sys.stderr)
+        except (OSError, StyleError, StyleSyntaxError) as e:
+            raise DTShTheme.Error(str(e)) from e
 
 
 _dtshtheme = DTShTheme()
```

### Comparing `dtsh-0.2.2/src/dtsh/rich/tui.py` & `dtsh-0.2rc1/src/dtsh/rich/tui.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/rl.py` & `dtsh-0.2rc1/src/dtsh/rl.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/src/dtsh/session.py` & `dtsh-0.2rc1/src/dtsh/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # Copyright (c) 2023 Christophe Dufaza <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-"""Base devicetree shell session.
+"""Base interactive devicetree shell session.
 
-A session binds a shell and I/O streams, then enters a loop:
-- read command lines from input stream
-- execute shell commands with the appropriate output stream
-- exit on EOF or "quit"
+A session binds a devicetree shell and a VT to run an interactive loop.
 """
 
 from types import FrameType
 from typing import Any, Optional, Sequence, List
 
-import errno
 import signal
 import sys
 
 from devicetree import edtlib
 
 from dtsh.model import DTModel
 from dtsh.rl import DTShReadline
@@ -36,23 +32,33 @@
 from dtsh.builtins.pwd import DTShBuiltinPwd
 from dtsh.builtins.cd import DTShBuiltinCd
 from dtsh.builtins.ls import DTShBuiltinLs
 from dtsh.builtins.tree import DTShBuiltinTree
 from dtsh.builtins.find import DTShBuiltinFind
 from dtsh.builtins.alias import DTShBuiltinAlias
 from dtsh.builtins.chosen import DTShBuiltinChosen
-from dtsh.builtins.cat import DTShBuiltinCat
-from dtsh.builtins.board import DTShBuiltinBoard
 
 
 _dtshconf: DTShConfig = DTShConfig.getinstance()
 
 
 class DTShSession:
-    """Base for devicetree shell sessions."""
+    """Base for interactive devicetree shell sessions.
+
+    A session binds a devicetree shell and a VT to run
+    an interactive loop until the user quits or EOF (aka CTRL-D).
+
+    The session is also responsible for:
+
+    - initializing the auto-completion support (depends on GNU readline)
+    - handling command output redirection streams
+
+    The run loop will trigger events which handlers may be overridden
+    by derived (rich) sessions.
+    """
 
     _dtsh: DTSh
     _vt: DTShVT
 
     _rl: DTShReadline
     _autocomp: DTShAutocomp
 
@@ -65,36 +71,48 @@
         """Create a new devicetree shell session.
 
         Args:
             dts_path: Path to the Devicetree source to open the session with.
             binding_dirs: List of directories to search for
               the YAML binding files this Devicetree depends on.
 
-        Returns:
-            An initialized session.
-
         Raises:
             DTShError: Typically DTS file not found or invalid,
               or missing or invalid bindings.
         """
-        dt = cls._create_dtmodel(dts_path, binding_dirs)
-        sh = cls._create_dtsh(dt)
+        try:
+            dt = DTModel.create(dts_path, binding_dirs)
+        except (OSError, edtlib.EDTError) as e:
+            raise DTShError(f"DTS error: {e}") from e
+
+        sh = DTSh(
+            dt,
+            [
+                DTShBuiltinPwd(),
+                DTShBuiltinCd(),
+                DTShBuiltinLs(),
+                DTShBuiltinTree(),
+                DTShBuiltinFind(),
+                DTShBuiltinAlias(),
+                DTShBuiltinChosen(),
+            ],
+        )
         return cls(sh)
 
     def __init__(
         self,
         sh: DTSh,
         vt: Optional[DTShVT] = None,
         autocomp: Optional[DTShAutocomp] = None,
     ) -> None:
         """Initialize a session.
 
         Will initialize the VT and auto-completion support.
 
-        Won't start the loop until run().
+        Won't start the interactive loop.
 
         Args:
             sh: The session's shell.
             vt: The session's VT. Defaults to DTShVT.
             autocomp: GNU readline callbacks for completion and matches display.
               Defaults to DTShAutocomp().
         """
@@ -106,49 +124,59 @@
 
         self._rl = DTShReadline(
             self._vt,
             self._autocomp.complete,
             self._autocomp.display,
         )
 
-    def run(
-        self, interactive: bool = True
-    ) -> None:  # pylint: disable=too-many-branches
-        """Enter session loop.
+    def run(self) -> None:  # pylint: disable=too-many-branches
+        """Enter interactive loop.
 
-        If interactive, first run the preamble hook:
-        - handle SIGINT to work-around TTY issues
+        This will:
+        - disable the SIGINT signal
         - clear VT and print banner
-
-        Enter actual loop, until EOF or "quit" command:
-        - read next command line from input stream
-        - parse and execute command line, with the session's VT
-          or a redirection file as output stream
-
-        Eventually run the pre-exit hook if interactive,
-        and exit the devicetree shell.
+        - repeat until user quits or EOF (e.g. CTRL-D):
+            - run pre_input_hook()
+            - read a command line from VT
+            - parse the command line
+            - setup command output redirection if asked to
+            - execute the command string
+            - dispatch the event to its handler if an error occurs
+            - if the command output was redirected,
+              explicitly flush the redirection stream
         """
-        if interactive:
-            self._preamble_hook()
+        # closing() the session when the pager is active breaks the TTY.
+        # As a work-around, we ignore SIGINT.
+        signal.signal(signal.SIGINT, self._sig_handler)
+
+        self._vt.clear()
+        self.preamble_hook()
 
         # Session error state.
         self._last_err = None
 
         while True:
+            self.pre_input_hook()
+
             cmdline: Optional[str] = None
             try:
-                cmdline = self._vt.readline(self.mk_prompt())
+                cmdline = self._vt.readline(
+                    _dtshconf.prompt_alt
+                    if self._last_err
+                    else _dtshconf.prompt_default
+                )
             except EOFError:
+                self._vt.write()
                 # Exit DTSh on EOF.
-                self.close(interactive)
+                self.close()
 
             if cmdline:
                 if cmdline.strip() in ["q", "quit", "exit"]:
                     # Exit DTSh process.
-                    self.close(interactive)
+                    self.close()
 
                 cmd: DTShCommand
                 argv: List[str]
                 redir2: Optional[str]
                 try:
                     # Parse command line into the command to execute,
                     # its arguments, and the redirection directive, if any.
@@ -195,30 +223,32 @@
                             # Flush the file the command output
                             # was redirected to, even on error.
                             # Note that the shell (error) messages themselves
                             # are always written to the session VT,
                             # and never redirected.
                             out.flush()
 
-            # NOTE: Be sure to set prompt_sparse in preferences
-            # when running batch sessions.
-            if _dtshconf.prompt_sparse and self._vt.is_tty():
+            if _dtshconf.prompt_sparse:
                 self._vt.write()
 
-    def close(self, interactive: bool) -> None:
-        """Terminate session.
+    def close(self, status: int = 0) -> None:
+        """Terminate interactive session.
 
-        Will first run the pre-exit hook if interactive,
-        saving commands history, and exit the session's process.
+        This will:
+        - run pre_exit_hook()
+        - save readline history file, if supported
+        - close the session's VT
+        - exit the dtsh process
 
-        Exits with status code -EINVAL if the last command line failed.
+        Args:
+            status: exit status, defaults to 0, aka "no error".
         """
-        if interactive:
-            self._pre_exit_hook()
-        sys.exit(-errno.EINVAL if self._last_err else 0)
+        self.pre_exit_hook(status)
+        self._rl.save_history()
+        sys.exit(status)
 
     def open_redir2(self, redir2: str) -> DTShOutput:
         """Open DTSh redirection output stream.
 
         Args:
             redir2: Command line redirection.
 
@@ -227,14 +257,23 @@
 
         Raises:
             DTShRedirect.Error: Failed to setup redirection output.
         """
         redirect = DTShRedirect(redir2)
         return DTShOutputFile(redirect.path, redirect.append)
 
+    def preamble_hook(self) -> None:
+        """Session's preamble, aka banner."""
+        self._vt.write("dtsh: shell-like interface with Zephyr Devicetree")
+        self._vt.write()
+
+    def pre_input_hook(self) -> None:
+        """Hook called before the session prompts for the next command line."""
+        self._vt.write(self._dtsh.pwd)
+
     def on_cmd_help(self, cmd: DTShCommand) -> None:
         """Called when the user's asked for a command's help.
 
         Args:
             cmd: The command to help with.
         """
         self._vt.write(f"usage: {cmd.synopsis}")
@@ -269,87 +308,24 @@
         """Called when failed to setup redirection stream.
 
         Args:
             e: The error event.
         """
         self._vt.write(f"dtsh: {e}")
 
-    def mk_prompt(self) -> Sequence[Any]:
-        """Make multiple-line prompt to use for the next command.
+    def pre_exit_hook(self, status: int) -> None:
+        """Hook called when the user terminates the session.
 
-        Returns:
-            A valid multiple-line prompt: optional state lines of any type,
-            followed by the actual ANSI prompt.
-        """
-        return [
-            self._dtsh.pwd,
-            _dtshconf.prompt_alt
-            if self._last_err
-            else _dtshconf.prompt_default,
-        ]
-
-    def mk_prologue(self) -> Sequence[Any]:
-        """Shell prologue.
-
-        Returns:
-            The shell multiple-line banner.
-        """
-        return ["dtsh: A Devicetree Shell"]
-
-    def mk_epilogue(self) -> Sequence[Any]:
-        """Shell epilogue.
-
-        Returns:
-            A goodbye message.
+        Args:
+            status: The exit status.
         """
-        return ["bye."]
-
-    def _preamble_hook(self) -> None:
-        # Hook called when an interactive session starts.
-
-        # Closing with SIGINT when the pager is active breaks the TTY.
-        # As a work-around, we ignore SIGINT in interactive sessions.
-        signal.signal(signal.SIGINT, self._sig_handler)
-
-        self._vt.clear()
-        for line in self.mk_prologue():
-            self._vt.write(line)
-        self._vt.write()
-
-    def _pre_exit_hook(self) -> None:
-        # Hook called when an interactive session terminates.
-        self._rl.save_history()
-        for line in self.mk_epilogue():
-            self._vt.write(line)
-
-    @classmethod
-    def _create_dtmodel(
-        cls, dts_path: str, binding_dirs: Optional[Sequence[str]]
-    ) -> DTModel:
-        try:
-            return DTModel.create(dts_path, binding_dirs)
-        except (OSError, edtlib.EDTError) as e:
-            raise DTShError(f"DTS error: {e}") from e
-
-    @classmethod
-    def _create_dtsh(cls, dt: DTModel) -> DTSh:
-        return DTSh(
-            dt,
-            [
-                DTShBuiltinPwd(),
-                DTShBuiltinCd(),
-                DTShBuiltinLs(),
-                DTShBuiltinTree(),
-                DTShBuiltinFind(),
-                DTShBuiltinAlias(),
-                DTShBuiltinChosen(),
-                DTShBuiltinCat(),
-                DTShBuiltinBoard(),
-            ],
-        )
+        if status:
+            self._vt.write(f"bye ({status}).")
+        else:
+            self._vt.write("bye.")
 
     def _sig_handler(self, signum: int, frame: Optional[FrameType]) -> Any:
         # closing() the session when the pager is active breaks the TTY.
         # As a work-around, we ignore SIGINT.
         del frame  # Unused.
         if signum == signal.SIGINT:
             pass
```

### Comparing `dtsh-0.2.2/src/dtsh/shell.py` & `dtsh-0.2rc1/src/dtsh/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,15 +724,15 @@
 
     - hierarchical file-system metaphor: view the device tree from a
       current working branch, support for relative paths and path references
     - built-in commands to walk, search and describe the devicetree
     - parse command lines and execute command strings
     """
 
-    VERSION_STRING = "0.2.2"
+    VERSION_STRING = "0.2rc1"
     """The devicetree shell version string.
 
     This version identifies:
 
     - the Zephyr West command syntax and arguments
     - the devicetree shell command line syntax
     - the defined built-in devicetree shell commands,
```

### Comparing `dtsh-0.2.2/src/dtsh.egg-info/SOURCES.txt` & `dtsh-0.2rc1/src/dtsh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 src/dtsh.egg-info/SOURCES.txt
 src/dtsh.egg-info/dependency_links.txt
 src/dtsh.egg-info/entry_points.txt
 src/dtsh.egg-info/requires.txt
 src/dtsh.egg-info/top_level.txt
 src/dtsh/builtins/__init__.py
 src/dtsh/builtins/alias.py
-src/dtsh/builtins/board.py
-src/dtsh/builtins/cat.py
 src/dtsh/builtins/cd.py
 src/dtsh/builtins/chosen.py
 src/dtsh/builtins/find.py
 src/dtsh/builtins/ls.py
 src/dtsh/builtins/pwd.py
 src/dtsh/builtins/tree.py
 src/dtsh/rich/__init__.py
@@ -48,15 +46,14 @@
 src/dtsh/rich/svg.py
 src/dtsh/rich/text.py
 src/dtsh/rich/theme.ini
 src/dtsh/rich/theme.py
 src/dtsh/rich/tui.py
 tests/test_dtsh_autocomp.py
 tests/test_dtsh_builtin_alias.py
-tests/test_dtsh_builtin_cat.py
 tests/test_dtsh_builtin_cd.py
 tests/test_dtsh_builtin_chosen.py
 tests/test_dtsh_builtin_find.py
 tests/test_dtsh_builtin_ls.py
 tests/test_dtsh_builtin_pwd.py
 tests/test_dtsh_builtin_tree.py
 tests/test_dtsh_config.py
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_autocomp.py` & `dtsh-0.2rc1/tests/test_dtsh_autocomp.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,28 +438,7 @@
             "a.txt",
             "ab.txt",
         ] == [state.rlstr for state in autocomp.complete("", "ls > ", 5, 5)]
 
         # Command line: " ls >|"
         # Expects: missing space after ">".
         assert [] == autocomp.complete("", "ls >", 3, 3)
-
-
-def test_dtsh_autocomp_complete_dtpathx() -> None:
-    sh = DTSh(DTShTests.get_sample_dtmodel(), [])
-
-    # Should behave like complete_dtpath() when no "$" separator.
-    assert sorted(
-        [RlStateDTPath(node.name, node) for node in sh.dt.root.children]
-    ) == DTShAutocomp.complete_dtpathx("", sh)
-
-    assert [] == DTShAutocomp.complete_dtpathx("not-a-node$", sh)
-    assert [] == DTShAutocomp.complete_dtpathx("soc$not-a-property", sh)
-
-    assert sorted(
-        [f"${prop.name}" for prop in sh.dt.root.all_dtproperties()]
-    ) == [state.rlstr for state in DTShAutocomp.complete_dtpathx("$", sh)]
-
-    dt_power = sh.node_at("&power")
-    assert sorted(
-        [f"&power${prop.name}" for prop in dt_power.all_dtproperties()]
-    ) == [state.rlstr for state in DTShAutocomp.complete_dtpathx("&power$", sh)]
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_builtin_alias.py` & `dtsh-0.2rc1/tests/test_dtsh_builtin_alias.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_builtin_cat.py` & `dtsh-0.2rc1/tests/test_dtsh_builtin_cd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # Copyright (c) 2023 Christophe Dufaza <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-"""Unit tests for the dtsh.builtins.cat module."""
+"""Unit tests for the dtsh.builtins.cd module."""
 
 # Relax pylint a bit for unit tests.
 # pylint: disable=missing-function-docstring
 
 
 from dtsh.io import DTShOutput
 from dtsh.shell import DTSh
-from dtsh.builtins.cat import DTShBuiltinCat
+from dtsh.builtins.cd import DTShBuiltinCd
 
 from .dtsh_uthelpers import DTShTests
 
 _stdout = DTShOutput()
 
 
-def test_dtsh_builtin_cat() -> None:
-    cmd = DTShBuiltinCat()
-    DTShTests.check_cmd_meta(cmd, "cat")
+def test_dtsh_builtin_cd() -> None:
+    cmd = DTShBuiltinCd()
+    DTShTests.check_cmd_meta(cmd, "cd")
 
 
-def test_dtsh_builtin_cat_flags() -> None:
-    cmd = DTShBuiltinCat()
+def test_dtsh_builtin_cd_param() -> None:
+    cmd = DTShBuiltinCd()
     sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
-    DTShTests.check_cmd_flags(cmd, sh, _stdout)
+    DTShTests.check_cmd_param_dtpath(cmd, sh, _stdout)
 
 
-def test_dtsh_builtin_cat_execute() -> None:
-    out = DTShOutput()
-    cmd = DTShBuiltinCat()
+def test_dtsh_builtin_cd_execute() -> None:
+    cmd = DTShBuiltinCd()
     sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
 
-    DTShTests.check_cmd_execute(cmd, sh, out)
+    DTShTests.check_cmd_execute(cmd, sh, _stdout)
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_builtin_cd.py` & `dtsh-0.2rc1/tests/test_dtsh_builtin_chosen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 # Copyright (c) 2023 Christophe Dufaza <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-"""Unit tests for the dtsh.builtins.cd module."""
+"""Unit tests for the dtsh.builtins.chosen module."""
 
 # Relax pylint a bit for unit tests.
 # pylint: disable=missing-function-docstring
 
 
 from dtsh.io import DTShOutput
 from dtsh.shell import DTSh
-from dtsh.builtins.cd import DTShBuiltinCd
+from dtsh.builtins.chosen import DTShBuiltinChosen
 
 from .dtsh_uthelpers import DTShTests
 
 _stdout = DTShOutput()
 
 
-def test_dtsh_builtin_cd() -> None:
-    cmd = DTShBuiltinCd()
-    DTShTests.check_cmd_meta(cmd, "cd")
+def test_dtsh_builtin_chosen() -> None:
+    cmd = DTShBuiltinChosen()
+    DTShTests.check_cmd_meta(cmd, "chosen")
 
 
-def test_dtsh_builtin_cd_param() -> None:
-    cmd = DTShBuiltinCd()
+def test_dtsh_builtin_chosen_flags() -> None:
+    cmd = DTShBuiltinChosen()
     sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
-    DTShTests.check_cmd_param_dtpath(cmd, sh, _stdout)
+    DTShTests.check_cmd_flags(cmd, sh, _stdout)
 
 
-def test_dtsh_builtin_cd_execute() -> None:
-    cmd = DTShBuiltinCd()
+def test_dtsh_builtin_chosen_arg_longfmt() -> None:
+    cmd = DTShBuiltinChosen()
     sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
+    DTShTests.check_cmd_arg_longfmt(cmd, sh, _stdout)
+
+
+def test_dtsh_builtin_chosen_param() -> None:
+    cmd = DTShBuiltinChosen()
+    sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
+    DTShTests.check_cmd_param_chosen(cmd, sh, _stdout)
+
+
+def test_dtsh_builtin_chosen_execute() -> None:
+    dtmodel = DTShTests.get_sample_dtmodel()
+    cmd = DTShBuiltinChosen()
+    sh = DTSh(dtmodel, [cmd])
 
     DTShTests.check_cmd_execute(cmd, sh, _stdout)
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_builtin_chosen.py` & `dtsh-0.2rc1/tests/test_dtsh_builtin_ls.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,60 @@
 # Copyright (c) 2023 Christophe Dufaza <chris@openmarl.org>
 #
 # SPDX-License-Identifier: Apache-2.0
 
-"""Unit tests for the dtsh.builtins.chosen module."""
+"""Unit tests for the dtsh.builtins.ls module."""
 
 # Relax pylint a bit for unit tests.
 # pylint: disable=missing-function-docstring
 
 
 from dtsh.io import DTShOutput
 from dtsh.shell import DTSh
-from dtsh.builtins.chosen import DTShBuiltinChosen
+from dtsh.builtins.ls import DTShBuiltinLs
 
 from .dtsh_uthelpers import DTShTests
 
 _stdout = DTShOutput()
 
 
-def test_dtsh_builtin_chosen() -> None:
-    cmd = DTShBuiltinChosen()
-    DTShTests.check_cmd_meta(cmd, "chosen")
+def test_dtsh_builtin_ls() -> None:
+    cmd = DTShBuiltinLs()
+    DTShTests.check_cmd_meta(cmd, "ls")
 
 
-def test_dtsh_builtin_chosen_flags() -> None:
-    cmd = DTShBuiltinChosen()
+def test_dtsh_builtin_ls_flags() -> None:
+    cmd = DTShBuiltinLs()
     sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
     DTShTests.check_cmd_flags(cmd, sh, _stdout)
 
 
-def test_dtsh_builtin_chosen_arg_longfmt() -> None:
-    cmd = DTShBuiltinChosen()
+def test_dtsh_builtin_ls_arg_orderby() -> None:
+    cmd = DTShBuiltinLs()
+    sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
+    DTShTests.check_cmd_arg_order_by(cmd, sh, _stdout)
+
+
+def test_dtsh_builtin_ls_arg_longfmt() -> None:
+    cmd = DTShBuiltinLs()
     sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
     DTShTests.check_cmd_arg_longfmt(cmd, sh, _stdout)
 
 
-def test_dtsh_builtin_chosen_param() -> None:
-    cmd = DTShBuiltinChosen()
+def test_dtsh_builtin_ls_arg_fixed_depth() -> None:
+    cmd = DTShBuiltinLs()
     sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
-    DTShTests.check_cmd_param_chosen(cmd, sh, _stdout)
+    DTShTests.check_cmd_arg_fixed_depth(cmd, sh, _stdout)
 
 
-def test_dtsh_builtin_chosen_execute() -> None:
-    dtmodel = DTShTests.get_sample_dtmodel()
-    cmd = DTShBuiltinChosen()
-    sh = DTSh(dtmodel, [cmd])
+def test_dtsh_builtin_ls_param() -> None:
+    cmd = DTShBuiltinLs()
+    sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
+    DTShTests.check_cmd_param_dtpaths(cmd, sh, _stdout)
+
+
+def test_dtsh_builtin_ls_execute() -> None:
+    out = DTShOutput()
+    cmd = DTShBuiltinLs()
+    sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
 
-    DTShTests.check_cmd_execute(cmd, sh, _stdout)
+    DTShTests.check_cmd_execute(cmd, sh, out)
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_builtin_find.py` & `dtsh-0.2rc1/tests/test_dtsh_builtin_find.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_builtin_pwd.py` & `dtsh-0.2rc1/tests/test_dtsh_builtin_pwd.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_builtin_tree.py` & `dtsh-0.2rc1/tests/test_dtsh_builtin_tree.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_config.py` & `dtsh-0.2rc1/tests/test_dtsh_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,17 +24,14 @@
     assert cfg.getstr("test.string") == "a string"
     assert cfg.getstr("not.an.option") == ""
     # 2. Load user's specific configuration (overrides defaults).
     cfg.load_ini_file(DTShTests.get_resource_path("ini", "override.ini"))
     assert cfg.getstr("test.string") == "overridden"
     assert cfg.getstr("test.new") == "new"
 
-    # Should not fault.
-    cfg.load_ini_file("not/a/config/file.ini", fail_early=False)
-
     with pytest.raises(DTShConfig.Error):
         cfg.load_ini_file("not/a/config/file.ini")
 
 
 def test_dtshconfig_getbool() -> None:
     cfg = DTShConfig(DTShTests.get_resource_path("ini", "test.ini"))
 
@@ -100,15 +97,14 @@
     assert 255 == cfg_defaults.pref_redir2_maxwidth
     assert not cfg_defaults.pref_always_longfmt
     assert cfg_defaults.pref_sizes_si
     assert not cfg_defaults.pref_hex_upper
     assert cfg_defaults.pref_fs_hide_dotted
     assert cfg_defaults.pref_fs_no_spaces
     assert cfg_defaults.pref_fs_no_overwrite
-    assert not cfg_defaults.pref_fs_no_overwrite_strict
     assert ActionableType.LINK == cfg_defaults.pref_actionable_type
 
     # List views.
     assert cfg_defaults.pref_list_headers
     assert not cfg_defaults.pref_list_placeholder
     assert cfg_defaults.pref_list_fmt
     assert ActionableType.LINK == ActionableType(
@@ -134,20 +130,7 @@
     assert "html" == cfg_defaults.pref_html_theme
     assert "Courier New" == cfg_defaults.pref_html_font_family
 
     # SVG.
     assert "svg" == cfg_defaults.pref_svg_theme
     assert "Courier New" == cfg_defaults.pref_svg_font_family
     assert 0.6 == cfg_defaults.pref_svg_font_ratio
-
-    # YAML.
-    assert "monokai" == cfg_defaults.pref_yaml_theme
-    assert cfg_defaults.pref_yaml_expand
-    assert ActionableType.ALT == cfg_defaults.pref_yaml_actionable_type
-
-    # DTS.
-    assert "monokai" == cfg_defaults.pref_dts_theme
-    assert ActionableType.ALT == cfg_defaults.pref_dts_actionable_type
-
-    # Forms.
-    assert cfg_defaults.pref_form_show_all
-    assert ActionableType.LINK == cfg_defaults.pref_form_actionable_type
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_dts.py` & `dtsh-0.2rc1/tests/test_dtsh_dts.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,24 +90,19 @@
             # Possibly set only when a CMake cache is available.
             assert dts.board_dir is None
             assert dts.board is None
             assert [] == dts.shield_dirs
             assert dts.fw_name is None
             assert dts.fw_version is None
 
-            # Default minimal bindings search path:
-            # - derived from app src dir, always exists
-            expect_dirs = [os.path.join(app_src_dir, "dts", "bindings")]
-            # - though cleared in environment, ZEPHYR_BASE may be derived
-            # from __file__ when distributed with Zephyr
-            if dts.zephyr_base:
-                expect_dirs.append(
-                    os.path.join(dts.zephyr_base, "dts", "bindings")
-                )
-            assert expect_dirs == dts.bindings_search_path
+            # Default minimal bindings search path.
+            assert [
+                os.path.join(app_src_dir, "dts", "bindings"),
+                os.path.join(dts.zephyr_base or "?", "dts", "bindings"),
+            ] == dts.bindings_search_path
 
 
 def test_dts_init_from_os_env() -> None:
     # Use case:
     # - CMake cache: not available
     # - OS environment: ZEPHYR_BASE, ZEPHYR_TOOLCHAIN_VARIANT
     tmpenv = {
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_io.py` & `dtsh-0.2rc1/tests/test_dtsh_io.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_model.py` & `dtsh-0.2rc1/tests/test_dtsh_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -975,61 +975,7 @@
     )
 
     # Logical negation.
     assert not dtmodel.find(DTNodeCriteria(negative_chain=True))
     assert not dtmodel.find(
         DTNodeCriteria([CriterionMatchAll()], negative_chain=True)
     )
-
-
-def test_dtnode_properties() -> None:
-    dtmodel = DTShTests.get_sample_dtmodel()
-    dt_qspi = dtmodel["/soc/qspi@40029000"]
-
-    assert dt_qspi.has_dtproperty("interrupts")
-    dtprop_irqs = dt_qspi.dtproperty("interrupts")
-    assert dtprop_irqs
-    assert "array" == dtprop_irqs.dttype
-    assert isinstance(dtprop_irqs.value, list)
-    assert [0x29, 0x1] == dtprop_irqs.value
-
-    assert dt_qspi.has_dtproperty("pinctrl-0")
-    dtprop_pinctrl0 = dt_qspi.dtproperty("pinctrl-0")
-    assert dtprop_pinctrl0
-    # NOTE: why isn't this a single phandle ?
-    assert "phandles" == dtprop_pinctrl0.dttype
-    assert isinstance(dtprop_pinctrl0.value, list)
-
-    assert dt_qspi.has_dtproperty("pinctrl-names")
-    dtprop_pinctrl_names = dt_qspi.dtproperty("pinctrl-names")
-    assert dtprop_pinctrl_names
-    assert "string-array" == dtprop_pinctrl_names.dttype
-    assert ["default", "sleep"] == dtprop_pinctrl_names.value
-
-    dt_mx25r64 = dt_qspi.get_child("mx25r6435f@0")
-    assert dt_mx25r64.has_dtproperty("jedec-id")
-    dtprop_jedec = dt_mx25r64.dtproperty("jedec-id")
-    assert dtprop_jedec
-    assert "uint8-array" == dtprop_jedec.dttype
-    assert isinstance(dtprop_jedec.value, bytes)
-    assert bytes([0xC2, 0x28, 0x17]) == dtprop_jedec.value
-
-    assert dt_mx25r64.has_dtproperty("has-dpd")
-    dtprop_dpd = dt_mx25r64.dtproperty("has-dpd")
-    assert dtprop_dpd
-    assert "boolean" == dtprop_dpd.dttype
-    assert isinstance(dtprop_dpd.value, bool)
-    assert dtprop_dpd.value is True
-
-    assert not dt_qspi.has_dtproperty("not-a-property")
-    with pytest.raises(KeyError):
-        # Properties MUST exist.
-        dt_qspi.dtproperty("not-a-property")
-
-    assert [
-        # Although these are properties of the root node in the DTS,
-        # they do not actually appear as properties via the edtlib API:
-        # - "#address-cells",
-        # - "#size-cells",
-        # - "model",
-        "compatible",
-    ] == [prop.name for prop in dtmodel.root.all_dtproperties()]
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_modelutils.py` & `dtsh-0.2rc1/tests/test_dtsh_modelutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
 # Relax pylint a bit for unit tests.
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-branches
 # pylint: disable=missing-function-docstring
 
 
-from typing import cast, List, Tuple, Type
+from typing import List, Tuple, Type
 import operator
 import re
 import sys
 
 import pytest
 
-from dtsh.model import DTNode, DTNodePHandleData, DTNodeSorter
+from dtsh.model import DTNode, DTNodeSorter
 from dtsh.modelutils import (
-    DTSUtil,
     # Text-based criteria.
     DTNodeTextCriterion,
     DTNodeWithPath,
     DTNodeWithName,
     DTNodeWithUnitName,
     DTNodeWithCompatible,
     DTNodeWithBinding,
@@ -1106,123 +1105,7 @@
         dt_flash0,
         dt_partitions,
         dt_partition0,
         dt_cpus,
         dt_cpu0,
         dt_cpu_itm,
     ] == list(walkable.walk(order_by=order_by, reverse=True))
-
-
-def test_dtsutil_mk_boolean() -> None:
-    assert "true" == DTSUtil.mk_boolean(True)
-    assert "false" == DTSUtil.mk_boolean(False)
-
-
-def test_dtsutil_mk_int() -> None:
-    assert "0x01" == DTSUtil.mk_int(1, as_cell=False)
-    assert "< 0x01 >" == DTSUtil.mk_int(1, as_cell=True)
-    assert "< 0xff >" == DTSUtil.mk_int(255, as_cell=True)
-    assert "0x0100" == DTSUtil.mk_int(256, as_cell=False)
-
-
-def test_dtsutil_mk_string() -> None:
-    assert '"str"' == DTSUtil.mk_string("str")
-
-
-def test_dtsutil_mk_bytes() -> None:
-    assert "[ 01 10 FF ]" == DTSUtil.mk_bytes(bytes([0x01, 0x010, 0xFF]))
-    assert "[  ]" == DTSUtil.mk_bytes(bytes([]))
-
-
-def test_dtsutil_mk_phandle() -> None:
-    dtmodel = DTShTests.get_sample_dtmodel()
-    dt_i2c = dtmodel["/soc/i2c@40003000"]
-    # Should be the first DT label when available.
-    assert "&i2c0" == DTSUtil.mk_phandle(dt_i2c, as_cell=False)
-    assert "< &i2c0 >" == DTSUtil.mk_phandle(dt_i2c, as_cell=True)
-    # Otherwise, the node's path (very few nodes don't have at least one label).
-    assert "/chosen" == DTSUtil.mk_phandle(dtmodel["/chosen"], as_cell=False)
-
-
-def test_dtsutil_mk_array() -> None:
-    assert "< 0x01 >" == DTSUtil.mk_array([1])
-    assert "< 0x01 0x0100 >" == DTSUtil.mk_array([1, 256])
-    assert "< 0x01 0x0100 >" == DTSUtil.mk_array([1, 256], as_cell=True)
-
-
-def test_dtsutil_mk_string_array() -> None:
-    assert '"str1", "str2"' == DTSUtil.mk_string_array(["str1", "str2"])
-
-
-def test_dtsutil_mk_phandles() -> None:
-    dtmodel = DTShTests.get_sample_dtmodel()
-    dt_i2c = dtmodel["/soc/i2c@40003000"]
-    dt_timer = dtmodel["/soc/timer@40008000"]
-    assert "< &i2c0 &timer0 >" == DTSUtil.mk_phandles([dt_i2c, dt_timer])
-
-
-def test_dtsutil_mk_phandle_array() -> None:
-    dtmodel = DTShTests.get_sample_dtmodel()
-    dt_led0 = dtmodel["/leds/led_0"]
-    prop_gpios = dt_led0.dtproperty("gpios")
-    assert "< &gpio0 0x0d 0x01 >" == DTSUtil.mk_phandle_array(
-        cast(List[DTNodePHandleData], prop_gpios.value)
-    )
-
-
-def test_dtsutil_mk_property_value() -> None:
-    dt = DTShTests.get_sample_dtmodel()
-
-    # bool:
-    prop = dt["/soc/pwm@4001c000"].dtproperty("center-aligned")
-    assert "boolean" == prop.dttype
-    assert isinstance(prop.value, bool)
-    assert prop.value is False
-    assert "false" == DTSUtil.mk_property_value(prop)
-
-    # int:
-    prop = dt["/soc/timer@40008000"].dtproperty("cc-num")
-    assert "int" == prop.dttype
-    assert isinstance(prop.value, int)
-    assert 0x4 == prop.value
-    assert "< 0x04 >" == DTSUtil.mk_property_value(prop)
-
-    # array:
-    prop = dt["/soc/pwm@4001c000"].dtproperty("interrupts")
-    assert "array" == prop.dttype
-    assert isinstance(prop.value, list)
-    assert [0x1C, 0x1] == prop.value
-    assert "< 0x1c 0x01 >" == DTSUtil.mk_property_value(prop)
-
-    # string:
-    prop = dt["/soc/clock@40000000"].dtproperty("status")
-    assert "string" == prop.dttype
-    assert isinstance(prop.value, str)
-    assert "okay" == prop.value
-    assert '"okay"' == DTSUtil.mk_property_value(prop)
-
-    # string-array:
-    prop = dt["/soc/i2c@40003000"].dtproperty("pinctrl-names")
-    assert "string-array" == prop.dttype
-    assert isinstance(prop.value, list)
-    assert ["default", "sleep"] == prop.value
-    assert '"default", "sleep"' == DTSUtil.mk_property_value(prop)
-
-    # bytes:
-    prop = dt["/soc/qspi@40029000/mx25r6435f@0"].dtproperty("jedec-id")
-    assert "uint8-array" == prop.dttype
-    assert isinstance(prop.value, bytes)
-    assert bytes([0xC2, 0x28, 0x17]) == prop.value
-    assert "[ C2 28 17 ]" == DTSUtil.mk_property_value(prop)
-
-    # phandle:
-    prop = dt["/sw-pwm"].dtproperty("generator")
-    assert "phandle" == prop.dttype
-    assert isinstance(prop.value, DTNode)
-    assert dt["/soc/timer@40009000"] == prop.value
-    assert "< &timer1 >" == DTSUtil.mk_property_value(prop)
-
-    # phandle-array:
-    prop = dt["/leds/led_0"].dtproperty("gpios")
-    assert "phandle-array" == prop.dttype
-    assert isinstance(prop.value, list)
-    assert "< &gpio0 0x0d 0x01 >" == DTSUtil.mk_property_value(prop)
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_rich_shellutils.py` & `dtsh-0.2rc1/tests/test_dtsh_rich_shellutils.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_rich_svg.py` & `dtsh-0.2rc1/tests/test_dtsh_rich_svg.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_shell.py` & `dtsh-0.2rc1/tests/test_dtsh_shell.py`

 * *Files identical despite different names*

### Comparing `dtsh-0.2.2/tests/test_dtsh_shellutils.py` & `dtsh-0.2rc1/tests/test_dtsh_shellutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 """Unit tests for the dtsh.shellutils module."""
 
 # Relax pylint a bit for unit tests.
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=pointless-statement
 # pylint: disable=too-many-statements
-# pylint: disable=protected-access
+# pylint: disable=too-many-statements
 
 from typing import List, Tuple
 
 import pytest
 
-from dtsh.shell import DTSh, DTShCommand, DTShError, DTShCommandError
+from dtsh.shell import DTSh, DTShCommand, DTShError
 from dtsh.modelutils import (
     # Text-based criteria.
     DTNodeWithPath,
     DTNodeWithName,
     DTNodeWithUnitName,
     DTNodeWithCompatible,
     DTNodeWithBinding,
@@ -67,19 +67,17 @@
     DTShArgIntCriterion,
     DTShArgNodeWithUnitAddr,
     DTShArgNodeWithIrqNumber,
     DTShArgNodeWithIrqPriority,
     DTShArgNodeWithRegAddr,
     DTShArgNodeWithRegSize,
     DTShArgNodeWithBindingDepth,
-    DTShArgNodeWithDepOrd,
     DTShArgOrderBy,
     DTShParamDTPath,
     DTShParamDTPaths,
-    DTShParamDTPathX,
     DTShParamAlias,
     DTShParamChosen,
     DTSH_NODE_ORDER_BY,
     DTSH_ARG_NODE_CRITERIA,
 )
 
 from .dtsh_uthelpers import DTShTests
@@ -161,15 +159,14 @@
     arg_on_attr: List[Tuple[DTShArgIntCriterion, str]] = [
         (DTShArgNodeWithUnitAddr(), "unit_addr"),
         (DTShArgNodeWithIrqNumber(), "interrupts"),
         (DTShArgNodeWithIrqPriority(), "interrupts"),
         (DTShArgNodeWithRegAddr(), "registers"),
         (DTShArgNodeWithRegSize(), "registers"),
         (DTShArgNodeWithBindingDepth(), "binding"),
-        (DTShArgNodeWithDepOrd(), "dep_ordinal"),
     ]
 
     # Check that no one has been forgotten.
     assert len(
         list(
             arg
             for arg in DTSH_ARG_NODE_CRITERIA
@@ -1388,120 +1385,14 @@
     ] == param.expand(cmd, sh)
 
     sh.cd("soc")
     param.parsed(["../leds*"])
     assert [DTSh.PathExpansion("..", [sh.dt["/leds"]])] == param.expand(cmd, sh)
 
 
-def test_dtshparam_dtpathx() -> None:
-    param = DTShParamDTPathX()
-    assert param.brief
-    assert "[XPATH]" == param.usage
-    # Default value.
-    assert not param.is_globexpr()
-    assert "" == param.xpath
-    assert ("", None) == param._xparse()
-
-    # Parameter's state and multiplicity.
-    DTShTests.check_param(param)
-
-    # Won't fault, path resolution is deferred to command execution.
-    param.parsed(["path"])
-    assert not param.is_globexpr()
-    assert "path" == param.xpath
-    assert ("path", None) == param._xparse()
-
-    param.parsed(["path$prop"])
-    assert not param.is_globexpr()
-    assert "path$prop" == param.xpath
-    assert ("path", "prop") == param._xparse()
-
-    param.parsed(["path$prop*"])
-    assert param.is_globexpr()
-    assert "path$prop*" == param.xpath
-    assert ("path", "prop*") == param._xparse()
-
-
-def test_dtshparam_dtpathx_xsplit() -> None:
-    param = DTShParamDTPathX()
-    cmd = DTShCommand("cmd", "", [], param)
-    sh = DTSh(DTShTests.get_sample_dtmodel(), [cmd])
-
-    param.parsed([""])
-    assert (sh.dt.root, None) == param.xsplit(cmd, sh)
-    assert not param.is_globexpr()
-
-    param.parsed(["$compatible"])
-    assert not param.is_globexpr()
-    assert (sh.dt.root, [sh.dt.root.dtproperty("compatible")]) == param.xsplit(
-        cmd, sh
-    )
-
-    param.parsed(["&nvic$reg"])
-    assert not param.is_globexpr()
-    assert (
-        sh.node_at("&nvic"),
-        [sh.node_at("&nvic").dtproperty("reg")],
-    ) == param.xsplit(cmd, sh)
-
-    sh.cd("&nvic")
-    param.parsed(["$reg"])
-    assert (
-        sh.node_at("&nvic"),
-        [sh.node_at("&nvic").dtproperty("reg")],
-    ) == param.xsplit(cmd, sh)
-
-    dt_uart0 = sh.node_at("&uart0")
-    param.parsed(["&uart0$pinctrl*"])
-    assert param.is_globexpr()
-    assert (
-        dt_uart0,
-        [
-            dt_uart0.dtproperty("pinctrl-0"),
-            dt_uart0.dtproperty("pinctrl-1"),
-            dt_uart0.dtproperty("pinctrl-names"),
-        ],
-    ) == param.xsplit(cmd, sh)
-
-    with pytest.raises(DTShCommandError):
-        # Fault on missing property name.
-        param.parsed(["$"])
-        param.xsplit(cmd, sh)
-
-    with pytest.raises(DTShCommandError):
-        # Fault on undefined property name.
-        param.parsed(["$not-a-prop"])
-        param.xsplit(cmd, sh)
-
-
-def test_dtshparam_dtpathx_autocomp() -> None:
-    dtmodel = DTShTests.get_sample_dtmodel()
-    sh = DTSh(dtmodel, [])
-    param = DTShParamDTPathX()
-
-    # Should behave like DTShParamDTPath when no "$".
-    # Auto-complete DT path.
-    assert sorted([node.name for node in dtmodel.root.children]) == [
-        state.rlstr for state in param.autocomp("", sh)
-    ]
-    # Exact match.
-    assert ["soc"] == [state.rlstr for state in param.autocomp("so", sh)]
-    # No match.
-    assert [] == param.autocomp("not/a/path", sh)
-
-    assert sorted(
-        [f"${prop.name}" for prop in dtmodel.root.all_dtproperties()]
-    ) == [state.rlstr for state in param.autocomp("$", sh)]
-
-    dt_power = sh.node_at("&power")
-    assert sorted(
-        [f"&power${prop.name}" for prop in dt_power.all_dtproperties()]
-    ) == [state.rlstr for state in param.autocomp("&power$", sh)]
-
-
 def test_dtshparam_alias() -> None:
     param = DTShParamAlias()
     assert param.brief
     assert "[NAME]" == param.usage
     assert [] == param.raw
     # Default value (means all aliased nodes).
     assert "" == param.alias
@@ -1555,12 +1446,7 @@
     ]
     # Exact match.
     assert ["zephyr,bt-mon-uart"] == [
         state.rlstr for state in param.autocomp("zephyr,bt-mon", sh)
     ]
     # No match.
     assert [] == param.autocomp("Zephyr,", sh)
-    assert ["zephyr,bt-mon-uart"] == [
-        state.rlstr for state in param.autocomp("zephyr,bt-mon", sh)
-    ]
-    # No match.
-    assert [] == param.autocomp("Zephyr,", sh)
```

### Comparing `dtsh-0.2.2/tests/test_dtsh_uthelpers.py` & `dtsh-0.2rc1/tests/test_dtsh_uthelpers.py`

 * *Files identical despite different names*

