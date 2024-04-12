# Comparing `tmp/introspection-1.7.8.tar.gz` & `tmp/introspection-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "introspection-1.7.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "introspection-1.7.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `introspection-1.7.8.tar` & `introspection-1.7.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1070 2019-10-05 20:23:15.010707 introspection-1.7.8/LICENSE
--rw-r--r--   0        0        0      423 2020-06-21 16:21:23.702593 introspection-1.7.8/README.md
--rw-r--r--   0        0        0        1 2018-02-07 23:45:28.000000 introspection-1.7.8/docs/.nojekyll
--rw-r--r--   0        0        0     8370 2022-01-11 18:29:27.165570 introspection-1.7.8/docs/Makefile
--rw-r--r--   0        0        0    50309 2023-09-27 09:04:29.286431 introspection-1.7.8/docs/build/doctrees/call_stack.doctree
--rw-r--r--   0        0        0   113126 2023-09-27 09:04:29.472424 introspection-1.7.8/docs/build/doctrees/classes.doctree
--rw-r--r--   0        0        0   123722 2023-09-27 09:04:29.603457 introspection-1.7.8/docs/build/doctrees/dundermethods.doctree
--rw-r--r--   0        0        0   150280 2023-09-27 09:04:30.168939 introspection-1.7.8/docs/build/doctrees/function_signatures.doctree
--rw-r--r--   0        0        0     4054 2023-09-27 09:04:30.173941 introspection-1.7.8/docs/build/doctrees/index.doctree
--rw-r--r--   0        0        0   112020 2023-09-27 09:04:30.356611 introspection-1.7.8/docs/build/doctrees/misc.doctree
--rw-r--r--   0        0        0   132622 2022-07-28 05:12:16.888430 introspection-1.7.8/docs/build/doctrees/typing.doctree
--rw-r--r--   0        0        0      234 2022-07-28 05:12:17.627586 introspection-1.7.8/docs/build/html/.buildinfo
--rw-r--r--   0        0        0     4418 2022-06-30 11:20:55.284834 introspection-1.7.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    16132 2022-07-28 05:12:17.556578 introspection-1.7.8/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0      313 2022-01-14 19:00:26.466660 introspection-1.7.8/docs/build/html/_static/check-solid.svg
--rw-r--r--   0        0        0     9031 2022-01-14 19:00:26.467661 introspection-1.7.8/docs/build/html/_static/clipboard.min.js
--rw-r--r--   0        0        0      434 2022-01-14 19:00:26.467661 introspection-1.7.8/docs/build/html/_static/copy-button.svg
--rw-r--r--   0        0        0     1754 2022-01-14 19:00:26.470668 introspection-1.7.8/docs/build/html/_static/copybutton.css
--rw-r--r--   0        0        0     6716 2022-07-28 05:12:17.625587 introspection-1.7.8/docs/build/html/_static/copybutton.js
--rw-r--r--   0        0        0     2198 2022-01-14 19:00:26.473668 introspection-1.7.8/docs/build/html/_static/copybutton_funcs.js
--rw-r--r--   0        0        0     8171 2022-06-30 11:20:55.286835 introspection-1.7.8/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      435 2022-07-28 05:12:17.566583 introspection-1.7.8/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.7.8/docs/build/html/_static/favicon.svg
--rw-r--r--   0        0        0      286 2022-01-11 18:34:47.961414 introspection-1.7.8/docs/build/html/_static/file.png
--rw-r--r--   0        0        0   287630 2022-01-11 18:34:47.963413 introspection-1.7.8/docs/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0        0        0   288580 2022-06-30 11:20:55.289835 introspection-1.7.8/docs/build/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2022-06-30 11:20:55.290835 introspection-1.7.8/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2022-07-28 05:12:17.575582 introspection-1.7.8/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2022-01-11 18:34:47.966416 introspection-1.7.8/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0     9096 2022-01-15 08:34:05.001989 introspection-1.7.8/docs/build/html/_static/nightsky.css
--rw-r--r--   0        0        0    12357 2022-01-15 11:08:27.758930 introspection-1.7.8/docs/build/html/_static/nightsky.styl
--rw-r--r--   0        0        0       85 2021-03-08 19:37:10.079040 introspection-1.7.8/docs/build/html/_static/package-lock.json
--rw-r--r--   0        0        0        3 2021-03-08 19:37:10.080250 introspection-1.7.8/docs/build/html/_static/package.json
--rw-r--r--   0        0        0       90 2022-01-11 18:34:47.967415 introspection-1.7.8/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     5119 2022-01-14 23:24:17.967774 introspection-1.7.8/docs/build/html/_static/pygments-cobalt2.css
--rw-r--r--   0        0        0     4919 2022-07-28 05:12:17.543568 introspection-1.7.8/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0     4633 2022-07-28 05:12:17.544569 introspection-1.7.8/docs/build/html/_static/pygments_dark.css
--rw-r--r--   0        0        0    17088 2022-06-30 11:20:55.294836 introspection-1.7.8/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     7067 2022-07-28 05:12:17.664594 introspection-1.7.8/docs/build/html/_static/theme_switcher.js
--rw-r--r--   0        0        0    68420 2022-01-11 18:34:47.969416 introspection-1.7.8/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2022-01-11 18:34:47.970415 introspection-1.7.8/docs/build/html/_static/underscore.js
--rw-r--r--   0        0        0    19915 2022-07-28 05:12:17.083464 introspection-1.7.8/docs/build/html/call_stack.html
--rw-r--r--   0        0        0    48881 2022-07-28 05:12:17.141485 introspection-1.7.8/docs/build/html/classes.html
--rw-r--r--   0        0        0    61201 2022-07-28 05:12:17.254511 introspection-1.7.8/docs/build/html/dundermethods.html
--rw-r--r--   0        0        0    62670 2022-07-28 05:12:17.327518 introspection-1.7.8/docs/build/html/function_signatures.html
--rw-r--r--   0        0        0    24122 2022-07-28 05:12:17.499557 introspection-1.7.8/docs/build/html/genindex.html
--rw-r--r--   0        0        0     4965 2022-07-28 05:12:17.340521 introspection-1.7.8/docs/build/html/index.html
--rw-r--r--   0        0        0    54576 2022-07-28 05:12:17.404537 introspection-1.7.8/docs/build/html/misc.html
--rw-r--r--   0        0        0     1394 2022-07-28 05:12:17.632588 introspection-1.7.8/docs/build/html/objects.inv
--rw-r--r--   0        0        0     5636 2022-07-28 05:12:17.525572 introspection-1.7.8/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     3786 2022-07-28 05:12:17.541568 introspection-1.7.8/docs/build/html/search.html
--rw-r--r--   0        0        0    19468 2022-07-28 05:12:17.629587 introspection-1.7.8/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    62944 2022-07-28 05:12:17.477563 introspection-1.7.8/docs/build/html/typing.html
--rw-r--r--   0        0        0      173 2018-02-07 20:12:32.000000 introspection-1.7.8/docs/index.html
--rwxr-xr-x   0        0        0     7793 2018-02-07 15:05:16.000000 introspection-1.7.8/docs/make.bat
--rw-r--r--   0        0        0      176 2020-06-21 11:11:00.000000 introspection-1.7.8/docs/source/call_stack.rst
--rw-r--r--   0        0        0      144 2020-06-21 11:52:08.000000 introspection-1.7.8/docs/source/classes.rst
--rw-r--r--   0        0        0     3889 2022-01-14 19:30:26.076283 introspection-1.7.8/docs/source/conf.py
--rw-r--r--   0        0        0     1605 2020-07-11 05:40:06.000000 introspection-1.7.8/docs/source/dundermethods.rst
--rw-r--r--   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.7.8/docs/source/favicon.svg
--rw-r--r--   0        0        0      579 2022-01-13 20:53:53.587095 introspection-1.7.8/docs/source/function_signatures.rst
--rw-r--r--   0        0        0      496 2020-07-11 05:40:06.000000 introspection-1.7.8/docs/source/index.rst
--rw-r--r--   0        0        0      210 2022-01-15 11:18:12.735064 introspection-1.7.8/docs/source/misc.rst
--rw-r--r--   0        0        0     1672 2022-07-26 08:59:09.533795 introspection-1.7.8/docs/source/typing.rst
--rw-r--r--   0        0        0      704 2024-01-23 22:19:47.180518 introspection-1.7.8/introspection/__init__.py
--rw-r--r--   0        0        0     1668 2024-01-18 08:25:36.597619 introspection-1.7.8/introspection/_utils.py
--rw-r--r--   0        0        0     1306 2024-01-18 08:25:42.808139 introspection-1.7.8/introspection/argument_bundle.py
--rw-r--r--   0        0        0     5213 2024-01-18 10:53:25.579010 introspection-1.7.8/introspection/bound_arguments.py
--rw-r--r--   0        0        0     5388 2024-01-18 23:04:07.035404 introspection-1.7.8/introspection/call_frame.py
--rw-r--r--   0        0        0     2531 2023-12-12 21:17:22.152565 introspection-1.7.8/introspection/call_stack.py
--rw-r--r--   0        0        0    18294 2024-01-19 09:49:33.862993 introspection-1.7.8/introspection/classes.py
--rw-r--r--   0        0        0      718 2022-12-07 10:42:15.146932 introspection-1.7.8/introspection/dunder.py
--rw-r--r--   0        0        0    16502 2024-01-18 23:07:13.842401 introspection-1.7.8/introspection/dundermethods.py
--rw-r--r--   0        0        0     6011 2024-01-18 08:25:41.852978 introspection-1.7.8/introspection/errors.py
--rw-r--r--   0        0        0     1512 2024-01-18 08:25:41.645930 introspection-1.7.8/introspection/exceptions.py
--rw-r--r--   0        0        0     2024 2024-01-18 09:17:05.536726 introspection-1.7.8/introspection/hazmat.py
--rw-r--r--   0        0        0    21330 2024-01-18 23:04:47.391839 introspection-1.7.8/introspection/misc.py
--rw-r--r--   0        0        0    10865 2024-01-19 10:46:29.091164 introspection-1.7.8/introspection/misc2.py
--rw-r--r--   0        0        0     5802 2024-01-18 08:25:40.454662 introspection-1.7.8/introspection/parameter.py
--rw-r--r--   0        0        0    40316 2024-01-18 19:55:08.715620 introspection-1.7.8/introspection/signature_.py
--rw-r--r--   0        0        0     1966 2024-01-18 20:15:05.854391 introspection-1.7.8/introspection/types.py
--rw-r--r--   0        0        0      199 2024-01-19 09:03:29.591495 introspection-1.7.8/introspection/typing/__init__.py
--rw-r--r--   0        0        0      163 2024-01-23 19:52:21.080258 introspection-1.7.8/introspection/typing/_compat.py
--rw-r--r--   0        0        0     2969 2024-01-23 21:51:57.641256 introspection-1.7.8/introspection/typing/_utils.py
--rw-r--r--   0        0        0      365 2024-01-18 20:14:58.591707 introspection-1.7.8/introspection/typing/i_hate_circular_imports.py
--rw-r--r--   0        0        0     9488 2024-01-23 22:09:32.275136 introspection-1.7.8/introspection/typing/instance_check.py
--rw-r--r--   0        0        0    35436 2024-01-19 22:48:36.960074 introspection-1.7.8/introspection/typing/introspection.py
--rw-r--r--   0        0        0    17489 2024-01-19 21:01:17.972022 introspection-1.7.8/introspection/typing/misc.py
--rw-r--r--   0        0        0     4486 2024-01-23 22:19:01.712250 introspection-1.7.8/introspection/typing/subtype_check.py
--rw-r--r--   0        0        0     7831 2024-01-19 21:00:24.103910 introspection-1.7.8/introspection/typing/type_compat.py
--rw-r--r--   0        0        0     2400 2024-01-19 09:02:05.166193 introspection-1.7.8/introspection/typing/type_info.py
--rw-r--r--   0        0        0      667 2022-12-27 16:52:40.582428 introspection-1.7.8/pyproject.toml
--rw-r--r--   0        0        0      702 2024-01-18 23:02:11.112358 introspection-1.7.8/tests/conftest.py
--rw-r--r--   0        0        0      998 2024-01-18 08:25:47.069324 introspection-1.7.8/tests/test_argument_bundle.py
--rw-r--r--   0        0        0     3863 2024-01-18 23:12:45.882041 introspection-1.7.8/tests/test_bound_arguments.py
--rw-r--r--   0        0        0     3620 2024-01-19 09:53:41.199622 introspection-1.7.8/tests/test_call_frame.py
--rw-r--r--   0        0        0      991 2023-09-26 21:21:15.576128 introspection-1.7.8/tests/test_call_stack.py
--rw-r--r--   0        0        0    14394 2024-01-18 23:17:45.860907 introspection-1.7.8/tests/test_class_functions.py
--rw-r--r--   0        0        0      300 2022-07-24 08:46:16.677569 introspection-1.7.8/tests/test_deprecations.py
--rw-r--r--   0        0        0     4548 2024-01-18 23:16:27.846736 introspection-1.7.8/tests/test_dunder_functions.py
--rw-r--r--   0        0        0    11193 2024-01-19 11:49:42.874121 introspection-1.7.8/tests/test_misc_functions.py
--rw-r--r--   0        0        0     3594 2022-12-27 16:52:40.434500 introspection-1.7.8/tests/test_parameter.py
--rw-r--r--   0        0        0    13881 2024-01-18 23:14:31.422176 introspection-1.7.8/tests/test_signature.py
--rw-r--r--   0        0        0    28366 2024-01-19 22:47:49.967274 introspection-1.7.8/tests/test_typing/test_introspection.py
--rw-r--r--   0        0        0     8901 2024-01-19 11:50:13.571180 introspection-1.7.8/tests/test_typing/test_misc.py
--rw-r--r--   0        0        0     3382 2024-01-23 22:15:36.047839 introspection-1.7.8/tests/test_typing/test_type_checks.py
--rw-r--r--   0        0        0     4910 2023-01-15 21:33:46.002055 introspection-1.7.8/tests/test_typing/test_type_compat.py
--rw-r--r--   0        0        0      815 2024-01-19 10:45:51.475169 introspection-1.7.8/tox.ini
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 introspection-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2019-10-05 20:23:15.010707 introspection-1.7.9/LICENSE
+-rw-r--r--   0        0        0      423 2020-06-21 16:21:23.702593 introspection-1.7.9/README.md
+-rw-r--r--   0        0        0        1 2018-02-07 23:45:28.000000 introspection-1.7.9/docs/.nojekyll
+-rw-r--r--   0        0        0     8370 2022-01-11 18:29:27.165570 introspection-1.7.9/docs/Makefile
+-rw-r--r--   0        0        0    50309 2023-09-27 09:04:29.286431 introspection-1.7.9/docs/build/doctrees/call_stack.doctree
+-rw-r--r--   0        0        0   113126 2023-09-27 09:04:29.472424 introspection-1.7.9/docs/build/doctrees/classes.doctree
+-rw-r--r--   0        0        0   123722 2023-09-27 09:04:29.603457 introspection-1.7.9/docs/build/doctrees/dundermethods.doctree
+-rw-r--r--   0        0        0   150280 2023-09-27 09:04:30.168939 introspection-1.7.9/docs/build/doctrees/function_signatures.doctree
+-rw-r--r--   0        0        0     4054 2023-09-27 09:04:30.173941 introspection-1.7.9/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0   112020 2023-09-27 09:04:30.356611 introspection-1.7.9/docs/build/doctrees/misc.doctree
+-rw-r--r--   0        0        0   132622 2022-07-28 05:12:16.888430 introspection-1.7.9/docs/build/doctrees/typing.doctree
+-rw-r--r--   0        0        0      234 2022-07-28 05:12:17.627586 introspection-1.7.9/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0     4418 2022-06-30 11:20:55.284834 introspection-1.7.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    16132 2022-07-28 05:12:17.556578 introspection-1.7.9/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0      313 2022-01-14 19:00:26.466660 introspection-1.7.9/docs/build/html/_static/check-solid.svg
+-rw-r--r--   0        0        0     9031 2022-01-14 19:00:26.467661 introspection-1.7.9/docs/build/html/_static/clipboard.min.js
+-rw-r--r--   0        0        0      434 2022-01-14 19:00:26.467661 introspection-1.7.9/docs/build/html/_static/copy-button.svg
+-rw-r--r--   0        0        0     1754 2022-01-14 19:00:26.470668 introspection-1.7.9/docs/build/html/_static/copybutton.css
+-rw-r--r--   0        0        0     6716 2022-07-28 05:12:17.625587 introspection-1.7.9/docs/build/html/_static/copybutton.js
+-rw-r--r--   0        0        0     2198 2022-01-14 19:00:26.473668 introspection-1.7.9/docs/build/html/_static/copybutton_funcs.js
+-rw-r--r--   0        0        0     8171 2022-06-30 11:20:55.286835 introspection-1.7.9/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      435 2022-07-28 05:12:17.566583 introspection-1.7.9/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.7.9/docs/build/html/_static/favicon.svg
+-rw-r--r--   0        0        0      286 2022-01-11 18:34:47.961414 introspection-1.7.9/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0   287630 2022-01-11 18:34:47.963413 introspection-1.7.9/docs/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0        0        0   288580 2022-06-30 11:20:55.289835 introspection-1.7.9/docs/build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2022-06-30 11:20:55.290835 introspection-1.7.9/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2022-07-28 05:12:17.575582 introspection-1.7.9/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2022-01-11 18:34:47.966416 introspection-1.7.9/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0     9096 2022-01-15 08:34:05.001989 introspection-1.7.9/docs/build/html/_static/nightsky.css
+-rw-r--r--   0        0        0    12357 2022-01-15 11:08:27.758930 introspection-1.7.9/docs/build/html/_static/nightsky.styl
+-rw-r--r--   0        0        0       85 2021-03-08 19:37:10.079040 introspection-1.7.9/docs/build/html/_static/package-lock.json
+-rw-r--r--   0        0        0        3 2021-03-08 19:37:10.080250 introspection-1.7.9/docs/build/html/_static/package.json
+-rw-r--r--   0        0        0       90 2022-01-11 18:34:47.967415 introspection-1.7.9/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5119 2022-01-14 23:24:17.967774 introspection-1.7.9/docs/build/html/_static/pygments-cobalt2.css
+-rw-r--r--   0        0        0     4919 2022-07-28 05:12:17.543568 introspection-1.7.9/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0     4633 2022-07-28 05:12:17.544569 introspection-1.7.9/docs/build/html/_static/pygments_dark.css
+-rw-r--r--   0        0        0    17088 2022-06-30 11:20:55.294836 introspection-1.7.9/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     7067 2022-07-28 05:12:17.664594 introspection-1.7.9/docs/build/html/_static/theme_switcher.js
+-rw-r--r--   0        0        0    68420 2022-01-11 18:34:47.969416 introspection-1.7.9/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2022-01-11 18:34:47.970415 introspection-1.7.9/docs/build/html/_static/underscore.js
+-rw-r--r--   0        0        0    19915 2022-07-28 05:12:17.083464 introspection-1.7.9/docs/build/html/call_stack.html
+-rw-r--r--   0        0        0    48881 2022-07-28 05:12:17.141485 introspection-1.7.9/docs/build/html/classes.html
+-rw-r--r--   0        0        0    61201 2022-07-28 05:12:17.254511 introspection-1.7.9/docs/build/html/dundermethods.html
+-rw-r--r--   0        0        0    62670 2022-07-28 05:12:17.327518 introspection-1.7.9/docs/build/html/function_signatures.html
+-rw-r--r--   0        0        0    24122 2022-07-28 05:12:17.499557 introspection-1.7.9/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     4965 2022-07-28 05:12:17.340521 introspection-1.7.9/docs/build/html/index.html
+-rw-r--r--   0        0        0    54576 2022-07-28 05:12:17.404537 introspection-1.7.9/docs/build/html/misc.html
+-rw-r--r--   0        0        0     1394 2022-07-28 05:12:17.632588 introspection-1.7.9/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     5636 2022-07-28 05:12:17.525572 introspection-1.7.9/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     3786 2022-07-28 05:12:17.541568 introspection-1.7.9/docs/build/html/search.html
+-rw-r--r--   0        0        0    19468 2022-07-28 05:12:17.629587 introspection-1.7.9/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    62944 2022-07-28 05:12:17.477563 introspection-1.7.9/docs/build/html/typing.html
+-rw-r--r--   0        0        0      173 2018-02-07 20:12:32.000000 introspection-1.7.9/docs/index.html
+-rwxr-xr-x   0        0        0     7793 2018-02-07 15:05:16.000000 introspection-1.7.9/docs/make.bat
+-rw-r--r--   0        0        0      176 2020-06-21 11:11:00.000000 introspection-1.7.9/docs/source/call_stack.rst
+-rw-r--r--   0        0        0      144 2020-06-21 11:52:08.000000 introspection-1.7.9/docs/source/classes.rst
+-rw-r--r--   0        0        0     3889 2022-01-14 19:30:26.076283 introspection-1.7.9/docs/source/conf.py
+-rw-r--r--   0        0        0     1605 2020-07-11 05:40:06.000000 introspection-1.7.9/docs/source/dundermethods.rst
+-rw-r--r--   0        0        0     2296 2022-01-11 21:41:53.887944 introspection-1.7.9/docs/source/favicon.svg
+-rw-r--r--   0        0        0      579 2022-01-13 20:53:53.587095 introspection-1.7.9/docs/source/function_signatures.rst
+-rw-r--r--   0        0        0      496 2020-07-11 05:40:06.000000 introspection-1.7.9/docs/source/index.rst
+-rw-r--r--   0        0        0      210 2022-01-15 11:18:12.735064 introspection-1.7.9/docs/source/misc.rst
+-rw-r--r--   0        0        0     1672 2022-07-26 08:59:09.533795 introspection-1.7.9/docs/source/typing.rst
+-rw-r--r--   0        0        0      704 2024-02-02 13:03:04.036033 introspection-1.7.9/introspection/__init__.py
+-rw-r--r--   0        0        0     1668 2024-01-18 08:25:36.597619 introspection-1.7.9/introspection/_utils.py
+-rw-r--r--   0        0        0     1306 2024-01-18 08:25:42.808139 introspection-1.7.9/introspection/argument_bundle.py
+-rw-r--r--   0        0        0     5213 2024-01-18 10:53:25.579010 introspection-1.7.9/introspection/bound_arguments.py
+-rw-r--r--   0        0        0     5388 2024-01-18 23:04:07.035404 introspection-1.7.9/introspection/call_frame.py
+-rw-r--r--   0        0        0     2531 2023-12-12 21:17:22.152565 introspection-1.7.9/introspection/call_stack.py
+-rw-r--r--   0        0        0    18294 2024-01-19 09:49:33.862993 introspection-1.7.9/introspection/classes.py
+-rw-r--r--   0        0        0      718 2022-12-07 10:42:15.146932 introspection-1.7.9/introspection/dunder.py
+-rw-r--r--   0        0        0    16502 2024-01-18 23:07:13.842401 introspection-1.7.9/introspection/dundermethods.py
+-rw-r--r--   0        0        0     6011 2024-01-18 08:25:41.852978 introspection-1.7.9/introspection/errors.py
+-rw-r--r--   0        0        0     1512 2024-01-18 08:25:41.645930 introspection-1.7.9/introspection/exceptions.py
+-rw-r--r--   0        0        0     2024 2024-01-18 09:17:05.536726 introspection-1.7.9/introspection/hazmat.py
+-rw-r--r--   0        0        0    21330 2024-01-18 23:04:47.391839 introspection-1.7.9/introspection/misc.py
+-rw-r--r--   0        0        0    10865 2024-01-19 10:46:29.091164 introspection-1.7.9/introspection/misc2.py
+-rw-r--r--   0        0        0     5802 2024-01-18 08:25:40.454662 introspection-1.7.9/introspection/parameter.py
+-rw-r--r--   0        0        0    40316 2024-01-18 19:55:08.715620 introspection-1.7.9/introspection/signature_.py
+-rw-r--r--   0        0        0     1966 2024-01-18 20:15:05.854391 introspection-1.7.9/introspection/types.py
+-rw-r--r--   0        0        0      199 2024-01-19 09:03:29.591495 introspection-1.7.9/introspection/typing/__init__.py
+-rw-r--r--   0        0        0      163 2024-01-23 19:52:21.080258 introspection-1.7.9/introspection/typing/_compat.py
+-rw-r--r--   0        0        0     2969 2024-01-23 21:51:57.641256 introspection-1.7.9/introspection/typing/_utils.py
+-rw-r--r--   0        0        0      365 2024-01-18 20:14:58.591707 introspection-1.7.9/introspection/typing/i_hate_circular_imports.py
+-rw-r--r--   0        0        0     9488 2024-01-23 22:09:32.275136 introspection-1.7.9/introspection/typing/instance_check.py
+-rw-r--r--   0        0        0    35436 2024-01-19 22:48:36.960074 introspection-1.7.9/introspection/typing/introspection.py
+-rw-r--r--   0        0        0    19030 2024-01-31 11:16:09.982816 introspection-1.7.9/introspection/typing/misc.py
+-rw-r--r--   0        0        0     4486 2024-01-23 22:19:01.712250 introspection-1.7.9/introspection/typing/subtype_check.py
+-rw-r--r--   0        0        0     7831 2024-01-19 21:00:24.103910 introspection-1.7.9/introspection/typing/type_compat.py
+-rw-r--r--   0        0        0     2400 2024-01-19 09:02:05.166193 introspection-1.7.9/introspection/typing/type_info.py
+-rw-r--r--   0        0        0      667 2022-12-27 16:52:40.582428 introspection-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0      702 2024-01-18 23:02:11.112358 introspection-1.7.9/tests/conftest.py
+-rw-r--r--   0        0        0      998 2024-01-18 08:25:47.069324 introspection-1.7.9/tests/test_argument_bundle.py
+-rw-r--r--   0        0        0     3863 2024-01-18 23:12:45.882041 introspection-1.7.9/tests/test_bound_arguments.py
+-rw-r--r--   0        0        0     3620 2024-01-19 09:53:41.199622 introspection-1.7.9/tests/test_call_frame.py
+-rw-r--r--   0        0        0      991 2023-09-26 21:21:15.576128 introspection-1.7.9/tests/test_call_stack.py
+-rw-r--r--   0        0        0    14394 2024-01-18 23:17:45.860907 introspection-1.7.9/tests/test_class_functions.py
+-rw-r--r--   0        0        0      300 2022-07-24 08:46:16.677569 introspection-1.7.9/tests/test_deprecations.py
+-rw-r--r--   0        0        0     4548 2024-01-18 23:16:27.846736 introspection-1.7.9/tests/test_dunder_functions.py
+-rw-r--r--   0        0        0    11193 2024-01-19 11:49:42.874121 introspection-1.7.9/tests/test_misc_functions.py
+-rw-r--r--   0        0        0     3594 2022-12-27 16:52:40.434500 introspection-1.7.9/tests/test_parameter.py
+-rw-r--r--   0        0        0    13881 2024-01-18 23:14:31.422176 introspection-1.7.9/tests/test_signature.py
+-rw-r--r--   0        0        0    28366 2024-01-19 22:47:49.967274 introspection-1.7.9/tests/test_typing/test_introspection.py
+-rw-r--r--   0        0        0     9027 2024-01-30 20:36:10.077258 introspection-1.7.9/tests/test_typing/test_misc.py
+-rw-r--r--   0        0        0     3382 2024-01-23 22:15:36.047839 introspection-1.7.9/tests/test_typing/test_type_checks.py
+-rw-r--r--   0        0        0     4910 2023-01-15 21:33:46.002055 introspection-1.7.9/tests/test_typing/test_type_compat.py
+-rw-r--r--   0        0        0      815 2024-01-19 10:45:51.475169 introspection-1.7.9/tox.ini
+-rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 introspection-1.7.9/PKG-INFO
```

### Comparing `introspection-1.7.8/LICENSE` & `introspection-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/Makefile` & `introspection-1.7.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/doctrees/call_stack.doctree` & `introspection-1.7.9/docs/build/doctrees/call_stack.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/doctrees/classes.doctree` & `introspection-1.7.9/docs/build/doctrees/classes.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/doctrees/dundermethods.doctree` & `introspection-1.7.9/docs/build/doctrees/dundermethods.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/doctrees/function_signatures.doctree` & `introspection-1.7.9/docs/build/doctrees/function_signatures.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/doctrees/index.doctree` & `introspection-1.7.9/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/doctrees/misc.doctree` & `introspection-1.7.9/docs/build/doctrees/misc.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/doctrees/typing.doctree` & `introspection-1.7.9/docs/build/doctrees/typing.doctree`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `introspection-1.7.9/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/basic.css` & `introspection-1.7.9/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/clipboard.min.js` & `introspection-1.7.9/docs/build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/copybutton.css` & `introspection-1.7.9/docs/build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/copybutton.js` & `introspection-1.7.9/docs/build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/copybutton_funcs.js` & `introspection-1.7.9/docs/build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/doctools.js` & `introspection-1.7.9/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/favicon.svg` & `introspection-1.7.9/docs/build/html/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/jquery-3.5.1.js` & `introspection-1.7.9/docs/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/jquery-3.6.0.js` & `introspection-1.7.9/docs/build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/jquery.js` & `introspection-1.7.9/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/language_data.js` & `introspection-1.7.9/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/nightsky.css` & `introspection-1.7.9/docs/build/html/_static/nightsky.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/nightsky.styl` & `introspection-1.7.9/docs/build/html/_static/nightsky.styl`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/pygments-cobalt2.css` & `introspection-1.7.9/docs/build/html/_static/pygments-cobalt2.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/pygments.css` & `introspection-1.7.9/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/pygments_dark.css` & `introspection-1.7.9/docs/build/html/_static/pygments_dark.css`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/searchtools.js` & `introspection-1.7.9/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/theme_switcher.js` & `introspection-1.7.9/docs/build/html/_static/theme_switcher.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/underscore-1.13.1.js` & `introspection-1.7.9/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/_static/underscore.js` & `introspection-1.7.9/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/call_stack.html` & `introspection-1.7.9/docs/build/html/call_stack.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/classes.html` & `introspection-1.7.9/docs/build/html/classes.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/dundermethods.html` & `introspection-1.7.9/docs/build/html/dundermethods.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/function_signatures.html` & `introspection-1.7.9/docs/build/html/function_signatures.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/genindex.html` & `introspection-1.7.9/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/index.html` & `introspection-1.7.9/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/misc.html` & `introspection-1.7.9/docs/build/html/misc.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/objects.inv` & `introspection-1.7.9/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/py-modindex.html` & `introspection-1.7.9/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/search.html` & `introspection-1.7.9/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/searchindex.js` & `introspection-1.7.9/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/build/html/typing.html` & `introspection-1.7.9/docs/build/html/typing.html`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/make.bat` & `introspection-1.7.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/source/conf.py` & `introspection-1.7.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/source/dundermethods.rst` & `introspection-1.7.9/docs/source/dundermethods.rst`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/source/favicon.svg` & `introspection-1.7.9/docs/source/favicon.svg`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/source/function_signatures.rst` & `introspection-1.7.9/docs/source/function_signatures.rst`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/docs/source/typing.rst` & `introspection-1.7.9/docs/source/typing.rst`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/__init__.py` & `introspection-1.7.9/introspection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 New and improved introspection functions
 """
 
-__version__ = "1.7.8"
+__version__ = "1.7.9"
 
 from .parameter import *
 from .signature_ import *
 from .argument_bundle import *
 from .bound_arguments import *
 from .call_stack import *
 from .call_frame import *
```

