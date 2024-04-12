# Comparing `tmp/pyodide_mkdocs_theme-0.2.2.tar.gz` & `tmp/pyodide_mkdocs_theme-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.2.2.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.2.3.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.2.2.tar` & `pyodide_mkdocs_theme-0.2.3.tar`

### file list

```diff
@@ -1,71 +1,75 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.2.2/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.2.2/README.md
--rw-r--r--   0        0        0     1347 2024-04-11 09:34:15.400245 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     6071 2024-04-08 19:01:06.315166 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-11 09:34:15.432246 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      752 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:33:52.871591 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4969 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21561 2024-04-11 09:33:52.875591 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4070 2024-04-11 09:33:52.875591 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11199 2024-04-11 09:33:52.891592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0     6656 2024-04-11 09:34:15.340243 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:33:52.891592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0     9077 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11631 2024-04-11 09:33:52.895592 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    12697 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     3236 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9916 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:33:52.915593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-11 09:34:15.340243 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6699 2024-04-11 09:33:52.927593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     4566 2024-04-11 09:33:52.927593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7349 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4290 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6467 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9685 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3530 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6582 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16559 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0    31978 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css
--rw-r--r--   0        0        0     1527 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4218 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12675 2024-04-11 09:33:52.931593 pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1689 2024-04-11 09:34:12.512161 pyodide_mkdocs_theme-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.2.3/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.2.3/README.md
+-rw-r--r--   0        0        0     1347 2024-04-12 21:47:48.830344 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2160 2024-04-12 21:47:09.917172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-12 21:47:48.866345 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4969 2024-04-09 19:35:36.226493 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21303 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4075 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11199 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    12363 2024-04-12 21:47:09.925172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0     9077 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11690 2024-04-12 21:47:09.933172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    12697 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     3236 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9993 2024-04-12 21:47:09.941172 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-12 21:47:48.822343 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6881 2024-04-12 21:47:09.957173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:47:48.826344 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:47:09.961173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3974 2024-04-12 21:47:48.830344 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5490 2024-04-12 21:47:09.973173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-12 21:47:09.973173 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4320 2024-04-12 21:47:09.981174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6467 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1214 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9780 2024-04-12 21:47:09.981174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:47:09.981174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6600 2024-04-12 21:47:09.985174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0    31978 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css
+-rw-r--r--   0        0        0     1527 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12675 2024-04-12 21:47:09.985174 pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1775 2024-04-12 21:47:46.082261 pyodide_mkdocs_theme-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.2.3/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.2.2/LICENSE` & `pyodide_mkdocs_theme-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/README.md` & `pyodide_mkdocs_theme-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,44 +13,20 @@
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
-from argparse import ArgumentParser
-from .__version__ import __version__
-
-
-
-parser = ArgumentParser(
-    'pyodide_mkdocs_theme',
-    description="Scripts for pyodide-mkdocs-theme",
-    epilog="""Copyleft GNU GPLv3 🄯 2024 Frédéric Zinelli
-
-This program comes with ABSOLUTELY NO WARRANTY."""
-)
-parser.add_argument(
-    '-V', '--version', action='version', version=f'pyodide-mkdocs-theme {__version__}'
-)
-parser.add_argument(
-    '-yml', action='store_true', help='Print a base configuration for the mkdocs.yml file.'
-)
-
-def main():
-    args = parser.parse_args()
-    print(args)
-
-    if args.yml:
-        display_yml()
-
-
-
 
 def display_yml():
+    """
+    Minimal mkdocs.yml configuration file for Pyodide-Mkdocs-Theme.
+    """
+
     print('''
 # Voici un exemple presque complet de configuration pour un fichier
 # mkdocs.yml utilisant pyodide-mkdocs-theme.
 
 site_url: "{>> L'adresse de votre site web ici <<}"
 site_name: "{>> Titre pour votre site <<}"
 # site_description: "(optionnel)"
@@ -155,12 +131,7 @@
 
 
 validation:                 # Si mkdocs est lancé en mode strict (mkdocs ... --strict), les warnings lèveront une erreur
   omitted_files: warn
   unrecognized_links: warn
 
 ''')
-
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-from .plugin.pyodide_macros_plugin import PyodideMacrosPlugin
+from .plugin.pyodide_macros_plugin import PyodideMacrosPlugin
+from .messages import Msg, MsgPlural, TestsToken, Tip
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files 6% similar despite different names*

```diff
@@ -329,15 +329,15 @@
                 functional calls.
             - The last span hides the code content of the IDE when loaded.
         """
         # Mark the page as needing this kind of scripts in the body section:
         self.my_env.set_current_page_insertion_needs(ScriptKind.pyodide)
 
         ide_layout = self.generate_empty_ide()
-        buttons = self.generate_row_of_buttons()
+        buttons = self.generate_buttons_row()
         global_layout = Html.div(
             ide_layout+buttons,
             id = f"{ Prefix.global_ }{ self.editor_name }",
             kls = HtmlClass.py_mk_ide,
         )
         solution_div = self.__build_corr_and_rem()
 
@@ -477,27 +477,33 @@
         # Join every item with extra gaps, to following md rendering requirements
         out = '\n\n'.join(md_div)
         return out
 
 
 
 
-    def generate_row_of_buttons(self) -> str:
+    def generate_buttons_row(self) -> str:
         """
         Build all buttons below an "ide" (editor+terminal).
         """
+        cnt_txt, cnt_or_inf = self.my_env.lang.attempts_left.msg, self.max_attempts_symbol
+        cnt_txt_span = Html.span(cnt_txt + " : ", kls=HtmlClass.compteur_txt)
+        cnt_n_span = Html.span(cnt_or_inf, id=f'{ Prefix.compteur_ }{ self.editor_name }')
+
         buttons = [
             self.create_button("play"),
-            self.create_validation_button(),
+            self.create_button("check", btn_kind="validate") if self.has_test else "",
             self.create_button("download", margin_left=1 ),
             self.create_upload_button(margin_right=1),
             self.create_button("restart"),
             self.create_button("save"),
+            Html.span(f"{ cnt_txt_span }{ cnt_n_span }/{ cnt_or_inf }", kls=HtmlClass.compteur),
         ]
-        return ''.join(buttons)
+        buttons_div = Html.div( ''.join(buttons), kls=HtmlClass.ide_buttons_div )
+        return buttons_div
 
 
 
     def create_button(
         self, button_name: str,
         *,
         btn_kind:str=None,
@@ -517,15 +523,15 @@
         if btn_kind is None:
             btn_kind = button_name.lower()
 
         tip: Tip     = getattr(self.my_env.lang, button_name)
         span_tooltip = Html.tooltip(tip, tip.em)
         lvl_up       = self.my_env.level_up_from_current_page()
         img_link     = self.ICON_TEMPLATE.format(lvl_up=lvl_up, button_name=button_name)
-        img          = Html.img(src=img_link)
+        img          = Html.img(src=img_link, kls=HtmlClass.skip_light_box)
         button_html  = Html.button(
             f'{ img }{ span_tooltip }{ extra_content }',
             kls = HtmlClass.tooltip,
             btn_kind = btn_kind,
             style = f"margin-left:{margin_left}em; margin-right:{margin_right}em;",
             **kwargs,
             type='button',
@@ -551,27 +557,7 @@
         )
         button = self.create_button(
             "upload",
             margin_right = margin_right,
             extra_content = input_button_controller,
         )
         return button
-
-
-
-    def create_validation_button(self) -> str:
-        """
-        @brief: Generate the button for IDE {id_ide} to perform the unit tests if a valid
-                test_script.py is present.
-        @details: Hide the content in a div that is called in the Javascript
-        """
-        html_validation_button = ""
-        if self.has_test:
-            html_validation_button = self.create_button("check", btn_kind="validate")
-
-        # The counter is always present:
-        span_attempts_counter = Html.span(
-            f"{ self.max_attempts_symbol }/{ self.max_attempts_symbol }",
-            id=f'{ Prefix.compteur_ }{ self.editor_name }',
-            kls=HtmlClass.compteur,
-        )
-        return html_validation_button + span_attempts_counter
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,30 +60,30 @@
     target = get_sibling_of_current_page(env, docs_dir, nom, tail='.py')
     _,content,public_tests = env.get_hdr_and_public_contents_from(target)
 
     # Split again if another token is provided
     if stop is not None:
         # rebuild "original" if another token is provided
         if public_tests:
-            content = f"{ content }\n\n# Tests\n\n{ public_tests }"
+            content = f"{ content }{ env.lang.tests.msg }{ public_tests }"
         content = re.split(stop, content)[0]
 
     id_pattern = "" if ID is None else rf".*?,\s*ID\s*=\s*{ ID }"
     macro_pattern = f"""['"]{ nom }['"]"""
     ide_jinja_reg = re.compile( rf"{ macro }\(\s*{ macro_pattern }{ id_pattern }" )
     indent = env.get_indent_in_current_page(ide_jinja_reg)
     out = build_code_fence(content, indent, lang=lang)
     return out
 
 
 
 def py(env:MaestroIDE):
     """
     Macro python rapide, pour insérer le contenu d'un fichier python. Les parties HDR sont
-    automatiquement supprimées, de même que les tests publiques. Si un argument @stop est
+    automatiquement supprimées, de même que les tests publics. Si un argument @stop est
     fourni, ce dot être une chaîne de caractère compatible avec re.split, SANS matching groups.
     Tout contenu après ce token sera ignoré (token compris) et "strippé".
 
     ATTENTION: Ne marche pas sur les exercices avec tous les codes python dans le même fichier.
     """
     @wraps(py)
     def wrapped(nom: str, stop=None, ID:int=None) -> str:
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,16 +195,17 @@
                 f"{opt_path_or_content!s}"
             )
 
         hdr = "" if len(lst)==1 else lst[1]
         content = lst[-1].strip()
         tests_cuts = self.lang.tests.as_pattern.split(content)
         if len(tests_cuts)>2:
+            pattern = self.lang.tests.as_pattern.pattern
             raise BuildError(
-                "Found more than one time the '# ?Tests' token (case insensitive) in:\n"
+                f'Found more than one time the token { pattern } (case insensitive) in:\n'
                 + opt_path_or_content
             )
         user_code, public_tests, *_ = map(str.strip, tests_cuts + [''])
         return hdr, user_code, public_tests
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,19 @@
 
 
         # Dump to main.html:
         dumping = [ f"\n  CONFIG.{ prop } = { val }" for prop,val in dct.items() ]
 
         del self.button_icons_directory
 
-        out = f'''<script type="application/javascript">\n{ "".join(dumping) }\n</script>'''
+        out = f'''\
+<script type="application/javascript">
+{ "".join(dumping) }
+CONFIG.lang.tests.as_pattern = new RegExp(CONFIG.lang.tests.as_pattern, 'i')
+</script>'''
         return out
 
 
 
     def _check_docs_paths_validity(self) -> None :
         """
         Travel through all paths in the docs_dir and raises an BuildError if "special characters"
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,20 +132,27 @@
 
     py_mk_wrapper = AutoDescriptor()
     """ Prefix for the class mode of the div holding an IDE """
 
     ide_separator = AutoDescriptor()
     """ might be used with the _v suffix """
 
+    skip_light_box = AutoDescriptor()
+    """ Img tab with this class won't be touched by glightbox """
+
     comment = AutoDescriptor()
 
     tooltip = AutoDescriptor()
 
     compteur = AutoDescriptor()
 