### Comparing `introspection-1.7.8/introspection/_utils.py` & `introspection-1.7.9/introspection/_utils.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/argument_bundle.py` & `introspection-1.7.9/introspection/argument_bundle.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/bound_arguments.py` & `introspection-1.7.9/introspection/bound_arguments.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/call_frame.py` & `introspection-1.7.9/introspection/call_frame.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/call_stack.py` & `introspection-1.7.9/introspection/call_stack.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/classes.py` & `introspection-1.7.9/introspection/classes.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/dunder.py` & `introspection-1.7.9/introspection/dunder.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/dundermethods.py` & `introspection-1.7.9/introspection/dundermethods.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/errors.py` & `introspection-1.7.9/introspection/errors.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/exceptions.py` & `introspection-1.7.9/introspection/exceptions.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/hazmat.py` & `introspection-1.7.9/introspection/hazmat.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/misc.py` & `introspection-1.7.9/introspection/misc.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/misc2.py` & `introspection-1.7.9/introspection/misc2.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/parameter.py` & `introspection-1.7.9/introspection/parameter.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/signature_.py` & `introspection-1.7.9/introspection/signature_.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/types.py` & `introspection-1.7.9/introspection/types.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/typing/_utils.py` & `introspection-1.7.9/introspection/typing/_utils.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/typing/instance_check.py` & `introspection-1.7.9/introspection/typing/instance_check.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/typing/introspection.py` & `introspection-1.7.9/introspection/typing/introspection.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/typing/misc.py` & `introspection-1.7.9/introspection/typing/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 def resolve_forward_refs(
     annotation: TypeAnnotation,
     context: ForwardRefContext = None,
     *,
     mode: Literal["eval", "getattr", "ast"] = "eval",
     strict: bool = True,
     max_depth: Optional[int] = None,
+    extra_globals: Mapping[str, object] = {},
     treat_name_errors_as_imports: bool = False,
 ) -> TypeAnnotation:
     ...
 
 
 @overload
 def resolve_forward_refs(
@@ -57,24 +58,26 @@
     module: typing.Optional[types.ModuleType] = None,
     eval_: bool = True,
     strict: bool = True,
 ) -> TypeAnnotation:
     ...
 
 
-def resolve_forward_refs(  # type: ignore[wtf]
+def resolve_forward_refs(  # type: ignore
     annotation: TypeAnnotation,
     context: ForwardRefContext = None,
     eval_: Optional[bool] = None,
     strict: bool = True,
     *,
     module: typing.Optional[types.ModuleType] = None,
     mode: Literal["eval", "getattr", "ast"] = "eval",
     max_depth: Optional[int] = None,
+    extra_globals: Mapping[str, object] = {},
     treat_name_errors_as_imports: bool = False,
+    _currently_evaluating: AbstractSet[Tuple[str, int]] = set(),
 ) -> TypeAnnotation:
     """
     Resolves forward references in a type annotation.
 
     Examples::
 
         >>> resolve_forward_refs(List['int'])
@@ -124,23 +127,32 @@
     def recurse(annotation: TypeAnnotation) -> TypeAnnotation:
         return resolve_forward_refs(
             annotation,
             context,
             mode=mode,
             strict=strict,
             max_depth=max_depth - 1,
+            extra_globals=extra_globals,
+            _currently_evaluating=_currently_evaluating,  # type: ignore
         )
 
     if isinstance(annotation, ForwardRef):
         if context is None:
             context = annotation.__forward_module__
 
         annotation = _get_forward_ref_code(annotation)
 
     if isinstance(annotation, str):
+        # First, check if this exact same forward reference is already being evaluated - i.e. it is
+        # a recursive type.
+        key = (annotation, id(context))
+        if key in _currently_evaluating:
+            return annotation
+        _currently_evaluating = _currently_evaluating | {key}
+
         scope: collections.ChainMap[str, object] = collections.ChainMap()
 
         if context is None:
             scope.maps.extend(
                 vars(module) for module in (collections.abc, collections, typing, typing_extensions)  # type: ignore
             )
         elif isinstance(context, types.ModuleType):
@@ -151,20 +163,23 @@
         elif isinstance(context, collections.abc.Mapping):
             scope.maps.append(context)  # type: ignore
         else:
             module = importlib.import_module(context.__module__)
             scope.maps.append(vars(module))
 
         scope.maps.append(vars(builtins))  # type: ignore
+        scope.maps.append(extra_globals)  # type: ignore
 
         if treat_name_errors_as_imports:
             from ._utils import ImporterDict
 
             scope.maps.append(ImporterDict())  # type: ignore
 
+        # Note: Annotations can be strings inside of strings, like `"'int'"`. So evaluating it once
+        # isn't necessarily enough; make sure to call `recurse()` with the result!
         if mode == "eval":
             try:
                 # The globals must be a real dict, so the scope will be used as
                 # the locals
                 annotation = eval(annotation, {}, scope)
             except Exception:
                 pass
@@ -178,25 +193,31 @@
             except KeyError:
                 pass
             else:
                 try:
                     for attr in attrs:
                         value = getattr(value, attr)
 
-                    return value  # type: ignore
+                    return recurse(value)  # type: ignore
                 except AttributeError:
                     pass
         elif mode == "ast":
             expr = ast.parse(annotation, mode="eval")
             try:
-                result = _eval_ast(expr.body, scope, strict=strict, max_depth=max_depth)
+                result = _eval_ast(
+                    expr.body,
+                    scope,
+                    strict=strict,
+                    max_depth=max_depth,
+                    treat_name_errors_as_imports=treat_name_errors_as_imports,
+                )
             except Exception:
                 pass
             else:
-                return result  # type: ignore
+                return recurse(result)  # type: ignore
         else:
             assert False, f"Invalid mode: {mode!r}"
 
         if annotation == "ellipsis":
             return type(...)
 
         if not strict:
@@ -259,28 +280,30 @@
 
     type_args = get_type_arguments(annotation)
     type_args = tuple(recurse(typ) for typ in type_args)  # type: ignore
     return parameterize(base, type_args)
 
 
 def _eval_ast(
-    node: ast.AST, scope: typing.Mapping[str, object], strict: bool, max_depth: int
+    node: ast.AST,
+    scope: typing.Mapping[str, object],
+    strict: bool,
+    max_depth: int,
+    treat_name_errors_as_imports: bool,
 ) -> object:
     # Compared to "eval" and "getattr", this method of evaluating forward refs
     # has the advantage of being able to perform partial evaluation. For
     # example, the forward ref `"ClassVar[NameThatCannotBeResolved]"` can be
     # turned into `ClassVar["NameThatCannotBeResolved"]`.
-    #
-    # Sometimes we need to know whether the forward ref was resolved or not.
-    # That's why this function returns a tuple of `(bool, object)`.
+
     def recurse(node: ast.AST) -> object:
         if max_depth <= 1:
             return ast.unparse(node)
 
-        return _eval_ast(node, scope, strict, max_depth - 1)
+        return _eval_ast(node, scope, strict, max_depth - 1, treat_name_errors_as_imports)
 
     if strict:
         safe_recurse = recurse
     else:
 
         def safe_recurse(node: ast.AST) -> object:
             try:
@@ -294,23 +317,42 @@
 
         return resolve_forward_refs(
             obj,  # type: ignore
             scope,
             mode="ast",
             strict=strict,
             max_depth=max_depth - 1,
-            treat_name_errors_as_imports=False,
+            treat_name_errors_as_imports=treat_name_errors_as_imports,
         )
 
     if type(node) is ast.Name:
         name = node.id
         return scope[name]
     elif type(node) is ast.Attribute:
         obj = recurse(node.value)
-        return getattr(obj, node.attr)
+
+        try:
+            return getattr(obj, node.attr)
+        except AttributeError:
+            # The parameter name is a little misleading, but we'll also treat AttributeErrors on
+            # modules as missing imports
+            if not treat_name_errors_as_imports or not isinstance(obj, types.ModuleType):
+                raise
+
+            try:
+                importlib.import_module(f"{obj.__name__}.{node.attr}")
+            except ImportError:
+                pass
+
+            try:
+                return getattr(obj, node.attr)
+            except AttributeError:
+                pass
+
+            raise
     elif type(node) is ast.Subscript:
         generic_type = recurse(node.value)
         subtype = safe_recurse(node.slice)
 
         # If we're dealing with `typing.Literal` or `typing.Annotated`, we must leave strings as
         # strings. But for any other type, we must treat them as forward references.
         if generic_type in LITERAL_TYPES:
```

### Comparing `introspection-1.7.8/introspection/typing/subtype_check.py` & `introspection-1.7.9/introspection/typing/subtype_check.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/typing/type_compat.py` & `introspection-1.7.9/introspection/typing/type_compat.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/introspection/typing/type_info.py` & `introspection-1.7.9/introspection/typing/type_info.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/pyproject.toml` & `introspection-1.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/conftest.py` & `introspection-1.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_argument_bundle.py` & `introspection-1.7.9/tests/test_argument_bundle.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_bound_arguments.py` & `introspection-1.7.9/tests/test_bound_arguments.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_call_frame.py` & `introspection-1.7.9/tests/test_call_frame.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_call_stack.py` & `introspection-1.7.9/tests/test_call_stack.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_class_functions.py` & `introspection-1.7.9/tests/test_class_functions.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_dunder_functions.py` & `introspection-1.7.9/tests/test_dunder_functions.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_misc_functions.py` & `introspection-1.7.9/tests/test_misc_functions.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_parameter.py` & `introspection-1.7.9/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_signature.py` & `introspection-1.7.9/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_typing/test_introspection.py` & `introspection-1.7.9/tests/test_typing/test_introspection.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_typing/test_misc.py` & `introspection-1.7.9/tests/test_typing/test_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import *
 from typing_extensions import ParamSpec
 
 from introspection.typing.misc import *
 
 
 T = TypeVar("T")
+RecursiveType = List["RecursiveType"]
 
 THIS_MODULE = sys.modules[__name__]
 
 
 @pytest.mark.parametrize(
     "expected",
     [
@@ -158,14 +159,16 @@
         (List["str"], List[str]),
         (Tuple[Dict["str", "int"]], Tuple[Dict[str, int]]),
         (Tuple["Dict[str, int]"], Tuple[Dict[str, int]]),
         (Callable[["int"], str], Callable[[int], str]),
         ("ellipsis", type(...)),
         ('List["int"]', List[int]),
         ('Literal["int"]', Literal["int"]),  # `Literal` arguments must be left as strings
+        ('"int"', int),  # Double stringified
+        ("RecursiveType", RecursiveType),
     ],
 )
 @pytest.mark.parametrize("mode", ["eval", "ast"])
 def test_resolve_forward_refs(mode, annotation, expected):
     assert resolve_forward_refs(annotation, globals(), mode=mode) == expected
```

### Comparing `introspection-1.7.8/tests/test_typing/test_type_checks.py` & `introspection-1.7.9/tests/test_typing/test_type_checks.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tests/test_typing/test_type_compat.py` & `introspection-1.7.9/tests/test_typing/test_type_compat.py`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/tox.ini` & `introspection-1.7.9/tox.ini`

 * *Files identical despite different names*

### Comparing `introspection-1.7.8/PKG-INFO` & `introspection-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: introspection
-Version: 1.7.8
+Version: 1.7.9
 Summary: New and improved introspection functions
 Author: Paul Pinterits
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: ordered-set
 Requires-Dist: renumerate
 Requires-Dist: sentinel
```