+    compteur_txt = AutoDescriptor()
+
+    ide_buttons_div = AutoDescriptor()
+
     stdout_ctrl = AutoDescriptor("stdout-ctrl")
 
 
 
 
     py_mk_admonition_qcm = AutoDescriptor()
     """ Admonition containing a QCM """
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -35,45 +35,45 @@
     buttonIconsDirectory: null,
     decreaseAttemptsOnUserCodeFailure: null,
     encryptCorrectionsAndRems: null,
     showAssertionCodeOnFailedTest: null,
     siteName: null,
     version: null,
     lang: {
-        successMsg: null,
+        comments: null,
+        tests: null,
         runScript: null,
+        successMsg: null,
         installStart: null,
         installDone: null,
-        qcmTitle: null,
-        tests: null,
+        feedback: null,
+        successHead: null,
+        successHeadExtra: null,
+        failHead: null,
+        successTail: null,
+        revealCorr: null,
+        revealJoin: null,
+        revealRem: null,
+        failTail: null,
         titleCorr: null,
         titleRem: null,
         corr: null,
         rem: null,
         play: null,
         check: null,
         download: null,
         upload: null,
         restart: null,
         save: null,
-        comments: null,
-        feedback: null,
-        successHead: null,
-        successHeadXtra: null,
-        failHead: null,
-        revealCorr: null,
-        revealJoin: null,
-        revealRem: null,
-        successTail: null,
-        failTail: null,
-        failTailPlural: null,
-        tipTrash: null,
-        tipQcmMask: null,
-        tipQcmCheck: null,
-        tipQcmRedo: null
+        attemptsLeft: null,
+        qcmTitle: null,
+        qcmMaskTip: null,
+        qcmCheckTip: null,
+        qcmRedoTip: null,
+        tipTrash: null
     },
     //CONFIG_DUMP
 
 
     ideProp: {}, // filled dynamically
 
     onDoneEvent: 'unload', // unused, so far...
@@ -110,16 +110,14 @@
 
     // (defined in the securedPagesData-libs.js file)
     // JS <-> python property names tracker
 
 
     cutFeedback: true,
 
-
-    publicTestsPattern: /^\s*#(\s*)test(s?)\s*$/i,
     COMMENTED_PATTERN: /(^\s*)(\S)(.?)/,
     // HDR_TOKEN_PATTERN:   /#\s*-[\s-]*HDR\s*-[\s-]*#/i,           // not used anymore
 
 
     ACE_COLOR_THEME: {
         customTheme: undefined,
         customThemeDefaultKey: "",
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -97,10 +97,11 @@
 
 
 /**Build the initial code content for an editor (initia user function + public tests).
  * */
 function getStartCode(editorName) {
     const userCode = securedExtraction(editorName, CONFIG.ideProp.userContent)
     const publicTests = securedExtraction(editorName, CONFIG.ideProp.publicTests)
-    const exerciseCode = [userCode, publicTests].filter(Boolean).join('\n\n# Tests\n\n') + "\n"
+    const joiner = CONFIG.lang.tests.msg
+    const exerciseCode = [userCode, publicTests].filter(Boolean).join(joiner) + "\n"
     return exerciseCode
 }
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -84,15 +84,17 @@
             decrease_count = stdErr = await runPythonCodeWithOptions(fullTests, terminal, options)
         }
 
         // On error, manage the counter of tries and the revelation of the solution, otherwise
         // reveal the solutions + setup success message (displayed in teardown step):
         if (!stdErr) {
             unhideSolutionAndRem(editorName)
-            finalMsg = buildSuccessMessage(editorName)
+            if (getAttemptsLeft(editorName) > 0) {
+                finalMsg = buildSuccessMessage(editorName)
+            }
 
         } else if (decrease_count) {
             const nAttemptsLeft = updateIdeCounter(editorName)
             if (unhideSolutionAndRem(editorName, nAttemptsLeft, false)) {
                 finalMsg = enhanceFailureMsg(editorName, stdErr)
             }
         }
@@ -228,15 +230,16 @@
  * Rules for toggling or not are:
  *      - leading spaces are ignored.
  *      - comment out if the first character is not "#".
  *      - if the first char is "#" and there is no spaces behind, uncomment.
  * */
 function toggleComments(editor) {
     const codeLines = editor.getSession().getValue().split('\n')
-    const iTestsToken = codeLines.findIndex(s => CONFIG.publicTestsPattern.test(s))
+    const pattern = CONFIG.lang.tests.as_pattern
+    const iTestsToken = codeLines.findIndex(s => pattern.test(s))
 
     /// No tests found:
     if (iTestsToken < 0) return;
 
     const toggled = codeLines.slice(iTestsToken + 1).map(s => {
         return s.replace(CONFIG.COMMENTED_PATTERN, (_, spaces, head, tail) => {
             if (head == '#' && tail != ' ') return spaces + tail
@@ -275,16 +278,15 @@
 
     const ide = jqThis.find("#" + editorName)[0]
     const aceEditor = setupAceEditor.call(ide, theme)
 
     const toggler = jqThis.find("[id^=comment_]")[0]
     toggler.addEventListener("click", () => toggleComments(aceEditor));
 
-
-    jqThis.children("button").each(function() {
+    jqThis.find("button").each(function() {
         const btn = $(this)
         const kind = btn.attr('btn_kind')
 
         let callback
         switch (kind) {
             case 'play':
                 callback = play(editorName);
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,15 @@
 
 .py_mk_ide .compteur {
   float: right;
   color: var(--main-theme);
   font-size: 1.2em
 }
 
-.py_mk_ide .compteur::before {
-  content: "Evaluations restantes : ";
-  color: var(--main-theme);
+.py_mk_ide .compteur_txt {
   font-size: 0.8em
 }
 
 
 
 /*
 -------------------------------------------------------------
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -120,31 +120,33 @@
 
 
 
 function updateIdeCounter(editorName) {
 
     let nAttempts = getAttemptsLeft(editorName) - 1
     securedUpdate(editorName, "attempts_left", nAttempts)
+    const encrypted = securedExtraction(editorName, CONFIG.ideProp.encrypted)
 
     // Update the GUI counter if needed
-    if (Number.isFinite(nAttempts) && nAttempts >= 0) {
-        const cntElement = document.getElementById("compteur_" + editorName);
-        const [_, top] = cntElement.textContent.split('/')
-        cntElement.textContent = `${ nAttempts }/${ top }`;
+    if (Number.isFinite(nAttempts) && nAttempts >= 0 && encrypted) {
+        const cntElement = document.getElementById("compteur_" + editorName)
+        cntElement.textContent = nAttempts
     }
     return nAttempts
 }
 
 
 
 /**Reveal the solution+rem if still encrypted and either success or no attempts left
  * */
 function unhideSolutionAndRem(editorName, nAttemptsLeft = Infinity, success = true) {
+
     let encrypted = securedExtraction(editorName, CONFIG.ideProp.encrypted)
     let something = securedExtraction(editorName, CONFIG.ideProp.corrRemMask)
+
     if (something && encrypted && (success || nAttemptsLeft < 1)) {
         const sol_div = document.getElementById("solution_" + editorName)
         const corr_content = decrypt_string(sol_div.innerHTML)
         sol_div.innerHTML = corr_content
         sol_div.classList = []
         mathJaxUpdate() // Enforce formatting, if ever...
         securedUpdate(editorName, 'encrypted', false) // Forbid coming back here
@@ -168,39 +170,39 @@
 
 
 /**Build the full success message
  * */
 function buildSuccessMessage(editorName) {
     const emo = choice(CONFIG.MSG.successEmojis)
     let info = getSolRemTxt(editorName, true)
-    return `${ success(CONFIG.lang.successHead.msg) } ${ emo } ${ CONFIG.lang.successTail.msg }${ info }`
+    return `${ success(CONFIG.lang.successHead.msg) } ${ emo } ${ CONFIG.lang.successHeadExtra.msg }${ info }`
 }
 
 
 
 /**Build the message for the terminal, announcing that correction and remarks becoming available.
  * */
 function getSolRemTxt(editorName, isSuccess) {
     const CorrRemMask = securedExtraction(editorName, CONFIG.ideProp.corrRemMask)
     if (!CorrRemMask) return ""
 
     const msg = []
-    if (isSuccess) msg.push("\n" + CONFIG.lang.successHeadXtra.msg)
+    if (isSuccess) msg.push("\n" + CONFIG.lang.successTail.msg)
     else msg.push(failure(CONFIG.lang.failHead.msg))
 
     const sentence = []
     if (CorrRemMask & 1) sentence.push(CONFIG.lang.revealCorr.msg)
     if (CorrRemMask == 3) sentence.push(CONFIG.lang.revealJoin.msg)
     if (CorrRemMask & 2) sentence.push(CONFIG.lang.revealRem.msg)
-    if (sentence.length) {
-        sentence[0] = _.capitalize(sentence[0])
-    }
-    msg.push(...sentence)
 
     if (!isSuccess) {
-        if (CorrRemMask & 2) msg.push(CONFIG.lang.failTailPlural.msg)
-        else if (CorrRemMask) msg.push(CONFIG.lang.failTail.msg)
+        if (sentence.length) sentence[0] = _.capitalize(sentence[0])
+
+        if (CorrRemMask & 2) sentence.push(CONFIG.lang.failTail.plural)
+        else if (CorrRemMask) sentence.push(CONFIG.lang.failTail.msg)
     }
+
+    msg.push(...sentence)
     msg[msg.length - 1] += "."
 
     return msg.join(' ')
 }
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/0_cdn-terminal-replacement-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.2.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.2.3/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -113,22 +113,22 @@
         )
 
         const divAdmo = $('.' + this.qcmClass)
         const children = [...divAdmo.children()].slice(1) // Exclude the title of the admonition
         const detached = children.map(child => $(child).detach())
 
         const innerDiv = $(`<div class="${ this.innerDivPath.slice(1) }"></div>`)
-        const mask = $(createSvgMask(95, 1.1, CONFIG.lang.tipQcmMask.msg, CONFIG.lang.tipQcmMask.em))
+        const mask = $(createSvgMask(95, 1.1, CONFIG.lang.qcmMaskTip.msg, CONFIG.lang.qcmMaskTip.em))
         const checkBtn = $(makeButton('check', {
-            tipWidth: CONFIG.lang.tipQcmCheck.em,
-            tipText: CONFIG.lang.tipQcmCheck.msg
+            tipWidth: CONFIG.lang.qcmCheckTip.em,
+            tipText: CONFIG.lang.qcmCheckTip.msg
         }))
         const restartBtn = $(makeButton('restart', {
-            tipWidth: CONFIG.lang.tipQcmRedo.em,
-            tipText: CONFIG.lang.tipQcmRedo.msg
+            tipWidth: CONFIG.lang.qcmRedoTip.em,
+            tipText: CONFIG.lang.qcmRedoTip.msg
         }))
         const counter = $(`<p class="${ CONFIG.element.qcmCounterCls.slice(1) }"></p>`)
         const wrapper = $(`<div class="${ CONFIG.element.qcmWrapper.slice(1) } ${ this.reveal?'give-away':'hidden' }"></div>`)
             .append(counter, mask, checkBtn, restartBtn)
 
         innerDiv.append(...detached, wrapper)
         divAdmo.append(innerDiv)
```

### Comparing `pyodide_mkdocs_theme-0.2.2/pyproject.toml` & `pyodide_mkdocs_theme-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.2.2"
+version = "0.2.3"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
@@ -44,12 +44,14 @@
 pylint = "^3.1"
 pytest = "^8.1"
 mkdocs-awesome-pages-plugin = "^2.9"
 mkdocs-exclude = "^1.0"
 mkdocs-exclude-search = "^0.6"
 mkdocs-enumerate-headings-plugin = "^0.6"
 mkdocs-addresses = "^0.3.1"
+mkdocstrings = {version = "^0.24.3", extras = ["python"]}
+mkdocs-glightbox = "^0.3.7"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyodide_mkdocs_theme-0.2.2/PKG-INFO` & `pyodide_mkdocs_theme-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

